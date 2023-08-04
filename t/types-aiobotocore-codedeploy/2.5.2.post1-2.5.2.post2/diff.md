# Comparing `tmp/types-aiobotocore-codedeploy-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codedeploy-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codedeploy-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-codedeploy-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:36 2023, max compression
```

## Comparing `types-aiobotocore-codedeploy-2.5.2.post1.tar` & `types-aiobotocore-codedeploy-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.569625 types-aiobotocore-codedeploy-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-08-02 14:52:02.565625 types-aiobotocore-codedeploy-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.569625 types-aiobotocore-codedeploy-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.565625 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48641 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48575 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-08-02 14:35:06.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-08-02 14:35:06.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-08-02 14:35:05.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53972 2023-08-02 14:35:07.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53939 2023-08-02 14:35:06.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:04.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-02 14:35:05.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-02 14:35:05.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.565625 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:02.000000 types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.655540 types-aiobotocore-codedeploy-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-08-04 12:00:36.655540 types-aiobotocore-codedeploy-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13696 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:36.655540 types-aiobotocore-codedeploy-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.643540 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48531 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48465 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-08-04 11:42:22.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14447 2023-08-04 11:42:22.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50667 2023-08-04 11:42:23.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50634 2023-08-04 11:42:22.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-04 11:42:21.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.655540 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15226 2023-08-04 12:00:36.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-04 12:00:36.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:36.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:36.000000 types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/LICENSE` & `types-aiobotocore-codedeploy-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/setup.py` & `types-aiobotocore-codedeploy-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codedeploy",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codedeploy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeDeploy 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__init__.py` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__init__.pyi` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/__main__.py` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeDeploy 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CodeDeploy 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy\nOther"
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

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/client.py` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     ListDeploymentInstancesPaginator,
     ListDeploymentsPaginator,
     ListDeploymentTargetsPaginator,
     ListGitHubAccountTokenNamesPaginator,
     ListOnPremisesInstancesPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationUnionTypeDef,
-    AutoRollbackConfigurationUnionTypeDef,
+    AlarmConfigurationTypeDef,
+    AutoRollbackConfigurationTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     BatchGetApplicationsOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
@@ -61,15 +61,15 @@
     CreateDeploymentConfigOutputTypeDef,
     CreateDeploymentGroupOutputTypeDef,
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
-    EC2TagSetUnionTypeDef,
+    EC2TagSetTypeDef,
     ECSServiceTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationOutputTypeDef,
     GetApplicationRevisionOutputTypeDef,
     GetDeploymentConfigOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
@@ -82,26 +82,26 @@
     ListDeploymentGroupsOutputTypeDef,
     ListDeploymentInstancesOutputTypeDef,
     ListDeploymentsOutputTypeDef,
     ListDeploymentTargetsOutputTypeDef,
     ListGitHubAccountTokenNamesOutputTypeDef,
     ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoadBalancerInfoUnionTypeDef,
+    LoadBalancerInfoTypeDef,
     MinimumHealthyHostsTypeDef,
-    OnPremisesTagSetUnionTypeDef,
+    OnPremisesTagSetTypeDef,
     PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RevisionLocationTypeDef,
     StopDeploymentOutputTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
-    TargetInstancesUnionTypeDef,
+    TargetInstancesTypeDef,
     TimeRangeTypeDef,
     TrafficRoutingConfigTypeDef,
-    TriggerConfigUnionTypeDef,
+    TriggerConfigTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
 )
 from .waiter import DeploymentSuccessfulWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -379,19 +379,19 @@
         *,
         applicationName: str,
         deploymentGroupName: str = ...,
         revision: RevisionLocationTypeDef = ...,
         deploymentConfigName: str = ...,
         description: str = ...,
         ignoreApplicationStopFailures: bool = ...,
-        targetInstances: TargetInstancesUnionTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
+        targetInstances: TargetInstancesTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
         updateOutdatedInstancesOnly: bool = ...,
         fileExistsBehavior: FileExistsBehaviorType = ...,
-        overrideAlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        overrideAlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> CreateDeploymentOutputTypeDef:
         """
         Deploys an application revision through the specified deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment)
         """
@@ -417,24 +417,24 @@
         applicationName: str,
         deploymentGroupName: str,
         serviceRoleArn: str,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
-        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
-        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
+        triggerConfigurations: Sequence[TriggerConfigTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
-        ec2TagSet: EC2TagSetUnionTypeDef = ...,
+        loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
+        ec2TagSet: EC2TagSetTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...,
+        onPremisesTagSet: OnPremisesTagSetTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDeploymentGroupOutputTypeDef:
         """
         Creates a deployment group to which application revisions are deployed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment_group)
@@ -816,24 +816,24 @@
         currentDeploymentGroupName: str,
         newDeploymentGroupName: str = ...,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
         serviceRoleArn: str = ...,
-        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
-        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
+        triggerConfigurations: Sequence[TriggerConfigTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
-        ec2TagSet: EC2TagSetUnionTypeDef = ...,
+        loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
+        ec2TagSet: EC2TagSetTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...
+        onPremisesTagSet: OnPremisesTagSetTypeDef = ...
     ) -> UpdateDeploymentGroupOutputTypeDef:
         """
         Changes information about a deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.update_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#update_deployment_group)
         """
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/client.pyi` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     ListDeploymentInstancesPaginator,
     ListDeploymentsPaginator,
     ListDeploymentTargetsPaginator,
     ListGitHubAccountTokenNamesPaginator,
     ListOnPremisesInstancesPaginator,
 )
 from .type_defs import (
-    AlarmConfigurationUnionTypeDef,
-    AutoRollbackConfigurationUnionTypeDef,
+    AlarmConfigurationTypeDef,
+    AutoRollbackConfigurationTypeDef,
     BatchGetApplicationRevisionsOutputTypeDef,
     BatchGetApplicationsOutputTypeDef,
     BatchGetDeploymentGroupsOutputTypeDef,
     BatchGetDeploymentInstancesOutputTypeDef,
     BatchGetDeploymentsOutputTypeDef,
     BatchGetDeploymentTargetsOutputTypeDef,
     BatchGetOnPremisesInstancesOutputTypeDef,
@@ -61,15 +61,15 @@
     CreateDeploymentConfigOutputTypeDef,
     CreateDeploymentGroupOutputTypeDef,
     CreateDeploymentOutputTypeDef,
     DeleteDeploymentGroupOutputTypeDef,
     DeleteGitHubAccountTokenOutputTypeDef,
     DeploymentStyleTypeDef,
     EC2TagFilterTypeDef,
-    EC2TagSetUnionTypeDef,
+    EC2TagSetTypeDef,
     ECSServiceTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationOutputTypeDef,
     GetApplicationRevisionOutputTypeDef,
     GetDeploymentConfigOutputTypeDef,
     GetDeploymentGroupOutputTypeDef,
     GetDeploymentInstanceOutputTypeDef,
@@ -82,26 +82,26 @@
     ListDeploymentGroupsOutputTypeDef,
     ListDeploymentInstancesOutputTypeDef,
     ListDeploymentsOutputTypeDef,
     ListDeploymentTargetsOutputTypeDef,
     ListGitHubAccountTokenNamesOutputTypeDef,
     ListOnPremisesInstancesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoadBalancerInfoUnionTypeDef,
+    LoadBalancerInfoTypeDef,
     MinimumHealthyHostsTypeDef,
-    OnPremisesTagSetUnionTypeDef,
+    OnPremisesTagSetTypeDef,
     PutLifecycleEventHookExecutionStatusOutputTypeDef,
     RevisionLocationTypeDef,
     StopDeploymentOutputTypeDef,
     TagFilterTypeDef,
     TagTypeDef,
-    TargetInstancesUnionTypeDef,
+    TargetInstancesTypeDef,
     TimeRangeTypeDef,
     TrafficRoutingConfigTypeDef,
-    TriggerConfigUnionTypeDef,
+    TriggerConfigTypeDef,
     UpdateDeploymentGroupOutputTypeDef,
 )
 from .waiter import DeploymentSuccessfulWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -362,19 +362,19 @@
         *,
         applicationName: str,
         deploymentGroupName: str = ...,
         revision: RevisionLocationTypeDef = ...,
         deploymentConfigName: str = ...,
         description: str = ...,
         ignoreApplicationStopFailures: bool = ...,
-        targetInstances: TargetInstancesUnionTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
+        targetInstances: TargetInstancesTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
         updateOutdatedInstancesOnly: bool = ...,
         fileExistsBehavior: FileExistsBehaviorType = ...,
-        overrideAlarmConfiguration: AlarmConfigurationUnionTypeDef = ...
+        overrideAlarmConfiguration: AlarmConfigurationTypeDef = ...
     ) -> CreateDeploymentOutputTypeDef:
         """
         Deploys an application revision through the specified deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment)
         """
@@ -398,24 +398,24 @@
         applicationName: str,
         deploymentGroupName: str,
         serviceRoleArn: str,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
-        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
-        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
+        triggerConfigurations: Sequence[TriggerConfigTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
-        ec2TagSet: EC2TagSetUnionTypeDef = ...,
+        loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
+        ec2TagSet: EC2TagSetTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...,
+        onPremisesTagSet: OnPremisesTagSetTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDeploymentGroupOutputTypeDef:
         """
         Creates a deployment group to which application revisions are deployed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.create_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#create_deployment_group)
@@ -762,24 +762,24 @@
         currentDeploymentGroupName: str,
         newDeploymentGroupName: str = ...,
         deploymentConfigName: str = ...,
         ec2TagFilters: Sequence[EC2TagFilterTypeDef] = ...,
         onPremisesInstanceTagFilters: Sequence[TagFilterTypeDef] = ...,
         autoScalingGroups: Sequence[str] = ...,
         serviceRoleArn: str = ...,
-        triggerConfigurations: Sequence[TriggerConfigUnionTypeDef] = ...,
-        alarmConfiguration: AlarmConfigurationUnionTypeDef = ...,
-        autoRollbackConfiguration: AutoRollbackConfigurationUnionTypeDef = ...,
+        triggerConfigurations: Sequence[TriggerConfigTypeDef] = ...,
+        alarmConfiguration: AlarmConfigurationTypeDef = ...,
+        autoRollbackConfiguration: AutoRollbackConfigurationTypeDef = ...,
         outdatedInstancesStrategy: OutdatedInstancesStrategyType = ...,
         deploymentStyle: DeploymentStyleTypeDef = ...,
         blueGreenDeploymentConfiguration: BlueGreenDeploymentConfigurationTypeDef = ...,
-        loadBalancerInfo: LoadBalancerInfoUnionTypeDef = ...,
-        ec2TagSet: EC2TagSetUnionTypeDef = ...,
+        loadBalancerInfo: LoadBalancerInfoTypeDef = ...,
+        ec2TagSet: EC2TagSetTypeDef = ...,
         ecsServices: Sequence[ECSServiceTypeDef] = ...,
-        onPremisesTagSet: OnPremisesTagSetUnionTypeDef = ...
+        onPremisesTagSet: OnPremisesTagSetTypeDef = ...
     ) -> UpdateDeploymentGroupOutputTypeDef:
         """
         Changes information about a deployment group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Client.update_deployment_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codedeploy/client/#update_deployment_group)
         """
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/literals.py` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/literals.pyi` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/paginator.py` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/paginator.pyi` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/type_defs.py` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 
 
 __all__ = (
     "TagTypeDef",
     "AlarmTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
-    "AutoRollbackConfigurationOutputTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetApplicationsInputRequestTypeDef",
     "BatchGetDeploymentGroupsInputRequestTypeDef",
     "BatchGetDeploymentInstancesInputRequestTypeDef",
     "BatchGetDeploymentTargetsInputRequestTypeDef",
@@ -77,21 +76,21 @@
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
     "MinimumHealthyHostsTypeDef",
     "DeploymentStyleTypeDef",
     "EC2TagFilterTypeDef",
     "ECSServiceTypeDef",
     "TagFilterTypeDef",
+    "TriggerConfigTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     "LastDeploymentInfoTypeDef",
-    "TriggerConfigOutputTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
     "TargetGroupInfoTypeDef",
@@ -118,30 +117,26 @@
     "ListTagsForResourceInputRequestTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
-    "TrafficRouteOutputTypeDef",
     "TrafficRouteTypeDef",
     "TimeBasedCanaryTypeDef",
     "TimeBasedLinearTypeDef",
     "TimestampTypeDef",
-    "TriggerConfigTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
     "InstanceInfoTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
-    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
-    "AutoRollbackConfigurationUnionTypeDef",
     "BatchGetApplicationsOutputTypeDef",
     "CreateApplicationOutputTypeDef",
     "CreateDeploymentConfigOutputTypeDef",
     "CreateDeploymentGroupOutputTypeDef",
     "CreateDeploymentOutputTypeDef",
     "DeleteDeploymentGroupOutputTypeDef",
     "DeleteGitHubAccountTokenOutputTypeDef",
@@ -156,70 +151,59 @@
     "ListGitHubAccountTokenNamesOutputTypeDef",
     "ListOnPremisesInstancesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "PutLifecycleEventHookExecutionStatusOutputTypeDef",
     "StopDeploymentOutputTypeDef",
     "UpdateDeploymentGroupOutputTypeDef",
     "BlueGreenDeploymentConfigurationTypeDef",
-    "EC2TagSetOutputTypeDef",
     "EC2TagSetTypeDef",
     "ListOnPremisesInstancesInputRequestTypeDef",
-    "OnPremisesTagSetOutputTypeDef",
     "OnPremisesTagSetTypeDef",
     "LifecycleEventTypeDef",
     "ECSTaskSetTypeDef",
     "GetDeploymentInputDeploymentSuccessfulWaitTypeDef",
     "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "RevisionLocationTypeDef",
-    "TargetGroupPairInfoOutputTypeDef",
     "TargetGroupPairInfoTypeDef",
     "TrafficRoutingConfigTypeDef",
     "TimeRangeTypeDef",
-    "TriggerConfigUnionTypeDef",
     "BatchGetOnPremisesInstancesOutputTypeDef",
     "GetOnPremisesInstanceOutputTypeDef",
-    "AlarmConfigurationUnionTypeDef",
-    "TargetInstancesOutputTypeDef",
-    "EC2TagSetUnionTypeDef",
     "TargetInstancesTypeDef",
-    "OnPremisesTagSetUnionTypeDef",
     "CloudFormationTargetTypeDef",
     "InstanceSummaryTypeDef",
     "InstanceTargetTypeDef",
     "LambdaTargetTypeDef",
     "ECSTargetTypeDef",
     "BatchGetApplicationRevisionsInputRequestTypeDef",
     "GetApplicationRevisionInputRequestTypeDef",
     "GetApplicationRevisionOutputTypeDef",
     "ListApplicationRevisionsOutputTypeDef",
     "RegisterApplicationRevisionInputRequestTypeDef",
     "RevisionInfoTypeDef",
-    "LoadBalancerInfoOutputTypeDef",
     "LoadBalancerInfoTypeDef",
     "CreateDeploymentConfigInputRequestTypeDef",
     "DeploymentConfigInfoTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
     "CreateDeploymentInputRequestTypeDef",
-    "TargetInstancesUnionTypeDef",
     "BatchGetDeploymentInstancesOutputTypeDef",
     "GetDeploymentInstanceOutputTypeDef",
     "DeploymentTargetTypeDef",
     "BatchGetApplicationRevisionsOutputTypeDef",
+    "CreateDeploymentGroupInputRequestTypeDef",
     "DeploymentGroupInfoTypeDef",
     "DeploymentInfoTypeDef",
-    "CreateDeploymentGroupInputRequestTypeDef",
-    "LoadBalancerInfoUnionTypeDef",
     "UpdateDeploymentGroupInputRequestTypeDef",
     "GetDeploymentConfigOutputTypeDef",
     "BatchGetDeploymentTargetsOutputTypeDef",
     "GetDeploymentTargetOutputTypeDef",
     "BatchGetDeploymentGroupsOutputTypeDef",
     "GetDeploymentGroupOutputTypeDef",
     "BatchGetDeploymentsOutputTypeDef",
@@ -261,28 +245,19 @@
         "linkedToGitHub": bool,
         "gitHubAccountName": str,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
-AutoRollbackConfigurationOutputTypeDef = TypedDict(
-    "AutoRollbackConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-        "events": List[AutoRollbackEventType],
-    },
-    total=False,
-)
-
 AutoRollbackConfigurationTypeDef = TypedDict(
     "AutoRollbackConfigurationTypeDef",
     {
         "enabled": bool,
-        "events": Sequence[AutoRollbackEventType],
+        "events": List[AutoRollbackEventType],
     },
     total=False,
 )
 
 AutoScalingGroupTypeDef = TypedDict(
     "AutoScalingGroupTypeDef",
     {
@@ -427,14 +402,24 @@
         "Key": str,
         "Value": str,
         "Type": TagFilterTypeType,
     },
     total=False,
 )
 
+TriggerConfigTypeDef = TypedDict(
+    "TriggerConfigTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": List[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 DeleteApplicationInputRequestTypeDef = TypedDict(
     "DeleteApplicationInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 
@@ -476,24 +461,14 @@
         "status": DeploymentStatusType,
         "endTime": datetime,
         "createTime": datetime,
     },
     total=False,
 )
 
-TriggerConfigOutputTypeDef = TypedDict(
-    "TriggerConfigOutputTypeDef",
-    {
-        "triggerName": str,
-        "triggerTargetArn": str,
-        "triggerEvents": List[TriggerEventTypeType],
-    },
-    total=False,
-)
-
 DeploymentOverviewTypeDef = TypedDict(
     "DeploymentOverviewTypeDef",
     {
         "Pending": int,
         "InProgress": int,
         "Succeeded": int,
         "Failed": int,
@@ -877,26 +852,18 @@
 
 class StopDeploymentInputRequestTypeDef(
     _RequiredStopDeploymentInputRequestTypeDef, _OptionalStopDeploymentInputRequestTypeDef
 ):
     pass
 
 
-TrafficRouteOutputTypeDef = TypedDict(
-    "TrafficRouteOutputTypeDef",
-    {
-        "listenerArns": List[str],
-    },
-    total=False,
-)
-
 TrafficRouteTypeDef = TypedDict(
     "TrafficRouteTypeDef",
     {
-        "listenerArns": Sequence[str],
+        "listenerArns": List[str],
     },
     total=False,
 )
 
 TimeBasedCanaryTypeDef = TypedDict(
     "TimeBasedCanaryTypeDef",
     {
@@ -912,24 +879,14 @@
         "linearPercentage": int,
         "linearInterval": int,
     },
     total=False,
 )
 
 TimestampTypeDef = Union[datetime, str]
-TriggerConfigTypeDef = TypedDict(
-    "TriggerConfigTypeDef",
-    {
-        "triggerName": str,
-        "triggerTargetArn": str,
-        "triggerEvents": Sequence[TriggerEventTypeType],
-    },
-    total=False,
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -999,37 +956,24 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-AlarmConfigurationOutputTypeDef = TypedDict(
-    "AlarmConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-        "ignorePollAlarmFailure": bool,
-        "alarms": List[AlarmTypeDef],
-    },
-    total=False,
-)
-
 AlarmConfigurationTypeDef = TypedDict(
     "AlarmConfigurationTypeDef",
     {
         "enabled": bool,
         "ignorePollAlarmFailure": bool,
-        "alarms": Sequence[AlarmTypeDef],
+        "alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
-AutoRollbackConfigurationUnionTypeDef = Union[
-    AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
-]
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
         "applicationsInfo": List[ApplicationInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1210,52 +1154,36 @@
         "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionTypeDef,
         "deploymentReadyOption": DeploymentReadyOptionTypeDef,
         "greenFleetProvisioningOption": GreenFleetProvisioningOptionTypeDef,
     },
     total=False,
 )
 
-EC2TagSetOutputTypeDef = TypedDict(
-    "EC2TagSetOutputTypeDef",
-    {
-        "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
-    },
-    total=False,
-)
-
 EC2TagSetTypeDef = TypedDict(
     "EC2TagSetTypeDef",
     {
-        "ec2TagSetList": Sequence[Sequence[EC2TagFilterTypeDef]],
+        "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
 ListOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "ListOnPremisesInstancesInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
-OnPremisesTagSetOutputTypeDef = TypedDict(
-    "OnPremisesTagSetOutputTypeDef",
-    {
-        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
-    },
-    total=False,
-)
-
 OnPremisesTagSetTypeDef = TypedDict(
     "OnPremisesTagSetTypeDef",
     {
-        "onPremisesTagSetList": Sequence[Sequence[TagFilterTypeDef]],
+        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
     },
     total=False,
 )
 
 LifecycleEventTypeDef = TypedDict(
     "LifecycleEventTypeDef",
     {
@@ -1430,28 +1358,18 @@
         "gitHubLocation": GitHubLocationTypeDef,
         "string": RawStringTypeDef,
         "appSpecContent": AppSpecContentTypeDef,
     },
     total=False,
 )
 
-TargetGroupPairInfoOutputTypeDef = TypedDict(
-    "TargetGroupPairInfoOutputTypeDef",
-    {
-        "targetGroups": List[TargetGroupInfoTypeDef],
-        "prodTrafficRoute": TrafficRouteOutputTypeDef,
-        "testTrafficRoute": TrafficRouteOutputTypeDef,
-    },
-    total=False,
-)
-
 TargetGroupPairInfoTypeDef = TypedDict(
     "TargetGroupPairInfoTypeDef",
     {
-        "targetGroups": Sequence[TargetGroupInfoTypeDef],
+        "targetGroups": List[TargetGroupInfoTypeDef],
         "prodTrafficRoute": TrafficRouteTypeDef,
         "testTrafficRoute": TrafficRouteTypeDef,
     },
     total=False,
 )
 
 TrafficRoutingConfigTypeDef = TypedDict(
@@ -1469,15 +1387,14 @@
     {
         "start": TimestampTypeDef,
         "end": TimestampTypeDef,
     },
     total=False,
 )
 
-TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesOutputTypeDef",
     {
         "instanceInfos": List[InstanceInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1486,37 +1403,24 @@
     "GetOnPremisesInstanceOutputTypeDef",
     {
         "instanceInfo": InstanceInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
-TargetInstancesOutputTypeDef = TypedDict(
-    "TargetInstancesOutputTypeDef",
-    {
-        "tagFilters": List[EC2TagFilterTypeDef],
-        "autoScalingGroups": List[str],
-        "ec2TagSet": EC2TagSetOutputTypeDef,
-    },
-    total=False,
-)
-
-EC2TagSetUnionTypeDef = Union[EC2TagSetTypeDef, EC2TagSetOutputTypeDef]
 TargetInstancesTypeDef = TypedDict(
     "TargetInstancesTypeDef",
     {
-        "tagFilters": Sequence[EC2TagFilterTypeDef],
-        "autoScalingGroups": Sequence[str],
+        "tagFilters": List[EC2TagFilterTypeDef],
+        "autoScalingGroups": List[str],
         "ec2TagSet": EC2TagSetTypeDef,
     },
     total=False,
 )
 
-OnPremisesTagSetUnionTypeDef = Union[OnPremisesTagSetTypeDef, OnPremisesTagSetOutputTypeDef]
 CloudFormationTargetTypeDef = TypedDict(
     "CloudFormationTargetTypeDef",
     {
         "deploymentId": str,
         "targetId": str,
         "lastUpdatedAt": datetime,
         "lifecycleEvents": List[LifecycleEventTypeDef],
@@ -1645,30 +1549,20 @@
     {
         "revisionLocation": RevisionLocationTypeDef,
         "genericRevisionInfo": GenericRevisionInfoTypeDef,
     },
     total=False,
 )
 
-LoadBalancerInfoOutputTypeDef = TypedDict(
-    "LoadBalancerInfoOutputTypeDef",
-    {
-        "elbInfoList": List[ELBInfoTypeDef],
-        "targetGroupInfoList": List[TargetGroupInfoTypeDef],
-        "targetGroupPairInfoList": List[TargetGroupPairInfoOutputTypeDef],
-    },
-    total=False,
-)
-
 LoadBalancerInfoTypeDef = TypedDict(
     "LoadBalancerInfoTypeDef",
     {
-        "elbInfoList": Sequence[ELBInfoTypeDef],
-        "targetGroupInfoList": Sequence[TargetGroupInfoTypeDef],
-        "targetGroupPairInfoList": Sequence[TargetGroupPairInfoTypeDef],
+        "elbInfoList": List[ELBInfoTypeDef],
+        "targetGroupInfoList": List[TargetGroupInfoTypeDef],
+        "targetGroupPairInfoList": List[TargetGroupPairInfoTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateDeploymentConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentConfigInputRequestTypeDef",
     {
@@ -1758,15 +1652,14 @@
 
 class CreateDeploymentInputRequestTypeDef(
     _RequiredCreateDeploymentInputRequestTypeDef, _OptionalCreateDeploymentInputRequestTypeDef
 ):
     pass
 
 
-TargetInstancesUnionTypeDef = Union[TargetInstancesTypeDef, TargetInstancesOutputTypeDef]
 BatchGetDeploymentInstancesOutputTypeDef = TypedDict(
     "BatchGetDeploymentInstancesOutputTypeDef",
     {
         "instancesSummary": List[InstanceSummaryTypeDef],
         "errorMessage": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1798,37 +1691,75 @@
         "applicationName": str,
         "errorMessage": str,
         "revisions": List[RevisionInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "serviceRoleArn": str,
+    },
+)
+_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "deploymentConfigName": str,
+        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
+        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
+        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
+        "alarmConfiguration": AlarmConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
+        "deploymentStyle": DeploymentStyleTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "ec2TagSet": EC2TagSetTypeDef,
+        "ecsServices": Sequence[ECSServiceTypeDef],
+        "onPremisesTagSet": OnPremisesTagSetTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateDeploymentGroupInputRequestTypeDef(
+    _RequiredCreateDeploymentGroupInputRequestTypeDef,
+    _OptionalCreateDeploymentGroupInputRequestTypeDef,
+):
+    pass
+
+
 DeploymentGroupInfoTypeDef = TypedDict(
     "DeploymentGroupInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupId": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
         "ec2TagFilters": List[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": List[TagFilterTypeDef],
         "autoScalingGroups": List[AutoScalingGroupTypeDef],
         "serviceRoleArn": str,
         "targetRevision": RevisionLocationTypeDef,
-        "triggerConfigurations": List[TriggerConfigOutputTypeDef],
-        "alarmConfiguration": AlarmConfigurationOutputTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
+        "triggerConfigurations": List[TriggerConfigTypeDef],
+        "alarmConfiguration": AlarmConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "deploymentStyle": DeploymentStyleTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "lastSuccessfulDeployment": LastDeploymentInfoTypeDef,
         "lastAttemptedDeployment": LastDeploymentInfoTypeDef,
-        "ec2TagSet": EC2TagSetOutputTypeDef,
-        "onPremisesTagSet": OnPremisesTagSetOutputTypeDef,
+        "ec2TagSet": EC2TagSetTypeDef,
+        "onPremisesTagSet": OnPremisesTagSetTypeDef,
         "computePlatform": ComputePlatformType,
         "ecsServices": List[ECSServiceTypeDef],
     },
     total=False,
 )
 
 DeploymentInfoTypeDef = TypedDict(
@@ -1845,72 +1776,33 @@
         "createTime": datetime,
         "startTime": datetime,
         "completeTime": datetime,
         "deploymentOverview": DeploymentOverviewTypeDef,
         "description": str,
         "creator": DeploymentCreatorType,
         "ignoreApplicationStopFailures": bool,
-        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "updateOutdatedInstancesOnly": bool,
         "rollbackInfo": RollbackInfoTypeDef,
         "deploymentStyle": DeploymentStyleTypeDef,
-        "targetInstances": TargetInstancesOutputTypeDef,
+        "targetInstances": TargetInstancesTypeDef,
         "instanceTerminationWaitTimeStarted": bool,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "additionalDeploymentStatusInfo": str,
         "fileExistsBehavior": FileExistsBehaviorType,
         "deploymentStatusMessages": List[str],
         "computePlatform": ComputePlatformType,
         "externalId": str,
         "relatedDeployments": RelatedDeploymentsTypeDef,
-        "overrideAlarmConfiguration": AlarmConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroupName": str,
-        "serviceRoleArn": str,
-    },
-)
-_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "deploymentConfigName": str,
-        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
-        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
-        "autoScalingGroups": Sequence[str],
-        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
-        "alarmConfiguration": AlarmConfigurationTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
-        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
-        "deploymentStyle": DeploymentStyleTypeDef,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
-        "ec2TagSet": EC2TagSetTypeDef,
-        "ecsServices": Sequence[ECSServiceTypeDef],
-        "onPremisesTagSet": OnPremisesTagSetTypeDef,
-        "tags": Sequence[TagTypeDef],
+        "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class CreateDeploymentGroupInputRequestTypeDef(
-    _RequiredCreateDeploymentGroupInputRequestTypeDef,
-    _OptionalCreateDeploymentGroupInputRequestTypeDef,
-):
-    pass
-
-
-LoadBalancerInfoUnionTypeDef = Union[LoadBalancerInfoTypeDef, LoadBalancerInfoOutputTypeDef]
 _RequiredUpdateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
         "currentDeploymentGroupName": str,
     },
 )
@@ -1919,15 +1811,15 @@
     {
         "newDeploymentGroupName": str,
         "deploymentConfigName": str,
         "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
         "autoScalingGroups": Sequence[str],
         "serviceRoleArn": str,
-        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
+        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
         "alarmConfiguration": AlarmConfigurationTypeDef,
         "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "deploymentStyle": DeploymentStyleTypeDef,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "ec2TagSet": EC2TagSetTypeDef,
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/type_defs.pyi` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
     "AlarmTypeDef",
     "AppSpecContentTypeDef",
     "ApplicationInfoTypeDef",
-    "AutoRollbackConfigurationOutputTypeDef",
     "AutoRollbackConfigurationTypeDef",
     "AutoScalingGroupTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetApplicationsInputRequestTypeDef",
     "BatchGetDeploymentGroupsInputRequestTypeDef",
     "BatchGetDeploymentInstancesInputRequestTypeDef",
     "BatchGetDeploymentTargetsInputRequestTypeDef",
@@ -76,21 +75,21 @@
     "GreenFleetProvisioningOptionTypeDef",
     "ContinueDeploymentInputRequestTypeDef",
     "MinimumHealthyHostsTypeDef",
     "DeploymentStyleTypeDef",
     "EC2TagFilterTypeDef",
     "ECSServiceTypeDef",
     "TagFilterTypeDef",
+    "TriggerConfigTypeDef",
     "DeleteApplicationInputRequestTypeDef",
     "DeleteDeploymentConfigInputRequestTypeDef",
     "DeleteDeploymentGroupInputRequestTypeDef",
     "DeleteGitHubAccountTokenInputRequestTypeDef",
     "DeleteResourcesByExternalIdInputRequestTypeDef",
     "LastDeploymentInfoTypeDef",
-    "TriggerConfigOutputTypeDef",
     "DeploymentOverviewTypeDef",
     "ErrorInformationTypeDef",
     "RelatedDeploymentsTypeDef",
     "RollbackInfoTypeDef",
     "DeregisterOnPremisesInstanceInputRequestTypeDef",
     "DiagnosticsTypeDef",
     "TargetGroupInfoTypeDef",
@@ -117,30 +116,26 @@
     "ListTagsForResourceInputRequestTypeDef",
     "PutLifecycleEventHookExecutionStatusInputRequestTypeDef",
     "RawStringTypeDef",
     "RegisterOnPremisesInstanceInputRequestTypeDef",
     "S3LocationTypeDef",
     "SkipWaitTimeForInstanceTerminationInputRequestTypeDef",
     "StopDeploymentInputRequestTypeDef",
-    "TrafficRouteOutputTypeDef",
     "TrafficRouteTypeDef",
     "TimeBasedCanaryTypeDef",
     "TimeBasedLinearTypeDef",
     "TimestampTypeDef",
-    "TriggerConfigTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateApplicationInputRequestTypeDef",
     "AddTagsToOnPremisesInstancesInputRequestTypeDef",
     "CreateApplicationInputRequestTypeDef",
     "InstanceInfoTypeDef",
     "RemoveTagsFromOnPremisesInstancesInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
-    "AlarmConfigurationOutputTypeDef",
     "AlarmConfigurationTypeDef",
-    "AutoRollbackConfigurationUnionTypeDef",
     "BatchGetApplicationsOutputTypeDef",
     "CreateApplicationOutputTypeDef",
     "CreateDeploymentConfigOutputTypeDef",
     "CreateDeploymentGroupOutputTypeDef",
     "CreateDeploymentOutputTypeDef",
     "DeleteDeploymentGroupOutputTypeDef",
     "DeleteGitHubAccountTokenOutputTypeDef",
@@ -155,70 +150,59 @@
     "ListGitHubAccountTokenNamesOutputTypeDef",
     "ListOnPremisesInstancesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "PutLifecycleEventHookExecutionStatusOutputTypeDef",
     "StopDeploymentOutputTypeDef",
     "UpdateDeploymentGroupOutputTypeDef",
     "BlueGreenDeploymentConfigurationTypeDef",
-    "EC2TagSetOutputTypeDef",
     "EC2TagSetTypeDef",
     "ListOnPremisesInstancesInputRequestTypeDef",
-    "OnPremisesTagSetOutputTypeDef",
     "OnPremisesTagSetTypeDef",
     "LifecycleEventTypeDef",
     "ECSTaskSetTypeDef",
     "GetDeploymentInputDeploymentSuccessfulWaitTypeDef",
     "ListApplicationRevisionsInputListApplicationRevisionsPaginateTypeDef",
     "ListApplicationsInputListApplicationsPaginateTypeDef",
     "ListDeploymentConfigsInputListDeploymentConfigsPaginateTypeDef",
     "ListDeploymentGroupsInputListDeploymentGroupsPaginateTypeDef",
     "ListDeploymentInstancesInputListDeploymentInstancesPaginateTypeDef",
     "ListDeploymentTargetsInputListDeploymentTargetsPaginateTypeDef",
     "ListGitHubAccountTokenNamesInputListGitHubAccountTokenNamesPaginateTypeDef",
     "ListOnPremisesInstancesInputListOnPremisesInstancesPaginateTypeDef",
     "RevisionLocationTypeDef",
-    "TargetGroupPairInfoOutputTypeDef",
     "TargetGroupPairInfoTypeDef",
     "TrafficRoutingConfigTypeDef",
     "TimeRangeTypeDef",
-    "TriggerConfigUnionTypeDef",
     "BatchGetOnPremisesInstancesOutputTypeDef",
     "GetOnPremisesInstanceOutputTypeDef",
-    "AlarmConfigurationUnionTypeDef",
-    "TargetInstancesOutputTypeDef",
-    "EC2TagSetUnionTypeDef",
     "TargetInstancesTypeDef",
-    "OnPremisesTagSetUnionTypeDef",
     "CloudFormationTargetTypeDef",
     "InstanceSummaryTypeDef",
     "InstanceTargetTypeDef",
     "LambdaTargetTypeDef",
     "ECSTargetTypeDef",
     "BatchGetApplicationRevisionsInputRequestTypeDef",
     "GetApplicationRevisionInputRequestTypeDef",
     "GetApplicationRevisionOutputTypeDef",
     "ListApplicationRevisionsOutputTypeDef",
     "RegisterApplicationRevisionInputRequestTypeDef",
     "RevisionInfoTypeDef",
-    "LoadBalancerInfoOutputTypeDef",
     "LoadBalancerInfoTypeDef",
     "CreateDeploymentConfigInputRequestTypeDef",
     "DeploymentConfigInfoTypeDef",
     "ListDeploymentsInputListDeploymentsPaginateTypeDef",
     "ListDeploymentsInputRequestTypeDef",
     "CreateDeploymentInputRequestTypeDef",
-    "TargetInstancesUnionTypeDef",
     "BatchGetDeploymentInstancesOutputTypeDef",
     "GetDeploymentInstanceOutputTypeDef",
     "DeploymentTargetTypeDef",
     "BatchGetApplicationRevisionsOutputTypeDef",
+    "CreateDeploymentGroupInputRequestTypeDef",
     "DeploymentGroupInfoTypeDef",
     "DeploymentInfoTypeDef",
-    "CreateDeploymentGroupInputRequestTypeDef",
-    "LoadBalancerInfoUnionTypeDef",
     "UpdateDeploymentGroupInputRequestTypeDef",
     "GetDeploymentConfigOutputTypeDef",
     "BatchGetDeploymentTargetsOutputTypeDef",
     "GetDeploymentTargetOutputTypeDef",
     "BatchGetDeploymentGroupsOutputTypeDef",
     "GetDeploymentGroupOutputTypeDef",
     "BatchGetDeploymentsOutputTypeDef",
@@ -260,28 +244,19 @@
         "linkedToGitHub": bool,
         "gitHubAccountName": str,
         "computePlatform": ComputePlatformType,
     },
     total=False,
 )
 
-AutoRollbackConfigurationOutputTypeDef = TypedDict(
-    "AutoRollbackConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-        "events": List[AutoRollbackEventType],
-    },
-    total=False,
-)
-
 AutoRollbackConfigurationTypeDef = TypedDict(
     "AutoRollbackConfigurationTypeDef",
     {
         "enabled": bool,
-        "events": Sequence[AutoRollbackEventType],
+        "events": List[AutoRollbackEventType],
     },
     total=False,
 )
 
 AutoScalingGroupTypeDef = TypedDict(
     "AutoScalingGroupTypeDef",
     {
@@ -426,14 +401,24 @@
         "Key": str,
         "Value": str,
         "Type": TagFilterTypeType,
     },
     total=False,
 )
 
+TriggerConfigTypeDef = TypedDict(
+    "TriggerConfigTypeDef",
+    {
+        "triggerName": str,
+        "triggerTargetArn": str,
+        "triggerEvents": List[TriggerEventTypeType],
+    },
+    total=False,
+)
+
 DeleteApplicationInputRequestTypeDef = TypedDict(
     "DeleteApplicationInputRequestTypeDef",
     {
         "applicationName": str,
     },
 )
 
@@ -475,24 +460,14 @@
         "status": DeploymentStatusType,
         "endTime": datetime,
         "createTime": datetime,
     },
     total=False,
 )
 
-TriggerConfigOutputTypeDef = TypedDict(
-    "TriggerConfigOutputTypeDef",
-    {
-        "triggerName": str,
-        "triggerTargetArn": str,
-        "triggerEvents": List[TriggerEventTypeType],
-    },
-    total=False,
-)
-
 DeploymentOverviewTypeDef = TypedDict(
     "DeploymentOverviewTypeDef",
     {
         "Pending": int,
         "InProgress": int,
         "Succeeded": int,
         "Failed": int,
@@ -864,26 +839,18 @@
 )
 
 class StopDeploymentInputRequestTypeDef(
     _RequiredStopDeploymentInputRequestTypeDef, _OptionalStopDeploymentInputRequestTypeDef
 ):
     pass
 
-TrafficRouteOutputTypeDef = TypedDict(
-    "TrafficRouteOutputTypeDef",
-    {
-        "listenerArns": List[str],
-    },
-    total=False,
-)
-
 TrafficRouteTypeDef = TypedDict(
     "TrafficRouteTypeDef",
     {
-        "listenerArns": Sequence[str],
+        "listenerArns": List[str],
     },
     total=False,
 )
 
 TimeBasedCanaryTypeDef = TypedDict(
     "TimeBasedCanaryTypeDef",
     {
@@ -899,24 +866,14 @@
         "linearPercentage": int,
         "linearInterval": int,
     },
     total=False,
 )
 
 TimestampTypeDef = Union[datetime, str]
-TriggerConfigTypeDef = TypedDict(
-    "TriggerConfigTypeDef",
-    {
-        "triggerName": str,
-        "triggerTargetArn": str,
-        "triggerEvents": Sequence[TriggerEventTypeType],
-    },
-    total=False,
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -984,37 +941,24 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-AlarmConfigurationOutputTypeDef = TypedDict(
-    "AlarmConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-        "ignorePollAlarmFailure": bool,
-        "alarms": List[AlarmTypeDef],
-    },
-    total=False,
-)
-
 AlarmConfigurationTypeDef = TypedDict(
     "AlarmConfigurationTypeDef",
     {
         "enabled": bool,
         "ignorePollAlarmFailure": bool,
-        "alarms": Sequence[AlarmTypeDef],
+        "alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
-AutoRollbackConfigurationUnionTypeDef = Union[
-    AutoRollbackConfigurationTypeDef, AutoRollbackConfigurationOutputTypeDef
-]
 BatchGetApplicationsOutputTypeDef = TypedDict(
     "BatchGetApplicationsOutputTypeDef",
     {
         "applicationsInfo": List[ApplicationInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1195,52 +1139,36 @@
         "terminateBlueInstancesOnDeploymentSuccess": BlueInstanceTerminationOptionTypeDef,
         "deploymentReadyOption": DeploymentReadyOptionTypeDef,
         "greenFleetProvisioningOption": GreenFleetProvisioningOptionTypeDef,
     },
     total=False,
 )
 
-EC2TagSetOutputTypeDef = TypedDict(
-    "EC2TagSetOutputTypeDef",
-    {
-        "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
-    },
-    total=False,
-)
-
 EC2TagSetTypeDef = TypedDict(
     "EC2TagSetTypeDef",
     {
-        "ec2TagSetList": Sequence[Sequence[EC2TagFilterTypeDef]],
+        "ec2TagSetList": List[List[EC2TagFilterTypeDef]],
     },
     total=False,
 )
 
 ListOnPremisesInstancesInputRequestTypeDef = TypedDict(
     "ListOnPremisesInstancesInputRequestTypeDef",
     {
         "registrationStatus": RegistrationStatusType,
         "tagFilters": Sequence[TagFilterTypeDef],
         "nextToken": str,
     },
     total=False,
 )
 
-OnPremisesTagSetOutputTypeDef = TypedDict(
-    "OnPremisesTagSetOutputTypeDef",
-    {
-        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
-    },
-    total=False,
-)
-
 OnPremisesTagSetTypeDef = TypedDict(
     "OnPremisesTagSetTypeDef",
     {
-        "onPremisesTagSetList": Sequence[Sequence[TagFilterTypeDef]],
+        "onPremisesTagSetList": List[List[TagFilterTypeDef]],
     },
     total=False,
 )
 
 LifecycleEventTypeDef = TypedDict(
     "LifecycleEventTypeDef",
     {
@@ -1407,28 +1335,18 @@
         "gitHubLocation": GitHubLocationTypeDef,
         "string": RawStringTypeDef,
         "appSpecContent": AppSpecContentTypeDef,
     },
     total=False,
 )
 
-TargetGroupPairInfoOutputTypeDef = TypedDict(
-    "TargetGroupPairInfoOutputTypeDef",
-    {
-        "targetGroups": List[TargetGroupInfoTypeDef],
-        "prodTrafficRoute": TrafficRouteOutputTypeDef,
-        "testTrafficRoute": TrafficRouteOutputTypeDef,
-    },
-    total=False,
-)
-
 TargetGroupPairInfoTypeDef = TypedDict(
     "TargetGroupPairInfoTypeDef",
     {
-        "targetGroups": Sequence[TargetGroupInfoTypeDef],
+        "targetGroups": List[TargetGroupInfoTypeDef],
         "prodTrafficRoute": TrafficRouteTypeDef,
         "testTrafficRoute": TrafficRouteTypeDef,
     },
     total=False,
 )
 
 TrafficRoutingConfigTypeDef = TypedDict(
@@ -1446,15 +1364,14 @@
     {
         "start": TimestampTypeDef,
         "end": TimestampTypeDef,
     },
     total=False,
 )
 
-TriggerConfigUnionTypeDef = Union[TriggerConfigTypeDef, TriggerConfigOutputTypeDef]
 BatchGetOnPremisesInstancesOutputTypeDef = TypedDict(
     "BatchGetOnPremisesInstancesOutputTypeDef",
     {
         "instanceInfos": List[InstanceInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1463,37 +1380,24 @@
     "GetOnPremisesInstanceOutputTypeDef",
     {
         "instanceInfo": InstanceInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AlarmConfigurationUnionTypeDef = Union[AlarmConfigurationTypeDef, AlarmConfigurationOutputTypeDef]
-TargetInstancesOutputTypeDef = TypedDict(
-    "TargetInstancesOutputTypeDef",
-    {
-        "tagFilters": List[EC2TagFilterTypeDef],
-        "autoScalingGroups": List[str],
-        "ec2TagSet": EC2TagSetOutputTypeDef,
-    },
-    total=False,
-)
-
-EC2TagSetUnionTypeDef = Union[EC2TagSetTypeDef, EC2TagSetOutputTypeDef]
 TargetInstancesTypeDef = TypedDict(
     "TargetInstancesTypeDef",
     {
-        "tagFilters": Sequence[EC2TagFilterTypeDef],
-        "autoScalingGroups": Sequence[str],
+        "tagFilters": List[EC2TagFilterTypeDef],
+        "autoScalingGroups": List[str],
         "ec2TagSet": EC2TagSetTypeDef,
     },
     total=False,
 )
 
-OnPremisesTagSetUnionTypeDef = Union[OnPremisesTagSetTypeDef, OnPremisesTagSetOutputTypeDef]
 CloudFormationTargetTypeDef = TypedDict(
     "CloudFormationTargetTypeDef",
     {
         "deploymentId": str,
         "targetId": str,
         "lastUpdatedAt": datetime,
         "lifecycleEvents": List[LifecycleEventTypeDef],
@@ -1620,30 +1524,20 @@
     {
         "revisionLocation": RevisionLocationTypeDef,
         "genericRevisionInfo": GenericRevisionInfoTypeDef,
     },
     total=False,
 )
 
-LoadBalancerInfoOutputTypeDef = TypedDict(
-    "LoadBalancerInfoOutputTypeDef",
-    {
-        "elbInfoList": List[ELBInfoTypeDef],
-        "targetGroupInfoList": List[TargetGroupInfoTypeDef],
-        "targetGroupPairInfoList": List[TargetGroupPairInfoOutputTypeDef],
-    },
-    total=False,
-)
-
 LoadBalancerInfoTypeDef = TypedDict(
     "LoadBalancerInfoTypeDef",
     {
-        "elbInfoList": Sequence[ELBInfoTypeDef],
-        "targetGroupInfoList": Sequence[TargetGroupInfoTypeDef],
-        "targetGroupPairInfoList": Sequence[TargetGroupPairInfoTypeDef],
+        "elbInfoList": List[ELBInfoTypeDef],
+        "targetGroupInfoList": List[TargetGroupInfoTypeDef],
+        "targetGroupPairInfoList": List[TargetGroupPairInfoTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateDeploymentConfigInputRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentConfigInputRequestTypeDef",
     {
@@ -1729,15 +1623,14 @@
 )
 
 class CreateDeploymentInputRequestTypeDef(
     _RequiredCreateDeploymentInputRequestTypeDef, _OptionalCreateDeploymentInputRequestTypeDef
 ):
     pass
 
-TargetInstancesUnionTypeDef = Union[TargetInstancesTypeDef, TargetInstancesOutputTypeDef]
 BatchGetDeploymentInstancesOutputTypeDef = TypedDict(
     "BatchGetDeploymentInstancesOutputTypeDef",
     {
         "instancesSummary": List[InstanceSummaryTypeDef],
         "errorMessage": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1769,37 +1662,73 @@
         "applicationName": str,
         "errorMessage": str,
         "revisions": List[RevisionInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "applicationName": str,
+        "deploymentGroupName": str,
+        "serviceRoleArn": str,
+    },
+)
+_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
+    {
+        "deploymentConfigName": str,
+        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
+        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
+        "autoScalingGroups": Sequence[str],
+        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
+        "alarmConfiguration": AlarmConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
+        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
+        "deploymentStyle": DeploymentStyleTypeDef,
+        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoTypeDef,
+        "ec2TagSet": EC2TagSetTypeDef,
+        "ecsServices": Sequence[ECSServiceTypeDef],
+        "onPremisesTagSet": OnPremisesTagSetTypeDef,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateDeploymentGroupInputRequestTypeDef(
+    _RequiredCreateDeploymentGroupInputRequestTypeDef,
+    _OptionalCreateDeploymentGroupInputRequestTypeDef,
+):
+    pass
+
 DeploymentGroupInfoTypeDef = TypedDict(
     "DeploymentGroupInfoTypeDef",
     {
         "applicationName": str,
         "deploymentGroupId": str,
         "deploymentGroupName": str,
         "deploymentConfigName": str,
         "ec2TagFilters": List[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": List[TagFilterTypeDef],
         "autoScalingGroups": List[AutoScalingGroupTypeDef],
         "serviceRoleArn": str,
         "targetRevision": RevisionLocationTypeDef,
-        "triggerConfigurations": List[TriggerConfigOutputTypeDef],
-        "alarmConfiguration": AlarmConfigurationOutputTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
+        "triggerConfigurations": List[TriggerConfigTypeDef],
+        "alarmConfiguration": AlarmConfigurationTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "deploymentStyle": DeploymentStyleTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "lastSuccessfulDeployment": LastDeploymentInfoTypeDef,
         "lastAttemptedDeployment": LastDeploymentInfoTypeDef,
-        "ec2TagSet": EC2TagSetOutputTypeDef,
-        "onPremisesTagSet": OnPremisesTagSetOutputTypeDef,
+        "ec2TagSet": EC2TagSetTypeDef,
+        "onPremisesTagSet": OnPremisesTagSetTypeDef,
         "computePlatform": ComputePlatformType,
         "ecsServices": List[ECSServiceTypeDef],
     },
     total=False,
 )
 
 DeploymentInfoTypeDef = TypedDict(
@@ -1816,70 +1745,33 @@
         "createTime": datetime,
         "startTime": datetime,
         "completeTime": datetime,
         "deploymentOverview": DeploymentOverviewTypeDef,
         "description": str,
         "creator": DeploymentCreatorType,
         "ignoreApplicationStopFailures": bool,
-        "autoRollbackConfiguration": AutoRollbackConfigurationOutputTypeDef,
+        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "updateOutdatedInstancesOnly": bool,
         "rollbackInfo": RollbackInfoTypeDef,
         "deploymentStyle": DeploymentStyleTypeDef,
-        "targetInstances": TargetInstancesOutputTypeDef,
+        "targetInstances": TargetInstancesTypeDef,
         "instanceTerminationWaitTimeStarted": bool,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoOutputTypeDef,
+        "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "additionalDeploymentStatusInfo": str,
         "fileExistsBehavior": FileExistsBehaviorType,
         "deploymentStatusMessages": List[str],
         "computePlatform": ComputePlatformType,
         "externalId": str,
         "relatedDeployments": RelatedDeploymentsTypeDef,
-        "overrideAlarmConfiguration": AlarmConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "applicationName": str,
-        "deploymentGroupName": str,
-        "serviceRoleArn": str,
-    },
-)
-_OptionalCreateDeploymentGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentGroupInputRequestTypeDef",
-    {
-        "deploymentConfigName": str,
-        "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
-        "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
-        "autoScalingGroups": Sequence[str],
-        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
-        "alarmConfiguration": AlarmConfigurationTypeDef,
-        "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
-        "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
-        "deploymentStyle": DeploymentStyleTypeDef,
-        "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
-        "loadBalancerInfo": LoadBalancerInfoTypeDef,
-        "ec2TagSet": EC2TagSetTypeDef,
-        "ecsServices": Sequence[ECSServiceTypeDef],
-        "onPremisesTagSet": OnPremisesTagSetTypeDef,
-        "tags": Sequence[TagTypeDef],
+        "overrideAlarmConfiguration": AlarmConfigurationTypeDef,
     },
     total=False,
 )
 
-class CreateDeploymentGroupInputRequestTypeDef(
-    _RequiredCreateDeploymentGroupInputRequestTypeDef,
-    _OptionalCreateDeploymentGroupInputRequestTypeDef,
-):
-    pass
-
-LoadBalancerInfoUnionTypeDef = Union[LoadBalancerInfoTypeDef, LoadBalancerInfoOutputTypeDef]
 _RequiredUpdateDeploymentGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentGroupInputRequestTypeDef",
     {
         "applicationName": str,
         "currentDeploymentGroupName": str,
     },
 )
@@ -1888,15 +1780,15 @@
     {
         "newDeploymentGroupName": str,
         "deploymentConfigName": str,
         "ec2TagFilters": Sequence[EC2TagFilterTypeDef],
         "onPremisesInstanceTagFilters": Sequence[TagFilterTypeDef],
         "autoScalingGroups": Sequence[str],
         "serviceRoleArn": str,
-        "triggerConfigurations": Sequence[TriggerConfigUnionTypeDef],
+        "triggerConfigurations": Sequence[TriggerConfigTypeDef],
         "alarmConfiguration": AlarmConfigurationTypeDef,
         "autoRollbackConfiguration": AutoRollbackConfigurationTypeDef,
         "outdatedInstancesStrategy": OutdatedInstancesStrategyType,
         "deploymentStyle": DeploymentStyleTypeDef,
         "blueGreenDeploymentConfiguration": BlueGreenDeploymentConfigurationTypeDef,
         "loadBalancerInfo": LoadBalancerInfoTypeDef,
         "ec2TagSet": EC2TagSetTypeDef,
```

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/waiter.py` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy/waiter.pyi` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codedeploy-2.5.2.post1/types_aiobotocore_codedeploy.egg-info/SOURCES.txt` & `types-aiobotocore-codedeploy-2.5.2.post2/types_aiobotocore_codedeploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

