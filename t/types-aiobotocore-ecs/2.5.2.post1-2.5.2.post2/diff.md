# Comparing `tmp/types-aiobotocore-ecs-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ecs-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecs-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecs-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:50 2023, max compression
```

## Comparing `types-aiobotocore-ecs-2.5.2.post1.tar` & `types-aiobotocore-ecs-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.505594 types-aiobotocore-ecs-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-08-02 14:52:14.505594 types-aiobotocore-ecs-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24360 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.505594 types-aiobotocore-ecs-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.493594 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52644 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52566 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-08-02 14:37:58.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-08-02 14:37:58.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    96682 2023-08-02 14:38:01.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    96563 2023-08-02 14:37:59.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-08-02 14:37:57.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.505594 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25862 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:14.000000 types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.204058 types-aiobotocore-ecs-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:24.000000 types-aiobotocore-ecs-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-08-04 12:00:50.196058 types-aiobotocore-ecs-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-08-04 11:45:24.000000 types-aiobotocore-ecs-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:50.204058 types-aiobotocore-ecs-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:45:24.000000 types-aiobotocore-ecs-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.192058 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-04 11:45:24.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-08-04 11:45:24.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:45:24.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52529 2023-08-04 11:45:25.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52451 2023-08-04 11:45:24.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-08-04 11:45:25.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-08-04 11:45:25.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-08-04 11:45:25.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-08-04 11:45:25.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:24.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85486 2023-08-04 11:45:28.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85385 2023-08-04 11:45:27.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:24.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-08-04 11:45:25.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-08-04 11:45:25.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.196058 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14908 2023-08-04 12:00:49.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:00:50.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:49.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:49.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:49.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:49.000000 types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecs-2.5.2.post1/LICENSE` & `types-aiobotocore-ecs-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2.post1/setup.py` & `types-aiobotocore-ecs-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecs",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ECS 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__init__.py` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__init__.pyi` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/__main__.py` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ECS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\nOther"
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

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/client.py` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,28 +53,28 @@
     AttributeTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ClusterConfigurationTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterSettingTypeDef,
-    ContainerDefinitionUnionTypeDef,
+    ContainerDefinitionTypeDef,
     ContainerStateChangeTypeDef,
     CreateCapacityProviderResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateServiceResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteAccountSettingResponseTypeDef,
     DeleteAttributesResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
-    DeploymentConfigurationUnionTypeDef,
+    DeploymentConfigurationTypeDef,
     DeploymentControllerTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     DescribeClustersResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     DescribeServicesResponseTypeDef,
@@ -95,51 +95,51 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LoadBalancerTypeDef,
     ManagedAgentStateChangeTypeDef,
     NetworkBindingTypeDef,
-    NetworkConfigurationUnionTypeDef,
+    NetworkConfigurationTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     PlatformDeviceTypeDef,
-    ProxyConfigurationUnionTypeDef,
+    ProxyConfigurationTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     PutAttributesResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
-    ResourceUnionTypeDef,
+    ResourceTypeDef,
     RunTaskResponseTypeDef,
     RuntimePlatformTypeDef,
     ScaleTypeDef,
-    ServiceConnectConfigurationUnionTypeDef,
+    ServiceConnectConfigurationTypeDef,
     ServiceRegistryTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
     TagTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    TaskOverrideUnionTypeDef,
+    TaskOverrideTypeDef,
     TimestampTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     VersionInfoTypeDef,
-    VolumeUnionTypeDef,
+    VolumeTypeDef,
 )
 from .waiter import (
     ServicesInactiveWaiter,
     ServicesStableWaiter,
     TasksRunningWaiter,
     TasksStoppedWaiter,
 )
@@ -265,26 +265,26 @@
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         desiredCount: int = ...,
         clientToken: str = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         role: str = ...,
-        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
+        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
         enableExecuteCommand: bool = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_service)
@@ -293,15 +293,15 @@
     async def create_task_set(
         self,
         *,
         service: str,
         cluster: str,
         taskDefinition: str,
         externalId: str = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         scale: ScaleTypeDef = ...,
         clientToken: str = ...,
@@ -738,15 +738,15 @@
 
     async def register_container_instance(
         self,
         *,
         cluster: str = ...,
         instanceIdentityDocument: str = ...,
         instanceIdentityDocumentSignature: str = ...,
-        totalResources: Sequence[ResourceUnionTypeDef] = ...,
+        totalResources: Sequence[ResourceTypeDef] = ...,
         versionInfo: VersionInfoTypeDef = ...,
         containerInstanceArn: str = ...,
         attributes: Sequence[AttributeTypeDef] = ...,
         platformDevices: Sequence[PlatformDeviceTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> RegisterContainerInstanceResponseTypeDef:
         """
@@ -756,27 +756,27 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#register_container_instance)
         """
 
     async def register_task_definition(
         self,
         *,
         family: str,
-        containerDefinitions: Sequence[ContainerDefinitionUnionTypeDef],
+        containerDefinitions: Sequence[ContainerDefinitionTypeDef],
         taskRoleArn: str = ...,
         executionRoleArn: str = ...,
         networkMode: NetworkModeType = ...,
-        volumes: Sequence[VolumeUnionTypeDef] = ...,
+        volumes: Sequence[VolumeTypeDef] = ...,
         placementConstraints: Sequence[TaskDefinitionPlacementConstraintTypeDef] = ...,
         requiresCompatibilities: Sequence[CompatibilityType] = ...,
         cpu: str = ...,
         memory: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         pidMode: PidModeType = ...,
         ipcMode: IpcModeType = ...,
-        proxyConfiguration: ProxyConfigurationUnionTypeDef = ...,
+        proxyConfiguration: ProxyConfigurationTypeDef = ...,
         inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,
         ephemeralStorage: EphemeralStorageTypeDef = ...,
         runtimePlatform: RuntimePlatformTypeDef = ...
     ) -> RegisterTaskDefinitionResponseTypeDef:
         """
         Registers a new task definition from the supplied `family` and
         `containerDefinitions`.
@@ -792,16 +792,16 @@
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         cluster: str = ...,
         count: int = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
         launchType: LaunchTypeType = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
-        overrides: TaskOverrideUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        overrides: TaskOverrideTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -818,16 +818,16 @@
         *,
         containerInstances: Sequence[str],
         taskDefinition: str,
         cluster: str = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
-        overrides: TaskOverrideUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        overrides: TaskOverrideTypeDef = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartTaskResponseTypeDef:
         """
         Starts a new task from the specified task definition on the specified container
@@ -976,27 +976,27 @@
         self,
         *,
         service: str,
         cluster: str = ...,
         desiredCount: int = ...,
         taskDefinition: str = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
-        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_service)
         """
```

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/client.pyi` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -53,28 +53,28 @@
     AttributeTypeDef,
     AutoScalingGroupProviderTypeDef,
     AutoScalingGroupProviderUpdateTypeDef,
     CapacityProviderStrategyItemTypeDef,
     ClusterConfigurationTypeDef,
     ClusterServiceConnectDefaultsRequestTypeDef,
     ClusterSettingTypeDef,
-    ContainerDefinitionUnionTypeDef,
+    ContainerDefinitionTypeDef,
     ContainerStateChangeTypeDef,
     CreateCapacityProviderResponseTypeDef,
     CreateClusterResponseTypeDef,
     CreateServiceResponseTypeDef,
     CreateTaskSetResponseTypeDef,
     DeleteAccountSettingResponseTypeDef,
     DeleteAttributesResponseTypeDef,
     DeleteCapacityProviderResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DeleteServiceResponseTypeDef,
     DeleteTaskDefinitionsResponseTypeDef,
     DeleteTaskSetResponseTypeDef,
-    DeploymentConfigurationUnionTypeDef,
+    DeploymentConfigurationTypeDef,
     DeploymentControllerTypeDef,
     DeregisterContainerInstanceResponseTypeDef,
     DeregisterTaskDefinitionResponseTypeDef,
     DescribeCapacityProvidersResponseTypeDef,
     DescribeClustersResponseTypeDef,
     DescribeContainerInstancesResponseTypeDef,
     DescribeServicesResponseTypeDef,
@@ -95,51 +95,51 @@
     ListTagsForResourceResponseTypeDef,
     ListTaskDefinitionFamiliesResponseTypeDef,
     ListTaskDefinitionsResponseTypeDef,
     ListTasksResponseTypeDef,
     LoadBalancerTypeDef,
     ManagedAgentStateChangeTypeDef,
     NetworkBindingTypeDef,
-    NetworkConfigurationUnionTypeDef,
+    NetworkConfigurationTypeDef,
     PlacementConstraintTypeDef,
     PlacementStrategyTypeDef,
     PlatformDeviceTypeDef,
-    ProxyConfigurationUnionTypeDef,
+    ProxyConfigurationTypeDef,
     PutAccountSettingDefaultResponseTypeDef,
     PutAccountSettingResponseTypeDef,
     PutAttributesResponseTypeDef,
     PutClusterCapacityProvidersResponseTypeDef,
     RegisterContainerInstanceResponseTypeDef,
     RegisterTaskDefinitionResponseTypeDef,
-    ResourceUnionTypeDef,
+    ResourceTypeDef,
     RunTaskResponseTypeDef,
     RuntimePlatformTypeDef,
     ScaleTypeDef,
-    ServiceConnectConfigurationUnionTypeDef,
+    ServiceConnectConfigurationTypeDef,
     ServiceRegistryTypeDef,
     StartTaskResponseTypeDef,
     StopTaskResponseTypeDef,
     SubmitAttachmentStateChangesResponseTypeDef,
     SubmitContainerStateChangeResponseTypeDef,
     SubmitTaskStateChangeResponseTypeDef,
     TagTypeDef,
     TaskDefinitionPlacementConstraintTypeDef,
-    TaskOverrideUnionTypeDef,
+    TaskOverrideTypeDef,
     TimestampTypeDef,
     UpdateCapacityProviderResponseTypeDef,
     UpdateClusterResponseTypeDef,
     UpdateClusterSettingsResponseTypeDef,
     UpdateContainerAgentResponseTypeDef,
     UpdateContainerInstancesStateResponseTypeDef,
     UpdateServicePrimaryTaskSetResponseTypeDef,
     UpdateServiceResponseTypeDef,
     UpdateTaskProtectionResponseTypeDef,
     UpdateTaskSetResponseTypeDef,
     VersionInfoTypeDef,
-    VolumeUnionTypeDef,
+    VolumeTypeDef,
 )
 from .waiter import (
     ServicesInactiveWaiter,
     ServicesStableWaiter,
     TasksRunningWaiter,
     TasksStoppedWaiter,
 )
@@ -256,26 +256,26 @@
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         desiredCount: int = ...,
         clientToken: str = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         role: str = ...,
-        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
+        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
         healthCheckGracePeriodSeconds: int = ...,
         schedulingStrategy: SchedulingStrategyType = ...,
         deploymentController: DeploymentControllerTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         enableECSManagedTags: bool = ...,
         propagateTags: PropagateTagsType = ...,
         enableExecuteCommand: bool = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
     ) -> CreateServiceResponseTypeDef:
         """
         Runs and maintains your desired number of tasks from a specified task
         definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.create_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#create_service)
@@ -283,15 +283,15 @@
     async def create_task_set(
         self,
         *,
         service: str,
         cluster: str,
         taskDefinition: str,
         externalId: str = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
         launchType: LaunchTypeType = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         platformVersion: str = ...,
         scale: ScaleTypeDef = ...,
         clientToken: str = ...,
@@ -693,15 +693,15 @@
         """
     async def register_container_instance(
         self,
         *,
         cluster: str = ...,
         instanceIdentityDocument: str = ...,
         instanceIdentityDocumentSignature: str = ...,
-        totalResources: Sequence[ResourceUnionTypeDef] = ...,
+        totalResources: Sequence[ResourceTypeDef] = ...,
         versionInfo: VersionInfoTypeDef = ...,
         containerInstanceArn: str = ...,
         attributes: Sequence[AttributeTypeDef] = ...,
         platformDevices: Sequence[PlatformDeviceTypeDef] = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> RegisterContainerInstanceResponseTypeDef:
         """
@@ -710,27 +710,27 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_container_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#register_container_instance)
         """
     async def register_task_definition(
         self,
         *,
         family: str,
-        containerDefinitions: Sequence[ContainerDefinitionUnionTypeDef],
+        containerDefinitions: Sequence[ContainerDefinitionTypeDef],
         taskRoleArn: str = ...,
         executionRoleArn: str = ...,
         networkMode: NetworkModeType = ...,
-        volumes: Sequence[VolumeUnionTypeDef] = ...,
+        volumes: Sequence[VolumeTypeDef] = ...,
         placementConstraints: Sequence[TaskDefinitionPlacementConstraintTypeDef] = ...,
         requiresCompatibilities: Sequence[CompatibilityType] = ...,
         cpu: str = ...,
         memory: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         pidMode: PidModeType = ...,
         ipcMode: IpcModeType = ...,
-        proxyConfiguration: ProxyConfigurationUnionTypeDef = ...,
+        proxyConfiguration: ProxyConfigurationTypeDef = ...,
         inferenceAccelerators: Sequence[InferenceAcceleratorTypeDef] = ...,
         ephemeralStorage: EphemeralStorageTypeDef = ...,
         runtimePlatform: RuntimePlatformTypeDef = ...
     ) -> RegisterTaskDefinitionResponseTypeDef:
         """
         Registers a new task definition from the supplied `family` and
         `containerDefinitions`.
@@ -745,16 +745,16 @@
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
         cluster: str = ...,
         count: int = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
         launchType: LaunchTypeType = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
-        overrides: TaskOverrideUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        overrides: TaskOverrideTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
@@ -770,16 +770,16 @@
         *,
         containerInstances: Sequence[str],
         taskDefinition: str,
         cluster: str = ...,
         enableECSManagedTags: bool = ...,
         enableExecuteCommand: bool = ...,
         group: str = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
-        overrides: TaskOverrideUnionTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
+        overrides: TaskOverrideTypeDef = ...,
         propagateTags: PropagateTagsType = ...,
         referenceId: str = ...,
         startedBy: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> StartTaskResponseTypeDef:
         """
         Starts a new task from the specified task definition on the specified container
@@ -916,27 +916,27 @@
         self,
         *,
         service: str,
         cluster: str = ...,
         desiredCount: int = ...,
         taskDefinition: str = ...,
         capacityProviderStrategy: Sequence[CapacityProviderStrategyItemTypeDef] = ...,
-        deploymentConfiguration: DeploymentConfigurationUnionTypeDef = ...,
-        networkConfiguration: NetworkConfigurationUnionTypeDef = ...,
+        deploymentConfiguration: DeploymentConfigurationTypeDef = ...,
+        networkConfiguration: NetworkConfigurationTypeDef = ...,
         placementConstraints: Sequence[PlacementConstraintTypeDef] = ...,
         placementStrategy: Sequence[PlacementStrategyTypeDef] = ...,
         platformVersion: str = ...,
         forceNewDeployment: bool = ...,
         healthCheckGracePeriodSeconds: int = ...,
         enableExecuteCommand: bool = ...,
         enableECSManagedTags: bool = ...,
         loadBalancers: Sequence[LoadBalancerTypeDef] = ...,
         propagateTags: PropagateTagsType = ...,
         serviceRegistries: Sequence[ServiceRegistryTypeDef] = ...,
-        serviceConnectConfiguration: ServiceConnectConfigurationUnionTypeDef = ...
+        serviceConnectConfiguration: ServiceConnectConfigurationTypeDef = ...
     ) -> UpdateServiceResponseTypeDef:
         """
         Modifies the parameters of a service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.update_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecs/client/#update_service)
         """
```

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/literals.py` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/literals.pyi` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/paginator.py` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/paginator.pyi` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/type_defs.py` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,38 +73,35 @@
 
 
 __all__ = (
     "AttachmentStateChangeTypeDef",
     "KeyValuePairTypeDef",
     "AttributeTypeDef",
     "ManagedScalingTypeDef",
-    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
     "ClusterServiceConnectDefaultsRequestTypeDef",
     "ClusterServiceConnectDefaultsTypeDef",
     "ClusterSettingTypeDef",
     "ContainerDependencyTypeDef",
     "EnvironmentFileTypeDef",
-    "FirelensConfigurationOutputTypeDef",
-    "HealthCheckOutputTypeDef",
+    "FirelensConfigurationTypeDef",
+    "HealthCheckTypeDef",
     "HostEntryTypeDef",
     "MountPointTypeDef",
     "PortMappingTypeDef",
     "RepositoryCredentialsTypeDef",
     "ResourceRequirementTypeDef",
     "SecretTypeDef",
     "SystemControlTypeDef",
     "UlimitTypeDef",
     "VolumeFromTypeDef",
-    "FirelensConfigurationTypeDef",
-    "HealthCheckTypeDef",
     "InstanceHealthCheckResultTypeDef",
-    "ResourceOutputTypeDef",
+    "ResourceTypeDef",
     "VersionInfoTypeDef",
     "NetworkBindingTypeDef",
     "ManagedAgentTypeDef",
     "NetworkInterfaceTypeDef",
     "ResponseMetadataTypeDef",
     "DeploymentControllerTypeDef",
     "LoadBalancerTypeDef",
@@ -116,47 +113,42 @@
     "SettingTypeDef",
     "DeleteCapacityProviderRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     "FailureTypeDef",
     "DeleteTaskSetRequestRequestTypeDef",
-    "DeploymentAlarmsOutputTypeDef",
     "DeploymentAlarmsTypeDef",
     "DeploymentCircuitBreakerTypeDef",
     "ServiceConnectServiceResourceTypeDef",
     "DeregisterContainerInstanceRequestRequestTypeDef",
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     "DescribeCapacityProvidersRequestRequestTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeContainerInstancesRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
-    "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "DiscoverPollEndpointRequestRequestTypeDef",
-    "DockerVolumeConfigurationOutputTypeDef",
     "DockerVolumeConfigurationTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EphemeralStorageTypeDef",
     "ExecuteCommandLogConfigurationTypeDef",
     "ExecuteCommandRequestRequestTypeDef",
     "SessionTypeDef",
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     "GetTaskProtectionRequestRequestTypeDef",
     "ProtectedTaskTypeDef",
     "HostVolumePropertiesTypeDef",
     "InferenceAcceleratorOverrideTypeDef",
     "InferenceAcceleratorTypeDef",
-    "KernelCapabilitiesOutputTypeDef",
     "KernelCapabilitiesTypeDef",
-    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
     "ListAttributesRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListContainerInstancesRequestRequestTypeDef",
     "ListServicesByNamespaceRequestRequestTypeDef",
@@ -167,40 +159,35 @@
     "ListTasksRequestRequestTypeDef",
     "ManagedAgentStateChangeTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
-    "ResourceTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
     "StopTaskRequestRequestTypeDef",
     "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
-    "ProxyConfigurationOutputTypeDef",
     "ProxyConfigurationTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
     "PutAttributesRequestRequestTypeDef",
     "AutoScalingGroupProviderTypeDef",
     "AutoScalingGroupProviderUpdateTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "PutClusterCapacityProvidersRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UpdateClusterSettingsRequestRequestTypeDef",
-    "ContainerOverrideOutputTypeDef",
     "ContainerOverrideTypeDef",
-    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "ContainerInstanceHealthStatusTypeDef",
     "ContainerStateChangeTypeDef",
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
     "DeleteAttributesResponseTypeDef",
     "DiscoverPollEndpointResponseTypeDef",
@@ -218,87 +205,73 @@
     "SubmitContainerStateChangeResponseTypeDef",
     "SubmitTaskStateChangeResponseTypeDef",
     "UpdateTaskSetRequestRequestTypeDef",
     "DeleteAccountSettingResponseTypeDef",
     "ListAccountSettingsResponseTypeDef",
     "PutAccountSettingDefaultResponseTypeDef",
     "PutAccountSettingResponseTypeDef",
-    "DeploymentConfigurationOutputTypeDef",
     "DeploymentConfigurationTypeDef",
     "DescribeServicesRequestServicesInactiveWaitTypeDef",
     "DescribeServicesRequestServicesStableWaitTypeDef",
     "DescribeTasksRequestTasksRunningWaitTypeDef",
     "DescribeTasksRequestTasksStoppedWaitTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "ExecuteCommandConfigurationTypeDef",
     "ExecuteCommandResponseTypeDef",
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
-    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
     "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
     "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
-    "ResourceUnionTypeDef",
-    "ServiceConnectServiceOutputTypeDef",
+    "RegisterContainerInstanceRequestRequestTypeDef",
     "ServiceConnectServiceTypeDef",
-    "ProxyConfigurationUnionTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
-    "TaskSetTypeDef",
     "CreateTaskSetRequestRequestTypeDef",
-    "NetworkConfigurationUnionTypeDef",
-    "TaskOverrideOutputTypeDef",
+    "TaskSetTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
-    "DeploymentConfigurationUnionTypeDef",
     "ClusterConfigurationTypeDef",
-    "VolumeOutputTypeDef",
     "VolumeTypeDef",
-    "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
-    "RegisterContainerInstanceRequestRequestTypeDef",
-    "ServiceConnectConfigurationOutputTypeDef",
     "ServiceConnectConfigurationTypeDef",
     "CreateCapacityProviderResponseTypeDef",
     "DeleteCapacityProviderResponseTypeDef",
     "DescribeCapacityProvidersResponseTypeDef",
     "UpdateCapacityProviderResponseTypeDef",
     "CreateTaskSetResponseTypeDef",
     "DeleteTaskSetResponseTypeDef",
     "DescribeTaskSetsResponseTypeDef",
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     "UpdateTaskSetResponseTypeDef",
-    "TaskTypeDef",
     "RunTaskRequestRequestTypeDef",
     "StartTaskRequestRequestTypeDef",
-    "TaskOverrideUnionTypeDef",
+    "TaskTypeDef",
     "DeregisterContainerInstanceResponseTypeDef",
     "DescribeContainerInstancesResponseTypeDef",
     "RegisterContainerInstanceResponseTypeDef",
     "UpdateContainerAgentResponseTypeDef",
     "UpdateContainerInstancesStateResponseTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
-    "VolumeUnionTypeDef",
+    "RegisterTaskDefinitionRequestRequestTypeDef",
     "TaskDefinitionTypeDef",
-    "ContainerDefinitionUnionTypeDef",
-    "DeploymentTypeDef",
     "CreateServiceRequestRequestTypeDef",
-    "ServiceConnectConfigurationUnionTypeDef",
+    "DeploymentTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "DescribeTasksResponseTypeDef",
     "RunTaskResponseTypeDef",
     "StartTaskResponseTypeDef",
     "StopTaskResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
@@ -306,15 +279,14 @@
     "PutClusterCapacityProvidersResponseTypeDef",
     "UpdateClusterResponseTypeDef",
     "UpdateClusterSettingsResponseTypeDef",
     "DeleteTaskDefinitionsResponseTypeDef",
     "DeregisterTaskDefinitionResponseTypeDef",
     "DescribeTaskDefinitionResponseTypeDef",
     "RegisterTaskDefinitionResponseTypeDef",
-    "RegisterTaskDefinitionRequestRequestTypeDef",
     "ServiceTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "UpdateServiceResponseTypeDef",
 )
 
@@ -364,36 +336,14 @@
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
         "instanceWarmupPeriod": int,
     },
     total=False,
 )
 
-_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAwsVpcConfigurationOutputTypeDef",
-    {
-        "subnets": List[str],
-    },
-)
-_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAwsVpcConfigurationOutputTypeDef",
-    {
-        "securityGroups": List[str],
-        "assignPublicIp": AssignPublicIpType,
-    },
-    total=False,
-)
-
-
-class AwsVpcConfigurationOutputTypeDef(
-    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -479,56 +429,54 @@
     "EnvironmentFileTypeDef",
     {
         "value": str,
         "type": Literal["s3"],
     },
 )
 
-_RequiredFirelensConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFirelensConfigurationOutputTypeDef",
+_RequiredFirelensConfigurationTypeDef = TypedDict(
+    "_RequiredFirelensConfigurationTypeDef",
     {
         "type": FirelensConfigurationTypeType,
     },
 )
-_OptionalFirelensConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFirelensConfigurationOutputTypeDef",
+_OptionalFirelensConfigurationTypeDef = TypedDict(
+    "_OptionalFirelensConfigurationTypeDef",
     {
         "options": Dict[str, str],
     },
     total=False,
 )
 
 
-class FirelensConfigurationOutputTypeDef(
-    _RequiredFirelensConfigurationOutputTypeDef, _OptionalFirelensConfigurationOutputTypeDef
+class FirelensConfigurationTypeDef(
+    _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
 ):
     pass
 
 
-_RequiredHealthCheckOutputTypeDef = TypedDict(
-    "_RequiredHealthCheckOutputTypeDef",
+_RequiredHealthCheckTypeDef = TypedDict(
+    "_RequiredHealthCheckTypeDef",
     {
         "command": List[str],
     },
 )
-_OptionalHealthCheckOutputTypeDef = TypedDict(
-    "_OptionalHealthCheckOutputTypeDef",
+_OptionalHealthCheckTypeDef = TypedDict(
+    "_OptionalHealthCheckTypeDef",
     {
         "interval": int,
         "timeout": int,
         "retries": int,
         "startPeriod": int,
     },
     total=False,
 )
 
 
-class HealthCheckOutputTypeDef(
-    _RequiredHealthCheckOutputTypeDef, _OptionalHealthCheckOutputTypeDef
-):
+class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
 
 HostEntryTypeDef = TypedDict(
     "HostEntryTypeDef",
     {
         "hostname": str,
@@ -605,70 +553,27 @@
     {
         "sourceContainer": str,
         "readOnly": bool,
     },
     total=False,
 )
 
-_RequiredFirelensConfigurationTypeDef = TypedDict(
-    "_RequiredFirelensConfigurationTypeDef",
-    {
-        "type": FirelensConfigurationTypeType,
-    },
-)
-_OptionalFirelensConfigurationTypeDef = TypedDict(
-    "_OptionalFirelensConfigurationTypeDef",
-    {
-        "options": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class FirelensConfigurationTypeDef(
-    _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
-):
-    pass
-
-
-_RequiredHealthCheckTypeDef = TypedDict(
-    "_RequiredHealthCheckTypeDef",
-    {
-        "command": Sequence[str],
-    },
-)
-_OptionalHealthCheckTypeDef = TypedDict(
-    "_OptionalHealthCheckTypeDef",
-    {
-        "interval": int,
-        "timeout": int,
-        "retries": int,
-        "startPeriod": int,
-    },
-    total=False,
-)
-
-
-class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
-    pass
-
-
 InstanceHealthCheckResultTypeDef = TypedDict(
     "InstanceHealthCheckResultTypeDef",
     {
         "type": Literal["CONTAINER_RUNTIME"],
         "status": InstanceHealthCheckStateType,
         "lastUpdated": datetime,
         "lastStatusChange": datetime,
     },
     total=False,
 )
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
     {
         "name": str,
         "type": str,
         "doubleValue": float,
         "longValue": int,
         "integerValue": int,
         "stringSetValue": List[str],
@@ -891,23 +796,14 @@
 
 class DeleteTaskSetRequestRequestTypeDef(
     _RequiredDeleteTaskSetRequestRequestTypeDef, _OptionalDeleteTaskSetRequestRequestTypeDef
 ):
     pass
 
 
-DeploymentAlarmsOutputTypeDef = TypedDict(
-    "DeploymentAlarmsOutputTypeDef",
-    {
-        "alarmNames": List[str],
-        "enable": bool,
-        "rollback": bool,
-    },
-)
-
 DeploymentAlarmsTypeDef = TypedDict(
     "DeploymentAlarmsTypeDef",
     {
         "alarmNames": Sequence[str],
         "enable": bool,
         "rollback": bool,
     },
@@ -1097,45 +993,25 @@
 
 class DescribeTasksRequestRequestTypeDef(
     _RequiredDescribeTasksRequestRequestTypeDef, _OptionalDescribeTasksRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredDeviceOutputTypeDef = TypedDict(
-    "_RequiredDeviceOutputTypeDef",
-    {
-        "hostPath": str,
-    },
-)
-_OptionalDeviceOutputTypeDef = TypedDict(
-    "_OptionalDeviceOutputTypeDef",
-    {
-        "containerPath": str,
-        "permissions": List[DeviceCgroupPermissionType],
-    },
-    total=False,
-)
-
-
-class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
-    pass
-
-
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
     "_OptionalDeviceTypeDef",
     {
         "containerPath": str,
-        "permissions": Sequence[DeviceCgroupPermissionType],
+        "permissions": List[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
 
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
@@ -1146,34 +1022,22 @@
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
 )
 
-DockerVolumeConfigurationOutputTypeDef = TypedDict(
-    "DockerVolumeConfigurationOutputTypeDef",
-    {
-        "scope": ScopeType,
-        "autoprovision": bool,
-        "driver": str,
-        "driverOpts": Dict[str, str],
-        "labels": Dict[str, str],
-    },
-    total=False,
-)
-
 DockerVolumeConfigurationTypeDef = TypedDict(
     "DockerVolumeConfigurationTypeDef",
     {
         "scope": ScopeType,
         "autoprovision": bool,
         "driver": str,
-        "driverOpts": Mapping[str, str],
-        "labels": Mapping[str, str],
+        "driverOpts": Dict[str, str],
+        "labels": Dict[str, str],
     },
     total=False,
 )
 
 EFSAuthorizationConfigTypeDef = TypedDict(
     "EFSAuthorizationConfigTypeDef",
     {
@@ -1296,63 +1160,34 @@
     "InferenceAcceleratorTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
 )
 
-KernelCapabilitiesOutputTypeDef = TypedDict(
-    "KernelCapabilitiesOutputTypeDef",
-    {
-        "add": List[str],
-        "drop": List[str],
-    },
-    total=False,
-)
-
 KernelCapabilitiesTypeDef = TypedDict(
     "KernelCapabilitiesTypeDef",
     {
-        "add": Sequence[str],
-        "drop": Sequence[str],
-    },
-    total=False,
-)
-
-_RequiredTmpfsOutputTypeDef = TypedDict(
-    "_RequiredTmpfsOutputTypeDef",
-    {
-        "containerPath": str,
-        "size": int,
-    },
-)
-_OptionalTmpfsOutputTypeDef = TypedDict(
-    "_OptionalTmpfsOutputTypeDef",
-    {
-        "mountOptions": List[str],
+        "add": List[str],
+        "drop": List[str],
     },
     total=False,
 )
 
-
-class TmpfsOutputTypeDef(_RequiredTmpfsOutputTypeDef, _OptionalTmpfsOutputTypeDef):
-    pass
-
-
 _RequiredTmpfsTypeDef = TypedDict(
     "_RequiredTmpfsTypeDef",
     {
         "containerPath": str,
         "size": int,
     },
 )
 _OptionalTmpfsTypeDef = TypedDict(
     "_OptionalTmpfsTypeDef",
     {
-        "mountOptions": Sequence[str],
+        "mountOptions": List[str],
     },
     total=False,
 )
 
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
@@ -1583,27 +1418,14 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
     },
     total=False,
 )
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
-    {
-        "name": str,
-        "type": str,
-        "doubleValue": float,
-        "longValue": int,
-        "integerValue": int,
-        "stringSetValue": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
 )
 _OptionalServiceConnectClientAliasTypeDef = TypedDict(
@@ -1769,47 +1591,25 @@
         "type": str,
         "status": str,
         "details": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
-_RequiredProxyConfigurationOutputTypeDef = TypedDict(
-    "_RequiredProxyConfigurationOutputTypeDef",
-    {
-        "containerName": str,
-    },
-)
-_OptionalProxyConfigurationOutputTypeDef = TypedDict(
-    "_OptionalProxyConfigurationOutputTypeDef",
-    {
-        "type": Literal["APPMESH"],
-        "properties": List[KeyValuePairTypeDef],
-    },
-    total=False,
-)
-
-
-class ProxyConfigurationOutputTypeDef(
-    _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredProxyConfigurationTypeDef = TypedDict(
     "_RequiredProxyConfigurationTypeDef",
     {
         "containerName": str,
     },
 )
 _OptionalProxyConfigurationTypeDef = TypedDict(
     "_OptionalProxyConfigurationTypeDef",
     {
         "type": Literal["APPMESH"],
-        "properties": Sequence[KeyValuePairTypeDef],
+        "properties": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
 
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
@@ -1886,22 +1686,14 @@
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -1927,66 +1719,29 @@
     "UpdateClusterSettingsRequestRequestTypeDef",
     {
         "cluster": str,
         "settings": Sequence[ClusterSettingTypeDef],
     },
 )
 
-ContainerOverrideOutputTypeDef = TypedDict(
-    "ContainerOverrideOutputTypeDef",
+ContainerOverrideTypeDef = TypedDict(
+    "ContainerOverrideTypeDef",
     {
         "name": str,
         "command": List[str],
         "environment": List[KeyValuePairTypeDef],
         "environmentFiles": List[EnvironmentFileTypeDef],
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
         "resourceRequirements": List[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
-ContainerOverrideTypeDef = TypedDict(
-    "ContainerOverrideTypeDef",
-    {
-        "name": str,
-        "command": Sequence[str],
-        "environment": Sequence[KeyValuePairTypeDef],
-        "environmentFiles": Sequence[EnvironmentFileTypeDef],
-        "cpu": int,
-        "memory": int,
-        "memoryReservation": int,
-        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
-    },
-    total=False,
-)
-
-_RequiredLogConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLogConfigurationOutputTypeDef",
-    {
-        "logDriver": LogDriverType,
-    },
-)
-_OptionalLogConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLogConfigurationOutputTypeDef",
-    {
-        "options": Dict[str, str],
-        "secretOptions": List[SecretTypeDef],
-    },
-    total=False,
-)
-
-
-class LogConfigurationOutputTypeDef(
-    _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
@@ -2234,25 +1989,14 @@
     "PutAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeploymentConfigurationOutputTypeDef = TypedDict(
-    "DeploymentConfigurationOutputTypeDef",
-    {
-        "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
-        "maximumPercent": int,
-        "minimumHealthyPercent": int,
-        "alarms": DeploymentAlarmsOutputTypeDef,
-    },
-    total=False,
-)
-
 DeploymentConfigurationTypeDef = TypedDict(
     "DeploymentConfigurationTypeDef",
     {
         "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
         "maximumPercent": int,
         "minimumHealthyPercent": int,
         "alarms": DeploymentAlarmsTypeDef,
@@ -2426,36 +2170,22 @@
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LinuxParametersOutputTypeDef = TypedDict(
-    "LinuxParametersOutputTypeDef",
-    {
-        "capabilities": KernelCapabilitiesOutputTypeDef,
-        "devices": List[DeviceOutputTypeDef],
-        "initProcessEnabled": bool,
-        "sharedMemorySize": int,
-        "tmpfs": List[TmpfsOutputTypeDef],
-        "maxSwap": int,
-        "swappiness": int,
-    },
-    total=False,
-)
-
 LinuxParametersTypeDef = TypedDict(
     "LinuxParametersTypeDef",
     {
         "capabilities": KernelCapabilitiesTypeDef,
-        "devices": Sequence[DeviceTypeDef],
+        "devices": List[DeviceTypeDef],
         "initProcessEnabled": bool,
         "sharedMemorySize": int,
-        "tmpfs": Sequence[TmpfsTypeDef],
+        "tmpfs": List[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
 ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
@@ -2579,38 +2309,30 @@
         "desiredStatus": DesiredStatusType,
         "launchType": LaunchTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
-_RequiredServiceConnectServiceOutputTypeDef = TypedDict(
-    "_RequiredServiceConnectServiceOutputTypeDef",
-    {
-        "portName": str,
-    },
-)
-_OptionalServiceConnectServiceOutputTypeDef = TypedDict(
-    "_OptionalServiceConnectServiceOutputTypeDef",
+RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
+    "RegisterContainerInstanceRequestRequestTypeDef",
     {
-        "discoveryName": str,
-        "clientAliases": List[ServiceConnectClientAliasTypeDef],
-        "ingressPortOverride": int,
+        "cluster": str,
+        "instanceIdentityDocument": str,
+        "instanceIdentityDocumentSignature": str,
+        "totalResources": Sequence[ResourceTypeDef],
+        "versionInfo": VersionInfoTypeDef,
+        "containerInstanceArn": str,
+        "attributes": Sequence[AttributeTypeDef],
+        "platformDevices": Sequence[PlatformDeviceTypeDef],
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
-class ServiceConnectServiceOutputTypeDef(
-    _RequiredServiceConnectServiceOutputTypeDef, _OptionalServiceConnectServiceOutputTypeDef
-):
-    pass
-
-
 _RequiredServiceConnectServiceTypeDef = TypedDict(
     "_RequiredServiceConnectServiceTypeDef",
     {
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceTypeDef = TypedDict(
@@ -2626,15 +2348,14 @@
 
 class ServiceConnectServiceTypeDef(
     _RequiredServiceConnectServiceTypeDef, _OptionalServiceConnectServiceTypeDef
 ):
     pass
 
 
-ProxyConfigurationUnionTypeDef = Union[ProxyConfigurationTypeDef, ProxyConfigurationOutputTypeDef]
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
         "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
@@ -2672,45 +2393,14 @@
     "UpdateCapacityProviderRequestRequestTypeDef",
     {
         "name": str,
         "autoScalingGroupProvider": AutoScalingGroupProviderUpdateTypeDef,
     },
 )
 
-TaskSetTypeDef = TypedDict(
-    "TaskSetTypeDef",
-    {
-        "id": str,
-        "taskSetArn": str,
-        "serviceArn": str,
-        "clusterArn": str,
-        "startedBy": str,
-        "externalId": str,
-        "status": str,
-        "taskDefinition": str,
-        "computedDesiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
-        "loadBalancers": List[LoadBalancerTypeDef],
-        "serviceRegistries": List[ServiceRegistryTypeDef],
-        "scale": ScaleTypeDef,
-        "stabilityStatus": StabilityStatusType,
-        "stabilityStatusAt": datetime,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 _RequiredCreateTaskSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTaskSetRequestRequestTypeDef",
     {
         "service": str,
         "cluster": str,
         "taskDefinition": str,
     },
@@ -2735,37 +2425,51 @@
 
 class CreateTaskSetRequestRequestTypeDef(
     _RequiredCreateTaskSetRequestRequestTypeDef, _OptionalCreateTaskSetRequestRequestTypeDef
 ):
     pass
 
 
-NetworkConfigurationUnionTypeDef = Union[
-    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-]
-TaskOverrideOutputTypeDef = TypedDict(
-    "TaskOverrideOutputTypeDef",
+TaskSetTypeDef = TypedDict(
+    "TaskSetTypeDef",
     {
-        "containerOverrides": List[ContainerOverrideOutputTypeDef],
-        "cpu": str,
-        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
-        "executionRoleArn": str,
-        "memory": str,
-        "taskRoleArn": str,
-        "ephemeralStorage": EphemeralStorageTypeDef,
+        "id": str,
+        "taskSetArn": str,
+        "serviceArn": str,
+        "clusterArn": str,
+        "startedBy": str,
+        "externalId": str,
+        "status": str,
+        "taskDefinition": str,
+        "computedDesiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "launchType": LaunchTypeType,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "loadBalancers": List[LoadBalancerTypeDef],
+        "serviceRegistries": List[ServiceRegistryTypeDef],
+        "scale": ScaleTypeDef,
+        "stabilityStatus": StabilityStatusType,
+        "stabilityStatusAt": datetime,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 TaskOverrideTypeDef = TypedDict(
     "TaskOverrideTypeDef",
     {
-        "containerOverrides": Sequence[ContainerOverrideTypeDef],
+        "containerOverrides": List[ContainerOverrideTypeDef],
         "cpu": str,
-        "inferenceAcceleratorOverrides": Sequence[InferenceAcceleratorOverrideTypeDef],
+        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
         "executionRoleArn": str,
         "memory": str,
         "taskRoleArn": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
@@ -2774,16 +2478,16 @@
     "ContainerInstanceTypeDef",
     {
         "containerInstanceArn": str,
         "ec2InstanceId": str,
         "capacityProviderName": str,
         "version": int,
         "versionInfo": VersionInfoTypeDef,
-        "remainingResources": List[ResourceOutputTypeDef],
-        "registeredResources": List[ResourceOutputTypeDef],
+        "remainingResources": List[ResourceTypeDef],
+        "registeredResources": List[ResourceTypeDef],
         "status": str,
         "statusReason": str,
         "agentConnected": bool,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "agentUpdateStatus": AgentUpdateStatusType,
         "attributes": List[AttributeTypeDef],
@@ -2808,51 +2512,36 @@
         "pullStartedAt": TimestampTypeDef,
         "pullStoppedAt": TimestampTypeDef,
         "executionStoppedAt": TimestampTypeDef,
     },
     total=False,
 )
 
-DeploymentConfigurationUnionTypeDef = Union[
-    DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
-]
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
 
-VolumeOutputTypeDef = TypedDict(
-    "VolumeOutputTypeDef",
-    {
-        "name": str,
-        "host": HostVolumePropertiesTypeDef,
-        "dockerVolumeConfiguration": DockerVolumeConfigurationOutputTypeDef,
-        "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
-        "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
-    },
-    total=False,
-)
-
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "name": str,
         "host": HostVolumePropertiesTypeDef,
         "dockerVolumeConfiguration": DockerVolumeConfigurationTypeDef,
         "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
         "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-ContainerDefinitionOutputTypeDef = TypedDict(
-    "ContainerDefinitionOutputTypeDef",
+ContainerDefinitionTypeDef = TypedDict(
+    "ContainerDefinitionTypeDef",
     {
         "name": str,
         "image": str,
         "repositoryCredentials": RepositoryCredentialsTypeDef,
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
@@ -2861,15 +2550,15 @@
         "essential": bool,
         "entryPoint": List[str],
         "command": List[str],
         "environment": List[KeyValuePairTypeDef],
         "environmentFiles": List[EnvironmentFileTypeDef],
         "mountPoints": List[MountPointTypeDef],
         "volumesFrom": List[VolumeFromTypeDef],
-        "linuxParameters": LinuxParametersOutputTypeDef,
+        "linuxParameters": LinuxParametersTypeDef,
         "secrets": List[SecretTypeDef],
         "dependsOn": List[ContainerDependencyTypeDef],
         "startTimeout": int,
         "stopTimeout": int,
         "hostname": str,
         "user": str,
         "workingDirectory": str,
@@ -2880,109 +2569,23 @@
         "dnsSearchDomains": List[str],
         "extraHosts": List[HostEntryTypeDef],
         "dockerSecurityOptions": List[str],
         "interactive": bool,
         "pseudoTerminal": bool,
         "dockerLabels": Dict[str, str],
         "ulimits": List[UlimitTypeDef],
-        "logConfiguration": LogConfigurationOutputTypeDef,
-        "healthCheck": HealthCheckOutputTypeDef,
-        "systemControls": List[SystemControlTypeDef],
-        "resourceRequirements": List[ResourceRequirementTypeDef],
-        "firelensConfiguration": FirelensConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-ContainerDefinitionTypeDef = TypedDict(
-    "ContainerDefinitionTypeDef",
-    {
-        "name": str,
-        "image": str,
-        "repositoryCredentials": RepositoryCredentialsTypeDef,
-        "cpu": int,
-        "memory": int,
-        "memoryReservation": int,
-        "links": Sequence[str],
-        "portMappings": Sequence[PortMappingTypeDef],
-        "essential": bool,
-        "entryPoint": Sequence[str],
-        "command": Sequence[str],
-        "environment": Sequence[KeyValuePairTypeDef],
-        "environmentFiles": Sequence[EnvironmentFileTypeDef],
-        "mountPoints": Sequence[MountPointTypeDef],
-        "volumesFrom": Sequence[VolumeFromTypeDef],
-        "linuxParameters": LinuxParametersTypeDef,
-        "secrets": Sequence[SecretTypeDef],
-        "dependsOn": Sequence[ContainerDependencyTypeDef],
-        "startTimeout": int,
-        "stopTimeout": int,
-        "hostname": str,
-        "user": str,
-        "workingDirectory": str,
-        "disableNetworking": bool,
-        "privileged": bool,
-        "readonlyRootFilesystem": bool,
-        "dnsServers": Sequence[str],
-        "dnsSearchDomains": Sequence[str],
-        "extraHosts": Sequence[HostEntryTypeDef],
-        "dockerSecurityOptions": Sequence[str],
-        "interactive": bool,
-        "pseudoTerminal": bool,
-        "dockerLabels": Mapping[str, str],
-        "ulimits": Sequence[UlimitTypeDef],
         "logConfiguration": LogConfigurationTypeDef,
         "healthCheck": HealthCheckTypeDef,
-        "systemControls": Sequence[SystemControlTypeDef],
-        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
+        "systemControls": List[SystemControlTypeDef],
+        "resourceRequirements": List[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
     },
     total=False,
 )
 
-RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
-    "RegisterContainerInstanceRequestRequestTypeDef",
-    {
-        "cluster": str,
-        "instanceIdentityDocument": str,
-        "instanceIdentityDocumentSignature": str,
-        "totalResources": Sequence[ResourceUnionTypeDef],
-        "versionInfo": VersionInfoTypeDef,
-        "containerInstanceArn": str,
-        "attributes": Sequence[AttributeTypeDef],
-        "platformDevices": Sequence[PlatformDeviceTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-_RequiredServiceConnectConfigurationOutputTypeDef = TypedDict(
-    "_RequiredServiceConnectConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalServiceConnectConfigurationOutputTypeDef = TypedDict(
-    "_OptionalServiceConnectConfigurationOutputTypeDef",
-    {
-        "namespace": str,
-        "services": List[ServiceConnectServiceOutputTypeDef],
-        "logConfiguration": LogConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ServiceConnectConfigurationOutputTypeDef(
-    _RequiredServiceConnectConfigurationOutputTypeDef,
-    _OptionalServiceConnectConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredServiceConnectConfigurationTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalServiceConnectConfigurationTypeDef = TypedDict(
@@ -3073,57 +2676,14 @@
     "UpdateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TaskTypeDef = TypedDict(
-    "TaskTypeDef",
-    {
-        "attachments": List[AttachmentTypeDef],
-        "attributes": List[AttributeTypeDef],
-        "availabilityZone": str,
-        "capacityProviderName": str,
-        "clusterArn": str,
-        "connectivity": ConnectivityType,
-        "connectivityAt": datetime,
-        "containerInstanceArn": str,
-        "containers": List[ContainerTypeDef],
-        "cpu": str,
-        "createdAt": datetime,
-        "desiredStatus": str,
-        "enableExecuteCommand": bool,
-        "executionStoppedAt": datetime,
-        "group": str,
-        "healthStatus": HealthStatusType,
-        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
-        "lastStatus": str,
-        "launchType": LaunchTypeType,
-        "memory": str,
-        "overrides": TaskOverrideOutputTypeDef,
-        "platformVersion": str,
-        "platformFamily": str,
-        "pullStartedAt": datetime,
-        "pullStoppedAt": datetime,
-        "startedAt": datetime,
-        "startedBy": str,
-        "stopCode": TaskStopCodeType,
-        "stoppedAt": datetime,
-        "stoppedReason": str,
-        "stoppingAt": datetime,
-        "tags": List[TagTypeDef],
-        "taskArn": str,
-        "taskDefinitionArn": str,
-        "version": int,
-        "ephemeralStorage": EphemeralStorageTypeDef,
-    },
-    total=False,
-)
-
 _RequiredRunTaskRequestRequestTypeDef = TypedDict(
     "_RequiredRunTaskRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
 )
 _OptionalRunTaskRequestRequestTypeDef = TypedDict(
@@ -3183,15 +2743,57 @@
 
 class StartTaskRequestRequestTypeDef(
     _RequiredStartTaskRequestRequestTypeDef, _OptionalStartTaskRequestRequestTypeDef
 ):
     pass
 
 
-TaskOverrideUnionTypeDef = Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef]
+TaskTypeDef = TypedDict(
+    "TaskTypeDef",
+    {
+        "attachments": List[AttachmentTypeDef],
+        "attributes": List[AttributeTypeDef],
+        "availabilityZone": str,
+        "capacityProviderName": str,
+        "clusterArn": str,
+        "connectivity": ConnectivityType,
+        "connectivityAt": datetime,
+        "containerInstanceArn": str,
+        "containers": List[ContainerTypeDef],
+        "cpu": str,
+        "createdAt": datetime,
+        "desiredStatus": str,
+        "enableExecuteCommand": bool,
+        "executionStoppedAt": datetime,
+        "group": str,
+        "healthStatus": HealthStatusType,
+        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
+        "lastStatus": str,
+        "launchType": LaunchTypeType,
+        "memory": str,
+        "overrides": TaskOverrideTypeDef,
+        "platformVersion": str,
+        "platformFamily": str,
+        "pullStartedAt": datetime,
+        "pullStoppedAt": datetime,
+        "startedAt": datetime,
+        "startedBy": str,
+        "stopCode": TaskStopCodeType,
+        "stoppedAt": datetime,
+        "stoppedReason": str,
+        "stoppingAt": datetime,
+        "tags": List[TagTypeDef],
+        "taskArn": str,
+        "taskDefinitionArn": str,
+        "version": int,
+        "ephemeralStorage": EphemeralStorageTypeDef,
+    },
+    total=False,
+)
+
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3286,74 +2888,82 @@
 
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
 
-VolumeUnionTypeDef = Union[VolumeTypeDef, VolumeOutputTypeDef]
+_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "family": str,
+        "containerDefinitions": Sequence[ContainerDefinitionTypeDef],
+    },
+)
+_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "taskRoleArn": str,
+        "executionRoleArn": str,
+        "networkMode": NetworkModeType,
+        "volumes": Sequence[VolumeTypeDef],
+        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
+        "requiresCompatibilities": Sequence[CompatibilityType],
+        "cpu": str,
+        "memory": str,
+        "tags": Sequence[TagTypeDef],
+        "pidMode": PidModeType,
+        "ipcMode": IpcModeType,
+        "proxyConfiguration": ProxyConfigurationTypeDef,
+        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
+        "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
+    },
+    total=False,
+)
+
+
+class RegisterTaskDefinitionRequestRequestTypeDef(
+    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
+    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
 TaskDefinitionTypeDef = TypedDict(
     "TaskDefinitionTypeDef",
     {
         "taskDefinitionArn": str,
-        "containerDefinitions": List[ContainerDefinitionOutputTypeDef],
+        "containerDefinitions": List[ContainerDefinitionTypeDef],
         "family": str,
         "taskRoleArn": str,
         "executionRoleArn": str,
         "networkMode": NetworkModeType,
         "revision": int,
-        "volumes": List[VolumeOutputTypeDef],
+        "volumes": List[VolumeTypeDef],
         "status": TaskDefinitionStatusType,
         "requiresAttributes": List[AttributeTypeDef],
         "placementConstraints": List[TaskDefinitionPlacementConstraintTypeDef],
         "compatibilities": List[CompatibilityType],
         "runtimePlatform": RuntimePlatformTypeDef,
         "requiresCompatibilities": List[CompatibilityType],
         "cpu": str,
         "memory": str,
         "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
         "pidMode": PidModeType,
         "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "proxyConfiguration": ProxyConfigurationTypeDef,
         "registeredAt": datetime,
         "deregisteredAt": datetime,
         "registeredBy": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
-ContainerDefinitionUnionTypeDef = Union[
-    ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef
-]
-DeploymentTypeDef = TypedDict(
-    "DeploymentTypeDef",
-    {
-        "id": str,
-        "status": str,
-        "taskDefinition": str,
-        "desiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "failedTasks": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "launchType": LaunchTypeType,
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
-        "rolloutState": DeploymentRolloutStateType,
-        "rolloutStateReason": str,
-        "serviceConnectConfiguration": ServiceConnectConfigurationOutputTypeDef,
-        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
-    },
-    total=False,
-)
-
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 _OptionalCreateServiceRequestRequestTypeDef = TypedDict(
@@ -3388,17 +2998,39 @@
 
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
 
-ServiceConnectConfigurationUnionTypeDef = Union[
-    ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
-]
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
+    {
+        "id": str,
+        "status": str,
+        "taskDefinition": str,
+        "desiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "failedTasks": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "launchType": LaunchTypeType,
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "rolloutState": DeploymentRolloutStateType,
+        "rolloutStateReason": str,
+        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
+        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "service": str,
     },
 )
 _OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
@@ -3547,51 +3179,14 @@
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "family": str,
-        "containerDefinitions": Sequence[ContainerDefinitionUnionTypeDef],
-    },
-)
-_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "taskRoleArn": str,
-        "executionRoleArn": str,
-        "networkMode": NetworkModeType,
-        "volumes": Sequence[VolumeUnionTypeDef],
-        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
-        "requiresCompatibilities": Sequence[CompatibilityType],
-        "cpu": str,
-        "memory": str,
-        "tags": Sequence[TagTypeDef],
-        "pidMode": PidModeType,
-        "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationTypeDef,
-        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
-        "ephemeralStorage": EphemeralStorageTypeDef,
-        "runtimePlatform": RuntimePlatformTypeDef,
-    },
-    total=False,
-)
-
-
-class RegisterTaskDefinitionRequestRequestTypeDef(
-    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
-    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
         "serviceName": str,
         "clusterArn": str,
         "loadBalancers": List[LoadBalancerTypeDef],
@@ -3601,23 +3196,23 @@
         "runningCount": int,
         "pendingCount": int,
         "launchType": LaunchTypeType,
         "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "platformVersion": str,
         "platformFamily": str,
         "taskDefinition": str,
-        "deploymentConfiguration": DeploymentConfigurationOutputTypeDef,
+        "deploymentConfiguration": DeploymentConfigurationTypeDef,
         "taskSets": List[TaskSetTypeDef],
         "deployments": List[DeploymentTypeDef],
         "roleArn": str,
         "events": List[ServiceEventTypeDef],
         "createdAt": datetime,
         "placementConstraints": List[PlacementConstraintTypeDef],
         "placementStrategy": List[PlacementStrategyTypeDef],
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "networkConfiguration": NetworkConfigurationTypeDef,
         "healthCheckGracePeriodSeconds": int,
         "schedulingStrategy": SchedulingStrategyType,
         "deploymentController": DeploymentControllerTypeDef,
         "tags": List[TagTypeDef],
         "createdBy": str,
         "enableECSManagedTags": bool,
         "propagateTags": PropagateTagsType,
```

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/type_defs.pyi` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -72,38 +72,35 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttachmentStateChangeTypeDef",
     "KeyValuePairTypeDef",
     "AttributeTypeDef",
     "ManagedScalingTypeDef",
-    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
     "ClusterServiceConnectDefaultsRequestTypeDef",
     "ClusterServiceConnectDefaultsTypeDef",
     "ClusterSettingTypeDef",
     "ContainerDependencyTypeDef",
     "EnvironmentFileTypeDef",
-    "FirelensConfigurationOutputTypeDef",
-    "HealthCheckOutputTypeDef",
+    "FirelensConfigurationTypeDef",
+    "HealthCheckTypeDef",
     "HostEntryTypeDef",
     "MountPointTypeDef",
     "PortMappingTypeDef",
     "RepositoryCredentialsTypeDef",
     "ResourceRequirementTypeDef",
     "SecretTypeDef",
     "SystemControlTypeDef",
     "UlimitTypeDef",
     "VolumeFromTypeDef",
-    "FirelensConfigurationTypeDef",
-    "HealthCheckTypeDef",
     "InstanceHealthCheckResultTypeDef",
-    "ResourceOutputTypeDef",
+    "ResourceTypeDef",
     "VersionInfoTypeDef",
     "NetworkBindingTypeDef",
     "ManagedAgentTypeDef",
     "NetworkInterfaceTypeDef",
     "ResponseMetadataTypeDef",
     "DeploymentControllerTypeDef",
     "LoadBalancerTypeDef",
@@ -115,47 +112,42 @@
     "SettingTypeDef",
     "DeleteCapacityProviderRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteServiceRequestRequestTypeDef",
     "DeleteTaskDefinitionsRequestRequestTypeDef",
     "FailureTypeDef",
     "DeleteTaskSetRequestRequestTypeDef",
-    "DeploymentAlarmsOutputTypeDef",
     "DeploymentAlarmsTypeDef",
     "DeploymentCircuitBreakerTypeDef",
     "ServiceConnectServiceResourceTypeDef",
     "DeregisterContainerInstanceRequestRequestTypeDef",
     "DeregisterTaskDefinitionRequestRequestTypeDef",
     "DescribeCapacityProvidersRequestRequestTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "DescribeContainerInstancesRequestRequestTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeTaskDefinitionRequestRequestTypeDef",
     "DescribeTaskSetsRequestRequestTypeDef",
     "DescribeTasksRequestRequestTypeDef",
-    "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "DiscoverPollEndpointRequestRequestTypeDef",
-    "DockerVolumeConfigurationOutputTypeDef",
     "DockerVolumeConfigurationTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EphemeralStorageTypeDef",
     "ExecuteCommandLogConfigurationTypeDef",
     "ExecuteCommandRequestRequestTypeDef",
     "SessionTypeDef",
     "FSxWindowsFileServerAuthorizationConfigTypeDef",
     "GetTaskProtectionRequestRequestTypeDef",
     "ProtectedTaskTypeDef",
     "HostVolumePropertiesTypeDef",
     "InferenceAcceleratorOverrideTypeDef",
     "InferenceAcceleratorTypeDef",
-    "KernelCapabilitiesOutputTypeDef",
     "KernelCapabilitiesTypeDef",
-    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccountSettingsRequestRequestTypeDef",
     "ListAttributesRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListContainerInstancesRequestRequestTypeDef",
     "ListServicesByNamespaceRequestRequestTypeDef",
@@ -166,40 +158,35 @@
     "ListTasksRequestRequestTypeDef",
     "ManagedAgentStateChangeTypeDef",
     "PlatformDeviceTypeDef",
     "PutAccountSettingDefaultRequestRequestTypeDef",
     "PutAccountSettingRequestRequestTypeDef",
     "RuntimePlatformTypeDef",
     "TaskDefinitionPlacementConstraintTypeDef",
-    "ResourceTypeDef",
     "ServiceConnectClientAliasTypeDef",
     "ServiceEventTypeDef",
     "StopTaskRequestRequestTypeDef",
     "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContainerAgentRequestRequestTypeDef",
     "UpdateContainerInstancesStateRequestRequestTypeDef",
     "UpdateServicePrimaryTaskSetRequestRequestTypeDef",
     "UpdateTaskProtectionRequestRequestTypeDef",
     "SubmitAttachmentStateChangesRequestRequestTypeDef",
     "AttachmentTypeDef",
-    "ProxyConfigurationOutputTypeDef",
     "ProxyConfigurationTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
     "PutAttributesRequestRequestTypeDef",
     "AutoScalingGroupProviderTypeDef",
     "AutoScalingGroupProviderUpdateTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "PutClusterCapacityProvidersRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UpdateClusterSettingsRequestRequestTypeDef",
-    "ContainerOverrideOutputTypeDef",
     "ContainerOverrideTypeDef",
-    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "ContainerInstanceHealthStatusTypeDef",
     "ContainerStateChangeTypeDef",
     "SubmitContainerStateChangeRequestRequestTypeDef",
     "ContainerTypeDef",
     "DeleteAttributesResponseTypeDef",
     "DiscoverPollEndpointResponseTypeDef",
@@ -217,87 +204,73 @@
     "SubmitContainerStateChangeResponseTypeDef",
     "SubmitTaskStateChangeResponseTypeDef",
     "UpdateTaskSetRequestRequestTypeDef",
     "DeleteAccountSettingResponseTypeDef",
     "ListAccountSettingsResponseTypeDef",
     "PutAccountSettingDefaultResponseTypeDef",
     "PutAccountSettingResponseTypeDef",
-    "DeploymentConfigurationOutputTypeDef",
     "DeploymentConfigurationTypeDef",
     "DescribeServicesRequestServicesInactiveWaitTypeDef",
     "DescribeServicesRequestServicesStableWaitTypeDef",
     "DescribeTasksRequestTasksRunningWaitTypeDef",
     "DescribeTasksRequestTasksStoppedWaitTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "ExecuteCommandConfigurationTypeDef",
     "ExecuteCommandResponseTypeDef",
     "FSxWindowsFileServerVolumeConfigurationTypeDef",
     "GetTaskProtectionResponseTypeDef",
     "UpdateTaskProtectionResponseTypeDef",
-    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "ListAccountSettingsRequestListAccountSettingsPaginateTypeDef",
     "ListAttributesRequestListAttributesPaginateTypeDef",
     "ListClustersRequestListClustersPaginateTypeDef",
     "ListContainerInstancesRequestListContainerInstancesPaginateTypeDef",
     "ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef",
     "ListServicesRequestListServicesPaginateTypeDef",
     "ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef",
     "ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef",
     "ListTasksRequestListTasksPaginateTypeDef",
-    "ResourceUnionTypeDef",
-    "ServiceConnectServiceOutputTypeDef",
+    "RegisterContainerInstanceRequestRequestTypeDef",
     "ServiceConnectServiceTypeDef",
-    "ProxyConfigurationUnionTypeDef",
     "CapacityProviderTypeDef",
     "CreateCapacityProviderRequestRequestTypeDef",
     "UpdateCapacityProviderRequestRequestTypeDef",
-    "TaskSetTypeDef",
     "CreateTaskSetRequestRequestTypeDef",
-    "NetworkConfigurationUnionTypeDef",
-    "TaskOverrideOutputTypeDef",
+    "TaskSetTypeDef",
     "TaskOverrideTypeDef",
     "ContainerInstanceTypeDef",
     "SubmitTaskStateChangeRequestRequestTypeDef",
-    "DeploymentConfigurationUnionTypeDef",
     "ClusterConfigurationTypeDef",
-    "VolumeOutputTypeDef",
     "VolumeTypeDef",
-    "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
-    "RegisterContainerInstanceRequestRequestTypeDef",
-    "ServiceConnectConfigurationOutputTypeDef",
     "ServiceConnectConfigurationTypeDef",
     "CreateCapacityProviderResponseTypeDef",
     "DeleteCapacityProviderResponseTypeDef",
     "DescribeCapacityProvidersResponseTypeDef",
     "UpdateCapacityProviderResponseTypeDef",
     "CreateTaskSetResponseTypeDef",
     "DeleteTaskSetResponseTypeDef",
     "DescribeTaskSetsResponseTypeDef",
     "UpdateServicePrimaryTaskSetResponseTypeDef",
     "UpdateTaskSetResponseTypeDef",
-    "TaskTypeDef",
     "RunTaskRequestRequestTypeDef",
     "StartTaskRequestRequestTypeDef",
-    "TaskOverrideUnionTypeDef",
+    "TaskTypeDef",
     "DeregisterContainerInstanceResponseTypeDef",
     "DescribeContainerInstancesResponseTypeDef",
     "RegisterContainerInstanceResponseTypeDef",
     "UpdateContainerAgentResponseTypeDef",
     "UpdateContainerInstancesStateResponseTypeDef",
     "ClusterTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
-    "VolumeUnionTypeDef",
+    "RegisterTaskDefinitionRequestRequestTypeDef",
     "TaskDefinitionTypeDef",
-    "ContainerDefinitionUnionTypeDef",
-    "DeploymentTypeDef",
     "CreateServiceRequestRequestTypeDef",
-    "ServiceConnectConfigurationUnionTypeDef",
+    "DeploymentTypeDef",
     "UpdateServiceRequestRequestTypeDef",
     "DescribeTasksResponseTypeDef",
     "RunTaskResponseTypeDef",
     "StartTaskResponseTypeDef",
     "StopTaskResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
@@ -305,15 +278,14 @@
     "PutClusterCapacityProvidersResponseTypeDef",
     "UpdateClusterResponseTypeDef",
     "UpdateClusterSettingsResponseTypeDef",
     "DeleteTaskDefinitionsResponseTypeDef",
     "DeregisterTaskDefinitionResponseTypeDef",
     "DescribeTaskDefinitionResponseTypeDef",
     "RegisterTaskDefinitionResponseTypeDef",
-    "RegisterTaskDefinitionRequestRequestTypeDef",
     "ServiceTypeDef",
     "CreateServiceResponseTypeDef",
     "DeleteServiceResponseTypeDef",
     "DescribeServicesResponseTypeDef",
     "UpdateServiceResponseTypeDef",
 )
 
@@ -361,34 +333,14 @@
         "minimumScalingStepSize": int,
         "maximumScalingStepSize": int,
         "instanceWarmupPeriod": int,
     },
     total=False,
 )
 
-_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAwsVpcConfigurationOutputTypeDef",
-    {
-        "subnets": List[str],
-    },
-)
-_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAwsVpcConfigurationOutputTypeDef",
-    {
-        "securityGroups": List[str],
-        "assignPublicIp": AssignPublicIpType,
-    },
-    total=False,
-)
-
-class AwsVpcConfigurationOutputTypeDef(
-    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
         "subnets": Sequence[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
@@ -470,53 +422,51 @@
     "EnvironmentFileTypeDef",
     {
         "value": str,
         "type": Literal["s3"],
     },
 )
 
-_RequiredFirelensConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFirelensConfigurationOutputTypeDef",
+_RequiredFirelensConfigurationTypeDef = TypedDict(
+    "_RequiredFirelensConfigurationTypeDef",
     {
         "type": FirelensConfigurationTypeType,
     },
 )
-_OptionalFirelensConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFirelensConfigurationOutputTypeDef",
+_OptionalFirelensConfigurationTypeDef = TypedDict(
+    "_OptionalFirelensConfigurationTypeDef",
     {
         "options": Dict[str, str],
     },
     total=False,
 )
 
-class FirelensConfigurationOutputTypeDef(
-    _RequiredFirelensConfigurationOutputTypeDef, _OptionalFirelensConfigurationOutputTypeDef
+class FirelensConfigurationTypeDef(
+    _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
 ):
     pass
 
-_RequiredHealthCheckOutputTypeDef = TypedDict(
-    "_RequiredHealthCheckOutputTypeDef",
+_RequiredHealthCheckTypeDef = TypedDict(
+    "_RequiredHealthCheckTypeDef",
     {
         "command": List[str],
     },
 )
-_OptionalHealthCheckOutputTypeDef = TypedDict(
-    "_OptionalHealthCheckOutputTypeDef",
+_OptionalHealthCheckTypeDef = TypedDict(
+    "_OptionalHealthCheckTypeDef",
     {
         "interval": int,
         "timeout": int,
         "retries": int,
         "startPeriod": int,
     },
     total=False,
 )
 
-class HealthCheckOutputTypeDef(
-    _RequiredHealthCheckOutputTypeDef, _OptionalHealthCheckOutputTypeDef
-):
+class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
 HostEntryTypeDef = TypedDict(
     "HostEntryTypeDef",
     {
         "hostname": str,
         "ipAddress": str,
@@ -592,66 +542,27 @@
     {
         "sourceContainer": str,
         "readOnly": bool,
     },
     total=False,
 )
 
-_RequiredFirelensConfigurationTypeDef = TypedDict(
-    "_RequiredFirelensConfigurationTypeDef",
-    {
-        "type": FirelensConfigurationTypeType,
-    },
-)
-_OptionalFirelensConfigurationTypeDef = TypedDict(
-    "_OptionalFirelensConfigurationTypeDef",
-    {
-        "options": Mapping[str, str],
-    },
-    total=False,
-)
-
-class FirelensConfigurationTypeDef(
-    _RequiredFirelensConfigurationTypeDef, _OptionalFirelensConfigurationTypeDef
-):
-    pass
-
-_RequiredHealthCheckTypeDef = TypedDict(
-    "_RequiredHealthCheckTypeDef",
-    {
-        "command": Sequence[str],
-    },
-)
-_OptionalHealthCheckTypeDef = TypedDict(
-    "_OptionalHealthCheckTypeDef",
-    {
-        "interval": int,
-        "timeout": int,
-        "retries": int,
-        "startPeriod": int,
-    },
-    total=False,
-)
-
-class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
-    pass
-
 InstanceHealthCheckResultTypeDef = TypedDict(
     "InstanceHealthCheckResultTypeDef",
     {
         "type": Literal["CONTAINER_RUNTIME"],
         "status": InstanceHealthCheckStateType,
         "lastUpdated": datetime,
         "lastStatusChange": datetime,
     },
     total=False,
 )
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
     {
         "name": str,
         "type": str,
         "doubleValue": float,
         "longValue": int,
         "integerValue": int,
         "stringSetValue": List[str],
@@ -868,23 +779,14 @@
 )
 
 class DeleteTaskSetRequestRequestTypeDef(
     _RequiredDeleteTaskSetRequestRequestTypeDef, _OptionalDeleteTaskSetRequestRequestTypeDef
 ):
     pass
 
-DeploymentAlarmsOutputTypeDef = TypedDict(
-    "DeploymentAlarmsOutputTypeDef",
-    {
-        "alarmNames": List[str],
-        "enable": bool,
-        "rollback": bool,
-    },
-)
-
 DeploymentAlarmsTypeDef = TypedDict(
     "DeploymentAlarmsTypeDef",
     {
         "alarmNames": Sequence[str],
         "enable": bool,
         "rollback": bool,
     },
@@ -1062,43 +964,25 @@
 )
 
 class DescribeTasksRequestRequestTypeDef(
     _RequiredDescribeTasksRequestRequestTypeDef, _OptionalDescribeTasksRequestRequestTypeDef
 ):
     pass
 
-_RequiredDeviceOutputTypeDef = TypedDict(
-    "_RequiredDeviceOutputTypeDef",
-    {
-        "hostPath": str,
-    },
-)
-_OptionalDeviceOutputTypeDef = TypedDict(
-    "_OptionalDeviceOutputTypeDef",
-    {
-        "containerPath": str,
-        "permissions": List[DeviceCgroupPermissionType],
-    },
-    total=False,
-)
-
-class DeviceOutputTypeDef(_RequiredDeviceOutputTypeDef, _OptionalDeviceOutputTypeDef):
-    pass
-
 _RequiredDeviceTypeDef = TypedDict(
     "_RequiredDeviceTypeDef",
     {
         "hostPath": str,
     },
 )
 _OptionalDeviceTypeDef = TypedDict(
     "_OptionalDeviceTypeDef",
     {
         "containerPath": str,
-        "permissions": Sequence[DeviceCgroupPermissionType],
+        "permissions": List[DeviceCgroupPermissionType],
     },
     total=False,
 )
 
 class DeviceTypeDef(_RequiredDeviceTypeDef, _OptionalDeviceTypeDef):
     pass
 
@@ -1107,34 +991,22 @@
     {
         "containerInstance": str,
         "cluster": str,
     },
     total=False,
 )
 
-DockerVolumeConfigurationOutputTypeDef = TypedDict(
-    "DockerVolumeConfigurationOutputTypeDef",
-    {
-        "scope": ScopeType,
-        "autoprovision": bool,
-        "driver": str,
-        "driverOpts": Dict[str, str],
-        "labels": Dict[str, str],
-    },
-    total=False,
-)
-
 DockerVolumeConfigurationTypeDef = TypedDict(
     "DockerVolumeConfigurationTypeDef",
     {
         "scope": ScopeType,
         "autoprovision": bool,
         "driver": str,
-        "driverOpts": Mapping[str, str],
-        "labels": Mapping[str, str],
+        "driverOpts": Dict[str, str],
+        "labels": Dict[str, str],
     },
     total=False,
 )
 
 EFSAuthorizationConfigTypeDef = TypedDict(
     "EFSAuthorizationConfigTypeDef",
     {
@@ -1253,61 +1125,34 @@
     "InferenceAcceleratorTypeDef",
     {
         "deviceName": str,
         "deviceType": str,
     },
 )
 
-KernelCapabilitiesOutputTypeDef = TypedDict(
-    "KernelCapabilitiesOutputTypeDef",
-    {
-        "add": List[str],
-        "drop": List[str],
-    },
-    total=False,
-)
-
 KernelCapabilitiesTypeDef = TypedDict(
     "KernelCapabilitiesTypeDef",
     {
-        "add": Sequence[str],
-        "drop": Sequence[str],
-    },
-    total=False,
-)
-
-_RequiredTmpfsOutputTypeDef = TypedDict(
-    "_RequiredTmpfsOutputTypeDef",
-    {
-        "containerPath": str,
-        "size": int,
-    },
-)
-_OptionalTmpfsOutputTypeDef = TypedDict(
-    "_OptionalTmpfsOutputTypeDef",
-    {
-        "mountOptions": List[str],
+        "add": List[str],
+        "drop": List[str],
     },
     total=False,
 )
 
-class TmpfsOutputTypeDef(_RequiredTmpfsOutputTypeDef, _OptionalTmpfsOutputTypeDef):
-    pass
-
 _RequiredTmpfsTypeDef = TypedDict(
     "_RequiredTmpfsTypeDef",
     {
         "containerPath": str,
         "size": int,
     },
 )
 _OptionalTmpfsTypeDef = TypedDict(
     "_OptionalTmpfsTypeDef",
     {
-        "mountOptions": Sequence[str],
+        "mountOptions": List[str],
     },
     total=False,
 )
 
 class TmpfsTypeDef(_RequiredTmpfsTypeDef, _OptionalTmpfsTypeDef):
     pass
 
@@ -1528,27 +1373,14 @@
     {
         "type": Literal["memberOf"],
         "expression": str,
     },
     total=False,
 )
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
-    {
-        "name": str,
-        "type": str,
-        "doubleValue": float,
-        "longValue": int,
-        "integerValue": int,
-        "stringSetValue": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredServiceConnectClientAliasTypeDef = TypedDict(
     "_RequiredServiceConnectClientAliasTypeDef",
     {
         "port": int,
     },
 )
 _OptionalServiceConnectClientAliasTypeDef = TypedDict(
@@ -1702,45 +1534,25 @@
         "type": str,
         "status": str,
         "details": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
-_RequiredProxyConfigurationOutputTypeDef = TypedDict(
-    "_RequiredProxyConfigurationOutputTypeDef",
-    {
-        "containerName": str,
-    },
-)
-_OptionalProxyConfigurationOutputTypeDef = TypedDict(
-    "_OptionalProxyConfigurationOutputTypeDef",
-    {
-        "type": Literal["APPMESH"],
-        "properties": List[KeyValuePairTypeDef],
-    },
-    total=False,
-)
-
-class ProxyConfigurationOutputTypeDef(
-    _RequiredProxyConfigurationOutputTypeDef, _OptionalProxyConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredProxyConfigurationTypeDef = TypedDict(
     "_RequiredProxyConfigurationTypeDef",
     {
         "containerName": str,
     },
 )
 _OptionalProxyConfigurationTypeDef = TypedDict(
     "_OptionalProxyConfigurationTypeDef",
     {
         "type": Literal["APPMESH"],
-        "properties": Sequence[KeyValuePairTypeDef],
+        "properties": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
 class ProxyConfigurationTypeDef(
     _RequiredProxyConfigurationTypeDef, _OptionalProxyConfigurationTypeDef
 ):
@@ -1809,22 +1621,14 @@
     {
         "managedScaling": ManagedScalingTypeDef,
         "managedTerminationProtection": ManagedTerminationProtectionType,
     },
     total=False,
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -1850,64 +1654,29 @@
     "UpdateClusterSettingsRequestRequestTypeDef",
     {
         "cluster": str,
         "settings": Sequence[ClusterSettingTypeDef],
     },
 )
 
-ContainerOverrideOutputTypeDef = TypedDict(
-    "ContainerOverrideOutputTypeDef",
+ContainerOverrideTypeDef = TypedDict(
+    "ContainerOverrideTypeDef",
     {
         "name": str,
         "command": List[str],
         "environment": List[KeyValuePairTypeDef],
         "environmentFiles": List[EnvironmentFileTypeDef],
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
         "resourceRequirements": List[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
-ContainerOverrideTypeDef = TypedDict(
-    "ContainerOverrideTypeDef",
-    {
-        "name": str,
-        "command": Sequence[str],
-        "environment": Sequence[KeyValuePairTypeDef],
-        "environmentFiles": Sequence[EnvironmentFileTypeDef],
-        "cpu": int,
-        "memory": int,
-        "memoryReservation": int,
-        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
-    },
-    total=False,
-)
-
-_RequiredLogConfigurationOutputTypeDef = TypedDict(
-    "_RequiredLogConfigurationOutputTypeDef",
-    {
-        "logDriver": LogDriverType,
-    },
-)
-_OptionalLogConfigurationOutputTypeDef = TypedDict(
-    "_OptionalLogConfigurationOutputTypeDef",
-    {
-        "options": Dict[str, str],
-        "secretOptions": List[SecretTypeDef],
-    },
-    total=False,
-)
-
-class LogConfigurationOutputTypeDef(
-    _RequiredLogConfigurationOutputTypeDef, _OptionalLogConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredLogConfigurationTypeDef = TypedDict(
     "_RequiredLogConfigurationTypeDef",
     {
         "logDriver": LogDriverType,
     },
 )
 _OptionalLogConfigurationTypeDef = TypedDict(
@@ -2153,25 +1922,14 @@
     "PutAccountSettingResponseTypeDef",
     {
         "setting": SettingTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeploymentConfigurationOutputTypeDef = TypedDict(
-    "DeploymentConfigurationOutputTypeDef",
-    {
-        "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
-        "maximumPercent": int,
-        "minimumHealthyPercent": int,
-        "alarms": DeploymentAlarmsOutputTypeDef,
-    },
-    total=False,
-)
-
 DeploymentConfigurationTypeDef = TypedDict(
     "DeploymentConfigurationTypeDef",
     {
         "deploymentCircuitBreaker": DeploymentCircuitBreakerTypeDef,
         "maximumPercent": int,
         "minimumHealthyPercent": int,
         "alarms": DeploymentAlarmsTypeDef,
@@ -2335,36 +2093,22 @@
     {
         "protectedTasks": List[ProtectedTaskTypeDef],
         "failures": List[FailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LinuxParametersOutputTypeDef = TypedDict(
-    "LinuxParametersOutputTypeDef",
-    {
-        "capabilities": KernelCapabilitiesOutputTypeDef,
-        "devices": List[DeviceOutputTypeDef],
-        "initProcessEnabled": bool,
-        "sharedMemorySize": int,
-        "tmpfs": List[TmpfsOutputTypeDef],
-        "maxSwap": int,
-        "swappiness": int,
-    },
-    total=False,
-)
-
 LinuxParametersTypeDef = TypedDict(
     "LinuxParametersTypeDef",
     {
         "capabilities": KernelCapabilitiesTypeDef,
-        "devices": Sequence[DeviceTypeDef],
+        "devices": List[DeviceTypeDef],
         "initProcessEnabled": bool,
         "sharedMemorySize": int,
-        "tmpfs": Sequence[TmpfsTypeDef],
+        "tmpfs": List[TmpfsTypeDef],
         "maxSwap": int,
         "swappiness": int,
     },
     total=False,
 )
 
 ListAccountSettingsRequestListAccountSettingsPaginateTypeDef = TypedDict(
@@ -2484,36 +2228,30 @@
         "desiredStatus": DesiredStatusType,
         "launchType": LaunchTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
-_RequiredServiceConnectServiceOutputTypeDef = TypedDict(
-    "_RequiredServiceConnectServiceOutputTypeDef",
-    {
-        "portName": str,
-    },
-)
-_OptionalServiceConnectServiceOutputTypeDef = TypedDict(
-    "_OptionalServiceConnectServiceOutputTypeDef",
+RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
+    "RegisterContainerInstanceRequestRequestTypeDef",
     {
-        "discoveryName": str,
-        "clientAliases": List[ServiceConnectClientAliasTypeDef],
-        "ingressPortOverride": int,
+        "cluster": str,
+        "instanceIdentityDocument": str,
+        "instanceIdentityDocumentSignature": str,
+        "totalResources": Sequence[ResourceTypeDef],
+        "versionInfo": VersionInfoTypeDef,
+        "containerInstanceArn": str,
+        "attributes": Sequence[AttributeTypeDef],
+        "platformDevices": Sequence[PlatformDeviceTypeDef],
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class ServiceConnectServiceOutputTypeDef(
-    _RequiredServiceConnectServiceOutputTypeDef, _OptionalServiceConnectServiceOutputTypeDef
-):
-    pass
-
 _RequiredServiceConnectServiceTypeDef = TypedDict(
     "_RequiredServiceConnectServiceTypeDef",
     {
         "portName": str,
     },
 )
 _OptionalServiceConnectServiceTypeDef = TypedDict(
@@ -2527,15 +2265,14 @@
 )
 
 class ServiceConnectServiceTypeDef(
     _RequiredServiceConnectServiceTypeDef, _OptionalServiceConnectServiceTypeDef
 ):
     pass
 
-ProxyConfigurationUnionTypeDef = Union[ProxyConfigurationTypeDef, ProxyConfigurationOutputTypeDef]
 CapacityProviderTypeDef = TypedDict(
     "CapacityProviderTypeDef",
     {
         "capacityProviderArn": str,
         "name": str,
         "status": CapacityProviderStatusType,
         "autoScalingGroupProvider": AutoScalingGroupProviderTypeDef,
@@ -2571,45 +2308,14 @@
     "UpdateCapacityProviderRequestRequestTypeDef",
     {
         "name": str,
         "autoScalingGroupProvider": AutoScalingGroupProviderUpdateTypeDef,
     },
 )
 
-TaskSetTypeDef = TypedDict(
-    "TaskSetTypeDef",
-    {
-        "id": str,
-        "taskSetArn": str,
-        "serviceArn": str,
-        "clusterArn": str,
-        "startedBy": str,
-        "externalId": str,
-        "status": str,
-        "taskDefinition": str,
-        "computedDesiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "launchType": LaunchTypeType,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
-        "loadBalancers": List[LoadBalancerTypeDef],
-        "serviceRegistries": List[ServiceRegistryTypeDef],
-        "scale": ScaleTypeDef,
-        "stabilityStatus": StabilityStatusType,
-        "stabilityStatusAt": datetime,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 _RequiredCreateTaskSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTaskSetRequestRequestTypeDef",
     {
         "service": str,
         "cluster": str,
         "taskDefinition": str,
     },
@@ -2632,37 +2338,51 @@
 )
 
 class CreateTaskSetRequestRequestTypeDef(
     _RequiredCreateTaskSetRequestRequestTypeDef, _OptionalCreateTaskSetRequestRequestTypeDef
 ):
     pass
 
-NetworkConfigurationUnionTypeDef = Union[
-    NetworkConfigurationTypeDef, NetworkConfigurationOutputTypeDef
-]
-TaskOverrideOutputTypeDef = TypedDict(
-    "TaskOverrideOutputTypeDef",
+TaskSetTypeDef = TypedDict(
+    "TaskSetTypeDef",
     {
-        "containerOverrides": List[ContainerOverrideOutputTypeDef],
-        "cpu": str,
-        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
-        "executionRoleArn": str,
-        "memory": str,
-        "taskRoleArn": str,
-        "ephemeralStorage": EphemeralStorageTypeDef,
+        "id": str,
+        "taskSetArn": str,
+        "serviceArn": str,
+        "clusterArn": str,
+        "startedBy": str,
+        "externalId": str,
+        "status": str,
+        "taskDefinition": str,
+        "computedDesiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "launchType": LaunchTypeType,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "loadBalancers": List[LoadBalancerTypeDef],
+        "serviceRegistries": List[ServiceRegistryTypeDef],
+        "scale": ScaleTypeDef,
+        "stabilityStatus": StabilityStatusType,
+        "stabilityStatusAt": datetime,
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 TaskOverrideTypeDef = TypedDict(
     "TaskOverrideTypeDef",
     {
-        "containerOverrides": Sequence[ContainerOverrideTypeDef],
+        "containerOverrides": List[ContainerOverrideTypeDef],
         "cpu": str,
-        "inferenceAcceleratorOverrides": Sequence[InferenceAcceleratorOverrideTypeDef],
+        "inferenceAcceleratorOverrides": List[InferenceAcceleratorOverrideTypeDef],
         "executionRoleArn": str,
         "memory": str,
         "taskRoleArn": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
@@ -2671,16 +2391,16 @@
     "ContainerInstanceTypeDef",
     {
         "containerInstanceArn": str,
         "ec2InstanceId": str,
         "capacityProviderName": str,
         "version": int,
         "versionInfo": VersionInfoTypeDef,
-        "remainingResources": List[ResourceOutputTypeDef],
-        "registeredResources": List[ResourceOutputTypeDef],
+        "remainingResources": List[ResourceTypeDef],
+        "registeredResources": List[ResourceTypeDef],
         "status": str,
         "statusReason": str,
         "agentConnected": bool,
         "runningTasksCount": int,
         "pendingTasksCount": int,
         "agentUpdateStatus": AgentUpdateStatusType,
         "attributes": List[AttributeTypeDef],
@@ -2705,51 +2425,36 @@
         "pullStartedAt": TimestampTypeDef,
         "pullStoppedAt": TimestampTypeDef,
         "executionStoppedAt": TimestampTypeDef,
     },
     total=False,
 )
 
-DeploymentConfigurationUnionTypeDef = Union[
-    DeploymentConfigurationTypeDef, DeploymentConfigurationOutputTypeDef
-]
 ClusterConfigurationTypeDef = TypedDict(
     "ClusterConfigurationTypeDef",
     {
         "executeCommandConfiguration": ExecuteCommandConfigurationTypeDef,
     },
     total=False,
 )
 
-VolumeOutputTypeDef = TypedDict(
-    "VolumeOutputTypeDef",
-    {
-        "name": str,
-        "host": HostVolumePropertiesTypeDef,
-        "dockerVolumeConfiguration": DockerVolumeConfigurationOutputTypeDef,
-        "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
-        "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
-    },
-    total=False,
-)
-
 VolumeTypeDef = TypedDict(
     "VolumeTypeDef",
     {
         "name": str,
         "host": HostVolumePropertiesTypeDef,
         "dockerVolumeConfiguration": DockerVolumeConfigurationTypeDef,
         "efsVolumeConfiguration": EFSVolumeConfigurationTypeDef,
         "fsxWindowsFileServerVolumeConfiguration": FSxWindowsFileServerVolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-ContainerDefinitionOutputTypeDef = TypedDict(
-    "ContainerDefinitionOutputTypeDef",
+ContainerDefinitionTypeDef = TypedDict(
+    "ContainerDefinitionTypeDef",
     {
         "name": str,
         "image": str,
         "repositoryCredentials": RepositoryCredentialsTypeDef,
         "cpu": int,
         "memory": int,
         "memoryReservation": int,
@@ -2758,15 +2463,15 @@
         "essential": bool,
         "entryPoint": List[str],
         "command": List[str],
         "environment": List[KeyValuePairTypeDef],
         "environmentFiles": List[EnvironmentFileTypeDef],
         "mountPoints": List[MountPointTypeDef],
         "volumesFrom": List[VolumeFromTypeDef],
-        "linuxParameters": LinuxParametersOutputTypeDef,
+        "linuxParameters": LinuxParametersTypeDef,
         "secrets": List[SecretTypeDef],
         "dependsOn": List[ContainerDependencyTypeDef],
         "startTimeout": int,
         "stopTimeout": int,
         "hostname": str,
         "user": str,
         "workingDirectory": str,
@@ -2777,107 +2482,23 @@
         "dnsSearchDomains": List[str],
         "extraHosts": List[HostEntryTypeDef],
         "dockerSecurityOptions": List[str],
         "interactive": bool,
         "pseudoTerminal": bool,
         "dockerLabels": Dict[str, str],
         "ulimits": List[UlimitTypeDef],
-        "logConfiguration": LogConfigurationOutputTypeDef,
-        "healthCheck": HealthCheckOutputTypeDef,
-        "systemControls": List[SystemControlTypeDef],
-        "resourceRequirements": List[ResourceRequirementTypeDef],
-        "firelensConfiguration": FirelensConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-ContainerDefinitionTypeDef = TypedDict(
-    "ContainerDefinitionTypeDef",
-    {
-        "name": str,
-        "image": str,
-        "repositoryCredentials": RepositoryCredentialsTypeDef,
-        "cpu": int,
-        "memory": int,
-        "memoryReservation": int,
-        "links": Sequence[str],
-        "portMappings": Sequence[PortMappingTypeDef],
-        "essential": bool,
-        "entryPoint": Sequence[str],
-        "command": Sequence[str],
-        "environment": Sequence[KeyValuePairTypeDef],
-        "environmentFiles": Sequence[EnvironmentFileTypeDef],
-        "mountPoints": Sequence[MountPointTypeDef],
-        "volumesFrom": Sequence[VolumeFromTypeDef],
-        "linuxParameters": LinuxParametersTypeDef,
-        "secrets": Sequence[SecretTypeDef],
-        "dependsOn": Sequence[ContainerDependencyTypeDef],
-        "startTimeout": int,
-        "stopTimeout": int,
-        "hostname": str,
-        "user": str,
-        "workingDirectory": str,
-        "disableNetworking": bool,
-        "privileged": bool,
-        "readonlyRootFilesystem": bool,
-        "dnsServers": Sequence[str],
-        "dnsSearchDomains": Sequence[str],
-        "extraHosts": Sequence[HostEntryTypeDef],
-        "dockerSecurityOptions": Sequence[str],
-        "interactive": bool,
-        "pseudoTerminal": bool,
-        "dockerLabels": Mapping[str, str],
-        "ulimits": Sequence[UlimitTypeDef],
         "logConfiguration": LogConfigurationTypeDef,
         "healthCheck": HealthCheckTypeDef,
-        "systemControls": Sequence[SystemControlTypeDef],
-        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
+        "systemControls": List[SystemControlTypeDef],
+        "resourceRequirements": List[ResourceRequirementTypeDef],
         "firelensConfiguration": FirelensConfigurationTypeDef,
     },
     total=False,
 )
 
-RegisterContainerInstanceRequestRequestTypeDef = TypedDict(
-    "RegisterContainerInstanceRequestRequestTypeDef",
-    {
-        "cluster": str,
-        "instanceIdentityDocument": str,
-        "instanceIdentityDocumentSignature": str,
-        "totalResources": Sequence[ResourceUnionTypeDef],
-        "versionInfo": VersionInfoTypeDef,
-        "containerInstanceArn": str,
-        "attributes": Sequence[AttributeTypeDef],
-        "platformDevices": Sequence[PlatformDeviceTypeDef],
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-_RequiredServiceConnectConfigurationOutputTypeDef = TypedDict(
-    "_RequiredServiceConnectConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalServiceConnectConfigurationOutputTypeDef = TypedDict(
-    "_OptionalServiceConnectConfigurationOutputTypeDef",
-    {
-        "namespace": str,
-        "services": List[ServiceConnectServiceOutputTypeDef],
-        "logConfiguration": LogConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class ServiceConnectConfigurationOutputTypeDef(
-    _RequiredServiceConnectConfigurationOutputTypeDef,
-    _OptionalServiceConnectConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredServiceConnectConfigurationTypeDef = TypedDict(
     "_RequiredServiceConnectConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalServiceConnectConfigurationTypeDef = TypedDict(
@@ -2966,57 +2587,14 @@
     "UpdateTaskSetResponseTypeDef",
     {
         "taskSet": TaskSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TaskTypeDef = TypedDict(
-    "TaskTypeDef",
-    {
-        "attachments": List[AttachmentTypeDef],
-        "attributes": List[AttributeTypeDef],
-        "availabilityZone": str,
-        "capacityProviderName": str,
-        "clusterArn": str,
-        "connectivity": ConnectivityType,
-        "connectivityAt": datetime,
-        "containerInstanceArn": str,
-        "containers": List[ContainerTypeDef],
-        "cpu": str,
-        "createdAt": datetime,
-        "desiredStatus": str,
-        "enableExecuteCommand": bool,
-        "executionStoppedAt": datetime,
-        "group": str,
-        "healthStatus": HealthStatusType,
-        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
-        "lastStatus": str,
-        "launchType": LaunchTypeType,
-        "memory": str,
-        "overrides": TaskOverrideOutputTypeDef,
-        "platformVersion": str,
-        "platformFamily": str,
-        "pullStartedAt": datetime,
-        "pullStoppedAt": datetime,
-        "startedAt": datetime,
-        "startedBy": str,
-        "stopCode": TaskStopCodeType,
-        "stoppedAt": datetime,
-        "stoppedReason": str,
-        "stoppingAt": datetime,
-        "tags": List[TagTypeDef],
-        "taskArn": str,
-        "taskDefinitionArn": str,
-        "version": int,
-        "ephemeralStorage": EphemeralStorageTypeDef,
-    },
-    total=False,
-)
-
 _RequiredRunTaskRequestRequestTypeDef = TypedDict(
     "_RequiredRunTaskRequestRequestTypeDef",
     {
         "taskDefinition": str,
     },
 )
 _OptionalRunTaskRequestRequestTypeDef = TypedDict(
@@ -3072,15 +2650,57 @@
 )
 
 class StartTaskRequestRequestTypeDef(
     _RequiredStartTaskRequestRequestTypeDef, _OptionalStartTaskRequestRequestTypeDef
 ):
     pass
 
-TaskOverrideUnionTypeDef = Union[TaskOverrideTypeDef, TaskOverrideOutputTypeDef]
+TaskTypeDef = TypedDict(
+    "TaskTypeDef",
+    {
+        "attachments": List[AttachmentTypeDef],
+        "attributes": List[AttributeTypeDef],
+        "availabilityZone": str,
+        "capacityProviderName": str,
+        "clusterArn": str,
+        "connectivity": ConnectivityType,
+        "connectivityAt": datetime,
+        "containerInstanceArn": str,
+        "containers": List[ContainerTypeDef],
+        "cpu": str,
+        "createdAt": datetime,
+        "desiredStatus": str,
+        "enableExecuteCommand": bool,
+        "executionStoppedAt": datetime,
+        "group": str,
+        "healthStatus": HealthStatusType,
+        "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
+        "lastStatus": str,
+        "launchType": LaunchTypeType,
+        "memory": str,
+        "overrides": TaskOverrideTypeDef,
+        "platformVersion": str,
+        "platformFamily": str,
+        "pullStartedAt": datetime,
+        "pullStoppedAt": datetime,
+        "startedAt": datetime,
+        "startedBy": str,
+        "stopCode": TaskStopCodeType,
+        "stoppedAt": datetime,
+        "stoppedReason": str,
+        "stoppingAt": datetime,
+        "tags": List[TagTypeDef],
+        "taskArn": str,
+        "taskDefinitionArn": str,
+        "version": int,
+        "ephemeralStorage": EphemeralStorageTypeDef,
+    },
+    total=False,
+)
+
 DeregisterContainerInstanceResponseTypeDef = TypedDict(
     "DeregisterContainerInstanceResponseTypeDef",
     {
         "containerInstance": ContainerInstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3173,74 +2793,80 @@
 )
 
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
-VolumeUnionTypeDef = Union[VolumeTypeDef, VolumeOutputTypeDef]
+_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "family": str,
+        "containerDefinitions": Sequence[ContainerDefinitionTypeDef],
+    },
+)
+_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
+    {
+        "taskRoleArn": str,
+        "executionRoleArn": str,
+        "networkMode": NetworkModeType,
+        "volumes": Sequence[VolumeTypeDef],
+        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
+        "requiresCompatibilities": Sequence[CompatibilityType],
+        "cpu": str,
+        "memory": str,
+        "tags": Sequence[TagTypeDef],
+        "pidMode": PidModeType,
+        "ipcMode": IpcModeType,
+        "proxyConfiguration": ProxyConfigurationTypeDef,
+        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
+        "ephemeralStorage": EphemeralStorageTypeDef,
+        "runtimePlatform": RuntimePlatformTypeDef,
+    },
+    total=False,
+)
+
+class RegisterTaskDefinitionRequestRequestTypeDef(
+    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
+    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
+):
+    pass
+
 TaskDefinitionTypeDef = TypedDict(
     "TaskDefinitionTypeDef",
     {
         "taskDefinitionArn": str,
-        "containerDefinitions": List[ContainerDefinitionOutputTypeDef],
+        "containerDefinitions": List[ContainerDefinitionTypeDef],
         "family": str,
         "taskRoleArn": str,
         "executionRoleArn": str,
         "networkMode": NetworkModeType,
         "revision": int,
-        "volumes": List[VolumeOutputTypeDef],
+        "volumes": List[VolumeTypeDef],
         "status": TaskDefinitionStatusType,
         "requiresAttributes": List[AttributeTypeDef],
         "placementConstraints": List[TaskDefinitionPlacementConstraintTypeDef],
         "compatibilities": List[CompatibilityType],
         "runtimePlatform": RuntimePlatformTypeDef,
         "requiresCompatibilities": List[CompatibilityType],
         "cpu": str,
         "memory": str,
         "inferenceAccelerators": List[InferenceAcceleratorTypeDef],
         "pidMode": PidModeType,
         "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationOutputTypeDef,
+        "proxyConfiguration": ProxyConfigurationTypeDef,
         "registeredAt": datetime,
         "deregisteredAt": datetime,
         "registeredBy": str,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
-ContainerDefinitionUnionTypeDef = Union[
-    ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef
-]
-DeploymentTypeDef = TypedDict(
-    "DeploymentTypeDef",
-    {
-        "id": str,
-        "status": str,
-        "taskDefinition": str,
-        "desiredCount": int,
-        "pendingCount": int,
-        "runningCount": int,
-        "failedTasks": int,
-        "createdAt": datetime,
-        "updatedAt": datetime,
-        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "launchType": LaunchTypeType,
-        "platformVersion": str,
-        "platformFamily": str,
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
-        "rolloutState": DeploymentRolloutStateType,
-        "rolloutStateReason": str,
-        "serviceConnectConfiguration": ServiceConnectConfigurationOutputTypeDef,
-        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
-    },
-    total=False,
-)
-
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 _OptionalCreateServiceRequestRequestTypeDef = TypedDict(
@@ -3273,17 +2899,39 @@
 )
 
 class CreateServiceRequestRequestTypeDef(
     _RequiredCreateServiceRequestRequestTypeDef, _OptionalCreateServiceRequestRequestTypeDef
 ):
     pass
 
-ServiceConnectConfigurationUnionTypeDef = Union[
-    ServiceConnectConfigurationTypeDef, ServiceConnectConfigurationOutputTypeDef
-]
+DeploymentTypeDef = TypedDict(
+    "DeploymentTypeDef",
+    {
+        "id": str,
+        "status": str,
+        "taskDefinition": str,
+        "desiredCount": int,
+        "pendingCount": int,
+        "runningCount": int,
+        "failedTasks": int,
+        "createdAt": datetime,
+        "updatedAt": datetime,
+        "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
+        "launchType": LaunchTypeType,
+        "platformVersion": str,
+        "platformFamily": str,
+        "networkConfiguration": NetworkConfigurationTypeDef,
+        "rolloutState": DeploymentRolloutStateType,
+        "rolloutStateReason": str,
+        "serviceConnectConfiguration": ServiceConnectConfigurationTypeDef,
+        "serviceConnectResources": List[ServiceConnectServiceResourceTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServiceRequestRequestTypeDef",
     {
         "service": str,
     },
 )
 _OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
@@ -3430,49 +3078,14 @@
     {
         "taskDefinition": TaskDefinitionTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "family": str,
-        "containerDefinitions": Sequence[ContainerDefinitionUnionTypeDef],
-    },
-)
-_OptionalRegisterTaskDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterTaskDefinitionRequestRequestTypeDef",
-    {
-        "taskRoleArn": str,
-        "executionRoleArn": str,
-        "networkMode": NetworkModeType,
-        "volumes": Sequence[VolumeUnionTypeDef],
-        "placementConstraints": Sequence[TaskDefinitionPlacementConstraintTypeDef],
-        "requiresCompatibilities": Sequence[CompatibilityType],
-        "cpu": str,
-        "memory": str,
-        "tags": Sequence[TagTypeDef],
-        "pidMode": PidModeType,
-        "ipcMode": IpcModeType,
-        "proxyConfiguration": ProxyConfigurationTypeDef,
-        "inferenceAccelerators": Sequence[InferenceAcceleratorTypeDef],
-        "ephemeralStorage": EphemeralStorageTypeDef,
-        "runtimePlatform": RuntimePlatformTypeDef,
-    },
-    total=False,
-)
-
-class RegisterTaskDefinitionRequestRequestTypeDef(
-    _RequiredRegisterTaskDefinitionRequestRequestTypeDef,
-    _OptionalRegisterTaskDefinitionRequestRequestTypeDef,
-):
-    pass
-
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "serviceArn": str,
         "serviceName": str,
         "clusterArn": str,
         "loadBalancers": List[LoadBalancerTypeDef],
@@ -3482,23 +3095,23 @@
         "runningCount": int,
         "pendingCount": int,
         "launchType": LaunchTypeType,
         "capacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "platformVersion": str,
         "platformFamily": str,
         "taskDefinition": str,
-        "deploymentConfiguration": DeploymentConfigurationOutputTypeDef,
+        "deploymentConfiguration": DeploymentConfigurationTypeDef,
         "taskSets": List[TaskSetTypeDef],
         "deployments": List[DeploymentTypeDef],
         "roleArn": str,
         "events": List[ServiceEventTypeDef],
         "createdAt": datetime,
         "placementConstraints": List[PlacementConstraintTypeDef],
         "placementStrategy": List[PlacementStrategyTypeDef],
-        "networkConfiguration": NetworkConfigurationOutputTypeDef,
+        "networkConfiguration": NetworkConfigurationTypeDef,
         "healthCheckGracePeriodSeconds": int,
         "schedulingStrategy": SchedulingStrategyType,
         "deploymentController": DeploymentControllerTypeDef,
         "tags": List[TagTypeDef],
         "createdBy": str,
         "enableECSManagedTags": bool,
         "propagateTags": PropagateTagsType,
```

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/waiter.py` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs/waiter.pyi` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecs-2.5.2.post1/types_aiobotocore_ecs.egg-info/SOURCES.txt` & `types-aiobotocore-ecs-2.5.2.post2/types_aiobotocore_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

