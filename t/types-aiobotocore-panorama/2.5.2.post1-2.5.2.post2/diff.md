# Comparing `tmp/types-aiobotocore-panorama-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-panorama-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-panorama-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-panorama-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-panorama-2.5.2.post1.tar` & `types-aiobotocore-panorama-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.853503 types-aiobotocore-panorama-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-08-02 14:52:45.853503 types-aiobotocore-panorama-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:45.853503 types-aiobotocore-panorama-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.849503 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25632 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25589 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39025 2023-08-02 14:44:36.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38982 2023-08-02 14:44:36.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:35.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.853503 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:45.000000 types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.436643 types-aiobotocore-panorama-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12297 2023-08-04 13:59:20.436643 types-aiobotocore-panorama-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10775 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.436643 types-aiobotocore-panorama-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.436643 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      450 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      449 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25607 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25564 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11061 2023-08-04 13:46:24.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11059 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37316 2023-08-04 13:46:25.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37275 2023-08-04 13:46:24.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:22.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.436643 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12297 2023-08-04 13:59:20.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      751 2023-08-04 13:59:20.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:20.000000 types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-panorama-2.5.2.post1/LICENSE` & `types-aiobotocore-panorama-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-panorama-2.5.2.post1/setup.py` & `types-aiobotocore-panorama-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-panorama",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_panorama"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Panorama 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/__main__.py` & `types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Panorama 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Panorama 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama\nOther"
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

### Comparing `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/client.py` & `types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,28 +42,28 @@
     DescribeDeviceResponseTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DescribeNodeResponseTypeDef,
     DescribePackageImportJobResponseTypeDef,
     DescribePackageResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     DeviceJobConfigTypeDef,
-    JobResourceTagsUnionTypeDef,
+    JobResourceTagsTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesJobsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    NetworkPayloadUnionTypeDef,
+    NetworkPayloadTypeDef,
     NodeSignalTypeDef,
     PackageImportJobInputConfigTypeDef,
     PackageImportJobOutputConfigTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
 )
@@ -165,15 +165,15 @@
         self,
         *,
         NodeName: str,
         OutputPackageName: str,
         OutputPackageVersion: str,
         TemplateParameters: Mapping[str, str],
         TemplateType: Literal["RTSP_CAMERA_STREAM"],
-        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...,
+        JobTags: Sequence[JobResourceTagsTypeDef] = ...,
         NodeDescription: str = ...
     ) -> CreateNodeFromTemplateJobResponseTypeDef:
         """
         Creates a camera stream node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_node_from_template_job)
@@ -192,15 +192,15 @@
     async def create_package_import_job(
         self,
         *,
         ClientToken: str,
         InputConfig: PackageImportJobInputConfigTypeDef,
         JobType: PackageImportJobTypeType,
         OutputConfig: PackageImportJobOutputConfigTypeDef,
-        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...
+        JobTags: Sequence[JobResourceTagsTypeDef] = ...
     ) -> CreatePackageImportJobResponseTypeDef:
         """
         Imports a node package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_package_import_job)
         """
@@ -461,15 +461,15 @@
         """
 
     async def provision_device(
         self,
         *,
         Name: str,
         Description: str = ...,
-        NetworkingConfiguration: NetworkPayloadUnionTypeDef = ...,
+        NetworkingConfiguration: NetworkPayloadTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> ProvisionDeviceResponseTypeDef:
         """
         Creates a device and returns a configuration archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#provision_device)
```

### Comparing `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/client.pyi` & `types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -42,28 +42,28 @@
     DescribeDeviceResponseTypeDef,
     DescribeNodeFromTemplateJobResponseTypeDef,
     DescribeNodeResponseTypeDef,
     DescribePackageImportJobResponseTypeDef,
     DescribePackageResponseTypeDef,
     DescribePackageVersionResponseTypeDef,
     DeviceJobConfigTypeDef,
-    JobResourceTagsUnionTypeDef,
+    JobResourceTagsTypeDef,
     ListApplicationInstanceDependenciesResponseTypeDef,
     ListApplicationInstanceNodeInstancesResponseTypeDef,
     ListApplicationInstancesResponseTypeDef,
     ListDevicesJobsResponseTypeDef,
     ListDevicesResponseTypeDef,
     ListNodeFromTemplateJobsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListPackageImportJobsResponseTypeDef,
     ListPackagesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManifestOverridesPayloadTypeDef,
     ManifestPayloadTypeDef,
-    NetworkPayloadUnionTypeDef,
+    NetworkPayloadTypeDef,
     NodeSignalTypeDef,
     PackageImportJobInputConfigTypeDef,
     PackageImportJobOutputConfigTypeDef,
     ProvisionDeviceResponseTypeDef,
     SignalApplicationInstanceNodeInstancesResponseTypeDef,
     UpdateDeviceMetadataResponseTypeDef,
 )
@@ -156,15 +156,15 @@
         self,
         *,
         NodeName: str,
         OutputPackageName: str,
         OutputPackageVersion: str,
         TemplateParameters: Mapping[str, str],
         TemplateType: Literal["RTSP_CAMERA_STREAM"],
-        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...,
+        JobTags: Sequence[JobResourceTagsTypeDef] = ...,
         NodeDescription: str = ...
     ) -> CreateNodeFromTemplateJobResponseTypeDef:
         """
         Creates a camera stream node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_node_from_template_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_node_from_template_job)
@@ -181,15 +181,15 @@
     async def create_package_import_job(
         self,
         *,
         ClientToken: str,
         InputConfig: PackageImportJobInputConfigTypeDef,
         JobType: PackageImportJobTypeType,
         OutputConfig: PackageImportJobOutputConfigTypeDef,
-        JobTags: Sequence[JobResourceTagsUnionTypeDef] = ...
+        JobTags: Sequence[JobResourceTagsTypeDef] = ...
     ) -> CreatePackageImportJobResponseTypeDef:
         """
         Imports a node package.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.create_package_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#create_package_import_job)
         """
@@ -426,15 +426,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#list_tags_for_resource)
         """
     async def provision_device(
         self,
         *,
         Name: str,
         Description: str = ...,
-        NetworkingConfiguration: NetworkPayloadUnionTypeDef = ...,
+        NetworkingConfiguration: NetworkPayloadTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> ProvisionDeviceResponseTypeDef:
         """
         Creates a device and returns a configuration archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#Panorama.Client.provision_device)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_panorama/client/#provision_device)
```

### Comparing `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/literals.py` & `types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
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
@@ -242,14 +243,15 @@
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
@@ -328,26 +330,28 @@
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

### Comparing `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/literals.pyi` & `types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
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
@@ -240,14 +241,15 @@
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
@@ -326,26 +328,28 @@
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

### Comparing `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/type_defs.py` & `types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_panorama.type_defs import AlternateSoftwareMetadataTypeDef
 
     data: AlternateSoftwareMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ApplicationInstanceHealthStatusType,
     ApplicationInstanceStatusType,
     ConnectionTypeType,
     DesiredStateType,
     DeviceAggregatedStatusType,
@@ -55,36 +55,34 @@
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
     "ResponseMetadataTypeDef",
     "JobTypeDef",
+    "JobResourceTagsTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
-    "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
-    "StaticIpConnectionInfoOutputTypeDef",
     "StaticIpConnectionInfoTypeDef",
     "EthernetStatusTypeDef",
-    "JobResourceTagsTypeDef",
     "ListApplicationInstanceDependenciesRequestRequestTypeDef",
     "PackageObjectTypeDef",
     "ListApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "NodeInstanceTypeDef",
     "ListApplicationInstancesRequestRequestTypeDef",
     "ListDevicesJobsRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
@@ -93,15 +91,14 @@
     "ListNodesRequestRequestTypeDef",
     "NodeTypeDef",
     "ListPackageImportJobsRequestRequestTypeDef",
     "PackageImportJobTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageListItemTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "NtpPayloadOutputTypeDef",
     "NtpPayloadTypeDef",
     "NtpStatusTypeDef",
     "NodeInputPortTypeDef",
     "NodeOutputPortTypeDef",
     "NodeSignalTypeDef",
     "OutPutS3LocationTypeDef",
     "PackageVersionOutputConfigTypeDef",
@@ -122,23 +119,22 @@
     "DescribeDeviceJobResponseTypeDef",
     "DescribePackageVersionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ProvisionDeviceResponseTypeDef",
     "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
+    "CreateNodeFromTemplateJobRequestRequestTypeDef",
+    "DescribeNodeFromTemplateJobResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
     "DeviceTypeDef",
-    "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
-    "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
-    "JobResourceTagsUnionTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     "ListNodeFromTemplateJobsResponseTypeDef",
     "ListNodesResponseTypeDef",
     "ListPackageImportJobsResponseTypeDef",
     "ListPackagesResponseTypeDef",
     "NetworkStatusTypeDef",
@@ -146,21 +142,18 @@
     "SignalApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "PackageImportJobOutputTypeDef",
     "PackageImportJobOutputConfigTypeDef",
     "PackageVersionInputConfigTypeDef",
     "ListApplicationInstancesResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "CreateJobForDevicesRequestRequestTypeDef",
-    "NetworkPayloadOutputTypeDef",
     "NetworkPayloadTypeDef",
-    "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "DescribeNodeResponseTypeDef",
     "PackageImportJobInputConfigTypeDef",
     "DescribeDeviceResponseTypeDef",
-    "NetworkPayloadUnionTypeDef",
     "ProvisionDeviceRequestRequestTypeDef",
     "CreatePackageImportJobRequestRequestTypeDef",
     "DescribePackageImportJobResponseTypeDef",
 )
 
 AlternateSoftwareMetadataTypeDef = TypedDict(
     "AlternateSoftwareMetadataTypeDef",
@@ -212,14 +205,22 @@
     {
         "DeviceId": str,
         "JobId": str,
     },
     total=False,
 )
 
+JobResourceTagsTypeDef = TypedDict(
+    "JobResourceTagsTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Mapping[str, str],
+    },
+)
+
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "PackageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -342,22 +343,14 @@
 DescribeNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-JobResourceTagsOutputTypeDef = TypedDict(
-    "JobResourceTagsOutputTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Dict[str, str],
-    },
-)
-
 _RequiredDescribeNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeRequestRequestTypeDef",
     {
         "NodeId": str,
     },
 )
 _OptionalDescribeNodeRequestRequestTypeDef = TypedDict(
@@ -440,29 +433,19 @@
         "DeviceName": str,
         "JobId": str,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
-StaticIpConnectionInfoOutputTypeDef = TypedDict(
-    "StaticIpConnectionInfoOutputTypeDef",
-    {
-        "DefaultGateway": str,
-        "Dns": List[str],
-        "IpAddress": str,
-        "Mask": str,
-    },
-)
-
 StaticIpConnectionInfoTypeDef = TypedDict(
     "StaticIpConnectionInfoTypeDef",
     {
         "DefaultGateway": str,
-        "Dns": Sequence[str],
+        "Dns": List[str],
         "IpAddress": str,
         "Mask": str,
     },
 )
 
 EthernetStatusTypeDef = TypedDict(
     "EthernetStatusTypeDef",
@@ -470,22 +453,14 @@
         "ConnectionStatus": NetworkConnectionStatusType,
         "HwAddress": str,
         "IpAddress": str,
     },
     total=False,
 )
 
-JobResourceTagsTypeDef = TypedDict(
-    "JobResourceTagsTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Mapping[str, str],
-    },
-)
-
 _RequiredListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationInstanceDependenciesRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 _OptionalListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
@@ -705,25 +680,18 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-NtpPayloadOutputTypeDef = TypedDict(
-    "NtpPayloadOutputTypeDef",
-    {
-        "NtpServers": List[str],
-    },
-)
-
 NtpPayloadTypeDef = TypedDict(
     "NtpPayloadTypeDef",
     {
-        "NtpServers": Sequence[str],
+        "NtpServers": List[str],
     },
 )
 
 NtpStatusTypeDef = TypedDict(
     "NtpStatusTypeDef",
     {
         "ConnectionStatus": NetworkConnectionStatusType,
@@ -1072,14 +1040,60 @@
     "CreateJobForDevicesResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "TemplateParameters": Mapping[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+    },
+)
+_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "JobTags": Sequence[JobResourceTagsTypeDef],
+        "NodeDescription": str,
+    },
+    total=False,
+)
+
+
+class CreateNodeFromTemplateJobRequestRequestTypeDef(
+    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
+    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
+):
+    pass
+
+
+DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "DescribeNodeFromTemplateJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsTypeDef],
+        "LastUpdatedTime": datetime,
+        "NodeDescription": str,
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "Status": NodeFromTemplateJobStatusType,
+        "StatusMessage": str,
+        "TemplateParameters": Dict[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1117,33 +1131,14 @@
         "ProvisioningStatus": DeviceStatusType,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
     },
     total=False,
 )
 
-DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "DescribeNodeFromTemplateJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsOutputTypeDef],
-        "LastUpdatedTime": datetime,
-        "NodeDescription": str,
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "Status": NodeFromTemplateJobStatusType,
-        "StatusMessage": str,
-        "TemplateParameters": Dict[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeviceJobConfigTypeDef = TypedDict(
     "DeviceJobConfigTypeDef",
     {
         "OTAJobConfig": OTAJobConfigTypeDef,
     },
     total=False,
 )
@@ -1153,35 +1148,14 @@
     {
         "DeviceJobs": List[DeviceJobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEthernetPayloadOutputTypeDef = TypedDict(
-    "_RequiredEthernetPayloadOutputTypeDef",
-    {
-        "ConnectionType": ConnectionTypeType,
-    },
-)
-_OptionalEthernetPayloadOutputTypeDef = TypedDict(
-    "_OptionalEthernetPayloadOutputTypeDef",
-    {
-        "StaticIpConnectionInfo": StaticIpConnectionInfoOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EthernetPayloadOutputTypeDef(
-    _RequiredEthernetPayloadOutputTypeDef, _OptionalEthernetPayloadOutputTypeDef
-):
-    pass
-
-
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
     },
 )
 _OptionalEthernetPayloadTypeDef = TypedDict(
@@ -1193,15 +1167,14 @@
 )
 
 
 class EthernetPayloadTypeDef(_RequiredEthernetPayloadTypeDef, _OptionalEthernetPayloadTypeDef):
     pass
 
 
-JobResourceTagsUnionTypeDef = Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1341,61 +1314,24 @@
 class CreateJobForDevicesRequestRequestTypeDef(
     _RequiredCreateJobForDevicesRequestRequestTypeDef,
     _OptionalCreateJobForDevicesRequestRequestTypeDef,
 ):
     pass
 
 
-NetworkPayloadOutputTypeDef = TypedDict(
-    "NetworkPayloadOutputTypeDef",
-    {
-        "Ethernet0": EthernetPayloadOutputTypeDef,
-        "Ethernet1": EthernetPayloadOutputTypeDef,
-        "Ntp": NtpPayloadOutputTypeDef,
-    },
-    total=False,
-)
-
 NetworkPayloadTypeDef = TypedDict(
     "NetworkPayloadTypeDef",
     {
         "Ethernet0": EthernetPayloadTypeDef,
         "Ethernet1": EthernetPayloadTypeDef,
         "Ntp": NtpPayloadTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
-    {
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "TemplateParameters": Mapping[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-    },
-)
-_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
-    {
-        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
-        "NodeDescription": str,
-    },
-    total=False,
-)
-
-
-class CreateNodeFromTemplateJobRequestRequestTypeDef(
-    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
-    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeNodeResponseTypeDef = TypedDict(
     "DescribeNodeResponseTypeDef",
     {
         "AssetName": str,
         "Category": NodeCategoryType,
         "CreatedTime": datetime,
         "Description": str,
@@ -1435,24 +1371,23 @@
         "DeviceConnectionStatus": DeviceConnectionStatusType,
         "DeviceId": str,
         "LatestAlternateSoftware": str,
         "LatestDeviceJob": LatestDeviceJobTypeDef,
         "LatestSoftware": str,
         "LeaseExpirationTime": datetime,
         "Name": str,
-        "NetworkingConfiguration": NetworkPayloadOutputTypeDef,
+        "NetworkingConfiguration": NetworkPayloadTypeDef,
         "ProvisioningStatus": DeviceStatusType,
         "SerialNumber": str,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NetworkPayloadUnionTypeDef = Union[NetworkPayloadTypeDef, NetworkPayloadOutputTypeDef]
 _RequiredProvisionDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionDeviceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalProvisionDeviceRequestRequestTypeDef = TypedDict(
@@ -1480,15 +1415,15 @@
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
     },
 )
 _OptionalCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePackageImportJobRequestRequestTypeDef",
     {
-        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
+        "JobTags": Sequence[JobResourceTagsTypeDef],
     },
     total=False,
 )
 
 
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
@@ -1500,15 +1435,15 @@
 DescribePackageImportJobResponseTypeDef = TypedDict(
     "DescribePackageImportJobResponseTypeDef",
     {
         "ClientToken": str,
         "CreatedTime": datetime,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobId": str,
-        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "JobTags": List[JobResourceTagsTypeDef],
         "JobType": PackageImportJobTypeType,
         "LastUpdatedTime": datetime,
         "Output": PackageImportJobOutputTypeDef,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
         "Status": PackageImportJobStatusType,
         "StatusMessage": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama/type_defs.pyi` & `types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_panorama.type_defs import AlternateSoftwareMetadataTypeDef
 
     data: AlternateSoftwareMetadataTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ApplicationInstanceHealthStatusType,
     ApplicationInstanceStatusType,
     ConnectionTypeType,
     DesiredStateType,
     DeviceAggregatedStatusType,
@@ -54,36 +54,34 @@
 __all__ = (
     "AlternateSoftwareMetadataTypeDef",
     "ReportedRuntimeContextStateTypeDef",
     "ManifestOverridesPayloadTypeDef",
     "ManifestPayloadTypeDef",
     "ResponseMetadataTypeDef",
     "JobTypeDef",
+    "JobResourceTagsTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "StorageLocationTypeDef",
     "DeleteDeviceRequestRequestTypeDef",
     "DeletePackageRequestRequestTypeDef",
     "DeregisterPackageVersionRequestRequestTypeDef",
     "DescribeApplicationInstanceDetailsRequestRequestTypeDef",
     "DescribeApplicationInstanceRequestRequestTypeDef",
     "DescribeDeviceJobRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "LatestDeviceJobTypeDef",
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
-    "JobResourceTagsOutputTypeDef",
     "DescribeNodeRequestRequestTypeDef",
     "DescribePackageImportJobRequestRequestTypeDef",
     "DescribePackageRequestRequestTypeDef",
     "DescribePackageVersionRequestRequestTypeDef",
     "OTAJobConfigTypeDef",
     "DeviceJobTypeDef",
-    "StaticIpConnectionInfoOutputTypeDef",
     "StaticIpConnectionInfoTypeDef",
     "EthernetStatusTypeDef",
-    "JobResourceTagsTypeDef",
     "ListApplicationInstanceDependenciesRequestRequestTypeDef",
     "PackageObjectTypeDef",
     "ListApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "NodeInstanceTypeDef",
     "ListApplicationInstancesRequestRequestTypeDef",
     "ListDevicesJobsRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
@@ -92,15 +90,14 @@
     "ListNodesRequestRequestTypeDef",
     "NodeTypeDef",
     "ListPackageImportJobsRequestRequestTypeDef",
     "PackageImportJobTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageListItemTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "NtpPayloadOutputTypeDef",
     "NtpPayloadTypeDef",
     "NtpStatusTypeDef",
     "NodeInputPortTypeDef",
     "NodeOutputPortTypeDef",
     "NodeSignalTypeDef",
     "OutPutS3LocationTypeDef",
     "PackageVersionOutputConfigTypeDef",
@@ -121,23 +118,22 @@
     "DescribeDeviceJobResponseTypeDef",
     "DescribePackageVersionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ProvisionDeviceResponseTypeDef",
     "SignalApplicationInstanceNodeInstancesResponseTypeDef",
     "UpdateDeviceMetadataResponseTypeDef",
     "CreateJobForDevicesResponseTypeDef",
+    "CreateNodeFromTemplateJobRequestRequestTypeDef",
+    "DescribeNodeFromTemplateJobResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DescribePackageResponseTypeDef",
     "DeviceTypeDef",
-    "DescribeNodeFromTemplateJobResponseTypeDef",
     "DeviceJobConfigTypeDef",
     "ListDevicesJobsResponseTypeDef",
-    "EthernetPayloadOutputTypeDef",
     "EthernetPayloadTypeDef",
-    "JobResourceTagsUnionTypeDef",
     "ListApplicationInstanceDependenciesResponseTypeDef",
     "ListApplicationInstanceNodeInstancesResponseTypeDef",
     "ListNodeFromTemplateJobsResponseTypeDef",
     "ListNodesResponseTypeDef",
     "ListPackageImportJobsResponseTypeDef",
     "ListPackagesResponseTypeDef",
     "NetworkStatusTypeDef",
@@ -145,21 +141,18 @@
     "SignalApplicationInstanceNodeInstancesRequestRequestTypeDef",
     "PackageImportJobOutputTypeDef",
     "PackageImportJobOutputConfigTypeDef",
     "PackageVersionInputConfigTypeDef",
     "ListApplicationInstancesResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "CreateJobForDevicesRequestRequestTypeDef",
-    "NetworkPayloadOutputTypeDef",
     "NetworkPayloadTypeDef",
-    "CreateNodeFromTemplateJobRequestRequestTypeDef",
     "DescribeNodeResponseTypeDef",
     "PackageImportJobInputConfigTypeDef",
     "DescribeDeviceResponseTypeDef",
-    "NetworkPayloadUnionTypeDef",
     "ProvisionDeviceRequestRequestTypeDef",
     "CreatePackageImportJobRequestRequestTypeDef",
     "DescribePackageImportJobResponseTypeDef",
 )
 
 AlternateSoftwareMetadataTypeDef = TypedDict(
     "AlternateSoftwareMetadataTypeDef",
@@ -211,14 +204,22 @@
     {
         "DeviceId": str,
         "JobId": str,
     },
     total=False,
 )
 
+JobResourceTagsTypeDef = TypedDict(
+    "JobResourceTagsTypeDef",
+    {
+        "ResourceType": Literal["PACKAGE"],
+        "Tags": Mapping[str, str],
+    },
+)
+
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "PackageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -335,22 +336,14 @@
 DescribeNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
     "DescribeNodeFromTemplateJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
-JobResourceTagsOutputTypeDef = TypedDict(
-    "JobResourceTagsOutputTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Dict[str, str],
-    },
-)
-
 _RequiredDescribeNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeNodeRequestRequestTypeDef",
     {
         "NodeId": str,
     },
 )
 _OptionalDescribeNodeRequestRequestTypeDef = TypedDict(
@@ -427,29 +420,19 @@
         "DeviceName": str,
         "JobId": str,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
-StaticIpConnectionInfoOutputTypeDef = TypedDict(
-    "StaticIpConnectionInfoOutputTypeDef",
-    {
-        "DefaultGateway": str,
-        "Dns": List[str],
-        "IpAddress": str,
-        "Mask": str,
-    },
-)
-
 StaticIpConnectionInfoTypeDef = TypedDict(
     "StaticIpConnectionInfoTypeDef",
     {
         "DefaultGateway": str,
-        "Dns": Sequence[str],
+        "Dns": List[str],
         "IpAddress": str,
         "Mask": str,
     },
 )
 
 EthernetStatusTypeDef = TypedDict(
     "EthernetStatusTypeDef",
@@ -457,22 +440,14 @@
         "ConnectionStatus": NetworkConnectionStatusType,
         "HwAddress": str,
         "IpAddress": str,
     },
     total=False,
 )
 
-JobResourceTagsTypeDef = TypedDict(
-    "JobResourceTagsTypeDef",
-    {
-        "ResourceType": Literal["PACKAGE"],
-        "Tags": Mapping[str, str],
-    },
-)
-
 _RequiredListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationInstanceDependenciesRequestRequestTypeDef",
     {
         "ApplicationInstanceId": str,
     },
 )
 _OptionalListApplicationInstanceDependenciesRequestRequestTypeDef = TypedDict(
@@ -684,25 +659,18 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-NtpPayloadOutputTypeDef = TypedDict(
-    "NtpPayloadOutputTypeDef",
-    {
-        "NtpServers": List[str],
-    },
-)
-
 NtpPayloadTypeDef = TypedDict(
     "NtpPayloadTypeDef",
     {
-        "NtpServers": Sequence[str],
+        "NtpServers": List[str],
     },
 )
 
 NtpStatusTypeDef = TypedDict(
     "NtpStatusTypeDef",
     {
         "ConnectionStatus": NetworkConnectionStatusType,
@@ -1041,14 +1009,58 @@
     "CreateJobForDevicesResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "TemplateParameters": Mapping[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+    },
+)
+_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
+    {
+        "JobTags": Sequence[JobResourceTagsTypeDef],
+        "NodeDescription": str,
+    },
+    total=False,
+)
+
+class CreateNodeFromTemplateJobRequestRequestTypeDef(
+    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
+    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
+):
+    pass
+
+DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
+    "DescribeNodeFromTemplateJobResponseTypeDef",
+    {
+        "CreatedTime": datetime,
+        "JobId": str,
+        "JobTags": List[JobResourceTagsTypeDef],
+        "LastUpdatedTime": datetime,
+        "NodeDescription": str,
+        "NodeName": str,
+        "OutputPackageName": str,
+        "OutputPackageVersion": str,
+        "Status": NodeFromTemplateJobStatusType,
+        "StatusMessage": str,
+        "TemplateParameters": Dict[str, str],
+        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreatePackageResponseTypeDef = TypedDict(
     "CreatePackageResponseTypeDef",
     {
         "Arn": str,
         "PackageId": str,
         "StorageLocation": StorageLocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1086,33 +1098,14 @@
         "ProvisioningStatus": DeviceStatusType,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
     },
     total=False,
 )
 
-DescribeNodeFromTemplateJobResponseTypeDef = TypedDict(
-    "DescribeNodeFromTemplateJobResponseTypeDef",
-    {
-        "CreatedTime": datetime,
-        "JobId": str,
-        "JobTags": List[JobResourceTagsOutputTypeDef],
-        "LastUpdatedTime": datetime,
-        "NodeDescription": str,
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "Status": NodeFromTemplateJobStatusType,
-        "StatusMessage": str,
-        "TemplateParameters": Dict[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DeviceJobConfigTypeDef = TypedDict(
     "DeviceJobConfigTypeDef",
     {
         "OTAJobConfig": OTAJobConfigTypeDef,
     },
     total=False,
 )
@@ -1122,33 +1115,14 @@
     {
         "DeviceJobs": List[DeviceJobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEthernetPayloadOutputTypeDef = TypedDict(
-    "_RequiredEthernetPayloadOutputTypeDef",
-    {
-        "ConnectionType": ConnectionTypeType,
-    },
-)
-_OptionalEthernetPayloadOutputTypeDef = TypedDict(
-    "_OptionalEthernetPayloadOutputTypeDef",
-    {
-        "StaticIpConnectionInfo": StaticIpConnectionInfoOutputTypeDef,
-    },
-    total=False,
-)
-
-class EthernetPayloadOutputTypeDef(
-    _RequiredEthernetPayloadOutputTypeDef, _OptionalEthernetPayloadOutputTypeDef
-):
-    pass
-
 _RequiredEthernetPayloadTypeDef = TypedDict(
     "_RequiredEthernetPayloadTypeDef",
     {
         "ConnectionType": ConnectionTypeType,
     },
 )
 _OptionalEthernetPayloadTypeDef = TypedDict(
@@ -1158,15 +1132,14 @@
     },
     total=False,
 )
 
 class EthernetPayloadTypeDef(_RequiredEthernetPayloadTypeDef, _OptionalEthernetPayloadTypeDef):
     pass
 
-JobResourceTagsUnionTypeDef = Union[JobResourceTagsTypeDef, JobResourceTagsOutputTypeDef]
 ListApplicationInstanceDependenciesResponseTypeDef = TypedDict(
     "ListApplicationInstanceDependenciesResponseTypeDef",
     {
         "NextToken": str,
         "PackageObjects": List[PackageObjectTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1304,59 +1277,24 @@
 
 class CreateJobForDevicesRequestRequestTypeDef(
     _RequiredCreateJobForDevicesRequestRequestTypeDef,
     _OptionalCreateJobForDevicesRequestRequestTypeDef,
 ):
     pass
 
-NetworkPayloadOutputTypeDef = TypedDict(
-    "NetworkPayloadOutputTypeDef",
-    {
-        "Ethernet0": EthernetPayloadOutputTypeDef,
-        "Ethernet1": EthernetPayloadOutputTypeDef,
-        "Ntp": NtpPayloadOutputTypeDef,
-    },
-    total=False,
-)
-
 NetworkPayloadTypeDef = TypedDict(
     "NetworkPayloadTypeDef",
     {
         "Ethernet0": EthernetPayloadTypeDef,
         "Ethernet1": EthernetPayloadTypeDef,
         "Ntp": NtpPayloadTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNodeFromTemplateJobRequestRequestTypeDef",
-    {
-        "NodeName": str,
-        "OutputPackageName": str,
-        "OutputPackageVersion": str,
-        "TemplateParameters": Mapping[str, str],
-        "TemplateType": Literal["RTSP_CAMERA_STREAM"],
-    },
-)
-_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNodeFromTemplateJobRequestRequestTypeDef",
-    {
-        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
-        "NodeDescription": str,
-    },
-    total=False,
-)
-
-class CreateNodeFromTemplateJobRequestRequestTypeDef(
-    _RequiredCreateNodeFromTemplateJobRequestRequestTypeDef,
-    _OptionalCreateNodeFromTemplateJobRequestRequestTypeDef,
-):
-    pass
-
 DescribeNodeResponseTypeDef = TypedDict(
     "DescribeNodeResponseTypeDef",
     {
         "AssetName": str,
         "Category": NodeCategoryType,
         "CreatedTime": datetime,
         "Description": str,
@@ -1396,24 +1334,23 @@
         "DeviceConnectionStatus": DeviceConnectionStatusType,
         "DeviceId": str,
         "LatestAlternateSoftware": str,
         "LatestDeviceJob": LatestDeviceJobTypeDef,
         "LatestSoftware": str,
         "LeaseExpirationTime": datetime,
         "Name": str,
-        "NetworkingConfiguration": NetworkPayloadOutputTypeDef,
+        "NetworkingConfiguration": NetworkPayloadTypeDef,
         "ProvisioningStatus": DeviceStatusType,
         "SerialNumber": str,
         "Tags": Dict[str, str],
         "Type": DeviceTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NetworkPayloadUnionTypeDef = Union[NetworkPayloadTypeDef, NetworkPayloadOutputTypeDef]
 _RequiredProvisionDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredProvisionDeviceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalProvisionDeviceRequestRequestTypeDef = TypedDict(
@@ -1439,15 +1376,15 @@
         "JobType": PackageImportJobTypeType,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
     },
 )
 _OptionalCreatePackageImportJobRequestRequestTypeDef = TypedDict(
     "_OptionalCreatePackageImportJobRequestRequestTypeDef",
     {
-        "JobTags": Sequence[JobResourceTagsUnionTypeDef],
+        "JobTags": Sequence[JobResourceTagsTypeDef],
     },
     total=False,
 )
 
 class CreatePackageImportJobRequestRequestTypeDef(
     _RequiredCreatePackageImportJobRequestRequestTypeDef,
     _OptionalCreatePackageImportJobRequestRequestTypeDef,
@@ -1457,15 +1394,15 @@
 DescribePackageImportJobResponseTypeDef = TypedDict(
     "DescribePackageImportJobResponseTypeDef",
     {
         "ClientToken": str,
         "CreatedTime": datetime,
         "InputConfig": PackageImportJobInputConfigTypeDef,
         "JobId": str,
-        "JobTags": List[JobResourceTagsOutputTypeDef],
+        "JobTags": List[JobResourceTagsTypeDef],
         "JobType": PackageImportJobTypeType,
         "LastUpdatedTime": datetime,
         "Output": PackageImportJobOutputTypeDef,
         "OutputConfig": PackageImportJobOutputConfigTypeDef,
         "Status": PackageImportJobStatusType,
         "StatusMessage": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `types-aiobotocore-panorama-2.5.2.post1/types_aiobotocore_panorama.egg-info/SOURCES.txt` & `types-aiobotocore-panorama-2.5.2.post2/types_aiobotocore_panorama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

