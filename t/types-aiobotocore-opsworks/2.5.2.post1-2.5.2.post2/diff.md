# Comparing `tmp/types-aiobotocore-opsworks-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-opsworks-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opsworks-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-opsworks-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-opsworks-2.5.2.post1.tar` & `types-aiobotocore-opsworks-2.5.2.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.285505 types-aiobotocore-opsworks-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:22.000000 types-aiobotocore-opsworks-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-08-02 14:52:45.285505 types-aiobotocore-opsworks-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22255 2023-08-02 14:44:22.000000 types-aiobotocore-opsworks-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:45.285505 types-aiobotocore-opsworks-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:44:22.000000 types-aiobotocore-opsworks-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.285505 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-08-02 14:44:22.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:44:22.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:44:22.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54819 2023-08-02 14:44:23.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54729 2023-08-02 14:44:23.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-08-02 14:44:23.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12438 2023-08-02 14:44:23.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-02 14:44:23.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-02 14:44:23.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:22.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21633 2023-08-02 14:44:23.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    21595 2023-08-02 14:44:23.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    66128 2023-08-02 14:44:27.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    66059 2023-08-02 14:44:26.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:22.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-08-02 14:44:23.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-08-02 14:44:23.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.285505 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-08-02 14:52:45.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-02 14:52:45.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:45.000000 types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.146643 types-aiobotocore-opsworks-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:05.000000 types-aiobotocore-opsworks-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16491 2023-08-04 13:59:20.146643 types-aiobotocore-opsworks-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14969 2023-08-04 13:46:05.000000 types-aiobotocore-opsworks-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.146643 types-aiobotocore-opsworks-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:46:05.000000 types-aiobotocore-opsworks-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.146643 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2029 2023-08-04 13:46:05.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2027 2023-08-04 13:46:05.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:46:05.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    54754 2023-08-04 13:46:06.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    54664 2023-08-04 13:46:06.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12535 2023-08-04 13:46:07.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12533 2023-08-04 13:46:06.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2149 2023-08-04 13:46:06.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2146 2023-08-04 13:46:06.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:05.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21733 2023-08-04 13:46:06.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21695 2023-08-04 13:46:06.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    64057 2023-08-04 13:46:10.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    63990 2023-08-04 13:46:09.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:05.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7021 2023-08-04 13:46:06.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7015 2023-08-04 13:46:06.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.146643 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16491 2023-08-04 13:59:20.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1002 2023-08-04 13:59:20.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:20.000000 types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/LICENSE` & `types-aiobotocore-opsworks-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/setup.py` & `types-aiobotocore-opsworks-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opsworks",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_opsworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.OpsWorks 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/__init__.py` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/__init__.pyi` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/__main__.py` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpsWorks 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.OpsWorks 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks\nOther"
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

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/client.py` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,27 @@
     AutoScalingTypeType,
     LayerAttributesKeysType,
     LayerTypeType,
     RootDeviceTypeType,
 )
 from .paginator import DescribeEcsClustersPaginator
 from .type_defs import (
-    AutoScalingThresholdsUnionTypeDef,
+    AutoScalingThresholdsTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationTypeDef,
     CloneStackResultTypeDef,
-    CloudWatchLogsConfigurationUnionTypeDef,
+    CloudWatchLogsConfigurationTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DataSourceTypeDef,
-    DeploymentCommandUnionTypeDef,
+    DeploymentCommandTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeCommandsResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
@@ -69,24 +69,24 @@
     EmptyResponseMetadataTypeDef,
     EnvironmentVariableTypeDef,
     GetHostnameSuggestionResultTypeDef,
     GrantAccessResultTypeDef,
     InstanceIdentityTypeDef,
     LifecycleEventConfigurationTypeDef,
     ListTagsResultTypeDef,
-    RecipesUnionTypeDef,
+    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceTypeDef,
     SslConfigurationTypeDef,
     StackConfigurationManagerTypeDef,
     VolumeConfigurationTypeDef,
-    WeeklyAutoScalingScheduleUnionTypeDef,
+    WeeklyAutoScalingScheduleTypeDef,
 )
 from .waiter import (
     AppExistsWaiter,
     DeploymentSuccessfulWaiter,
     InstanceOnlineWaiter,
     InstanceRegisteredWaiter,
     InstanceStoppedWaiter,
@@ -247,15 +247,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_app)
         """
 
     async def create_deployment(
         self,
         *,
         StackId: str,
-        Command: DeploymentCommandUnionTypeDef,
+        Command: DeploymentCommandTypeDef,
         AppId: str = ...,
         InstanceIds: Sequence[str] = ...,
         LayerIds: Sequence[str] = ...,
         Comment: str = ...,
         CustomJson: str = ...
     ) -> CreateDeploymentResultTypeDef:
         """
@@ -298,24 +298,24 @@
         self,
         *,
         StackId: str,
         Type: LayerTypeType,
         Name: str,
         Shortname: str,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesUnionTypeDef = ...,
+        CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> CreateLayerResultTypeDef:
         """
         Creates a layer.
 
@@ -809,16 +809,16 @@
         """
 
     async def set_load_based_auto_scaling(
         self,
         *,
         LayerId: str,
         Enable: bool = ...,
-        UpScaling: AutoScalingThresholdsUnionTypeDef = ...,
-        DownScaling: AutoScalingThresholdsUnionTypeDef = ...
+        UpScaling: AutoScalingThresholdsTypeDef = ...,
+        DownScaling: AutoScalingThresholdsTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the load-based auto scaling configuration for a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_load_based_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#set_load_based_auto_scaling)
         """
@@ -836,15 +836,15 @@
         Specifies a user's permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#set_permission)
         """
 
     async def set_time_based_auto_scaling(
-        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleUnionTypeDef = ...
+        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the time-based auto scaling configuration for a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_time_based_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#set_time_based_auto_scaling)
         """
@@ -977,24 +977,24 @@
     async def update_layer(
         self,
         *,
         LayerId: str,
         Name: str = ...,
         Shortname: str = ...,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesUnionTypeDef = ...,
+        CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified layer.
```

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/client.pyi` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,27 +27,27 @@
     AutoScalingTypeType,
     LayerAttributesKeysType,
     LayerTypeType,
     RootDeviceTypeType,
 )
 from .paginator import DescribeEcsClustersPaginator
 from .type_defs import (
-    AutoScalingThresholdsUnionTypeDef,
+    AutoScalingThresholdsTypeDef,
     BlockDeviceMappingTypeDef,
     ChefConfigurationTypeDef,
     CloneStackResultTypeDef,
-    CloudWatchLogsConfigurationUnionTypeDef,
+    CloudWatchLogsConfigurationTypeDef,
     CreateAppResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateInstanceResultTypeDef,
     CreateLayerResultTypeDef,
     CreateStackResultTypeDef,
     CreateUserProfileResultTypeDef,
     DataSourceTypeDef,
-    DeploymentCommandUnionTypeDef,
+    DeploymentCommandTypeDef,
     DescribeAgentVersionsResultTypeDef,
     DescribeAppsResultTypeDef,
     DescribeCommandsResultTypeDef,
     DescribeDeploymentsResultTypeDef,
     DescribeEcsClustersResultTypeDef,
     DescribeElasticIpsResultTypeDef,
     DescribeElasticLoadBalancersResultTypeDef,
@@ -69,24 +69,24 @@
     EmptyResponseMetadataTypeDef,
     EnvironmentVariableTypeDef,
     GetHostnameSuggestionResultTypeDef,
     GrantAccessResultTypeDef,
     InstanceIdentityTypeDef,
     LifecycleEventConfigurationTypeDef,
     ListTagsResultTypeDef,
-    RecipesUnionTypeDef,
+    RecipesTypeDef,
     RegisterEcsClusterResultTypeDef,
     RegisterElasticIpResultTypeDef,
     RegisterInstanceResultTypeDef,
     RegisterVolumeResultTypeDef,
     SourceTypeDef,
     SslConfigurationTypeDef,
     StackConfigurationManagerTypeDef,
     VolumeConfigurationTypeDef,
-    WeeklyAutoScalingScheduleUnionTypeDef,
+    WeeklyAutoScalingScheduleTypeDef,
 )
 from .waiter import (
     AppExistsWaiter,
     DeploymentSuccessfulWaiter,
     InstanceOnlineWaiter,
     InstanceRegisteredWaiter,
     InstanceStoppedWaiter,
@@ -234,15 +234,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#create_app)
         """
     async def create_deployment(
         self,
         *,
         StackId: str,
-        Command: DeploymentCommandUnionTypeDef,
+        Command: DeploymentCommandTypeDef,
         AppId: str = ...,
         InstanceIds: Sequence[str] = ...,
         LayerIds: Sequence[str] = ...,
         Comment: str = ...,
         CustomJson: str = ...
     ) -> CreateDeploymentResultTypeDef:
         """
@@ -283,24 +283,24 @@
         self,
         *,
         StackId: str,
         Type: LayerTypeType,
         Name: str,
         Shortname: str,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesUnionTypeDef = ...,
+        CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> CreateLayerResultTypeDef:
         """
         Creates a layer.
 
@@ -747,16 +747,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#register_volume)
         """
     async def set_load_based_auto_scaling(
         self,
         *,
         LayerId: str,
         Enable: bool = ...,
-        UpScaling: AutoScalingThresholdsUnionTypeDef = ...,
-        DownScaling: AutoScalingThresholdsUnionTypeDef = ...
+        UpScaling: AutoScalingThresholdsTypeDef = ...,
+        DownScaling: AutoScalingThresholdsTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the load-based auto scaling configuration for a specified layer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_load_based_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#set_load_based_auto_scaling)
         """
@@ -772,15 +772,15 @@
         """
         Specifies a user's permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#set_permission)
         """
     async def set_time_based_auto_scaling(
-        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleUnionTypeDef = ...
+        self, *, InstanceId: str, AutoScalingSchedule: WeeklyAutoScalingScheduleTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Specify the time-based auto scaling configuration for a specified instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client.set_time_based_auto_scaling)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworks/client/#set_time_based_auto_scaling)
         """
@@ -901,24 +901,24 @@
     async def update_layer(
         self,
         *,
         LayerId: str,
         Name: str = ...,
         Shortname: str = ...,
         Attributes: Mapping[LayerAttributesKeysType, str] = ...,
-        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationUnionTypeDef = ...,
+        CloudWatchLogsConfiguration: CloudWatchLogsConfigurationTypeDef = ...,
         CustomInstanceProfileArn: str = ...,
         CustomJson: str = ...,
         CustomSecurityGroupIds: Sequence[str] = ...,
         Packages: Sequence[str] = ...,
         VolumeConfigurations: Sequence[VolumeConfigurationTypeDef] = ...,
         EnableAutoHealing: bool = ...,
         AutoAssignElasticIps: bool = ...,
         AutoAssignPublicIps: bool = ...,
-        CustomRecipes: RecipesUnionTypeDef = ...,
+        CustomRecipes: RecipesTypeDef = ...,
         InstallUpdatesOnBoot: bool = ...,
         UseEbsOptimizedInstances: bool = ...,
         LifecycleEventConfiguration: LifecycleEventConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a specified layer.
```

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/literals.py` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,14 +232,15 @@
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
@@ -335,14 +336,15 @@
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
@@ -421,26 +423,28 @@
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

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/literals.pyi` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,15 @@
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
@@ -333,14 +334,15 @@
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
@@ -419,26 +421,28 @@
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

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/paginator.py` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/paginator.pyi` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/service_resource.py` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 from typing import AsyncIterator, Awaitable, Dict, List, Mapping, NoReturn, Sequence
 
 from .client import OpsWorksClient
 from .literals import LayerAttributesKeysType, LayerTypeType, RootDeviceTypeType
 from .type_defs import (
     ChefConfigurationResponseTypeDef,
     ChefConfigurationTypeDef,
+    CloudWatchLogsConfigurationResponseTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     InstancesCountResponseTypeDef,
     LifecycleEventConfigurationResponseTypeDef,
     LifecycleEventConfigurationTypeDef,
+    RecipesResponseTypeDef,
     RecipesTypeDef,
     SourceResponseTypeDef,
     SourceTypeDef,
     StackConfigurationManagerResponseTypeDef,
     StackConfigurationManagerTypeDef,
     VolumeConfigurationTypeDef,
 )
@@ -181,26 +183,26 @@
     arn: Awaitable[str]
     stack_id: Awaitable[str]
     layer_id: Awaitable[str]
     type: Awaitable[LayerTypeType]
     name: Awaitable[str]
     shortname: Awaitable[str]
     attributes: Awaitable[Dict[LayerAttributesKeysType, str]]
-    cloud_watch_logs_configuration: Awaitable[CloudWatchLogsConfigurationTypeDef]
+    cloud_watch_logs_configuration: Awaitable[CloudWatchLogsConfigurationResponseTypeDef]
     custom_instance_profile_arn: Awaitable[str]
     custom_json: Awaitable[str]
     custom_security_group_ids: Awaitable[List[str]]
     default_security_group_names: Awaitable[List[str]]
     packages: Awaitable[List[str]]
     volume_configurations: Awaitable[List[VolumeConfigurationTypeDef]]
     enable_auto_healing: Awaitable[bool]
     auto_assign_elastic_ips: Awaitable[bool]
     auto_assign_public_ips: Awaitable[bool]
-    default_recipes: Awaitable[RecipesTypeDef]
-    custom_recipes: Awaitable[RecipesTypeDef]
+    default_recipes: Awaitable[RecipesResponseTypeDef]
+    custom_recipes: Awaitable[RecipesResponseTypeDef]
     created_at: Awaitable[str]
     install_updates_on_boot: Awaitable[bool]
     use_ebs_optimized_instances: Awaitable[bool]
     lifecycle_event_configuration: Awaitable[LifecycleEventConfigurationResponseTypeDef]
     id: str
     stack: "Stack"
```

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/service_resource.pyi` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 from typing import AsyncIterator, Awaitable, Dict, List, Mapping, NoReturn, Sequence
 
 from .client import OpsWorksClient
 from .literals import LayerAttributesKeysType, LayerTypeType, RootDeviceTypeType
 from .type_defs import (
     ChefConfigurationResponseTypeDef,
     ChefConfigurationTypeDef,
+    CloudWatchLogsConfigurationResponseTypeDef,
     CloudWatchLogsConfigurationTypeDef,
     InstancesCountResponseTypeDef,
     LifecycleEventConfigurationResponseTypeDef,
     LifecycleEventConfigurationTypeDef,
+    RecipesResponseTypeDef,
     RecipesTypeDef,
     SourceResponseTypeDef,
     SourceTypeDef,
     StackConfigurationManagerResponseTypeDef,
     StackConfigurationManagerTypeDef,
     VolumeConfigurationTypeDef,
 )
@@ -165,26 +167,26 @@
     arn: Awaitable[str]
     stack_id: Awaitable[str]
     layer_id: Awaitable[str]
     type: Awaitable[LayerTypeType]
     name: Awaitable[str]
     shortname: Awaitable[str]
     attributes: Awaitable[Dict[LayerAttributesKeysType, str]]
-    cloud_watch_logs_configuration: Awaitable[CloudWatchLogsConfigurationTypeDef]
+    cloud_watch_logs_configuration: Awaitable[CloudWatchLogsConfigurationResponseTypeDef]
     custom_instance_profile_arn: Awaitable[str]
     custom_json: Awaitable[str]
     custom_security_group_ids: Awaitable[List[str]]
     default_security_group_names: Awaitable[List[str]]
     packages: Awaitable[List[str]]
     volume_configurations: Awaitable[List[VolumeConfigurationTypeDef]]
     enable_auto_healing: Awaitable[bool]
     auto_assign_elastic_ips: Awaitable[bool]
     auto_assign_public_ips: Awaitable[bool]
-    default_recipes: Awaitable[RecipesTypeDef]
-    custom_recipes: Awaitable[RecipesTypeDef]
+    default_recipes: Awaitable[RecipesResponseTypeDef]
+    custom_recipes: Awaitable[RecipesResponseTypeDef]
     created_at: Awaitable[str]
     install_updates_on_boot: Awaitable[bool]
     use_ebs_optimized_instances: Awaitable[bool]
     lifecycle_event_configuration: Awaitable[LifecycleEventConfigurationResponseTypeDef]
     id: str
     stack: "Stack"
```

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/type_defs.py` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_opsworks.type_defs import StackConfigurationManagerTypeDef
 
     data: StackConfigurationManagerTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AppAttributesKeysType,
     AppTypeType,
     ArchitectureType,
     AutoScalingTypeType,
     CloudWatchLogsEncodingType,
@@ -47,15 +47,14 @@
     "EnvironmentVariableTypeDef",
     "SourceTypeDef",
     "SslConfigurationTypeDef",
     "AssignInstanceRequestRequestTypeDef",
     "AssignVolumeRequestRequestTypeDef",
     "AssociateElasticIpRequestRequestTypeDef",
     "AttachElasticLoadBalancerRequestRequestTypeDef",
-    "AutoScalingThresholdsOutputTypeDef",
     "AutoScalingThresholdsTypeDef",
     "EbsBlockDeviceTypeDef",
     "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
     "DeploymentCommandTypeDef",
@@ -63,15 +62,14 @@
     "VolumeConfigurationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
-    "DeploymentCommandOutputTypeDef",
     "DeregisterEcsClusterRequestRequestTypeDef",
     "DeregisterElasticIpRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
     "DeregisterRdsDbInstanceRequestRequestTypeDef",
     "DeregisterVolumeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAppsRequestRequestTypeDef",
@@ -108,15 +106,14 @@
     "DisassociateElasticIpRequestRequestTypeDef",
     "GetHostnameSuggestionRequestRequestTypeDef",
     "GrantAccessRequestRequestTypeDef",
     "TemporaryCredentialTypeDef",
     "InstanceIdentityTypeDef",
     "ReportedOsTypeDef",
     "InstancesCountTypeDef",
-    "RecipesOutputTypeDef",
     "ShutdownEventConfigurationTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OperatingSystemConfigurationManagerTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RegisterEcsClusterRequestRequestTypeDef",
     "RegisterElasticIpRequestRequestTypeDef",
     "RegisterRdsDbInstanceRequestRequestTypeDef",
@@ -124,15 +121,14 @@
     "SetPermissionRequestRequestTypeDef",
     "WeeklyAutoScalingScheduleTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartStackRequestRequestTypeDef",
     "StopInstanceRequestRequestTypeDef",
     "StopStackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "WeeklyAutoScalingScheduleOutputTypeDef",
     "UnassignInstanceRequestRequestTypeDef",
     "UnassignVolumeRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateElasticIpRequestRequestTypeDef",
     "UpdateInstanceRequestRequestTypeDef",
     "UpdateMyUserProfileRequestRequestTypeDef",
     "UpdateRdsDbInstanceRequestRequestTypeDef",
@@ -140,15 +136,14 @@
     "UpdateVolumeRequestRequestTypeDef",
     "AgentVersionTypeDef",
     "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
-    "AutoScalingThresholdsUnionTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "ChefConfigurationResponseTypeDef",
     "CloneStackResultTypeDef",
     "CreateAppResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "CreateInstanceResultTypeDef",
@@ -156,30 +151,30 @@
     "CreateStackResultTypeDef",
     "CreateUserProfileResultTypeDef",
     "DescribeStackProvisioningParametersResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionResultTypeDef",
     "InstancesCountResponseTypeDef",
     "ListTagsResultTypeDef",
+    "RecipesResponseTypeDef",
     "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpResultTypeDef",
     "RegisterInstanceResultTypeDef",
     "RegisterVolumeResultTypeDef",
     "SourceResponseTypeDef",
     "StackConfigurationManagerResponseTypeDef",
     "CloneStackRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "CreateStackRequestServiceResourceCreateStackTypeDef",
     "StackTypeDef",
     "UpdateStackRequestRequestTypeDef",
-    "CloudWatchLogsConfigurationOutputTypeDef",
+    "CloudWatchLogsConfigurationResponseTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
     "DescribeCommandsResultTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "DeploymentCommandUnionTypeDef",
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
     "DescribeInstancesRequestInstanceTerminatedWaitTypeDef",
@@ -193,28 +188,25 @@
     "DescribeRdsDbInstancesResultTypeDef",
     "DescribeServiceErrorsResultTypeDef",
     "DescribeUserProfilesResultTypeDef",
     "DescribeVolumesResultTypeDef",
     "GrantAccessResultTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
     "StackSummaryTypeDef",
-    "RecipesUnionTypeDef",
     "LifecycleEventConfigurationResponseTypeDef",
     "LifecycleEventConfigurationTypeDef",
     "OperatingSystemTypeDef",
     "SetTimeBasedAutoScalingRequestRequestTypeDef",
     "TimeBasedAutoScalingConfigurationTypeDef",
-    "WeeklyAutoScalingScheduleUnionTypeDef",
     "DescribeAgentVersionsResultTypeDef",
     "DescribeAppsResultTypeDef",
     "DescribeLoadBasedAutoScalingResultTypeDef",
     "CreateInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "DescribeStacksResultTypeDef",
-    "CloudWatchLogsConfigurationUnionTypeDef",
     "DescribeDeploymentsResultTypeDef",
     "DescribeStackSummaryResultTypeDef",
     "CreateLayerRequestRequestTypeDef",
     "CreateLayerRequestStackCreateLayerTypeDef",
     "LayerTypeDef",
     "UpdateLayerRequestRequestTypeDef",
     "DescribeOperatingSystemsResponseTypeDef",
@@ -352,38 +344,24 @@
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     {
         "ElasticLoadBalancerName": str,
         "LayerId": str,
     },
 )
 
-AutoScalingThresholdsOutputTypeDef = TypedDict(
-    "AutoScalingThresholdsOutputTypeDef",
-    {
-        "InstanceCount": int,
-        "ThresholdsWaitTime": int,
-        "IgnoreMetricsTime": int,
-        "CpuThreshold": float,
-        "MemoryThreshold": float,
-        "LoadThreshold": float,
-        "Alarms": List[str],
-    },
-    total=False,
-)
-
 AutoScalingThresholdsTypeDef = TypedDict(
     "AutoScalingThresholdsTypeDef",
     {
         "InstanceCount": int,
         "ThresholdsWaitTime": int,
         "IgnoreMetricsTime": int,
         "CpuThreshold": float,
         "MemoryThreshold": float,
         "LoadThreshold": float,
-        "Alarms": Sequence[str],
+        "Alarms": List[str],
     },
     total=False,
 )
 
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
@@ -579,35 +557,14 @@
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
 
-_RequiredDeploymentCommandOutputTypeDef = TypedDict(
-    "_RequiredDeploymentCommandOutputTypeDef",
-    {
-        "Name": DeploymentCommandNameType,
-    },
-)
-_OptionalDeploymentCommandOutputTypeDef = TypedDict(
-    "_OptionalDeploymentCommandOutputTypeDef",
-    {
-        "Args": Dict[str, List[str]],
-    },
-    total=False,
-)
-
-
-class DeploymentCommandOutputTypeDef(
-    _RequiredDeploymentCommandOutputTypeDef, _OptionalDeploymentCommandOutputTypeDef
-):
-    pass
-
-
 DeregisterEcsClusterRequestRequestTypeDef = TypedDict(
     "DeregisterEcsClusterRequestRequestTypeDef",
     {
         "EcsClusterArn": str,
     },
 )
 
@@ -1082,26 +1039,14 @@
         "Terminated": int,
         "Terminating": int,
         "Unassigning": int,
     },
     total=False,
 )
 
-RecipesOutputTypeDef = TypedDict(
-    "RecipesOutputTypeDef",
-    {
-        "Setup": List[str],
-        "Configure": List[str],
-        "Deploy": List[str],
-        "Undeploy": List[str],
-        "Shutdown": List[str],
-    },
-    total=False,
-)
-
 ShutdownEventConfigurationTypeDef = TypedDict(
     "ShutdownEventConfigurationTypeDef",
     {
         "ExecutionTimeout": int,
         "DelayUntilElbConnectionsDrained": bool,
     },
     total=False,
@@ -1215,21 +1160,21 @@
 ):
     pass
 
 
 WeeklyAutoScalingScheduleTypeDef = TypedDict(
     "WeeklyAutoScalingScheduleTypeDef",
     {
-        "Monday": Mapping[str, str],
-        "Tuesday": Mapping[str, str],
-        "Wednesday": Mapping[str, str],
-        "Thursday": Mapping[str, str],
-        "Friday": Mapping[str, str],
-        "Saturday": Mapping[str, str],
-        "Sunday": Mapping[str, str],
+        "Monday": Dict[str, str],
+        "Tuesday": Dict[str, str],
+        "Wednesday": Dict[str, str],
+        "Thursday": Dict[str, str],
+        "Friday": Dict[str, str],
+        "Saturday": Dict[str, str],
+        "Sunday": Dict[str, str],
     },
     total=False,
 )
 
 StartInstanceRequestRequestTypeDef = TypedDict(
     "StartInstanceRequestRequestTypeDef",
     {
@@ -1276,28 +1221,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
 
-WeeklyAutoScalingScheduleOutputTypeDef = TypedDict(
-    "WeeklyAutoScalingScheduleOutputTypeDef",
-    {
-        "Monday": Dict[str, str],
-        "Tuesday": Dict[str, str],
-        "Wednesday": Dict[str, str],
-        "Thursday": Dict[str, str],
-        "Friday": Dict[str, str],
-        "Saturday": Dict[str, str],
-        "Sunday": Dict[str, str],
-    },
-    total=False,
-)
-
 UnassignInstanceRequestRequestTypeDef = TypedDict(
     "UnassignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
@@ -1545,23 +1476,20 @@
 
 
 LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
     "LoadBasedAutoScalingConfigurationTypeDef",
     {
         "LayerId": str,
         "Enable": bool,
-        "UpScaling": AutoScalingThresholdsOutputTypeDef,
-        "DownScaling": AutoScalingThresholdsOutputTypeDef,
+        "UpScaling": AutoScalingThresholdsTypeDef,
+        "DownScaling": AutoScalingThresholdsTypeDef,
     },
     total=False,
 )
 
-AutoScalingThresholdsUnionTypeDef = Union[
-    AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef
-]
 _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
     "_RequiredSetLoadBasedAutoScalingRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
@@ -1715,14 +1643,26 @@
     {
         "Tags": Dict[str, str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RecipesResponseTypeDef = TypedDict(
+    "RecipesResponseTypeDef",
+    {
+        "Setup": List[str],
+        "Configure": List[str],
+        "Deploy": List[str],
+        "Undeploy": List[str],
+        "Shutdown": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RegisterEcsClusterResultTypeDef = TypedDict(
     "RegisterEcsClusterResultTypeDef",
     {
         "EcsClusterArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1953,30 +1893,30 @@
 
 class UpdateStackRequestRequestTypeDef(
     _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
 ):
     pass
 
 
-CloudWatchLogsConfigurationOutputTypeDef = TypedDict(
-    "CloudWatchLogsConfigurationOutputTypeDef",
+CloudWatchLogsConfigurationResponseTypeDef = TypedDict(
+    "CloudWatchLogsConfigurationResponseTypeDef",
     {
         "Enabled": bool,
         "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
-        "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LogStreams": Sequence[CloudWatchLogsLogStreamTypeDef],
     },
+    total=False,
 )
 
 DescribeCommandsResultTypeDef = TypedDict(
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2005,27 +1945,26 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-DeploymentCommandUnionTypeDef = Union[DeploymentCommandTypeDef, DeploymentCommandOutputTypeDef]
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "DeploymentId": str,
         "StackId": str,
         "AppId": str,
         "CreatedAt": str,
         "CompletedAt": str,
         "Duration": int,
         "IamUserArn": str,
         "Comment": str,
-        "Command": DeploymentCommandOutputTypeDef,
+        "Command": DeploymentCommandTypeDef,
         "Status": str,
         "CustomJson": str,
         "InstanceIds": List[str],
     },
     total=False,
 )
 
@@ -2228,15 +2167,14 @@
         "LayersCount": int,
         "AppsCount": int,
         "InstancesCount": InstancesCountTypeDef,
     },
     total=False,
 )
 
-RecipesUnionTypeDef = Union[RecipesTypeDef, RecipesOutputTypeDef]
 LifecycleEventConfigurationResponseTypeDef = TypedDict(
     "LifecycleEventConfigurationResponseTypeDef",
     {
         "Shutdown": ShutdownEventConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2285,22 +2223,19 @@
     pass
 
 
 TimeBasedAutoScalingConfigurationTypeDef = TypedDict(
     "TimeBasedAutoScalingConfigurationTypeDef",
     {
         "InstanceId": str,
-        "AutoScalingSchedule": WeeklyAutoScalingScheduleOutputTypeDef,
+        "AutoScalingSchedule": WeeklyAutoScalingScheduleTypeDef,
     },
     total=False,
 )
 
-WeeklyAutoScalingScheduleUnionTypeDef = Union[
-    WeeklyAutoScalingScheduleTypeDef, WeeklyAutoScalingScheduleOutputTypeDef
-]
 DescribeAgentVersionsResultTypeDef = TypedDict(
     "DescribeAgentVersionsResultTypeDef",
     {
         "AgentVersions": List[AgentVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2410,17 +2345,14 @@
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CloudWatchLogsConfigurationUnionTypeDef = Union[
-    CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
-]
 DescribeDeploymentsResultTypeDef = TypedDict(
     "DescribeDeploymentsResultTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2513,26 +2445,26 @@
         "Arn": str,
         "StackId": str,
         "LayerId": str,
         "Type": LayerTypeType,
         "Name": str,
         "Shortname": str,
         "Attributes": Dict[LayerAttributesKeysType, str],
-        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationOutputTypeDef,
+        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationTypeDef,
         "CustomInstanceProfileArn": str,
         "CustomJson": str,
         "CustomSecurityGroupIds": List[str],
         "DefaultSecurityGroupNames": List[str],
         "Packages": List[str],
         "VolumeConfigurations": List[VolumeConfigurationTypeDef],
         "EnableAutoHealing": bool,
         "AutoAssignElasticIps": bool,
         "AutoAssignPublicIps": bool,
-        "DefaultRecipes": RecipesOutputTypeDef,
-        "CustomRecipes": RecipesOutputTypeDef,
+        "DefaultRecipes": RecipesTypeDef,
+        "CustomRecipes": RecipesTypeDef,
         "CreatedAt": str,
         "InstallUpdatesOnBoot": bool,
         "UseEbsOptimizedInstances": bool,
         "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/type_defs.pyi` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_opsworks.type_defs import StackConfigurationManagerTypeDef
 
     data: StackConfigurationManagerTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AppAttributesKeysType,
     AppTypeType,
     ArchitectureType,
     AutoScalingTypeType,
     CloudWatchLogsEncodingType,
@@ -46,15 +46,14 @@
     "EnvironmentVariableTypeDef",
     "SourceTypeDef",
     "SslConfigurationTypeDef",
     "AssignInstanceRequestRequestTypeDef",
     "AssignVolumeRequestRequestTypeDef",
     "AssociateElasticIpRequestRequestTypeDef",
     "AttachElasticLoadBalancerRequestRequestTypeDef",
-    "AutoScalingThresholdsOutputTypeDef",
     "AutoScalingThresholdsTypeDef",
     "EbsBlockDeviceTypeDef",
     "ResponseMetadataTypeDef",
     "ChefConfigurationTypeDef",
     "CloudWatchLogsLogStreamTypeDef",
     "CommandTypeDef",
     "DeploymentCommandTypeDef",
@@ -62,15 +61,14 @@
     "VolumeConfigurationTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteInstanceRequestRequestTypeDef",
     "DeleteLayerRequestRequestTypeDef",
     "DeleteStackRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
-    "DeploymentCommandOutputTypeDef",
     "DeregisterEcsClusterRequestRequestTypeDef",
     "DeregisterElasticIpRequestRequestTypeDef",
     "DeregisterInstanceRequestRequestTypeDef",
     "DeregisterRdsDbInstanceRequestRequestTypeDef",
     "DeregisterVolumeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeAppsRequestRequestTypeDef",
@@ -107,15 +105,14 @@
     "DisassociateElasticIpRequestRequestTypeDef",
     "GetHostnameSuggestionRequestRequestTypeDef",
     "GrantAccessRequestRequestTypeDef",
     "TemporaryCredentialTypeDef",
     "InstanceIdentityTypeDef",
     "ReportedOsTypeDef",
     "InstancesCountTypeDef",
-    "RecipesOutputTypeDef",
     "ShutdownEventConfigurationTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OperatingSystemConfigurationManagerTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RegisterEcsClusterRequestRequestTypeDef",
     "RegisterElasticIpRequestRequestTypeDef",
     "RegisterRdsDbInstanceRequestRequestTypeDef",
@@ -123,15 +120,14 @@
     "SetPermissionRequestRequestTypeDef",
     "WeeklyAutoScalingScheduleTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartStackRequestRequestTypeDef",
     "StopInstanceRequestRequestTypeDef",
     "StopStackRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "WeeklyAutoScalingScheduleOutputTypeDef",
     "UnassignInstanceRequestRequestTypeDef",
     "UnassignVolumeRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateElasticIpRequestRequestTypeDef",
     "UpdateInstanceRequestRequestTypeDef",
     "UpdateMyUserProfileRequestRequestTypeDef",
     "UpdateRdsDbInstanceRequestRequestTypeDef",
@@ -139,15 +135,14 @@
     "UpdateVolumeRequestRequestTypeDef",
     "AgentVersionTypeDef",
     "DescribeAgentVersionsRequestRequestTypeDef",
     "AppTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
     "LoadBasedAutoScalingConfigurationTypeDef",
-    "AutoScalingThresholdsUnionTypeDef",
     "SetLoadBasedAutoScalingRequestRequestTypeDef",
     "BlockDeviceMappingTypeDef",
     "ChefConfigurationResponseTypeDef",
     "CloneStackResultTypeDef",
     "CreateAppResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "CreateInstanceResultTypeDef",
@@ -155,30 +150,30 @@
     "CreateStackResultTypeDef",
     "CreateUserProfileResultTypeDef",
     "DescribeStackProvisioningParametersResultTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetHostnameSuggestionResultTypeDef",
     "InstancesCountResponseTypeDef",
     "ListTagsResultTypeDef",
+    "RecipesResponseTypeDef",
     "RegisterEcsClusterResultTypeDef",
     "RegisterElasticIpResultTypeDef",
     "RegisterInstanceResultTypeDef",
     "RegisterVolumeResultTypeDef",
     "SourceResponseTypeDef",
     "StackConfigurationManagerResponseTypeDef",
     "CloneStackRequestRequestTypeDef",
     "CreateStackRequestRequestTypeDef",
     "CreateStackRequestServiceResourceCreateStackTypeDef",
     "StackTypeDef",
     "UpdateStackRequestRequestTypeDef",
-    "CloudWatchLogsConfigurationOutputTypeDef",
+    "CloudWatchLogsConfigurationResponseTypeDef",
     "CloudWatchLogsConfigurationTypeDef",
     "DescribeCommandsResultTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "DeploymentCommandUnionTypeDef",
     "DeploymentTypeDef",
     "DescribeAppsRequestAppExistsWaitTypeDef",
     "DescribeDeploymentsRequestDeploymentSuccessfulWaitTypeDef",
     "DescribeInstancesRequestInstanceOnlineWaitTypeDef",
     "DescribeInstancesRequestInstanceRegisteredWaitTypeDef",
     "DescribeInstancesRequestInstanceStoppedWaitTypeDef",
     "DescribeInstancesRequestInstanceTerminatedWaitTypeDef",
@@ -192,28 +187,25 @@
     "DescribeRdsDbInstancesResultTypeDef",
     "DescribeServiceErrorsResultTypeDef",
     "DescribeUserProfilesResultTypeDef",
     "DescribeVolumesResultTypeDef",
     "GrantAccessResultTypeDef",
     "RegisterInstanceRequestRequestTypeDef",
     "StackSummaryTypeDef",
-    "RecipesUnionTypeDef",
     "LifecycleEventConfigurationResponseTypeDef",
     "LifecycleEventConfigurationTypeDef",
     "OperatingSystemTypeDef",
     "SetTimeBasedAutoScalingRequestRequestTypeDef",
     "TimeBasedAutoScalingConfigurationTypeDef",
-    "WeeklyAutoScalingScheduleUnionTypeDef",
     "DescribeAgentVersionsResultTypeDef",
     "DescribeAppsResultTypeDef",
     "DescribeLoadBasedAutoScalingResultTypeDef",
     "CreateInstanceRequestRequestTypeDef",
     "InstanceTypeDef",
     "DescribeStacksResultTypeDef",
-    "CloudWatchLogsConfigurationUnionTypeDef",
     "DescribeDeploymentsResultTypeDef",
     "DescribeStackSummaryResultTypeDef",
     "CreateLayerRequestRequestTypeDef",
     "CreateLayerRequestStackCreateLayerTypeDef",
     "LayerTypeDef",
     "UpdateLayerRequestRequestTypeDef",
     "DescribeOperatingSystemsResponseTypeDef",
@@ -343,38 +335,24 @@
     "AttachElasticLoadBalancerRequestRequestTypeDef",
     {
         "ElasticLoadBalancerName": str,
         "LayerId": str,
     },
 )
 
-AutoScalingThresholdsOutputTypeDef = TypedDict(
-    "AutoScalingThresholdsOutputTypeDef",
-    {
-        "InstanceCount": int,
-        "ThresholdsWaitTime": int,
-        "IgnoreMetricsTime": int,
-        "CpuThreshold": float,
-        "MemoryThreshold": float,
-        "LoadThreshold": float,
-        "Alarms": List[str],
-    },
-    total=False,
-)
-
 AutoScalingThresholdsTypeDef = TypedDict(
     "AutoScalingThresholdsTypeDef",
     {
         "InstanceCount": int,
         "ThresholdsWaitTime": int,
         "IgnoreMetricsTime": int,
         "CpuThreshold": float,
         "MemoryThreshold": float,
         "LoadThreshold": float,
-        "Alarms": Sequence[str],
+        "Alarms": List[str],
     },
     total=False,
 )
 
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
@@ -562,33 +540,14 @@
 DeleteUserProfileRequestRequestTypeDef = TypedDict(
     "DeleteUserProfileRequestRequestTypeDef",
     {
         "IamUserArn": str,
     },
 )
 
-_RequiredDeploymentCommandOutputTypeDef = TypedDict(
-    "_RequiredDeploymentCommandOutputTypeDef",
-    {
-        "Name": DeploymentCommandNameType,
-    },
-)
-_OptionalDeploymentCommandOutputTypeDef = TypedDict(
-    "_OptionalDeploymentCommandOutputTypeDef",
-    {
-        "Args": Dict[str, List[str]],
-    },
-    total=False,
-)
-
-class DeploymentCommandOutputTypeDef(
-    _RequiredDeploymentCommandOutputTypeDef, _OptionalDeploymentCommandOutputTypeDef
-):
-    pass
-
 DeregisterEcsClusterRequestRequestTypeDef = TypedDict(
     "DeregisterEcsClusterRequestRequestTypeDef",
     {
         "EcsClusterArn": str,
     },
 )
 
@@ -1059,26 +1018,14 @@
         "Terminated": int,
         "Terminating": int,
         "Unassigning": int,
     },
     total=False,
 )
 
-RecipesOutputTypeDef = TypedDict(
-    "RecipesOutputTypeDef",
-    {
-        "Setup": List[str],
-        "Configure": List[str],
-        "Deploy": List[str],
-        "Undeploy": List[str],
-        "Shutdown": List[str],
-    },
-    total=False,
-)
-
 ShutdownEventConfigurationTypeDef = TypedDict(
     "ShutdownEventConfigurationTypeDef",
     {
         "ExecutionTimeout": int,
         "DelayUntilElbConnectionsDrained": bool,
     },
     total=False,
@@ -1186,21 +1133,21 @@
     _RequiredSetPermissionRequestRequestTypeDef, _OptionalSetPermissionRequestRequestTypeDef
 ):
     pass
 
 WeeklyAutoScalingScheduleTypeDef = TypedDict(
     "WeeklyAutoScalingScheduleTypeDef",
     {
-        "Monday": Mapping[str, str],
-        "Tuesday": Mapping[str, str],
-        "Wednesday": Mapping[str, str],
-        "Thursday": Mapping[str, str],
-        "Friday": Mapping[str, str],
-        "Saturday": Mapping[str, str],
-        "Sunday": Mapping[str, str],
+        "Monday": Dict[str, str],
+        "Tuesday": Dict[str, str],
+        "Wednesday": Dict[str, str],
+        "Thursday": Dict[str, str],
+        "Friday": Dict[str, str],
+        "Saturday": Dict[str, str],
+        "Sunday": Dict[str, str],
     },
     total=False,
 )
 
 StartInstanceRequestRequestTypeDef = TypedDict(
     "StartInstanceRequestRequestTypeDef",
     {
@@ -1245,28 +1192,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
 
-WeeklyAutoScalingScheduleOutputTypeDef = TypedDict(
-    "WeeklyAutoScalingScheduleOutputTypeDef",
-    {
-        "Monday": Dict[str, str],
-        "Tuesday": Dict[str, str],
-        "Wednesday": Dict[str, str],
-        "Thursday": Dict[str, str],
-        "Friday": Dict[str, str],
-        "Saturday": Dict[str, str],
-        "Sunday": Dict[str, str],
-    },
-    total=False,
-)
-
 UnassignInstanceRequestRequestTypeDef = TypedDict(
     "UnassignInstanceRequestRequestTypeDef",
     {
         "InstanceId": str,
     },
 )
 
@@ -1500,23 +1433,20 @@
     pass
 
 LoadBasedAutoScalingConfigurationTypeDef = TypedDict(
     "LoadBasedAutoScalingConfigurationTypeDef",
     {
         "LayerId": str,
         "Enable": bool,
-        "UpScaling": AutoScalingThresholdsOutputTypeDef,
-        "DownScaling": AutoScalingThresholdsOutputTypeDef,
+        "UpScaling": AutoScalingThresholdsTypeDef,
+        "DownScaling": AutoScalingThresholdsTypeDef,
     },
     total=False,
 )
 
-AutoScalingThresholdsUnionTypeDef = Union[
-    AutoScalingThresholdsTypeDef, AutoScalingThresholdsOutputTypeDef
-]
 _RequiredSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
     "_RequiredSetLoadBasedAutoScalingRequestRequestTypeDef",
     {
         "LayerId": str,
     },
 )
 _OptionalSetLoadBasedAutoScalingRequestRequestTypeDef = TypedDict(
@@ -1668,14 +1598,26 @@
     {
         "Tags": Dict[str, str],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RecipesResponseTypeDef = TypedDict(
+    "RecipesResponseTypeDef",
+    {
+        "Setup": List[str],
+        "Configure": List[str],
+        "Deploy": List[str],
+        "Undeploy": List[str],
+        "Shutdown": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 RegisterEcsClusterResultTypeDef = TypedDict(
     "RegisterEcsClusterResultTypeDef",
     {
         "EcsClusterArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1898,30 +1840,30 @@
 )
 
 class UpdateStackRequestRequestTypeDef(
     _RequiredUpdateStackRequestRequestTypeDef, _OptionalUpdateStackRequestRequestTypeDef
 ):
     pass
 
-CloudWatchLogsConfigurationOutputTypeDef = TypedDict(
-    "CloudWatchLogsConfigurationOutputTypeDef",
+CloudWatchLogsConfigurationResponseTypeDef = TypedDict(
+    "CloudWatchLogsConfigurationResponseTypeDef",
     {
         "Enabled": bool,
         "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 CloudWatchLogsConfigurationTypeDef = TypedDict(
     "CloudWatchLogsConfigurationTypeDef",
     {
         "Enabled": bool,
-        "LogStreams": List[CloudWatchLogsLogStreamTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "LogStreams": Sequence[CloudWatchLogsLogStreamTypeDef],
     },
+    total=False,
 )
 
 DescribeCommandsResultTypeDef = TypedDict(
     "DescribeCommandsResultTypeDef",
     {
         "Commands": List[CommandTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1948,27 +1890,26 @@
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-DeploymentCommandUnionTypeDef = Union[DeploymentCommandTypeDef, DeploymentCommandOutputTypeDef]
 DeploymentTypeDef = TypedDict(
     "DeploymentTypeDef",
     {
         "DeploymentId": str,
         "StackId": str,
         "AppId": str,
         "CreatedAt": str,
         "CompletedAt": str,
         "Duration": int,
         "IamUserArn": str,
         "Comment": str,
-        "Command": DeploymentCommandOutputTypeDef,
+        "Command": DeploymentCommandTypeDef,
         "Status": str,
         "CustomJson": str,
         "InstanceIds": List[str],
     },
     total=False,
 )
 
@@ -2169,15 +2110,14 @@
         "LayersCount": int,
         "AppsCount": int,
         "InstancesCount": InstancesCountTypeDef,
     },
     total=False,
 )
 
-RecipesUnionTypeDef = Union[RecipesTypeDef, RecipesOutputTypeDef]
 LifecycleEventConfigurationResponseTypeDef = TypedDict(
     "LifecycleEventConfigurationResponseTypeDef",
     {
         "Shutdown": ShutdownEventConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2224,22 +2164,19 @@
 ):
     pass
 
 TimeBasedAutoScalingConfigurationTypeDef = TypedDict(
     "TimeBasedAutoScalingConfigurationTypeDef",
     {
         "InstanceId": str,
-        "AutoScalingSchedule": WeeklyAutoScalingScheduleOutputTypeDef,
+        "AutoScalingSchedule": WeeklyAutoScalingScheduleTypeDef,
     },
     total=False,
 )
 
-WeeklyAutoScalingScheduleUnionTypeDef = Union[
-    WeeklyAutoScalingScheduleTypeDef, WeeklyAutoScalingScheduleOutputTypeDef
-]
 DescribeAgentVersionsResultTypeDef = TypedDict(
     "DescribeAgentVersionsResultTypeDef",
     {
         "AgentVersions": List[AgentVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2347,17 +2284,14 @@
     "DescribeStacksResultTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CloudWatchLogsConfigurationUnionTypeDef = Union[
-    CloudWatchLogsConfigurationTypeDef, CloudWatchLogsConfigurationOutputTypeDef
-]
 DescribeDeploymentsResultTypeDef = TypedDict(
     "DescribeDeploymentsResultTypeDef",
     {
         "Deployments": List[DeploymentTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2446,26 +2380,26 @@
         "Arn": str,
         "StackId": str,
         "LayerId": str,
         "Type": LayerTypeType,
         "Name": str,
         "Shortname": str,
         "Attributes": Dict[LayerAttributesKeysType, str],
-        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationOutputTypeDef,
+        "CloudWatchLogsConfiguration": CloudWatchLogsConfigurationTypeDef,
         "CustomInstanceProfileArn": str,
         "CustomJson": str,
         "CustomSecurityGroupIds": List[str],
         "DefaultSecurityGroupNames": List[str],
         "Packages": List[str],
         "VolumeConfigurations": List[VolumeConfigurationTypeDef],
         "EnableAutoHealing": bool,
         "AutoAssignElasticIps": bool,
         "AutoAssignPublicIps": bool,
-        "DefaultRecipes": RecipesOutputTypeDef,
-        "CustomRecipes": RecipesOutputTypeDef,
+        "DefaultRecipes": RecipesTypeDef,
+        "CustomRecipes": RecipesTypeDef,
         "CreatedAt": str,
         "InstallUpdatesOnBoot": bool,
         "UseEbsOptimizedInstances": bool,
         "LifecycleEventConfiguration": LifecycleEventConfigurationTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/waiter.py` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks/waiter.pyi` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworks-2.5.2.post1/types_aiobotocore_opsworks.egg-info/SOURCES.txt` & `types-aiobotocore-opsworks-2.5.2.post2/types_aiobotocore_opsworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

