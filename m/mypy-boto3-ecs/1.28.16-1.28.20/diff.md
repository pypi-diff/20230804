# Comparing `tmp/mypy-boto3-ecs-1.28.16.tar.gz` & `tmp/mypy-boto3-ecs-1.28.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ecs-1.28.16.tar", last modified: Tue Aug  1 11:36:42 2023, max compression
+gzip compressed data, was "mypy-boto3-ecs-1.28.20.tar", last modified: Fri Aug  4 19:47:53 2023, max compression
```

## Comparing `mypy-boto3-ecs-1.28.16.tar` & `mypy-boto3-ecs-1.28.20.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.440901 mypy-boto3-ecs-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-08-01 11:36:42.432901 mypy-boto3-ecs-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23931 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.428901 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50078 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    50002 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15762 2023-08-01 11:16:58.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15760 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    96742 2023-08-01 11:17:00.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    96623 2023-08-01 11:16:59.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-08-01 11:16:56.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:42.432901 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 11:36:42.000000 mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:42.440901 mypy-boto3-ecs-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-01 11:16:55.000000 mypy-boto3-ecs-1.28.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:47:53.020761 mypy-boto3-ecs-1.28.20/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 19:47:11.000000 mypy-boto3-ecs-1.28.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-08-04 19:47:53.020761 mypy-boto3-ecs-1.28.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-08-04 19:47:11.000000 mypy-boto3-ecs-1.28.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:47:53.016761 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-08-04 19:47:11.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-04 19:47:11.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-04 19:47:11.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49963 2023-08-04 19:47:12.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49887 2023-08-04 19:47:11.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15782 2023-08-04 19:47:13.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-08-04 19:47:13.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-08-04 19:47:12.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-08-04 19:47:12.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:47:11.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    85504 2023-08-04 19:47:15.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85403 2023-08-04 19:47:14.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-04 19:47:11.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-08-04 19:47:12.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-08-04 19:47:12.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:47:53.020761 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-08-04 19:47:52.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-04 19:47:52.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:47:52.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:47:52.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 19:47:52.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 19:47:52.000000 mypy-boto3-ecs-1.28.20/mypy_boto3_ecs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:47:53.020761 mypy-boto3-ecs-1.28.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-04 19:47:11.000000 mypy-boto3-ecs-1.28.20/setup.py
```

### Comparing `mypy-boto3-ecs-1.28.16/LICENSE` & `mypy-boto3-ecs-1.28.20/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__init__.py` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__init__.pyi` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/__main__.py` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ECS 1.28.16\nVersion:         1.28.16\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for boto3.ECS 1.28.20\nVersion:         1.28.20\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.16")
+    print("1.28.20")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/client.py` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,28 +51,28 @@
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
@@ -93,51 +93,51 @@
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
@@ -263,26 +263,26 @@
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_service)
@@ -291,15 +291,15 @@
     def create_task_set(
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
@@ -734,15 +734,15 @@
 
     def register_container_instance(
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
@@ -752,27 +752,27 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#register_container_instance)
         """
 
     def register_task_definition(
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
@@ -788,16 +788,16 @@
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
@@ -814,16 +814,16 @@
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
@@ -972,27 +972,27 @@
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_service)
         """
```

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/client.pyi` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -51,28 +51,28 @@
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
@@ -93,51 +93,51 @@
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
@@ -254,26 +254,26 @@
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#create_service)
@@ -281,15 +281,15 @@
     def create_task_set(
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
@@ -689,15 +689,15 @@
         """
     def register_container_instance(
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
@@ -706,27 +706,27 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client.register_container_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#register_container_instance)
         """
     def register_task_definition(
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
@@ -741,16 +741,16 @@
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
@@ -766,16 +766,16 @@
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
@@ -912,27 +912,27 @@
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
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ecs/client/#update_service)
         """
```

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/literals.py` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,14 +619,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/literals.pyi` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -617,14 +617,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/paginator.py` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/paginator.pyi` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/type_defs.py` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/type_defs.py`

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
@@ -2880,111 +2569,24 @@
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
-        "credentialSpecs": List[str],
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
-        "credentialSpecs": Sequence[str],
-    },
-    total=False,
-)
-
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
+        "credentialSpecs": List[str],
     },
     total=False,
 )
 
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
@@ -3075,57 +2677,14 @@
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
@@ -3185,15 +2744,57 @@
 
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
@@ -3288,74 +2889,82 @@
 
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
@@ -3390,17 +2999,39 @@
 
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
@@ -3549,51 +3180,14 @@
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
@@ -3603,23 +3197,23 @@
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

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/type_defs.pyi` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/type_defs.pyi`

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
@@ -2777,109 +2482,24 @@
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
-        "credentialSpecs": List[str],
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
-        "credentialSpecs": Sequence[str],
-    },
-    total=False,
-)
-
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
+        "credentialSpecs": List[str],
     },
     total=False,
 )
 
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
@@ -2968,57 +2588,14 @@
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
@@ -3074,15 +2651,57 @@
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
@@ -3175,74 +2794,80 @@
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
@@ -3275,17 +2900,39 @@
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
@@ -3432,49 +3079,14 @@
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
@@ -3484,23 +3096,23 @@
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

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/waiter.py` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs/waiter.pyi` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.16/mypy_boto3_ecs.egg-info/SOURCES.txt` & `mypy-boto3-ecs-1.28.20/mypy_boto3_ecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ecs-1.28.16/setup.py` & `mypy-boto3-ecs-1.28.20/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ecs",
-    version="1.28.16",
+    version="1.28.20",
     packages=["mypy_boto3_ecs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ECS 1.28.16 service generated with mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.ECS 1.28.20 service generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

