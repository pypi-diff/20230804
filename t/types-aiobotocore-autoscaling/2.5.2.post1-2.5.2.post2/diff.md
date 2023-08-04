# Comparing `tmp/types-aiobotocore-autoscaling-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-autoscaling-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-autoscaling-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-autoscaling-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:28 2023, max compression
```

## Comparing `types-aiobotocore-autoscaling-2.5.2.post1.tar` & `types-aiobotocore-autoscaling-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.141648 types-aiobotocore-autoscaling-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-08-02 14:51:55.141648 types-aiobotocore-autoscaling-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.141648 types-aiobotocore-autoscaling-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.137648 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55242 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55158 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-08-02 14:33:38.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    86393 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    86258 2023-08-02 14:33:38.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:37.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.141648 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24094 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:51:54.000000 types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.199221 types-aiobotocore-autoscaling-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:47.000000 types-aiobotocore-autoscaling-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-08-04 12:00:28.195221 types-aiobotocore-autoscaling-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-08-04 11:40:47.000000 types-aiobotocore-autoscaling-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:28.199221 types-aiobotocore-autoscaling-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-04 11:40:47.000000 types-aiobotocore-autoscaling-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.195221 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-08-04 11:40:48.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-08-04 11:40:47.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-04 11:40:48.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55187 2023-08-04 11:40:48.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55103 2023-08-04 11:40:48.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13612 2023-08-04 11:40:48.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-08-04 11:40:48.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-08-04 11:40:48.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-08-04 11:40:48.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:48.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75359 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75242 2023-08-04 11:40:50.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:47.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.195221 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-08-04 12:00:27.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-04 12:00:28.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:27.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:27.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:27.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 12:00:28.000000 types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/LICENSE` & `types-aiobotocore-autoscaling-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/setup.py` & `types-aiobotocore-autoscaling-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-autoscaling",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AutoScaling 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__init__.py` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__init__.pyi` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/__main__.py` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AutoScaling 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.AutoScaling 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling\nOther"
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

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/client.py` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,41 +51,41 @@
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     DescribeWarmPoolAnswerTypeDef,
-    DesiredConfigurationUnionTypeDef,
+    DesiredConfigurationTypeDef,
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     FilterTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     InstanceReusePolicyTypeDef,
     LaunchConfigurationsTypeTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
-    MixedInstancesPolicyUnionTypeDef,
+    MixedInstancesPolicyTypeDef,
     PoliciesTypeTypeDef,
     PolicyARNTypeTypeDef,
-    PredictiveScalingConfigurationUnionTypeDef,
+    PredictiveScalingConfigurationTypeDef,
     ProcessesTypeTypeDef,
-    RefreshPreferencesUnionTypeDef,
+    RefreshPreferencesTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     ScheduledActionsTypeTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     StepAdjustmentTypeDef,
     TagsTypeTypeDef,
     TagTypeDef,
-    TargetTrackingConfigurationUnionTypeDef,
+    TargetTrackingConfigurationTypeDef,
     TimestampTypeDef,
     TrafficSourceIdentifierTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -245,15 +245,15 @@
         self,
         *,
         AutoScalingGroupName: str,
         MinSize: int,
         MaxSize: int,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
         InstanceId: str = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         LoadBalancerNames: Sequence[str] = ...,
         TargetGroupARNs: Sequence[str] = ...,
         HealthCheckType: str = ...,
@@ -819,17 +819,17 @@
         MinAdjustmentStep: int = ...,
         MinAdjustmentMagnitude: int = ...,
         ScalingAdjustment: int = ...,
         Cooldown: int = ...,
         MetricAggregationType: str = ...,
         StepAdjustments: Sequence[StepAdjustmentTypeDef] = ...,
         EstimatedInstanceWarmup: int = ...,
-        TargetTrackingConfiguration: TargetTrackingConfigurationUnionTypeDef = ...,
+        TargetTrackingConfiguration: TargetTrackingConfigurationTypeDef = ...,
         Enabled: bool = ...,
-        PredictiveScalingConfiguration: PredictiveScalingConfigurationUnionTypeDef = ...
+        PredictiveScalingConfiguration: PredictiveScalingConfigurationTypeDef = ...
     ) -> PolicyARNTypeTypeDef:
         """
         Creates or updates a scaling policy for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_scaling_policy)
         """
@@ -940,16 +940,16 @@
         """
 
     async def start_instance_refresh(
         self,
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
-        DesiredConfiguration: DesiredConfigurationUnionTypeDef = ...,
-        Preferences: RefreshPreferencesUnionTypeDef = ...
+        DesiredConfiguration: DesiredConfigurationTypeDef = ...,
+        Preferences: RefreshPreferencesTypeDef = ...
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
         Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#start_instance_refresh)
         """
@@ -977,15 +977,15 @@
 
     async def update_auto_scaling_group(
         self,
         *,
         AutoScalingGroupName: str,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         HealthCheckType: str = ...,
         HealthCheckGracePeriod: int = ...,
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/client.pyi` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -51,41 +51,41 @@
     DescribeLoadBalancersResponseTypeDef,
     DescribeLoadBalancerTargetGroupsResponseTypeDef,
     DescribeMetricCollectionTypesAnswerTypeDef,
     DescribeNotificationConfigurationsAnswerTypeDef,
     DescribeTerminationPolicyTypesAnswerTypeDef,
     DescribeTrafficSourcesResponseTypeDef,
     DescribeWarmPoolAnswerTypeDef,
-    DesiredConfigurationUnionTypeDef,
+    DesiredConfigurationTypeDef,
     DetachInstancesAnswerTypeDef,
     EmptyResponseMetadataTypeDef,
     EnterStandbyAnswerTypeDef,
     ExitStandbyAnswerTypeDef,
     FilterTypeDef,
     GetPredictiveScalingForecastAnswerTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstanceMonitoringTypeDef,
     InstanceReusePolicyTypeDef,
     LaunchConfigurationsTypeTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LifecycleHookSpecificationTypeDef,
-    MixedInstancesPolicyUnionTypeDef,
+    MixedInstancesPolicyTypeDef,
     PoliciesTypeTypeDef,
     PolicyARNTypeTypeDef,
-    PredictiveScalingConfigurationUnionTypeDef,
+    PredictiveScalingConfigurationTypeDef,
     ProcessesTypeTypeDef,
-    RefreshPreferencesUnionTypeDef,
+    RefreshPreferencesTypeDef,
     RollbackInstanceRefreshAnswerTypeDef,
     ScheduledActionsTypeTypeDef,
     ScheduledUpdateGroupActionRequestTypeDef,
     StartInstanceRefreshAnswerTypeDef,
     StepAdjustmentTypeDef,
     TagsTypeTypeDef,
     TagTypeDef,
-    TargetTrackingConfigurationUnionTypeDef,
+    TargetTrackingConfigurationTypeDef,
     TimestampTypeDef,
     TrafficSourceIdentifierTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -230,15 +230,15 @@
         self,
         *,
         AutoScalingGroupName: str,
         MinSize: int,
         MaxSize: int,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
         InstanceId: str = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         LoadBalancerNames: Sequence[str] = ...,
         TargetGroupARNs: Sequence[str] = ...,
         HealthCheckType: str = ...,
@@ -759,17 +759,17 @@
         MinAdjustmentStep: int = ...,
         MinAdjustmentMagnitude: int = ...,
         ScalingAdjustment: int = ...,
         Cooldown: int = ...,
         MetricAggregationType: str = ...,
         StepAdjustments: Sequence[StepAdjustmentTypeDef] = ...,
         EstimatedInstanceWarmup: int = ...,
-        TargetTrackingConfiguration: TargetTrackingConfigurationUnionTypeDef = ...,
+        TargetTrackingConfiguration: TargetTrackingConfigurationTypeDef = ...,
         Enabled: bool = ...,
-        PredictiveScalingConfiguration: PredictiveScalingConfigurationUnionTypeDef = ...
+        PredictiveScalingConfiguration: PredictiveScalingConfigurationTypeDef = ...
     ) -> PolicyARNTypeTypeDef:
         """
         Creates or updates a scaling policy for an Auto Scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#put_scaling_policy)
         """
@@ -871,16 +871,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#set_instance_protection)
         """
     async def start_instance_refresh(
         self,
         *,
         AutoScalingGroupName: str,
         Strategy: Literal["Rolling"] = ...,
-        DesiredConfiguration: DesiredConfigurationUnionTypeDef = ...,
-        Preferences: RefreshPreferencesUnionTypeDef = ...
+        DesiredConfiguration: DesiredConfigurationTypeDef = ...,
+        Preferences: RefreshPreferencesTypeDef = ...
     ) -> StartInstanceRefreshAnswerTypeDef:
         """
         Starts an instance refresh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Client.start_instance_refresh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling/client/#start_instance_refresh)
         """
@@ -905,15 +905,15 @@
         """
     async def update_auto_scaling_group(
         self,
         *,
         AutoScalingGroupName: str,
         LaunchConfigurationName: str = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
-        MixedInstancesPolicy: MixedInstancesPolicyUnionTypeDef = ...,
+        MixedInstancesPolicy: MixedInstancesPolicyTypeDef = ...,
         MinSize: int = ...,
         MaxSize: int = ...,
         DesiredCapacity: int = ...,
         DefaultCooldown: int = ...,
         AvailabilityZones: Sequence[str] = ...,
         HealthCheckType: str = ...,
         HealthCheckGracePeriod: int = ...,
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/literals.py` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/literals.pyi` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/paginator.py` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/paginator.pyi` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/type_defs.py` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     "DisableMetricsCollectionQueryRequestTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
-    "RefreshPreferencesOutputTypeDef",
+    "RefreshPreferencesTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyTypeDef",
@@ -131,15 +131,14 @@
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
-    "RefreshPreferencesTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
@@ -175,86 +174,64 @@
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
-    "MetricOutputTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
     "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsTypeRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "ScheduledUpdateGroupActionRequestTypeDef",
     "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
-    "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
     "PutWarmPoolTypeRequestTypeDef",
     "WarmPoolConfigurationTypeDef",
     "ProcessesTypeTypeDef",
-    "RefreshPreferencesUnionTypeDef",
     "ScheduledActionsTypeTypeDef",
     "AutoScalingInstancesTypeTypeDef",
     "CreateLaunchConfigurationTypeRequestTypeDef",
     "LaunchConfigurationTypeDef",
-    "MetricStatOutputTypeDef",
-    "TargetTrackingMetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "TargetTrackingMetricStatTypeDef",
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RollbackDetailsTypeDef",
-    "LaunchTemplateOverridesOutputTypeDef",
     "LaunchTemplateOverridesTypeDef",
     "DescribeWarmPoolAnswerTypeDef",
     "LaunchConfigurationsTypeTypeDef",
-    "MetricDataQueryOutputTypeDef",
-    "TargetTrackingMetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
-    "LaunchTemplateOutputTypeDef",
     "LaunchTemplateTypeDef",
-    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
-    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
-    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
-    "CustomizedMetricSpecificationOutputTypeDef",
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     "CustomizedMetricSpecificationTypeDef",
-    "MixedInstancesPolicyOutputTypeDef",
     "MixedInstancesPolicyTypeDef",
-    "PredictiveScalingMetricSpecificationOutputTypeDef",
-    "TargetTrackingConfigurationOutputTypeDef",
     "PredictiveScalingMetricSpecificationTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
-    "DesiredConfigurationOutputTypeDef",
     "CreateAutoScalingGroupTypeRequestTypeDef",
     "DesiredConfigurationTypeDef",
-    "MixedInstancesPolicyUnionTypeDef",
     "UpdateAutoScalingGroupTypeRequestTypeDef",
     "LoadForecastTypeDef",
-    "PredictiveScalingConfigurationOutputTypeDef",
     "PredictiveScalingConfigurationTypeDef",
-    "TargetTrackingConfigurationUnionTypeDef",
     "AutoScalingGroupsTypeTypeDef",
     "InstanceRefreshTypeDef",
-    "DesiredConfigurationUnionTypeDef",
     "StartInstanceRefreshTypeRequestTypeDef",
     "GetPredictiveScalingForecastAnswerTypeDef",
-    "ScalingPolicyTypeDef",
-    "PredictiveScalingConfigurationUnionTypeDef",
     "PutScalingPolicyTypeRequestTypeDef",
+    "ScalingPolicyTypeDef",
     "DescribeInstanceRefreshesAnswerTypeDef",
     "PoliciesTypeTypeDef",
 )
 
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
@@ -1121,16 +1098,16 @@
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
 )
 
-RefreshPreferencesOutputTypeDef = TypedDict(
-    "RefreshPreferencesOutputTypeDef",
+RefreshPreferencesTypeDef = TypedDict(
+    "RefreshPreferencesTypeDef",
     {
         "MinHealthyPercentage": int,
         "InstanceWarmup": int,
         "CheckpointPercentages": List[int],
         "CheckpointDelay": int,
         "SkipMatching": bool,
         "AutoRollback": bool,
@@ -1422,29 +1399,14 @@
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
 ):
     pass
 
 
-RefreshPreferencesTypeDef = TypedDict(
-    "RefreshPreferencesTypeDef",
-    {
-        "MinHealthyPercentage": int,
-        "InstanceWarmup": int,
-        "CheckpointPercentages": Sequence[int],
-        "CheckpointDelay": int,
-        "SkipMatching": bool,
-        "AutoRollback": bool,
-        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
-        "StandbyInstances": StandbyInstancesType,
-    },
-    total=False,
-)
-
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
     total=False,
 )
@@ -1935,45 +1897,25 @@
 DeleteTagsTypeRequestTypeDef = TypedDict(
     "DeleteTagsTypeRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredMetricOutputTypeDef = TypedDict(
-    "_RequiredMetricOutputTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-    },
-)
-_OptionalMetricOutputTypeDef = TypedDict(
-    "_OptionalMetricOutputTypeDef",
-    {
-        "Dimensions": List[MetricDimensionTypeDef],
-    },
-    total=False,
-)
-
-
-class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
-    pass
-
-
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
 _OptionalMetricTypeDef = TypedDict(
     "_OptionalMetricTypeDef",
     {
-        "Dimensions": Sequence[MetricDimensionTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
     },
     total=False,
 )
 
 
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
@@ -2130,56 +2072,14 @@
     {
         "LivePoolProgress": InstanceRefreshLivePoolProgressTypeDef,
         "WarmPoolProgress": InstanceRefreshWarmPoolProgressTypeDef,
     },
     total=False,
 )
 
-_RequiredInstanceRequirementsOutputTypeDef = TypedDict(
-    "_RequiredInstanceRequirementsOutputTypeDef",
-    {
-        "VCpuCount": VCpuCountRequestTypeDef,
-        "MemoryMiB": MemoryMiBRequestTypeDef,
-    },
-)
-_OptionalInstanceRequirementsOutputTypeDef = TypedDict(
-    "_OptionalInstanceRequirementsOutputTypeDef",
-    {
-        "CpuManufacturers": List[CpuManufacturerType],
-        "MemoryGiBPerVCpu": MemoryGiBPerVCpuRequestTypeDef,
-        "ExcludedInstanceTypes": List[str],
-        "InstanceGenerations": List[InstanceGenerationType],
-        "SpotMaxPricePercentageOverLowestPrice": int,
-        "OnDemandMaxPricePercentageOverLowestPrice": int,
-        "BareMetal": BareMetalType,
-        "BurstablePerformance": BurstablePerformanceType,
-        "RequireHibernateSupport": bool,
-        "NetworkInterfaceCount": NetworkInterfaceCountRequestTypeDef,
-        "LocalStorage": LocalStorageType,
-        "LocalStorageTypes": List[LocalStorageTypeType],
-        "TotalLocalStorageGB": TotalLocalStorageGBRequestTypeDef,
-        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsRequestTypeDef,
-        "AcceleratorTypes": List[AcceleratorTypeType],
-        "AcceleratorCount": AcceleratorCountRequestTypeDef,
-        "AcceleratorManufacturers": List[AcceleratorManufacturerType],
-        "AcceleratorNames": List[AcceleratorNameType],
-        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestTypeDef,
-        "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestTypeDef,
-        "AllowedInstanceTypes": List[str],
-    },
-    total=False,
-)
-
-
-class InstanceRequirementsOutputTypeDef(
-    _RequiredInstanceRequirementsOutputTypeDef, _OptionalInstanceRequirementsOutputTypeDef
-):
-    pass
-
-
 _RequiredInstanceRequirementsTypeDef = TypedDict(
     "_RequiredInstanceRequirementsTypeDef",
     {
         "VCpuCount": VCpuCountRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
@@ -2258,15 +2158,14 @@
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RefreshPreferencesUnionTypeDef = Union[RefreshPreferencesTypeDef, RefreshPreferencesOutputTypeDef]
 ScheduledActionsTypeTypeDef = TypedDict(
     "ScheduledActionsTypeTypeDef",
     {
         "ScheduledUpdateGroupActions": List[ScheduledUpdateGroupActionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2355,56 +2254,14 @@
 
 class LaunchConfigurationTypeDef(
     _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
 ):
     pass
 
 
-_RequiredMetricStatOutputTypeDef = TypedDict(
-    "_RequiredMetricStatOutputTypeDef",
-    {
-        "Metric": MetricOutputTypeDef,
-        "Stat": str,
-    },
-)
-_OptionalMetricStatOutputTypeDef = TypedDict(
-    "_OptionalMetricStatOutputTypeDef",
-    {
-        "Unit": str,
-    },
-    total=False,
-)
-
-
-class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
-    pass
-
-
-_RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingMetricStatOutputTypeDef",
-    {
-        "Metric": MetricOutputTypeDef,
-        "Stat": str,
-    },
-)
-_OptionalTargetTrackingMetricStatOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingMetricStatOutputTypeDef",
-    {
-        "Unit": str,
-    },
-    total=False,
-)
-
-
-class TargetTrackingMetricStatOutputTypeDef(
-    _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
-):
-    pass
-
-
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Stat": str,
     },
 )
@@ -2459,25 +2316,14 @@
         "PercentageCompleteOnRollback": int,
         "InstancesToUpdateOnRollback": int,
         "ProgressDetailsOnRollback": InstanceRefreshProgressDetailsTypeDef,
     },
     total=False,
 )
 
-LaunchTemplateOverridesOutputTypeDef = TypedDict(
-    "LaunchTemplateOverridesOutputTypeDef",
-    {
-        "InstanceType": str,
-        "WeightedCapacity": str,
-        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
-        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
-    },
-    total=False,
-)
-
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
@@ -2500,63 +2346,14 @@
     {
         "LaunchConfigurations": List[LaunchConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMetricDataQueryOutputTypeDef = TypedDict(
-    "_RequiredMetricDataQueryOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalMetricDataQueryOutputTypeDef = TypedDict(
-    "_OptionalMetricDataQueryOutputTypeDef",
-    {
-        "Expression": str,
-        "MetricStat": MetricStatOutputTypeDef,
-        "Label": str,
-        "ReturnData": bool,
-    },
-    total=False,
-)
-
-
-class MetricDataQueryOutputTypeDef(
-    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
-):
-    pass
-
-
-_RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingMetricDataQueryOutputTypeDef",
-    {
-        "Expression": str,
-        "MetricStat": TargetTrackingMetricStatOutputTypeDef,
-        "Label": str,
-        "ReturnData": bool,
-    },
-    total=False,
-)
-
-
-class TargetTrackingMetricDataQueryOutputTypeDef(
-    _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
-    _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
-):
-    pass
-
-
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -2595,173 +2392,66 @@
 
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
 
-LaunchTemplateOutputTypeDef = TypedDict(
-    "LaunchTemplateOutputTypeDef",
-    {
-        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
-        "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
-    },
-    total=False,
-)
-
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
     {
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[LaunchTemplateOverridesTypeDef],
     },
     total=False,
 )
 
-PredictiveScalingCustomizedCapacityMetricOutputTypeDef = TypedDict(
-    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
-    {
-        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
-    },
-)
-
-PredictiveScalingCustomizedLoadMetricOutputTypeDef = TypedDict(
-    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
-    {
-        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
-    },
-)
-
-PredictiveScalingCustomizedScalingMetricOutputTypeDef = TypedDict(
-    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
-    {
-        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
-    },
-)
-
-CustomizedMetricSpecificationOutputTypeDef = TypedDict(
-    "CustomizedMetricSpecificationOutputTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Dimensions": List[MetricDimensionTypeDef],
-        "Statistic": MetricStatisticType,
-        "Unit": str,
-        "Metrics": List[TargetTrackingMetricDataQueryOutputTypeDef],
-    },
-    total=False,
-)
-
 PredictiveScalingCustomizedCapacityMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     {
-        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
+        "MetricDataQueries": List[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedLoadMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     {
-        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
+        "MetricDataQueries": List[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedScalingMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     {
-        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
+        "MetricDataQueries": List[MetricDataQueryTypeDef],
     },
 )
 
 CustomizedMetricSpecificationTypeDef = TypedDict(
     "CustomizedMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
-        "Dimensions": Sequence[MetricDimensionTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
         "Unit": str,
-        "Metrics": Sequence[TargetTrackingMetricDataQueryTypeDef],
-    },
-    total=False,
-)
-
-MixedInstancesPolicyOutputTypeDef = TypedDict(
-    "MixedInstancesPolicyOutputTypeDef",
-    {
-        "LaunchTemplate": LaunchTemplateOutputTypeDef,
-        "InstancesDistribution": InstancesDistributionTypeDef,
+        "Metrics": List[TargetTrackingMetricDataQueryTypeDef],
     },
     total=False,
 )
 
 MixedInstancesPolicyTypeDef = TypedDict(
     "MixedInstancesPolicyTypeDef",
     {
         "LaunchTemplate": LaunchTemplateTypeDef,
         "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
 )
 
-_RequiredPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredPredictiveScalingMetricSpecificationOutputTypeDef",
-    {
-        "TargetValue": float,
-    },
-)
-_OptionalPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalPredictiveScalingMetricSpecificationOutputTypeDef",
-    {
-        "PredefinedMetricPairSpecification": PredictiveScalingPredefinedMetricPairTypeDef,
-        "PredefinedScalingMetricSpecification": PredictiveScalingPredefinedScalingMetricTypeDef,
-        "PredefinedLoadMetricSpecification": PredictiveScalingPredefinedLoadMetricTypeDef,
-        "CustomizedScalingMetricSpecification": (
-            PredictiveScalingCustomizedScalingMetricOutputTypeDef
-        ),
-        "CustomizedLoadMetricSpecification": PredictiveScalingCustomizedLoadMetricOutputTypeDef,
-        "CustomizedCapacityMetricSpecification": (
-            PredictiveScalingCustomizedCapacityMetricOutputTypeDef
-        ),
-    },
-    total=False,
-)
-
-
-class PredictiveScalingMetricSpecificationOutputTypeDef(
-    _RequiredPredictiveScalingMetricSpecificationOutputTypeDef,
-    _OptionalPredictiveScalingMetricSpecificationOutputTypeDef,
-):
-    pass
-
-
-_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingConfigurationOutputTypeDef",
-    {
-        "TargetValue": float,
-    },
-)
-_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingConfigurationOutputTypeDef",
-    {
-        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
-        "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
-        "DisableScaleIn": bool,
-    },
-    total=False,
-)
-
-
-class TargetTrackingConfigurationOutputTypeDef(
-    _RequiredTargetTrackingConfigurationOutputTypeDef,
-    _OptionalTargetTrackingConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredPredictiveScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredictiveScalingMetricSpecificationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalPredictiveScalingMetricSpecificationTypeDef = TypedDict(
@@ -2823,15 +2513,15 @@
 )
 _OptionalAutoScalingGroupTypeDef = TypedDict(
     "_OptionalAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupARN": str,
         "LaunchConfigurationName": str,
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
+        "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
         "PredictedCapacity": int,
         "LoadBalancerNames": List[str],
         "TargetGroupARNs": List[str],
         "HealthCheckGracePeriod": int,
         "Instances": List[InstanceTypeDef],
         "SuspendedProcesses": List[SuspendedProcessTypeDef],
         "PlacementGroup": str,
@@ -2855,23 +2545,14 @@
 )
 
 
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
 
-DesiredConfigurationOutputTypeDef = TypedDict(
-    "DesiredConfigurationOutputTypeDef",
-    {
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "MinSize": int,
         "MaxSize": int,
     },
@@ -2920,17 +2601,14 @@
     {
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
     },
     total=False,
 )
 
-MixedInstancesPolicyUnionTypeDef = Union[
-    MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
-]
 _RequiredUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredUpdateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
@@ -2969,47 +2647,22 @@
 
 
 LoadForecastTypeDef = TypedDict(
     "LoadForecastTypeDef",
     {
         "Timestamps": List[datetime],
         "Values": List[float],
-        "MetricSpecification": PredictiveScalingMetricSpecificationOutputTypeDef,
-    },
-)
-
-_RequiredPredictiveScalingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredPredictiveScalingConfigurationOutputTypeDef",
-    {
-        "MetricSpecifications": List[PredictiveScalingMetricSpecificationOutputTypeDef],
-    },
-)
-_OptionalPredictiveScalingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalPredictiveScalingConfigurationOutputTypeDef",
-    {
-        "Mode": PredictiveScalingModeType,
-        "SchedulingBufferTime": int,
-        "MaxCapacityBreachBehavior": PredictiveScalingMaxCapacityBreachBehaviorType,
-        "MaxCapacityBuffer": int,
+        "MetricSpecification": PredictiveScalingMetricSpecificationTypeDef,
     },
-    total=False,
 )
 
-
-class PredictiveScalingConfigurationOutputTypeDef(
-    _RequiredPredictiveScalingConfigurationOutputTypeDef,
-    _OptionalPredictiveScalingConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredPredictiveScalingConfigurationTypeDef = TypedDict(
     "_RequiredPredictiveScalingConfigurationTypeDef",
     {
-        "MetricSpecifications": Sequence[PredictiveScalingMetricSpecificationTypeDef],
+        "MetricSpecifications": List[PredictiveScalingMetricSpecificationTypeDef],
     },
 )
 _OptionalPredictiveScalingConfigurationTypeDef = TypedDict(
     "_OptionalPredictiveScalingConfigurationTypeDef",
     {
         "Mode": PredictiveScalingModeType,
         "SchedulingBufferTime": int,
@@ -3022,17 +2675,14 @@
 
 class PredictiveScalingConfigurationTypeDef(
     _RequiredPredictiveScalingConfigurationTypeDef, _OptionalPredictiveScalingConfigurationTypeDef
 ):
     pass
 
 
-TargetTrackingConfigurationUnionTypeDef = Union[
-    TargetTrackingConfigurationTypeDef, TargetTrackingConfigurationOutputTypeDef
-]
 AutoScalingGroupsTypeTypeDef = TypedDict(
     "AutoScalingGroupsTypeTypeDef",
     {
         "AutoScalingGroups": List[AutoScalingGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3046,24 +2696,21 @@
         "Status": InstanceRefreshStatusType,
         "StatusReason": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "PercentageComplete": int,
         "InstancesToUpdate": int,
         "ProgressDetails": InstanceRefreshProgressDetailsTypeDef,
-        "Preferences": RefreshPreferencesOutputTypeDef,
-        "DesiredConfiguration": DesiredConfigurationOutputTypeDef,
+        "Preferences": RefreshPreferencesTypeDef,
+        "DesiredConfiguration": DesiredConfigurationTypeDef,
         "RollbackDetails": RollbackDetailsTypeDef,
     },
     total=False,
 )
 
-DesiredConfigurationUnionTypeDef = Union[
-    DesiredConfigurationTypeDef, DesiredConfigurationOutputTypeDef
-]
 _RequiredStartInstanceRefreshTypeRequestTypeDef = TypedDict(
     "_RequiredStartInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalStartInstanceRefreshTypeRequestTypeDef = TypedDict(
@@ -3089,73 +2736,70 @@
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ScalingPolicyTypeDef = TypedDict(
-    "ScalingPolicyTypeDef",
+_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_RequiredPutScalingPolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-        "PolicyARN": str,
+    },
+)
+_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_OptionalPutScalingPolicyTypeRequestTypeDef",
+    {
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
-        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
+        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
-        "Alarms": List[AlarmTypeDef],
-        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
+        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "Enabled": bool,
-        "PredictiveScalingConfiguration": PredictiveScalingConfigurationOutputTypeDef,
+        "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
     },
     total=False,
 )
 
-PredictiveScalingConfigurationUnionTypeDef = Union[
-    PredictiveScalingConfigurationTypeDef, PredictiveScalingConfigurationOutputTypeDef
-]
-_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_RequiredPutScalingPolicyTypeRequestTypeDef",
+
+class PutScalingPolicyTypeRequestTypeDef(
+    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
+):
+    pass
+
+
+ScalingPolicyTypeDef = TypedDict(
+    "ScalingPolicyTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-    },
-)
-_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_OptionalPutScalingPolicyTypeRequestTypeDef",
-    {
+        "PolicyARN": str,
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
+        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
-        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
+        "Alarms": List[AlarmTypeDef],
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class PutScalingPolicyTypeRequestTypeDef(
-    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
-):
-    pass
-
-
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling/type_defs.pyi` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     "DisableMetricsCollectionQueryRequestTypeDef",
     "EnableMetricsCollectionQueryRequestTypeDef",
     "EnterStandbyQueryRequestTypeDef",
     "ExecutePolicyTypeRequestTypeDef",
     "ExitStandbyQueryRequestTypeDef",
     "InstanceRefreshLivePoolProgressTypeDef",
     "InstanceRefreshWarmPoolProgressTypeDef",
-    "RefreshPreferencesOutputTypeDef",
+    "RefreshPreferencesTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRequestTypeDef",
     "InstanceReusePolicyTypeDef",
@@ -130,15 +130,14 @@
     "PredictiveScalingPredefinedMetricPairTypeDef",
     "PredictiveScalingPredefinedScalingMetricTypeDef",
     "ProcessTypeTypeDef",
     "PutLifecycleHookTypeRequestTypeDef",
     "PutNotificationConfigurationTypeRequestTypeDef",
     "StepAdjustmentTypeDef",
     "RecordLifecycleActionHeartbeatTypeRequestTypeDef",
-    "RefreshPreferencesTypeDef",
     "RollbackInstanceRefreshTypeRequestTypeDef",
     "ScalingProcessQueryRequestTypeDef",
     "ScheduledUpdateGroupActionTypeDef",
     "SetDesiredCapacityTypeRequestTypeDef",
     "SetInstanceHealthQueryRequestTypeDef",
     "SetInstanceProtectionQueryRequestTypeDef",
     "TerminateInstanceInAutoScalingGroupTypeRequestTypeDef",
@@ -174,86 +173,64 @@
     "InstanceTypeDef",
     "TagsTypeTypeDef",
     "BatchDeleteScheduledActionAnswerTypeDef",
     "BatchPutScheduledUpdateGroupActionAnswerTypeDef",
     "BlockDeviceMappingTypeDef",
     "CreateOrUpdateTagsTypeRequestTypeDef",
     "DeleteTagsTypeRequestTypeDef",
-    "MetricOutputTypeDef",
     "MetricTypeDef",
     "DescribeLifecycleHooksAnswerTypeDef",
     "DescribeLoadBalancerTargetGroupsResponseTypeDef",
     "DescribeLoadBalancersResponseTypeDef",
     "DescribeMetricCollectionTypesAnswerTypeDef",
     "DescribeNotificationConfigurationsAnswerTypeDef",
     "DescribeScheduledActionsTypeDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsTypeRequestTypeDef",
     "GetPredictiveScalingForecastTypeRequestTypeDef",
     "PutScheduledUpdateGroupActionTypeRequestTypeDef",
     "ScheduledUpdateGroupActionRequestTypeDef",
     "DescribeTrafficSourcesResponseTypeDef",
     "InstanceRefreshProgressDetailsTypeDef",
-    "InstanceRequirementsOutputTypeDef",
     "InstanceRequirementsTypeDef",
     "PutWarmPoolTypeRequestTypeDef",
     "WarmPoolConfigurationTypeDef",
     "ProcessesTypeTypeDef",
-    "RefreshPreferencesUnionTypeDef",
     "ScheduledActionsTypeTypeDef",
     "AutoScalingInstancesTypeTypeDef",
     "CreateLaunchConfigurationTypeRequestTypeDef",
     "LaunchConfigurationTypeDef",
-    "MetricStatOutputTypeDef",
-    "TargetTrackingMetricStatOutputTypeDef",
     "MetricStatTypeDef",
     "TargetTrackingMetricStatTypeDef",
     "BatchPutScheduledUpdateGroupActionTypeRequestTypeDef",
     "RollbackDetailsTypeDef",
-    "LaunchTemplateOverridesOutputTypeDef",
     "LaunchTemplateOverridesTypeDef",
     "DescribeWarmPoolAnswerTypeDef",
     "LaunchConfigurationsTypeTypeDef",
-    "MetricDataQueryOutputTypeDef",
-    "TargetTrackingMetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
-    "LaunchTemplateOutputTypeDef",
     "LaunchTemplateTypeDef",
-    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
-    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
-    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
-    "CustomizedMetricSpecificationOutputTypeDef",
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     "CustomizedMetricSpecificationTypeDef",
-    "MixedInstancesPolicyOutputTypeDef",
     "MixedInstancesPolicyTypeDef",
-    "PredictiveScalingMetricSpecificationOutputTypeDef",
-    "TargetTrackingConfigurationOutputTypeDef",
     "PredictiveScalingMetricSpecificationTypeDef",
     "TargetTrackingConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
-    "DesiredConfigurationOutputTypeDef",
     "CreateAutoScalingGroupTypeRequestTypeDef",
     "DesiredConfigurationTypeDef",
-    "MixedInstancesPolicyUnionTypeDef",
     "UpdateAutoScalingGroupTypeRequestTypeDef",
     "LoadForecastTypeDef",
-    "PredictiveScalingConfigurationOutputTypeDef",
     "PredictiveScalingConfigurationTypeDef",
-    "TargetTrackingConfigurationUnionTypeDef",
     "AutoScalingGroupsTypeTypeDef",
     "InstanceRefreshTypeDef",
-    "DesiredConfigurationUnionTypeDef",
     "StartInstanceRefreshTypeRequestTypeDef",
     "GetPredictiveScalingForecastAnswerTypeDef",
-    "ScalingPolicyTypeDef",
-    "PredictiveScalingConfigurationUnionTypeDef",
     "PutScalingPolicyTypeRequestTypeDef",
+    "ScalingPolicyTypeDef",
     "DescribeInstanceRefreshesAnswerTypeDef",
     "PoliciesTypeTypeDef",
 )
 
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
@@ -1076,16 +1053,16 @@
     {
         "PercentageComplete": int,
         "InstancesToUpdate": int,
     },
     total=False,
 )
 
-RefreshPreferencesOutputTypeDef = TypedDict(
-    "RefreshPreferencesOutputTypeDef",
+RefreshPreferencesTypeDef = TypedDict(
+    "RefreshPreferencesTypeDef",
     {
         "MinHealthyPercentage": int,
         "InstanceWarmup": int,
         "CheckpointPercentages": List[int],
         "CheckpointDelay": int,
         "SkipMatching": bool,
         "AutoRollback": bool,
@@ -1359,29 +1336,14 @@
 
 class RecordLifecycleActionHeartbeatTypeRequestTypeDef(
     _RequiredRecordLifecycleActionHeartbeatTypeRequestTypeDef,
     _OptionalRecordLifecycleActionHeartbeatTypeRequestTypeDef,
 ):
     pass
 
-RefreshPreferencesTypeDef = TypedDict(
-    "RefreshPreferencesTypeDef",
-    {
-        "MinHealthyPercentage": int,
-        "InstanceWarmup": int,
-        "CheckpointPercentages": Sequence[int],
-        "CheckpointDelay": int,
-        "SkipMatching": bool,
-        "AutoRollback": bool,
-        "ScaleInProtectedInstances": ScaleInProtectedInstancesType,
-        "StandbyInstances": StandbyInstancesType,
-    },
-    total=False,
-)
-
 RollbackInstanceRefreshTypeRequestTypeDef = TypedDict(
     "RollbackInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
     total=False,
 )
@@ -1856,43 +1818,25 @@
 DeleteTagsTypeRequestTypeDef = TypedDict(
     "DeleteTagsTypeRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredMetricOutputTypeDef = TypedDict(
-    "_RequiredMetricOutputTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-    },
-)
-_OptionalMetricOutputTypeDef = TypedDict(
-    "_OptionalMetricOutputTypeDef",
-    {
-        "Dimensions": List[MetricDimensionTypeDef],
-    },
-    total=False,
-)
-
-class MetricOutputTypeDef(_RequiredMetricOutputTypeDef, _OptionalMetricOutputTypeDef):
-    pass
-
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
     },
 )
 _OptionalMetricTypeDef = TypedDict(
     "_OptionalMetricTypeDef",
     {
-        "Dimensions": Sequence[MetricDimensionTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
     },
     total=False,
 )
 
 class MetricTypeDef(_RequiredMetricTypeDef, _OptionalMetricTypeDef):
     pass
 
@@ -2043,54 +1987,14 @@
     {
         "LivePoolProgress": InstanceRefreshLivePoolProgressTypeDef,
         "WarmPoolProgress": InstanceRefreshWarmPoolProgressTypeDef,
     },
     total=False,
 )
 
-_RequiredInstanceRequirementsOutputTypeDef = TypedDict(
-    "_RequiredInstanceRequirementsOutputTypeDef",
-    {
-        "VCpuCount": VCpuCountRequestTypeDef,
-        "MemoryMiB": MemoryMiBRequestTypeDef,
-    },
-)
-_OptionalInstanceRequirementsOutputTypeDef = TypedDict(
-    "_OptionalInstanceRequirementsOutputTypeDef",
-    {
-        "CpuManufacturers": List[CpuManufacturerType],
-        "MemoryGiBPerVCpu": MemoryGiBPerVCpuRequestTypeDef,
-        "ExcludedInstanceTypes": List[str],
-        "InstanceGenerations": List[InstanceGenerationType],
-        "SpotMaxPricePercentageOverLowestPrice": int,
-        "OnDemandMaxPricePercentageOverLowestPrice": int,
-        "BareMetal": BareMetalType,
-        "BurstablePerformance": BurstablePerformanceType,
-        "RequireHibernateSupport": bool,
-        "NetworkInterfaceCount": NetworkInterfaceCountRequestTypeDef,
-        "LocalStorage": LocalStorageType,
-        "LocalStorageTypes": List[LocalStorageTypeType],
-        "TotalLocalStorageGB": TotalLocalStorageGBRequestTypeDef,
-        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsRequestTypeDef,
-        "AcceleratorTypes": List[AcceleratorTypeType],
-        "AcceleratorCount": AcceleratorCountRequestTypeDef,
-        "AcceleratorManufacturers": List[AcceleratorManufacturerType],
-        "AcceleratorNames": List[AcceleratorNameType],
-        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBRequestTypeDef,
-        "NetworkBandwidthGbps": NetworkBandwidthGbpsRequestTypeDef,
-        "AllowedInstanceTypes": List[str],
-    },
-    total=False,
-)
-
-class InstanceRequirementsOutputTypeDef(
-    _RequiredInstanceRequirementsOutputTypeDef, _OptionalInstanceRequirementsOutputTypeDef
-):
-    pass
-
 _RequiredInstanceRequirementsTypeDef = TypedDict(
     "_RequiredInstanceRequirementsTypeDef",
     {
         "VCpuCount": VCpuCountRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
@@ -2165,15 +2069,14 @@
     "ProcessesTypeTypeDef",
     {
         "Processes": List[ProcessTypeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RefreshPreferencesUnionTypeDef = Union[RefreshPreferencesTypeDef, RefreshPreferencesOutputTypeDef]
 ScheduledActionsTypeTypeDef = TypedDict(
     "ScheduledActionsTypeTypeDef",
     {
         "ScheduledUpdateGroupActions": List[ScheduledUpdateGroupActionTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2258,52 +2161,14 @@
 )
 
 class LaunchConfigurationTypeDef(
     _RequiredLaunchConfigurationTypeDef, _OptionalLaunchConfigurationTypeDef
 ):
     pass
 
-_RequiredMetricStatOutputTypeDef = TypedDict(
-    "_RequiredMetricStatOutputTypeDef",
-    {
-        "Metric": MetricOutputTypeDef,
-        "Stat": str,
-    },
-)
-_OptionalMetricStatOutputTypeDef = TypedDict(
-    "_OptionalMetricStatOutputTypeDef",
-    {
-        "Unit": str,
-    },
-    total=False,
-)
-
-class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
-    pass
-
-_RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingMetricStatOutputTypeDef",
-    {
-        "Metric": MetricOutputTypeDef,
-        "Stat": str,
-    },
-)
-_OptionalTargetTrackingMetricStatOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingMetricStatOutputTypeDef",
-    {
-        "Unit": str,
-    },
-    total=False,
-)
-
-class TargetTrackingMetricStatOutputTypeDef(
-    _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
-):
-    pass
-
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Stat": str,
     },
 )
@@ -2354,25 +2219,14 @@
         "PercentageCompleteOnRollback": int,
         "InstancesToUpdateOnRollback": int,
         "ProgressDetailsOnRollback": InstanceRefreshProgressDetailsTypeDef,
     },
     total=False,
 )
 
-LaunchTemplateOverridesOutputTypeDef = TypedDict(
-    "LaunchTemplateOverridesOutputTypeDef",
-    {
-        "InstanceType": str,
-        "WeightedCapacity": str,
-        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
-        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
-    },
-    total=False,
-)
-
 LaunchTemplateOverridesTypeDef = TypedDict(
     "LaunchTemplateOverridesTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": str,
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "InstanceRequirements": InstanceRequirementsTypeDef,
@@ -2395,59 +2249,14 @@
     {
         "LaunchConfigurations": List[LaunchConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMetricDataQueryOutputTypeDef = TypedDict(
-    "_RequiredMetricDataQueryOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalMetricDataQueryOutputTypeDef = TypedDict(
-    "_OptionalMetricDataQueryOutputTypeDef",
-    {
-        "Expression": str,
-        "MetricStat": MetricStatOutputTypeDef,
-        "Label": str,
-        "ReturnData": bool,
-    },
-    total=False,
-)
-
-class MetricDataQueryOutputTypeDef(
-    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
-):
-    pass
-
-_RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingMetricDataQueryOutputTypeDef",
-    {
-        "Expression": str,
-        "MetricStat": TargetTrackingMetricStatOutputTypeDef,
-        "Label": str,
-        "ReturnData": bool,
-    },
-    total=False,
-)
-
-class TargetTrackingMetricDataQueryOutputTypeDef(
-    _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
-    _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
-):
-    pass
-
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -2482,169 +2291,66 @@
 )
 
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
-LaunchTemplateOutputTypeDef = TypedDict(
-    "LaunchTemplateOutputTypeDef",
-    {
-        "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
-        "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
-    },
-    total=False,
-)
-
 LaunchTemplateTypeDef = TypedDict(
     "LaunchTemplateTypeDef",
     {
         "LaunchTemplateSpecification": LaunchTemplateSpecificationTypeDef,
         "Overrides": Sequence[LaunchTemplateOverridesTypeDef],
     },
     total=False,
 )
 
-PredictiveScalingCustomizedCapacityMetricOutputTypeDef = TypedDict(
-    "PredictiveScalingCustomizedCapacityMetricOutputTypeDef",
-    {
-        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
-    },
-)
-
-PredictiveScalingCustomizedLoadMetricOutputTypeDef = TypedDict(
-    "PredictiveScalingCustomizedLoadMetricOutputTypeDef",
-    {
-        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
-    },
-)
-
-PredictiveScalingCustomizedScalingMetricOutputTypeDef = TypedDict(
-    "PredictiveScalingCustomizedScalingMetricOutputTypeDef",
-    {
-        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
-    },
-)
-
-CustomizedMetricSpecificationOutputTypeDef = TypedDict(
-    "CustomizedMetricSpecificationOutputTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Dimensions": List[MetricDimensionTypeDef],
-        "Statistic": MetricStatisticType,
-        "Unit": str,
-        "Metrics": List[TargetTrackingMetricDataQueryOutputTypeDef],
-    },
-    total=False,
-)
-
 PredictiveScalingCustomizedCapacityMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedCapacityMetricTypeDef",
     {
-        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
+        "MetricDataQueries": List[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedLoadMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedLoadMetricTypeDef",
     {
-        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
+        "MetricDataQueries": List[MetricDataQueryTypeDef],
     },
 )
 
 PredictiveScalingCustomizedScalingMetricTypeDef = TypedDict(
     "PredictiveScalingCustomizedScalingMetricTypeDef",
     {
-        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
+        "MetricDataQueries": List[MetricDataQueryTypeDef],
     },
 )
 
 CustomizedMetricSpecificationTypeDef = TypedDict(
     "CustomizedMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
-        "Dimensions": Sequence[MetricDimensionTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
         "Unit": str,
-        "Metrics": Sequence[TargetTrackingMetricDataQueryTypeDef],
-    },
-    total=False,
-)
-
-MixedInstancesPolicyOutputTypeDef = TypedDict(
-    "MixedInstancesPolicyOutputTypeDef",
-    {
-        "LaunchTemplate": LaunchTemplateOutputTypeDef,
-        "InstancesDistribution": InstancesDistributionTypeDef,
+        "Metrics": List[TargetTrackingMetricDataQueryTypeDef],
     },
     total=False,
 )
 
 MixedInstancesPolicyTypeDef = TypedDict(
     "MixedInstancesPolicyTypeDef",
     {
         "LaunchTemplate": LaunchTemplateTypeDef,
         "InstancesDistribution": InstancesDistributionTypeDef,
     },
     total=False,
 )
 
-_RequiredPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredPredictiveScalingMetricSpecificationOutputTypeDef",
-    {
-        "TargetValue": float,
-    },
-)
-_OptionalPredictiveScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalPredictiveScalingMetricSpecificationOutputTypeDef",
-    {
-        "PredefinedMetricPairSpecification": PredictiveScalingPredefinedMetricPairTypeDef,
-        "PredefinedScalingMetricSpecification": PredictiveScalingPredefinedScalingMetricTypeDef,
-        "PredefinedLoadMetricSpecification": PredictiveScalingPredefinedLoadMetricTypeDef,
-        "CustomizedScalingMetricSpecification": (
-            PredictiveScalingCustomizedScalingMetricOutputTypeDef
-        ),
-        "CustomizedLoadMetricSpecification": PredictiveScalingCustomizedLoadMetricOutputTypeDef,
-        "CustomizedCapacityMetricSpecification": (
-            PredictiveScalingCustomizedCapacityMetricOutputTypeDef
-        ),
-    },
-    total=False,
-)
-
-class PredictiveScalingMetricSpecificationOutputTypeDef(
-    _RequiredPredictiveScalingMetricSpecificationOutputTypeDef,
-    _OptionalPredictiveScalingMetricSpecificationOutputTypeDef,
-):
-    pass
-
-_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingConfigurationOutputTypeDef",
-    {
-        "TargetValue": float,
-    },
-)
-_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingConfigurationOutputTypeDef",
-    {
-        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
-        "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
-        "DisableScaleIn": bool,
-    },
-    total=False,
-)
-
-class TargetTrackingConfigurationOutputTypeDef(
-    _RequiredTargetTrackingConfigurationOutputTypeDef,
-    _OptionalTargetTrackingConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredPredictiveScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredictiveScalingMetricSpecificationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalPredictiveScalingMetricSpecificationTypeDef = TypedDict(
@@ -2702,15 +2408,15 @@
 )
 _OptionalAutoScalingGroupTypeDef = TypedDict(
     "_OptionalAutoScalingGroupTypeDef",
     {
         "AutoScalingGroupARN": str,
         "LaunchConfigurationName": str,
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
+        "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
         "PredictedCapacity": int,
         "LoadBalancerNames": List[str],
         "TargetGroupARNs": List[str],
         "HealthCheckGracePeriod": int,
         "Instances": List[InstanceTypeDef],
         "SuspendedProcesses": List[SuspendedProcessTypeDef],
         "PlacementGroup": str,
@@ -2732,23 +2438,14 @@
     },
     total=False,
 )
 
 class AutoScalingGroupTypeDef(_RequiredAutoScalingGroupTypeDef, _OptionalAutoScalingGroupTypeDef):
     pass
 
-DesiredConfigurationOutputTypeDef = TypedDict(
-    "DesiredConfigurationOutputTypeDef",
-    {
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "MixedInstancesPolicy": MixedInstancesPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredCreateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "MinSize": int,
         "MaxSize": int,
     },
@@ -2795,17 +2492,14 @@
     {
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "MixedInstancesPolicy": MixedInstancesPolicyTypeDef,
     },
     total=False,
 )
 
-MixedInstancesPolicyUnionTypeDef = Union[
-    MixedInstancesPolicyTypeDef, MixedInstancesPolicyOutputTypeDef
-]
 _RequiredUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
     "_RequiredUpdateAutoScalingGroupTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalUpdateAutoScalingGroupTypeRequestTypeDef = TypedDict(
@@ -2842,45 +2536,22 @@
     pass
 
 LoadForecastTypeDef = TypedDict(
     "LoadForecastTypeDef",
     {
         "Timestamps": List[datetime],
         "Values": List[float],
-        "MetricSpecification": PredictiveScalingMetricSpecificationOutputTypeDef,
+        "MetricSpecification": PredictiveScalingMetricSpecificationTypeDef,
     },
 )
 
-_RequiredPredictiveScalingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredPredictiveScalingConfigurationOutputTypeDef",
-    {
-        "MetricSpecifications": List[PredictiveScalingMetricSpecificationOutputTypeDef],
-    },
-)
-_OptionalPredictiveScalingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalPredictiveScalingConfigurationOutputTypeDef",
-    {
-        "Mode": PredictiveScalingModeType,
-        "SchedulingBufferTime": int,
-        "MaxCapacityBreachBehavior": PredictiveScalingMaxCapacityBreachBehaviorType,
-        "MaxCapacityBuffer": int,
-    },
-    total=False,
-)
-
-class PredictiveScalingConfigurationOutputTypeDef(
-    _RequiredPredictiveScalingConfigurationOutputTypeDef,
-    _OptionalPredictiveScalingConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredPredictiveScalingConfigurationTypeDef = TypedDict(
     "_RequiredPredictiveScalingConfigurationTypeDef",
     {
-        "MetricSpecifications": Sequence[PredictiveScalingMetricSpecificationTypeDef],
+        "MetricSpecifications": List[PredictiveScalingMetricSpecificationTypeDef],
     },
 )
 _OptionalPredictiveScalingConfigurationTypeDef = TypedDict(
     "_OptionalPredictiveScalingConfigurationTypeDef",
     {
         "Mode": PredictiveScalingModeType,
         "SchedulingBufferTime": int,
@@ -2891,17 +2562,14 @@
 )
 
 class PredictiveScalingConfigurationTypeDef(
     _RequiredPredictiveScalingConfigurationTypeDef, _OptionalPredictiveScalingConfigurationTypeDef
 ):
     pass
 
-TargetTrackingConfigurationUnionTypeDef = Union[
-    TargetTrackingConfigurationTypeDef, TargetTrackingConfigurationOutputTypeDef
-]
 AutoScalingGroupsTypeTypeDef = TypedDict(
     "AutoScalingGroupsTypeTypeDef",
     {
         "AutoScalingGroups": List[AutoScalingGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2915,24 +2583,21 @@
         "Status": InstanceRefreshStatusType,
         "StatusReason": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "PercentageComplete": int,
         "InstancesToUpdate": int,
         "ProgressDetails": InstanceRefreshProgressDetailsTypeDef,
-        "Preferences": RefreshPreferencesOutputTypeDef,
-        "DesiredConfiguration": DesiredConfigurationOutputTypeDef,
+        "Preferences": RefreshPreferencesTypeDef,
+        "DesiredConfiguration": DesiredConfigurationTypeDef,
         "RollbackDetails": RollbackDetailsTypeDef,
     },
     total=False,
 )
 
-DesiredConfigurationUnionTypeDef = Union[
-    DesiredConfigurationTypeDef, DesiredConfigurationOutputTypeDef
-]
 _RequiredStartInstanceRefreshTypeRequestTypeDef = TypedDict(
     "_RequiredStartInstanceRefreshTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
     },
 )
 _OptionalStartInstanceRefreshTypeRequestTypeDef = TypedDict(
@@ -2956,71 +2621,68 @@
         "LoadForecast": List[LoadForecastTypeDef],
         "CapacityForecast": CapacityForecastTypeDef,
         "UpdateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ScalingPolicyTypeDef = TypedDict(
-    "ScalingPolicyTypeDef",
+_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_RequiredPutScalingPolicyTypeRequestTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-        "PolicyARN": str,
+    },
+)
+_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
+    "_OptionalPutScalingPolicyTypeRequestTypeDef",
+    {
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
-        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
+        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
-        "Alarms": List[AlarmTypeDef],
-        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
+        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "Enabled": bool,
-        "PredictiveScalingConfiguration": PredictiveScalingConfigurationOutputTypeDef,
+        "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
     },
     total=False,
 )
 
-PredictiveScalingConfigurationUnionTypeDef = Union[
-    PredictiveScalingConfigurationTypeDef, PredictiveScalingConfigurationOutputTypeDef
-]
-_RequiredPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_RequiredPutScalingPolicyTypeRequestTypeDef",
+class PutScalingPolicyTypeRequestTypeDef(
+    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
+):
+    pass
+
+ScalingPolicyTypeDef = TypedDict(
+    "ScalingPolicyTypeDef",
     {
         "AutoScalingGroupName": str,
         "PolicyName": str,
-    },
-)
-_OptionalPutScalingPolicyTypeRequestTypeDef = TypedDict(
-    "_OptionalPutScalingPolicyTypeRequestTypeDef",
-    {
+        "PolicyARN": str,
         "PolicyType": str,
         "AdjustmentType": str,
         "MinAdjustmentStep": int,
         "MinAdjustmentMagnitude": int,
         "ScalingAdjustment": int,
         "Cooldown": int,
+        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MetricAggregationType": str,
-        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
         "EstimatedInstanceWarmup": int,
+        "Alarms": List[AlarmTypeDef],
         "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
         "Enabled": bool,
         "PredictiveScalingConfiguration": PredictiveScalingConfigurationTypeDef,
     },
     total=False,
 )
 
-class PutScalingPolicyTypeRequestTypeDef(
-    _RequiredPutScalingPolicyTypeRequestTypeDef, _OptionalPutScalingPolicyTypeRequestTypeDef
-):
-    pass
-
 DescribeInstanceRefreshesAnswerTypeDef = TypedDict(
     "DescribeInstanceRefreshesAnswerTypeDef",
     {
         "InstanceRefreshes": List[InstanceRefreshTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-autoscaling-2.5.2.post1/types_aiobotocore_autoscaling.egg-info/SOURCES.txt` & `types-aiobotocore-autoscaling-2.5.2.post2/types_aiobotocore_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

