# Comparing `tmp/types-aiobotocore-snowball-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-snowball-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-snowball-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:03 2023, max compression
+gzip compressed data, was "types-aiobotocore-snowball-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-snowball-2.5.2.post1.tar` & `types-aiobotocore-snowball-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.137451 types-aiobotocore-snowball-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-08-02 14:53:03.133451 types-aiobotocore-snowball-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:03.137451 types-aiobotocore-snowball-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.133451 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25274 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25233 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10374 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28873 2023-08-02 14:49:55.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28852 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:54.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.133451 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:02.000000 types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.356643 types-aiobotocore-snowball-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13669 2023-08-04 13:59:27.356643 types-aiobotocore-snowball-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12147 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.356643 types-aiobotocore-snowball-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.356643 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1679 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1678 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26027 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25985 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10698 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10696 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7415 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7407 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28869 2023-08-04 13:53:54.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28848 2023-08-04 13:53:53.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:52.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.356643 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13669 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:27.000000 types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-snowball-2.5.2.post1/LICENSE` & `types-aiobotocore-snowball-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post1/setup.py` & `types-aiobotocore-snowball-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-snowball",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_snowball"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Snowball 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__init__.py` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__init__.pyi` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/__main__.py` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Snowball 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Snowball 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball\nOther"
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

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/client.py` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
+    ImpactLevelType,
     JobTypeType,
     LongTermPricingTypeType,
     RemoteManagementType,
     ServiceNameType,
     ShipmentStateType,
     ShippingOptionType,
     SnowballCapacityType,
@@ -52,23 +53,25 @@
     DescribeJobResultTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
     DeviceConfigurationTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesResultTypeDef,
-    JobResourceUnionTypeDef,
+    JobResourceTypeDef,
     ListClusterJobsResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
+    ListPickupLocationsResultTypeDef,
     ListServiceVersionsResultTypeDef,
-    NotificationUnionTypeDef,
+    NotificationTypeDef,
     OnDeviceServiceConfigurationTypeDef,
+    PickupDetailsTypeDef,
     TaxDocumentsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -160,20 +163,20 @@
     async def create_cluster(
         self,
         *,
         JobType: JobTypeType,
         AddressId: str,
         SnowballType: SnowballTypeType,
         ShippingOption: ShippingOptionType,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         InitialClusterSize: int = ...,
         ForceCreateJobs: bool = ...,
         LongTermPricingIds: Sequence[str] = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...
@@ -185,45 +188,47 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_cluster)
         """
 
     async def create_job(
         self,
         *,
         JobType: JobTypeType = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         AddressId: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ClusterId: str = ...,
         SnowballType: SnowballTypeType = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
-        LongTermPricingId: str = ...
+        LongTermPricingId: str = ...,
+        ImpactLevel: ImpactLevelType = ...,
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> CreateJobResultTypeDef:
         """
         Creates a job to import or export data between Amazon S3 and your on-premises
         data center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_job)
         """
 
     async def create_long_term_pricing(
         self,
         *,
         LongTermPricingType: LongTermPricingTypeType,
-        IsLongTermPricingAutoRenew: bool = ...,
-        SnowballType: SnowballTypeType = ...
+        SnowballType: SnowballTypeType,
+        IsLongTermPricingAutoRenew: bool = ...
     ) -> CreateLongTermPricingResultTypeDef:
         """
         Creates a job with the long-term usage option for a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_long_term_pricing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_long_term_pricing)
         """
@@ -356,17 +361,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#list_clusters)
         """
 
     async def list_compatible_images(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListCompatibleImagesResultTypeDef:
         """
-        This action returns a list of the different Amazon EC2 Amazon Machine Images
-        (AMIs) that are owned by your Amazon Web Services accountthat would be supported
-        for use on a Snow device.
+        This action returns a list of the different Amazon EC2-compatible Amazon Machine
+        Images (AMIs) that are owned by your Amazon Web Services accountthat would be
+        supported for use on a Snow device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_compatible_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#list_compatible_images)
         """
 
     async def list_jobs(
         self, *, MaxResults: int = ..., NextToken: str = ...
@@ -384,14 +389,24 @@
         """
         Lists all long-term pricing types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_long_term_pricing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#list_long_term_pricing)
         """
 
+    async def list_pickup_locations(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListPickupLocationsResultTypeDef:
+        """
+        A list of locations from which the customer can choose to pickup a device.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_pickup_locations)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#list_pickup_locations)
+        """
+
     async def list_service_versions(
         self,
         *,
         ServiceName: ServiceNameType,
         DependentServices: Sequence[DependentServiceTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -405,19 +420,19 @@
 
     async def update_cluster(
         self,
         *,
         ClusterId: str,
         RoleARN: str = ...,
         Description: str = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
         """
         While a cluster's `ClusterState` value is in the `AwaitingQuorum` state, you can
         update some of the information associated with a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_cluster)
@@ -425,22 +440,23 @@
         """
 
     async def update_job(
         self,
         *,
         JobId: str,
         RoleARN: str = ...,
-        Notification: NotificationUnionTypeDef = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
-        ForwardingAddressId: str = ...
+        ForwardingAddressId: str = ...,
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         While a job's `JobState` value is `New`, you can update some of the information
         associated with a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#update_job)
```

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/client.pyi` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
+    ImpactLevelType,
     JobTypeType,
     LongTermPricingTypeType,
     RemoteManagementType,
     ServiceNameType,
     ShipmentStateType,
     ShippingOptionType,
     SnowballCapacityType,
@@ -52,23 +53,25 @@
     DescribeJobResultTypeDef,
     DescribeReturnShippingLabelResultTypeDef,
     DeviceConfigurationTypeDef,
     GetJobManifestResultTypeDef,
     GetJobUnlockCodeResultTypeDef,
     GetSnowballUsageResultTypeDef,
     GetSoftwareUpdatesResultTypeDef,
-    JobResourceUnionTypeDef,
+    JobResourceTypeDef,
     ListClusterJobsResultTypeDef,
     ListClustersResultTypeDef,
     ListCompatibleImagesResultTypeDef,
     ListJobsResultTypeDef,
     ListLongTermPricingResultTypeDef,
+    ListPickupLocationsResultTypeDef,
     ListServiceVersionsResultTypeDef,
-    NotificationUnionTypeDef,
+    NotificationTypeDef,
     OnDeviceServiceConfigurationTypeDef,
+    PickupDetailsTypeDef,
     TaxDocumentsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -150,20 +153,20 @@
     async def create_cluster(
         self,
         *,
         JobType: JobTypeType,
         AddressId: str,
         SnowballType: SnowballTypeType,
         ShippingOption: ShippingOptionType,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
         InitialClusterSize: int = ...,
         ForceCreateJobs: bool = ...,
         LongTermPricingIds: Sequence[str] = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...
@@ -174,44 +177,46 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_cluster)
         """
     async def create_job(
         self,
         *,
         JobType: JobTypeType = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         Description: str = ...,
         AddressId: str = ...,
         KmsKeyARN: str = ...,
         RoleARN: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ClusterId: str = ...,
         SnowballType: SnowballTypeType = ...,
         ForwardingAddressId: str = ...,
         TaxDocuments: TaxDocumentsTypeDef = ...,
         DeviceConfiguration: DeviceConfigurationTypeDef = ...,
         RemoteManagement: RemoteManagementType = ...,
-        LongTermPricingId: str = ...
+        LongTermPricingId: str = ...,
+        ImpactLevel: ImpactLevelType = ...,
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> CreateJobResultTypeDef:
         """
         Creates a job to import or export data between Amazon S3 and your on-premises
         data center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_job)
         """
     async def create_long_term_pricing(
         self,
         *,
         LongTermPricingType: LongTermPricingTypeType,
-        IsLongTermPricingAutoRenew: bool = ...,
-        SnowballType: SnowballTypeType = ...
+        SnowballType: SnowballTypeType,
+        IsLongTermPricingAutoRenew: bool = ...
     ) -> CreateLongTermPricingResultTypeDef:
         """
         Creates a job with the long-term usage option for a device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.create_long_term_pricing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#create_long_term_pricing)
         """
@@ -330,17 +335,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#list_clusters)
         """
     async def list_compatible_images(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListCompatibleImagesResultTypeDef:
         """
-        This action returns a list of the different Amazon EC2 Amazon Machine Images
-        (AMIs) that are owned by your Amazon Web Services accountthat would be supported
-        for use on a Snow device.
+        This action returns a list of the different Amazon EC2-compatible Amazon Machine
+        Images (AMIs) that are owned by your Amazon Web Services accountthat would be
+        supported for use on a Snow device.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_compatible_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#list_compatible_images)
         """
     async def list_jobs(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListJobsResultTypeDef:
@@ -355,14 +360,23 @@
     ) -> ListLongTermPricingResultTypeDef:
         """
         Lists all long-term pricing types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_long_term_pricing)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#list_long_term_pricing)
         """
+    async def list_pickup_locations(
+        self, *, MaxResults: int = ..., NextToken: str = ...
+    ) -> ListPickupLocationsResultTypeDef:
+        """
+        A list of locations from which the customer can choose to pickup a device.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.list_pickup_locations)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#list_pickup_locations)
+        """
     async def list_service_versions(
         self,
         *,
         ServiceName: ServiceNameType,
         DependentServices: Sequence[DependentServiceTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
@@ -375,41 +389,42 @@
         """
     async def update_cluster(
         self,
         *,
         ClusterId: str,
         RoleARN: str = ...,
         Description: str = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
-        Notification: NotificationUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
         ForwardingAddressId: str = ...
     ) -> Dict[str, Any]:
         """
         While a cluster's `ClusterState` value is in the `AwaitingQuorum` state, you can
         update some of the information associated with a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#update_cluster)
         """
     async def update_job(
         self,
         *,
         JobId: str,
         RoleARN: str = ...,
-        Notification: NotificationUnionTypeDef = ...,
-        Resources: JobResourceUnionTypeDef = ...,
+        Notification: NotificationTypeDef = ...,
+        Resources: JobResourceTypeDef = ...,
         OnDeviceServiceConfiguration: OnDeviceServiceConfigurationTypeDef = ...,
         AddressId: str = ...,
         ShippingOption: ShippingOptionType = ...,
         Description: str = ...,
         SnowballCapacityPreference: SnowballCapacityType = ...,
-        ForwardingAddressId: str = ...
+        ForwardingAddressId: str = ...,
+        PickupDetails: PickupDetailsTypeDef = ...
     ) -> Dict[str, Any]:
         """
         While a job's `JobState` value is `New`, you can update some of the information
         associated with a job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client.update_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/client/#update_job)
```

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/literals.py` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 Type annotations for snowball service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_snowball.literals import ClusterStateType
+    from types_aiobotocore_snowball.literals import AddressTypeType
 
-    data: ClusterStateType = "AwaitingQuorum"
+    data: AddressTypeType = "AWS_SHIP"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
+    "AddressTypeType",
     "ClusterStateType",
     "DescribeAddressesPaginatorName",
     "DeviceServiceNameType",
+    "ImpactLevelType",
     "JobStateType",
     "JobTypeType",
     "ListClusterJobsPaginatorName",
     "ListClustersPaginatorName",
     "ListCompatibleImagesPaginatorName",
     "ListJobsPaginatorName",
     "ListLongTermPricingPaginatorName",
@@ -43,18 +44,19 @@
     "SnowballServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
+AddressTypeType = Literal["AWS_SHIP", "CUST_PICKUP"]
 ClusterStateType = Literal["AwaitingQuorum", "Cancelled", "Complete", "InUse", "Pending"]
 DescribeAddressesPaginatorName = Literal["describe_addresses"]
 DeviceServiceNameType = Literal["NFS_ON_DEVICE_SERVICE", "S3_ON_DEVICE_SERVICE"]
+ImpactLevelType = Literal["IL2", "IL4", "IL5", "IL6", "IL99"]
 JobStateType = Literal[
     "Cancelled",
     "Complete",
     "InProgress",
     "InTransitToAWS",
     "InTransitToCustomer",
     "Listing",
@@ -69,24 +71,33 @@
 JobTypeType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 ListClusterJobsPaginatorName = Literal["list_cluster_jobs"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListCompatibleImagesPaginatorName = Literal["list_compatible_images"]
 ListJobsPaginatorName = Literal["list_jobs"]
 ListLongTermPricingPaginatorName = Literal["list_long_term_pricing"]
 LongTermPricingTypeType = Literal["OneMonth", "OneYear", "ThreeYear"]
-RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY"]
+RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY", "NOT_INSTALLED"]
 ServiceNameType = Literal["EKS_ANYWHERE", "KUBERNETES"]
 ShipmentStateType = Literal["RECEIVED", "RETURNED"]
 ShippingLabelStatusType = Literal["Failed", "InProgress", "Succeeded", "TimedOut"]
 ShippingOptionType = Literal["EXPRESS", "NEXT_DAY", "SECOND_DAY", "STANDARD"]
 SnowballCapacityType = Literal[
-    "NoPreference", "T100", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
+    "NoPreference", "T100", "T13", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
 ]
 SnowballTypeType = Literal[
-    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C", "V3_5S"
+    "EDGE",
+    "EDGE_C",
+    "EDGE_CG",
+    "EDGE_S",
+    "RACK_5U_C",
+    "SNC1_HDD",
+    "SNC1_SSD",
+    "STANDARD",
+    "V3_5C",
+    "V3_5S",
 ]
 StorageUnitType = Literal["TB"]
 TransferOptionType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 SnowballServiceName = Literal["snowball"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -98,14 +109,15 @@
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
@@ -201,14 +213,15 @@
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
@@ -287,26 +300,28 @@
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

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/literals.pyi` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,33 @@
 Type annotations for snowball service literal definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_snowball/literals/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_snowball.literals import ClusterStateType
+    from types_aiobotocore_snowball.literals import AddressTypeType
 
-    data: ClusterStateType = "AwaitingQuorum"
+    data: AddressTypeType = "AWS_SHIP"
     ```
 """
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
+    "AddressTypeType",
     "ClusterStateType",
     "DescribeAddressesPaginatorName",
     "DeviceServiceNameType",
+    "ImpactLevelType",
     "JobStateType",
     "JobTypeType",
     "ListClusterJobsPaginatorName",
     "ListClustersPaginatorName",
     "ListCompatibleImagesPaginatorName",
     "ListJobsPaginatorName",
     "ListLongTermPricingPaginatorName",
@@ -42,17 +45,20 @@
     "SnowballServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
+AddressTypeType = Literal["AWS_SHIP", "CUST_PICKUP"]
 ClusterStateType = Literal["AwaitingQuorum", "Cancelled", "Complete", "InUse", "Pending"]
 DescribeAddressesPaginatorName = Literal["describe_addresses"]
 DeviceServiceNameType = Literal["NFS_ON_DEVICE_SERVICE", "S3_ON_DEVICE_SERVICE"]
+ImpactLevelType = Literal["IL2", "IL4", "IL5", "IL6", "IL99"]
 JobStateType = Literal[
     "Cancelled",
     "Complete",
     "InProgress",
     "InTransitToAWS",
     "InTransitToCustomer",
     "Listing",
@@ -67,24 +73,33 @@
 JobTypeType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 ListClusterJobsPaginatorName = Literal["list_cluster_jobs"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListCompatibleImagesPaginatorName = Literal["list_compatible_images"]
 ListJobsPaginatorName = Literal["list_jobs"]
 ListLongTermPricingPaginatorName = Literal["list_long_term_pricing"]
 LongTermPricingTypeType = Literal["OneMonth", "OneYear", "ThreeYear"]
-RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY"]
+RemoteManagementType = Literal["INSTALLED_AUTOSTART", "INSTALLED_ONLY", "NOT_INSTALLED"]
 ServiceNameType = Literal["EKS_ANYWHERE", "KUBERNETES"]
 ShipmentStateType = Literal["RECEIVED", "RETURNED"]
 ShippingLabelStatusType = Literal["Failed", "InProgress", "Succeeded", "TimedOut"]
 ShippingOptionType = Literal["EXPRESS", "NEXT_DAY", "SECOND_DAY", "STANDARD"]
 SnowballCapacityType = Literal[
-    "NoPreference", "T100", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
+    "NoPreference", "T100", "T13", "T14", "T240", "T32", "T42", "T50", "T8", "T80", "T98"
 ]
 SnowballTypeType = Literal[
-    "EDGE", "EDGE_C", "EDGE_CG", "EDGE_S", "SNC1_HDD", "SNC1_SSD", "STANDARD", "V3_5C", "V3_5S"
+    "EDGE",
+    "EDGE_C",
+    "EDGE_CG",
+    "EDGE_S",
+    "RACK_5U_C",
+    "SNC1_HDD",
+    "SNC1_SSD",
+    "STANDARD",
+    "V3_5C",
+    "V3_5S",
 ]
 StorageUnitType = Literal["TB"]
 TransferOptionType = Literal["EXPORT", "IMPORT", "LOCAL_USE"]
 SnowballServiceName = Literal["snowball"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -96,14 +111,15 @@
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
@@ -199,14 +215,15 @@
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
@@ -285,26 +302,28 @@
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

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/paginator.py` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/paginator.pyi` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/type_defs.py` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,18 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
+    AddressTypeType,
     ClusterStateType,
     DeviceServiceNameType,
+    ImpactLevelType,
     JobStateType,
     JobTypeType,
     LongTermPricingTypeType,
     RemoteManagementType,
     ServiceNameType,
     ShipmentStateType,
     ShippingLabelStatusType,
@@ -42,18 +44,17 @@
 
 
 __all__ = (
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
-    "NotificationOutputTypeDef",
+    "NotificationTypeDef",
     "CompatibleImageTypeDef",
     "ResponseMetadataTypeDef",
-    "NotificationTypeDef",
     "JobListEntryTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
     "DataTransferTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -72,17 +73,19 @@
     "KeyRangeTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
+    "ListPickupLocationsRequestRequestTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
     "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
+    "TimestampTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
     "CreateAddressRequestRequestTypeDef",
     "CreateAddressResultTypeDef",
@@ -94,42 +97,39 @@
     "DescribeReturnShippingLabelResultTypeDef",
     "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeResultTypeDef",
     "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesResultTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
-    "NotificationUnionTypeDef",
+    "ListPickupLocationsResultTypeDef",
     "CreateClusterResultTypeDef",
     "ListClusterJobsResultTypeDef",
     "ListJobsResultTypeDef",
     "DependentServiceTypeDef",
     "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
-    "LambdaResourceOutputTypeDef",
     "LambdaResourceTypeDef",
     "TaxDocumentsTypeDef",
     "ListLongTermPricingResultTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
-    "S3ResourceOutputTypeDef",
+    "PickupDetailsTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
     "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
-    "JobResourceOutputTypeDef",
     "JobResourceTypeDef",
     "DeviceConfigurationTypeDef",
     "ClusterMetadataTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "JobResourceUnionTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "CreateJobRequestRequestTypeDef",
     "JobMetadataTypeDef",
     "DescribeClusterResultTypeDef",
     "DescribeJobResultTypeDef",
 )
@@ -147,14 +147,15 @@
         "StateOrProvince": str,
         "PrefectureOrDistrict": str,
         "Landmark": str,
         "Country": str,
         "PostalCode": str,
         "PhoneNumber": str,
         "IsRestricted": bool,
+        "Type": AddressTypeType,
     },
     total=False,
 )
 
 CancelClusterRequestRequestTypeDef = TypedDict(
     "CancelClusterRequestRequestTypeDef",
     {
@@ -176,20 +177,21 @@
         "ClusterState": ClusterStateType,
         "CreationDate": datetime,
         "Description": str,
     },
     total=False,
 )
 
-NotificationOutputTypeDef = TypedDict(
-    "NotificationOutputTypeDef",
+NotificationTypeDef = TypedDict(
+    "NotificationTypeDef",
     {
         "SnsTopicARN": str,
-        "JobStatesToNotify": List[JobStateType],
+        "JobStatesToNotify": Sequence[JobStateType],
         "NotifyAll": bool,
+        "DevicePickupSnsTopicARN": str,
     },
     total=False,
 )
 
 CompatibleImageTypeDef = TypedDict(
     "CompatibleImageTypeDef",
     {
@@ -206,24 +208,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-NotificationTypeDef = TypedDict(
-    "NotificationTypeDef",
-    {
-        "SnsTopicARN": str,
-        "JobStatesToNotify": Sequence[JobStateType],
-        "NotifyAll": bool,
-    },
-    total=False,
-)
-
 JobListEntryTypeDef = TypedDict(
     "JobListEntryTypeDef",
     {
         "JobId": str,
         "JobState": JobStateType,
         "IsMaster": bool,
         "JobType": JobTypeType,
@@ -234,21 +226,21 @@
     total=False,
 )
 
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
+        "SnowballType": SnowballTypeType,
     },
 )
 _OptionalCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLongTermPricingRequestRequestTypeDef",
     {
         "IsLongTermPricingAutoRenew": bool,
-        "SnowballType": SnowballTypeType,
     },
     total=False,
 )
 
 
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
@@ -500,14 +492,23 @@
         "LongTermPricingStatus": str,
         "SnowballType": SnowballTypeType,
         "JobIds": List[str],
     },
     total=False,
 )
 
+ListPickupLocationsRequestRequestTypeDef = TypedDict(
+    "ListPickupLocationsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 NFSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "NFSOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
@@ -529,14 +530,15 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
     total=False,
@@ -703,15 +705,23 @@
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NotificationUnionTypeDef = Union[NotificationTypeDef, NotificationOutputTypeDef]
+ListPickupLocationsResultTypeDef = TypedDict(
+    "ListPickupLocationsResultTypeDef",
+    {
+        "Addresses": List[AddressTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "ClusterId": str,
         "JobListEntries": List[JobListEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -802,23 +812,14 @@
     "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-LambdaResourceOutputTypeDef = TypedDict(
-    "LambdaResourceOutputTypeDef",
-    {
-        "LambdaArn": str,
-        "EventTriggers": List[EventTriggerDefinitionTypeDef],
-    },
-    total=False,
-)
-
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": Sequence[EventTriggerDefinitionTypeDef],
     },
     total=False,
@@ -848,20 +849,24 @@
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
         "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
-S3ResourceOutputTypeDef = TypedDict(
-    "S3ResourceOutputTypeDef",
+PickupDetailsTypeDef = TypedDict(
+    "PickupDetailsTypeDef",
     {
-        "BucketArn": str,
-        "KeyRange": KeyRangeTypeDef,
-        "TargetOnDeviceServices": List[TargetOnDeviceServiceTypeDef],
+        "Name": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "IdentificationNumber": str,
+        "IdentificationExpirationDate": TimestampTypeDef,
+        "IdentificationIssuingOrg": str,
+        "DevicePickupId": str,
     },
     total=False,
 )
 
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
@@ -921,24 +926,14 @@
         "ServiceName": ServiceNameType,
         "DependentServices": List[DependentServiceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobResourceOutputTypeDef = TypedDict(
-    "JobResourceOutputTypeDef",
-    {
-        "S3Resources": List[S3ResourceOutputTypeDef],
-        "LambdaResources": List[LambdaResourceOutputTypeDef],
-        "Ec2AmiResources": List[Ec2AmiResourceTypeDef],
-    },
-    total=False,
-)
-
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
         "LambdaResources": Sequence[LambdaResourceTypeDef],
         "Ec2AmiResources": Sequence[Ec2AmiResourceTypeDef],
     },
@@ -960,18 +955,18 @@
         "Description": str,
         "KmsKeyARN": str,
         "RoleARN": str,
         "ClusterState": ClusterStateType,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
-        "Resources": JobResourceOutputTypeDef,
+        "Resources": JobResourceTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
-        "Notification": NotificationOutputTypeDef,
+        "Notification": NotificationTypeDef,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -1007,15 +1002,14 @@
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
 
-JobResourceUnionTypeDef = Union[JobResourceTypeDef, JobResourceOutputTypeDef]
 _RequiredUpdateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalUpdateClusterRequestRequestTypeDef = TypedDict(
@@ -1054,14 +1048,15 @@
         "Resources": JobResourceTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
         "Description": str,
         "SnowballCapacityPreference": SnowballCapacityType,
         "ForwardingAddressId": str,
+        "PickupDetails": PickupDetailsTypeDef,
     },
     total=False,
 )
 
 
 class UpdateJobRequestRequestTypeDef(
     _RequiredUpdateJobRequestRequestTypeDef, _OptionalUpdateJobRequestRequestTypeDef
@@ -1085,43 +1080,48 @@
         "ClusterId": str,
         "SnowballType": SnowballTypeType,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "DeviceConfiguration": DeviceConfigurationTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
+        "ImpactLevel": ImpactLevelType,
+        "PickupDetails": PickupDetailsTypeDef,
     },
     total=False,
 )
 
 JobMetadataTypeDef = TypedDict(
     "JobMetadataTypeDef",
     {
         "JobId": str,
         "JobState": JobStateType,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
-        "Resources": JobResourceOutputTypeDef,
+        "Resources": JobResourceTypeDef,
         "Description": str,
         "KmsKeyARN": str,
         "RoleARN": str,
         "AddressId": str,
         "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
-        "Notification": NotificationOutputTypeDef,
+        "Notification": NotificationTypeDef,
         "DataTransferProgress": DataTransferTypeDef,
         "JobLogInfo": JobLogsTypeDef,
         "ClusterId": str,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "DeviceConfiguration": DeviceConfigurationTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "ImpactLevel": ImpactLevelType,
+        "PickupDetails": PickupDetailsTypeDef,
+        "SnowballId": str,
     },
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
```

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball/type_defs.pyi` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,18 @@
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
+    AddressTypeType,
     ClusterStateType,
     DeviceServiceNameType,
+    ImpactLevelType,
     JobStateType,
     JobTypeType,
     LongTermPricingTypeType,
     RemoteManagementType,
     ServiceNameType,
     ShipmentStateType,
     ShippingLabelStatusType,
@@ -41,18 +43,17 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddressTypeDef",
     "CancelClusterRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ClusterListEntryTypeDef",
-    "NotificationOutputTypeDef",
+    "NotificationTypeDef",
     "CompatibleImageTypeDef",
     "ResponseMetadataTypeDef",
-    "NotificationTypeDef",
     "JobListEntryTypeDef",
     "CreateLongTermPricingRequestRequestTypeDef",
     "CreateReturnShippingLabelRequestRequestTypeDef",
     "DataTransferTypeDef",
     "ServiceVersionTypeDef",
     "DescribeAddressRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -71,17 +72,19 @@
     "KeyRangeTypeDef",
     "ListClusterJobsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListCompatibleImagesRequestRequestTypeDef",
     "ListJobsRequestRequestTypeDef",
     "ListLongTermPricingRequestRequestTypeDef",
     "LongTermPricingListEntryTypeDef",
+    "ListPickupLocationsRequestRequestTypeDef",
     "NFSOnDeviceServiceConfigurationTypeDef",
     "S3OnDeviceServiceConfigurationTypeDef",
     "TGWOnDeviceServiceConfigurationTypeDef",
+    "TimestampTypeDef",
     "TargetOnDeviceServiceTypeDef",
     "ShipmentTypeDef",
     "WirelessConnectionTypeDef",
     "UpdateJobShipmentStateRequestRequestTypeDef",
     "UpdateLongTermPricingRequestRequestTypeDef",
     "CreateAddressRequestRequestTypeDef",
     "CreateAddressResultTypeDef",
@@ -93,42 +96,39 @@
     "DescribeReturnShippingLabelResultTypeDef",
     "GetJobManifestResultTypeDef",
     "GetJobUnlockCodeResultTypeDef",
     "GetSnowballUsageResultTypeDef",
     "GetSoftwareUpdatesResultTypeDef",
     "ListClustersResultTypeDef",
     "ListCompatibleImagesResultTypeDef",
-    "NotificationUnionTypeDef",
+    "ListPickupLocationsResultTypeDef",
     "CreateClusterResultTypeDef",
     "ListClusterJobsResultTypeDef",
     "ListJobsResultTypeDef",
     "DependentServiceTypeDef",
     "DescribeAddressesRequestDescribeAddressesPaginateTypeDef",
     "ListClusterJobsRequestListClusterJobsPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
-    "LambdaResourceOutputTypeDef",
     "LambdaResourceTypeDef",
     "TaxDocumentsTypeDef",
     "ListLongTermPricingResultTypeDef",
     "OnDeviceServiceConfigurationTypeDef",
-    "S3ResourceOutputTypeDef",
+    "PickupDetailsTypeDef",
     "S3ResourceTypeDef",
     "ShippingDetailsTypeDef",
     "SnowconeDeviceConfigurationTypeDef",
     "ListServiceVersionsRequestRequestTypeDef",
     "ListServiceVersionsResultTypeDef",
-    "JobResourceOutputTypeDef",
     "JobResourceTypeDef",
     "DeviceConfigurationTypeDef",
     "ClusterMetadataTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "JobResourceUnionTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "CreateJobRequestRequestTypeDef",
     "JobMetadataTypeDef",
     "DescribeClusterResultTypeDef",
     "DescribeJobResultTypeDef",
 )
@@ -146,14 +146,15 @@
         "StateOrProvince": str,
         "PrefectureOrDistrict": str,
         "Landmark": str,
         "Country": str,
         "PostalCode": str,
         "PhoneNumber": str,
         "IsRestricted": bool,
+        "Type": AddressTypeType,
     },
     total=False,
 )
 
 CancelClusterRequestRequestTypeDef = TypedDict(
     "CancelClusterRequestRequestTypeDef",
     {
@@ -175,20 +176,21 @@
         "ClusterState": ClusterStateType,
         "CreationDate": datetime,
         "Description": str,
     },
     total=False,
 )
 
-NotificationOutputTypeDef = TypedDict(
-    "NotificationOutputTypeDef",
+NotificationTypeDef = TypedDict(
+    "NotificationTypeDef",
     {
         "SnsTopicARN": str,
-        "JobStatesToNotify": List[JobStateType],
+        "JobStatesToNotify": Sequence[JobStateType],
         "NotifyAll": bool,
+        "DevicePickupSnsTopicARN": str,
     },
     total=False,
 )
 
 CompatibleImageTypeDef = TypedDict(
     "CompatibleImageTypeDef",
     {
@@ -205,24 +207,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-NotificationTypeDef = TypedDict(
-    "NotificationTypeDef",
-    {
-        "SnsTopicARN": str,
-        "JobStatesToNotify": Sequence[JobStateType],
-        "NotifyAll": bool,
-    },
-    total=False,
-)
-
 JobListEntryTypeDef = TypedDict(
     "JobListEntryTypeDef",
     {
         "JobId": str,
         "JobState": JobStateType,
         "IsMaster": bool,
         "JobType": JobTypeType,
@@ -233,21 +225,21 @@
     total=False,
 )
 
 _RequiredCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLongTermPricingRequestRequestTypeDef",
     {
         "LongTermPricingType": LongTermPricingTypeType,
+        "SnowballType": SnowballTypeType,
     },
 )
 _OptionalCreateLongTermPricingRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLongTermPricingRequestRequestTypeDef",
     {
         "IsLongTermPricingAutoRenew": bool,
-        "SnowballType": SnowballTypeType,
     },
     total=False,
 )
 
 class CreateLongTermPricingRequestRequestTypeDef(
     _RequiredCreateLongTermPricingRequestRequestTypeDef,
     _OptionalCreateLongTermPricingRequestRequestTypeDef,
@@ -491,14 +483,23 @@
         "LongTermPricingStatus": str,
         "SnowballType": SnowballTypeType,
         "JobIds": List[str],
     },
     total=False,
 )
 
+ListPickupLocationsRequestRequestTypeDef = TypedDict(
+    "ListPickupLocationsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 NFSOnDeviceServiceConfigurationTypeDef = TypedDict(
     "NFSOnDeviceServiceConfigurationTypeDef",
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
@@ -520,14 +521,15 @@
     {
         "StorageLimit": int,
         "StorageUnit": Literal["TB"],
     },
     total=False,
 )
 
+TimestampTypeDef = Union[datetime, str]
 TargetOnDeviceServiceTypeDef = TypedDict(
     "TargetOnDeviceServiceTypeDef",
     {
         "ServiceName": DeviceServiceNameType,
         "TransferOption": TransferOptionType,
     },
     total=False,
@@ -692,15 +694,23 @@
     {
         "CompatibleImages": List[CompatibleImageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NotificationUnionTypeDef = Union[NotificationTypeDef, NotificationOutputTypeDef]
+ListPickupLocationsResultTypeDef = TypedDict(
+    "ListPickupLocationsResultTypeDef",
+    {
+        "Addresses": List[AddressTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateClusterResultTypeDef = TypedDict(
     "CreateClusterResultTypeDef",
     {
         "ClusterId": str,
         "JobListEntries": List[JobListEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -789,23 +799,14 @@
     "ListLongTermPricingRequestListLongTermPricingPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-LambdaResourceOutputTypeDef = TypedDict(
-    "LambdaResourceOutputTypeDef",
-    {
-        "LambdaArn": str,
-        "EventTriggers": List[EventTriggerDefinitionTypeDef],
-    },
-    total=False,
-)
-
 LambdaResourceTypeDef = TypedDict(
     "LambdaResourceTypeDef",
     {
         "LambdaArn": str,
         "EventTriggers": Sequence[EventTriggerDefinitionTypeDef],
     },
     total=False,
@@ -835,20 +836,24 @@
         "TGWOnDeviceService": TGWOnDeviceServiceConfigurationTypeDef,
         "EKSOnDeviceService": EKSOnDeviceServiceConfigurationTypeDef,
         "S3OnDeviceService": S3OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
-S3ResourceOutputTypeDef = TypedDict(
-    "S3ResourceOutputTypeDef",
+PickupDetailsTypeDef = TypedDict(
+    "PickupDetailsTypeDef",
     {
-        "BucketArn": str,
-        "KeyRange": KeyRangeTypeDef,
-        "TargetOnDeviceServices": List[TargetOnDeviceServiceTypeDef],
+        "Name": str,
+        "PhoneNumber": str,
+        "Email": str,
+        "IdentificationNumber": str,
+        "IdentificationExpirationDate": TimestampTypeDef,
+        "IdentificationIssuingOrg": str,
+        "DevicePickupId": str,
     },
     total=False,
 )
 
 S3ResourceTypeDef = TypedDict(
     "S3ResourceTypeDef",
     {
@@ -906,24 +911,14 @@
         "ServiceName": ServiceNameType,
         "DependentServices": List[DependentServiceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobResourceOutputTypeDef = TypedDict(
-    "JobResourceOutputTypeDef",
-    {
-        "S3Resources": List[S3ResourceOutputTypeDef],
-        "LambdaResources": List[LambdaResourceOutputTypeDef],
-        "Ec2AmiResources": List[Ec2AmiResourceTypeDef],
-    },
-    total=False,
-)
-
 JobResourceTypeDef = TypedDict(
     "JobResourceTypeDef",
     {
         "S3Resources": Sequence[S3ResourceTypeDef],
         "LambdaResources": Sequence[LambdaResourceTypeDef],
         "Ec2AmiResources": Sequence[Ec2AmiResourceTypeDef],
     },
@@ -945,18 +940,18 @@
         "Description": str,
         "KmsKeyARN": str,
         "RoleARN": str,
         "ClusterState": ClusterStateType,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
-        "Resources": JobResourceOutputTypeDef,
+        "Resources": JobResourceTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
-        "Notification": NotificationOutputTypeDef,
+        "Notification": NotificationTypeDef,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
     },
     total=False,
 )
 
@@ -990,15 +985,14 @@
 )
 
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-JobResourceUnionTypeDef = Union[JobResourceTypeDef, JobResourceOutputTypeDef]
 _RequiredUpdateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterRequestRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalUpdateClusterRequestRequestTypeDef = TypedDict(
@@ -1035,14 +1029,15 @@
         "Resources": JobResourceTypeDef,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
         "AddressId": str,
         "ShippingOption": ShippingOptionType,
         "Description": str,
         "SnowballCapacityPreference": SnowballCapacityType,
         "ForwardingAddressId": str,
+        "PickupDetails": PickupDetailsTypeDef,
     },
     total=False,
 )
 
 class UpdateJobRequestRequestTypeDef(
     _RequiredUpdateJobRequestRequestTypeDef, _OptionalUpdateJobRequestRequestTypeDef
 ):
@@ -1064,43 +1059,48 @@
         "ClusterId": str,
         "SnowballType": SnowballTypeType,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "DeviceConfiguration": DeviceConfigurationTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
+        "ImpactLevel": ImpactLevelType,
+        "PickupDetails": PickupDetailsTypeDef,
     },
     total=False,
 )
 
 JobMetadataTypeDef = TypedDict(
     "JobMetadataTypeDef",
     {
         "JobId": str,
         "JobState": JobStateType,
         "JobType": JobTypeType,
         "SnowballType": SnowballTypeType,
         "CreationDate": datetime,
-        "Resources": JobResourceOutputTypeDef,
+        "Resources": JobResourceTypeDef,
         "Description": str,
         "KmsKeyARN": str,
         "RoleARN": str,
         "AddressId": str,
         "ShippingDetails": ShippingDetailsTypeDef,
         "SnowballCapacityPreference": SnowballCapacityType,
-        "Notification": NotificationOutputTypeDef,
+        "Notification": NotificationTypeDef,
         "DataTransferProgress": DataTransferTypeDef,
         "JobLogInfo": JobLogsTypeDef,
         "ClusterId": str,
         "ForwardingAddressId": str,
         "TaxDocuments": TaxDocumentsTypeDef,
         "DeviceConfiguration": DeviceConfigurationTypeDef,
         "RemoteManagement": RemoteManagementType,
         "LongTermPricingId": str,
         "OnDeviceServiceConfiguration": OnDeviceServiceConfigurationTypeDef,
+        "ImpactLevel": ImpactLevelType,
+        "PickupDetails": PickupDetailsTypeDef,
+        "SnowballId": str,
     },
     total=False,
 )
 
 DescribeClusterResultTypeDef = TypedDict(
     "DescribeClusterResultTypeDef",
     {
```

### Comparing `types-aiobotocore-snowball-2.5.2.post1/types_aiobotocore_snowball.egg-info/SOURCES.txt` & `types-aiobotocore-snowball-2.5.2.post2/types_aiobotocore_snowball.egg-info/SOURCES.txt`

 * *Files identical despite different names*

