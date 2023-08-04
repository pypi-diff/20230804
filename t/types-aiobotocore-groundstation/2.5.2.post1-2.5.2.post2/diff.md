# Comparing `tmp/types-aiobotocore-groundstation-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-groundstation-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-groundstation-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-groundstation-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:58 2023, max compression
```

## Comparing `types-aiobotocore-groundstation-2.5.2.post1.tar` & `types-aiobotocore-groundstation-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.809576 types-aiobotocore-groundstation-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19789 2023-08-02 14:52:21.809576 types-aiobotocore-groundstation-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18247 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:21.809576 types-aiobotocore-groundstation-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.801576 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28823 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28773 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40955 2023-08-02 14:39:48.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40906 2023-08-02 14:39:48.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-02 14:39:47.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.809576 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19789 2023-08-02 14:52:21.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-02 14:52:21.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:21.000000 types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.680372 types-aiobotocore-groundstation-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:47:17.000000 types-aiobotocore-groundstation-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-08-04 12:00:58.672372 types-aiobotocore-groundstation-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-08-04 11:47:17.000000 types-aiobotocore-groundstation-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:58.680372 types-aiobotocore-groundstation-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-04 11:47:17.000000 types-aiobotocore-groundstation-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.672372 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-04 11:47:17.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-04 11:47:17.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 11:47:17.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28813 2023-08-04 11:47:18.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28763 2023-08-04 11:47:17.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-08-04 11:47:18.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-08-04 11:47:18.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-08-04 11:47:18.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9373 2023-08-04 11:47:18.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:47:17.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40155 2023-08-04 11:47:19.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-08-04 11:47:18.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:47:17.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-08-04 11:47:18.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-04 11:47:18.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.672372 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14865 2023-08-04 12:00:58.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-08-04 12:00:58.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:58.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:00:58.000000 types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/LICENSE` & `types-aiobotocore-groundstation-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/setup.py` & `types-aiobotocore-groundstation-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-groundstation",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.GroundStation 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/__init__.py` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/__init__.pyi` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/__main__.py` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.GroundStation 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
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

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/client.py` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ConfigIdResponseTypeDef,
     ConfigTypeDataTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DescribeContactResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
     DiscoveryDataTypeDef,
-    EndpointDetailsUnionTypeDef,
+    EndpointDetailsTypeDef,
     EphemerisDataTypeDef,
     EphemerisIdResponseTypeDef,
     GetAgentConfigurationResponseTypeDef,
     GetConfigResponseTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
     GetMissionProfileResponseTypeDef,
@@ -141,15 +141,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#create_config)
         """
 
     async def create_dataflow_endpoint_group(
         self,
         *,
-        endpointDetails: Sequence[EndpointDetailsUnionTypeDef],
+        endpointDetails: Sequence[EndpointDetailsTypeDef],
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         tags: Mapping[str, str] = ...
     ) -> DataflowEndpointGroupIdResponseTypeDef:
         """
         Creates a `DataflowEndpoint` group containing the specified list of
         `DataflowEndpoint` objects.
```

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/client.pyi` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ConfigIdResponseTypeDef,
     ConfigTypeDataTypeDef,
     ContactIdResponseTypeDef,
     DataflowEndpointGroupIdResponseTypeDef,
     DescribeContactResponseTypeDef,
     DescribeEphemerisResponseTypeDef,
     DiscoveryDataTypeDef,
-    EndpointDetailsUnionTypeDef,
+    EndpointDetailsTypeDef,
     EphemerisDataTypeDef,
     EphemerisIdResponseTypeDef,
     GetAgentConfigurationResponseTypeDef,
     GetConfigResponseTypeDef,
     GetDataflowEndpointGroupResponseTypeDef,
     GetMinuteUsageResponseTypeDef,
     GetMissionProfileResponseTypeDef,
@@ -132,15 +132,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_groundstation/client/#create_config)
         """
     async def create_dataflow_endpoint_group(
         self,
         *,
-        endpointDetails: Sequence[EndpointDetailsUnionTypeDef],
+        endpointDetails: Sequence[EndpointDetailsTypeDef],
         contactPostPassDurationSeconds: int = ...,
         contactPrePassDurationSeconds: int = ...,
         tags: Mapping[str, str] = ...
     ) -> DataflowEndpointGroupIdResponseTypeDef:
         """
         Creates a `DataflowEndpoint` group containing the specified list of
         `DataflowEndpoint` objects.
```

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/literals.py` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/literals.pyi` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/paginator.py` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/paginator.pyi` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/type_defs.py` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeContactRequestRequestTypeDef",
     "DescribeEphemerisRequestRequestTypeDef",
     "DiscoveryDataTypeDef",
-    "SecurityDetailsOutputTypeDef",
     "SecurityDetailsTypeDef",
     "S3ObjectTypeDef",
     "EphemerisMetaDataTypeDef",
     "FrequencyBandwidthTypeDef",
     "FrequencyTypeDef",
     "GetAgentConfigurationRequestRequestTypeDef",
     "GetConfigRequestRequestTypeDef",
@@ -153,23 +152,21 @@
     "DescribeEphemerisResponseTypeDef",
     "ConfigTypeDataTypeDef",
     "AwsGroundStationAgentEndpointTypeDef",
     "EphemerisDataTypeDef",
     "CreateConfigRequestRequestTypeDef",
     "GetConfigResponseTypeDef",
     "UpdateConfigRequestRequestTypeDef",
-    "EndpointDetailsOutputTypeDef",
     "EndpointDetailsTypeDef",
     "CreateEphemerisRequestRequestTypeDef",
     "ConfigDetailsTypeDef",
+    "CreateDataflowEndpointGroupRequestRequestTypeDef",
     "GetDataflowEndpointGroupResponseTypeDef",
-    "EndpointDetailsUnionTypeDef",
     "DestinationTypeDef",
     "SourceTypeDef",
-    "CreateDataflowEndpointGroupRequestRequestTypeDef",
     "DataflowDetailTypeDef",
     "DescribeContactResponseTypeDef",
 )
 
 ComponentVersionTypeDef = TypedDict(
     "ComponentVersionTypeDef",
     {
@@ -441,23 +438,14 @@
     {
         "capabilityArns": Sequence[str],
         "privateIpAddresses": Sequence[str],
         "publicIpAddresses": Sequence[str],
     },
 )
 
-SecurityDetailsOutputTypeDef = TypedDict(
-    "SecurityDetailsOutputTypeDef",
-    {
-        "roleArn": str,
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-    },
-)
-
 SecurityDetailsTypeDef = TypedDict(
     "SecurityDetailsTypeDef",
     {
         "roleArn": str,
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
     },
@@ -1503,26 +1491,14 @@
         "configData": ConfigTypeDataTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
     },
 )
 
-EndpointDetailsOutputTypeDef = TypedDict(
-    "EndpointDetailsOutputTypeDef",
-    {
-        "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
-        "endpoint": DataflowEndpointTypeDef,
-        "healthReasons": List[CapabilityHealthReasonType],
-        "healthStatus": CapabilityHealthType,
-        "securityDetails": SecurityDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
         "endpoint": DataflowEndpointTypeDef,
         "healthReasons": Sequence[CapabilityHealthReasonType],
         "healthStatus": CapabilityHealthType,
@@ -1558,34 +1534,57 @@
     pass
 
 
 ConfigDetailsTypeDef = TypedDict(
     "ConfigDetailsTypeDef",
     {
         "antennaDemodDecodeDetails": AntennaDemodDecodeDetailsTypeDef,
-        "endpointDetails": EndpointDetailsOutputTypeDef,
+        "endpointDetails": EndpointDetailsTypeDef,
         "s3RecordingDetails": S3RecordingDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
+    {
+        "endpointDetails": Sequence[EndpointDetailsTypeDef],
+    },
+)
+_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDataflowEndpointGroupRequestRequestTypeDef(
+    _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
+    _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
+):
+    pass
+
+
 GetDataflowEndpointGroupResponseTypeDef = TypedDict(
     "GetDataflowEndpointGroupResponseTypeDef",
     {
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
-        "endpointsDetails": List[EndpointDetailsOutputTypeDef],
+        "endpointsDetails": List[EndpointDetailsTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointDetailsUnionTypeDef = Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "configDetails": ConfigDetailsTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "dataflowDestinationRegion": str,
@@ -1600,38 +1599,14 @@
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "dataflowSourceRegion": str,
     },
     total=False,
 )
 
-_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
-    {
-        "endpointDetails": Sequence[EndpointDetailsUnionTypeDef],
-    },
-)
-_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
-    {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDataflowEndpointGroupRequestRequestTypeDef(
-    _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
-    _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
-):
-    pass
-
-
 DataflowDetailTypeDef = TypedDict(
     "DataflowDetailTypeDef",
     {
         "destination": DestinationTypeDef,
         "errorMessage": str,
         "source": SourceTypeDef,
     },
```

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/type_defs.pyi` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     "DeleteDataflowEndpointGroupRequestRequestTypeDef",
     "DeleteEphemerisRequestRequestTypeDef",
     "DeleteMissionProfileRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeContactRequestRequestTypeDef",
     "DescribeEphemerisRequestRequestTypeDef",
     "DiscoveryDataTypeDef",
-    "SecurityDetailsOutputTypeDef",
     "SecurityDetailsTypeDef",
     "S3ObjectTypeDef",
     "EphemerisMetaDataTypeDef",
     "FrequencyBandwidthTypeDef",
     "FrequencyTypeDef",
     "GetAgentConfigurationRequestRequestTypeDef",
     "GetConfigRequestRequestTypeDef",
@@ -152,23 +151,21 @@
     "DescribeEphemerisResponseTypeDef",
     "ConfigTypeDataTypeDef",
     "AwsGroundStationAgentEndpointTypeDef",
     "EphemerisDataTypeDef",
     "CreateConfigRequestRequestTypeDef",
     "GetConfigResponseTypeDef",
     "UpdateConfigRequestRequestTypeDef",
-    "EndpointDetailsOutputTypeDef",
     "EndpointDetailsTypeDef",
     "CreateEphemerisRequestRequestTypeDef",
     "ConfigDetailsTypeDef",
+    "CreateDataflowEndpointGroupRequestRequestTypeDef",
     "GetDataflowEndpointGroupResponseTypeDef",
-    "EndpointDetailsUnionTypeDef",
     "DestinationTypeDef",
     "SourceTypeDef",
-    "CreateDataflowEndpointGroupRequestRequestTypeDef",
     "DataflowDetailTypeDef",
     "DescribeContactResponseTypeDef",
 )
 
 ComponentVersionTypeDef = TypedDict(
     "ComponentVersionTypeDef",
     {
@@ -432,23 +429,14 @@
     {
         "capabilityArns": Sequence[str],
         "privateIpAddresses": Sequence[str],
         "publicIpAddresses": Sequence[str],
     },
 )
 
-SecurityDetailsOutputTypeDef = TypedDict(
-    "SecurityDetailsOutputTypeDef",
-    {
-        "roleArn": str,
-        "securityGroupIds": List[str],
-        "subnetIds": List[str],
-    },
-)
-
 SecurityDetailsTypeDef = TypedDict(
     "SecurityDetailsTypeDef",
     {
         "roleArn": str,
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
     },
@@ -1458,26 +1446,14 @@
         "configData": ConfigTypeDataTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "name": str,
     },
 )
 
-EndpointDetailsOutputTypeDef = TypedDict(
-    "EndpointDetailsOutputTypeDef",
-    {
-        "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
-        "endpoint": DataflowEndpointTypeDef,
-        "healthReasons": List[CapabilityHealthReasonType],
-        "healthStatus": CapabilityHealthType,
-        "securityDetails": SecurityDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "awsGroundStationAgentEndpoint": AwsGroundStationAgentEndpointTypeDef,
         "endpoint": DataflowEndpointTypeDef,
         "healthReasons": Sequence[CapabilityHealthReasonType],
         "healthStatus": CapabilityHealthType,
@@ -1511,34 +1487,55 @@
 ):
     pass
 
 ConfigDetailsTypeDef = TypedDict(
     "ConfigDetailsTypeDef",
     {
         "antennaDemodDecodeDetails": AntennaDemodDecodeDetailsTypeDef,
-        "endpointDetails": EndpointDetailsOutputTypeDef,
+        "endpointDetails": EndpointDetailsTypeDef,
         "s3RecordingDetails": S3RecordingDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
+    {
+        "endpointDetails": Sequence[EndpointDetailsTypeDef],
+    },
+)
+_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
+    {
+        "contactPostPassDurationSeconds": int,
+        "contactPrePassDurationSeconds": int,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDataflowEndpointGroupRequestRequestTypeDef(
+    _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
+    _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
+):
+    pass
+
 GetDataflowEndpointGroupResponseTypeDef = TypedDict(
     "GetDataflowEndpointGroupResponseTypeDef",
     {
         "contactPostPassDurationSeconds": int,
         "contactPrePassDurationSeconds": int,
         "dataflowEndpointGroupArn": str,
         "dataflowEndpointGroupId": str,
-        "endpointsDetails": List[EndpointDetailsOutputTypeDef],
+        "endpointsDetails": List[EndpointDetailsTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointDetailsUnionTypeDef = Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "configDetails": ConfigDetailsTypeDef,
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "dataflowDestinationRegion": str,
@@ -1553,36 +1550,14 @@
         "configId": str,
         "configType": ConfigCapabilityTypeType,
         "dataflowSourceRegion": str,
     },
     total=False,
 )
 
-_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDataflowEndpointGroupRequestRequestTypeDef",
-    {
-        "endpointDetails": Sequence[EndpointDetailsUnionTypeDef],
-    },
-)
-_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDataflowEndpointGroupRequestRequestTypeDef",
-    {
-        "contactPostPassDurationSeconds": int,
-        "contactPrePassDurationSeconds": int,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDataflowEndpointGroupRequestRequestTypeDef(
-    _RequiredCreateDataflowEndpointGroupRequestRequestTypeDef,
-    _OptionalCreateDataflowEndpointGroupRequestRequestTypeDef,
-):
-    pass
-
 DataflowDetailTypeDef = TypedDict(
     "DataflowDetailTypeDef",
     {
         "destination": DestinationTypeDef,
         "errorMessage": str,
         "source": SourceTypeDef,
     },
```

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/waiter.py` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation/waiter.pyi` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-groundstation-2.5.2.post1/types_aiobotocore_groundstation.egg-info/SOURCES.txt` & `types-aiobotocore-groundstation-2.5.2.post2/types_aiobotocore_groundstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

