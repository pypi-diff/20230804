# Comparing `tmp/types-aiobotocore-emr-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-emr-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-emr-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-emr-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:52 2023, max compression
```

## Comparing `types-aiobotocore-emr-2.5.2.post1.tar` & `types-aiobotocore-emr-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.933588 types-aiobotocore-emr-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:23.000000 types-aiobotocore-emr-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-08-02 14:52:16.917588 types-aiobotocore-emr-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23492 2023-08-02 14:38:23.000000 types-aiobotocore-emr-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:16.933588 types-aiobotocore-emr-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:38:23.000000 types-aiobotocore-emr-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.917588 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-02 14:38:23.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-02 14:38:23.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:38:23.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-08-02 14:38:25.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46366 2023-08-02 14:38:25.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-08-02 14:38:25.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15743 2023-08-02 14:38:25.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-08-02 14:38:25.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-08-02 14:38:25.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:23.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    85661 2023-08-02 14:38:27.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    85543 2023-08-02 14:38:26.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:23.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-02 14:38:25.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-02 14:38:25.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.917588 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-08-02 14:52:16.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:16.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:16.000000 types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.964162 types-aiobotocore-emr-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:52.000000 types-aiobotocore-emr-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-08-04 12:00:52.964162 types-aiobotocore-emr-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-04 11:45:52.000000 types-aiobotocore-emr-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:52.964162 types-aiobotocore-emr-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:45:52.000000 types-aiobotocore-emr-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.964162 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-04 11:45:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-04 11:45:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:45:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46357 2023-08-04 11:45:54.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-08-04 11:45:54.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-08-04 11:45:54.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15743 2023-08-04 11:45:54.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-08-04 11:45:54.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-08-04 11:45:54.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79599 2023-08-04 11:45:56.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79493 2023-08-04 11:45:55.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-08-04 11:45:54.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-08-04 11:45:54.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:52.964162 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-08-04 12:00:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:00:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:52.000000 types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-emr-2.5.2.post1/LICENSE` & `types-aiobotocore-emr-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post1/setup.py` & `types-aiobotocore-emr-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-emr",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EMR 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/__init__.py` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/__init__.pyi` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/__main__.py` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EMR 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.EMR 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR\nOther"
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

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/client.py` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,21 +46,21 @@
     ListStudioSessionMappingsPaginator,
     ListStudiosPaginator,
 )
 from .type_defs import (
     AddInstanceFleetOutputTypeDef,
     AddInstanceGroupsOutputTypeDef,
     AddJobFlowStepsOutputTypeDef,
-    ApplicationUnionTypeDef,
+    ApplicationTypeDef,
     AutoScalingPolicyTypeDef,
     AutoTerminationPolicyTypeDef,
-    BlockPublicAccessConfigurationUnionTypeDef,
-    BootstrapActionConfigUnionTypeDef,
+    BlockPublicAccessConfigurationTypeDef,
+    BootstrapActionConfigTypeDef,
     CancelStepsOutputTypeDef,
-    ConfigurationUnionTypeDef,
+    ConfigurationTypeDef,
     CreateSecurityConfigurationOutputTypeDef,
     CreateStudioOutputTypeDef,
     DescribeClusterOutputTypeDef,
     DescribeJobFlowsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     DescribeSecurityConfigurationOutputTypeDef,
@@ -96,15 +96,15 @@
     NotebookS3LocationFromInputTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
     PlacementGroupConfigTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     ReleaseLabelFilterTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
-    StepConfigUnionTypeDef,
+    StepConfigTypeDef,
     SupportedProductConfigTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 from .waiter import ClusterRunningWaiter, ClusterTerminatedWaiter, StepCompleteWaiter
 
 if sys.version_info >= (3, 9):
@@ -165,19 +165,15 @@
         Adds one or more instance groups to a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_instance_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#add_instance_groups)
         """
 
     async def add_job_flow_steps(
-        self,
-        *,
-        JobFlowId: str,
-        Steps: Sequence[StepConfigUnionTypeDef],
-        ExecutionRoleArn: str = ...
+        self, *, JobFlowId: str, Steps: Sequence[StepConfigTypeDef], ExecutionRoleArn: str = ...
     ) -> AddJobFlowStepsOutputTypeDef:
         """
         AddJobFlowSteps adds new steps to a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_job_flow_steps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#add_job_flow_steps)
         """
@@ -657,15 +653,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_auto_termination_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#put_auto_termination_policy)
         """
 
     async def put_block_public_access_configuration(
-        self, *, BlockPublicAccessConfiguration: BlockPublicAccessConfigurationUnionTypeDef
+        self, *, BlockPublicAccessConfiguration: BlockPublicAccessConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon EMR block public access configuration for your
         Amazon Web Services account in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_block_public_access_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#put_block_public_access_configuration)
@@ -723,20 +719,20 @@
         Name: str,
         Instances: JobFlowInstancesConfigTypeDef,
         LogUri: str = ...,
         LogEncryptionKmsKeyId: str = ...,
         AdditionalInfo: str = ...,
         AmiVersion: str = ...,
         ReleaseLabel: str = ...,
-        Steps: Sequence[StepConfigUnionTypeDef] = ...,
-        BootstrapActions: Sequence[BootstrapActionConfigUnionTypeDef] = ...,
+        Steps: Sequence[StepConfigTypeDef] = ...,
+        BootstrapActions: Sequence[BootstrapActionConfigTypeDef] = ...,
         SupportedProducts: Sequence[str] = ...,
         NewSupportedProducts: Sequence[SupportedProductConfigTypeDef] = ...,
-        Applications: Sequence[ApplicationUnionTypeDef] = ...,
-        Configurations: Sequence[ConfigurationUnionTypeDef] = ...,
+        Applications: Sequence[ApplicationTypeDef] = ...,
+        Configurations: Sequence["ConfigurationTypeDef"] = ...,
         VisibleToAllUsers: bool = ...,
         JobFlowRole: str = ...,
         ServiceRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SecurityConfiguration: str = ...,
         AutoScalingRole: str = ...,
         ScaleDownBehavior: ScaleDownBehaviorType = ...,
```

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/client.pyi` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,21 +46,21 @@
     ListStudioSessionMappingsPaginator,
     ListStudiosPaginator,
 )
 from .type_defs import (
     AddInstanceFleetOutputTypeDef,
     AddInstanceGroupsOutputTypeDef,
     AddJobFlowStepsOutputTypeDef,
-    ApplicationUnionTypeDef,
+    ApplicationTypeDef,
     AutoScalingPolicyTypeDef,
     AutoTerminationPolicyTypeDef,
-    BlockPublicAccessConfigurationUnionTypeDef,
-    BootstrapActionConfigUnionTypeDef,
+    BlockPublicAccessConfigurationTypeDef,
+    BootstrapActionConfigTypeDef,
     CancelStepsOutputTypeDef,
-    ConfigurationUnionTypeDef,
+    ConfigurationTypeDef,
     CreateSecurityConfigurationOutputTypeDef,
     CreateStudioOutputTypeDef,
     DescribeClusterOutputTypeDef,
     DescribeJobFlowsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     DescribeSecurityConfigurationOutputTypeDef,
@@ -96,15 +96,15 @@
     NotebookS3LocationFromInputTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
     PlacementGroupConfigTypeDef,
     PutAutoScalingPolicyOutputTypeDef,
     ReleaseLabelFilterTypeDef,
     RunJobFlowOutputTypeDef,
     StartNotebookExecutionOutputTypeDef,
-    StepConfigUnionTypeDef,
+    StepConfigTypeDef,
     SupportedProductConfigTypeDef,
     TagTypeDef,
     TimestampTypeDef,
 )
 from .waiter import ClusterRunningWaiter, ClusterTerminatedWaiter, StepCompleteWaiter
 
 if sys.version_info >= (3, 9):
@@ -158,19 +158,15 @@
         """
         Adds one or more instance groups to a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_instance_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#add_instance_groups)
         """
     async def add_job_flow_steps(
-        self,
-        *,
-        JobFlowId: str,
-        Steps: Sequence[StepConfigUnionTypeDef],
-        ExecutionRoleArn: str = ...
+        self, *, JobFlowId: str, Steps: Sequence[StepConfigTypeDef], ExecutionRoleArn: str = ...
     ) -> AddJobFlowStepsOutputTypeDef:
         """
         AddJobFlowSteps adds new steps to a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.add_job_flow_steps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#add_job_flow_steps)
         """
@@ -609,15 +605,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_auto_termination_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#put_auto_termination_policy)
         """
     async def put_block_public_access_configuration(
-        self, *, BlockPublicAccessConfiguration: BlockPublicAccessConfigurationUnionTypeDef
+        self, *, BlockPublicAccessConfiguration: BlockPublicAccessConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         Creates or updates an Amazon EMR block public access configuration for your
         Amazon Web Services account in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client.put_block_public_access_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr/client/#put_block_public_access_configuration)
@@ -669,20 +665,20 @@
         Name: str,
         Instances: JobFlowInstancesConfigTypeDef,
         LogUri: str = ...,
         LogEncryptionKmsKeyId: str = ...,
         AdditionalInfo: str = ...,
         AmiVersion: str = ...,
         ReleaseLabel: str = ...,
-        Steps: Sequence[StepConfigUnionTypeDef] = ...,
-        BootstrapActions: Sequence[BootstrapActionConfigUnionTypeDef] = ...,
+        Steps: Sequence[StepConfigTypeDef] = ...,
+        BootstrapActions: Sequence[BootstrapActionConfigTypeDef] = ...,
         SupportedProducts: Sequence[str] = ...,
         NewSupportedProducts: Sequence[SupportedProductConfigTypeDef] = ...,
-        Applications: Sequence[ApplicationUnionTypeDef] = ...,
-        Configurations: Sequence[ConfigurationUnionTypeDef] = ...,
+        Applications: Sequence[ApplicationTypeDef] = ...,
+        Configurations: Sequence["ConfigurationTypeDef"] = ...,
         VisibleToAllUsers: bool = ...,
         JobFlowRole: str = ...,
         ServiceRole: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SecurityConfiguration: str = ...,
         AutoScalingRole: str = ...,
         ScaleDownBehavior: ScaleDownBehaviorType = ...,
```

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/literals.py` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/literals.pyi` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/paginator.py` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/paginator.pyi` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/type_defs.py` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,37 +63,33 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "ApplicationOutputTypeDef",
     "ApplicationTypeDef",
     "ScalingConstraintsTypeDef",
     "AutoScalingPolicyStateChangeReasonTypeDef",
     "AutoTerminationPolicyTypeDef",
     "BlockPublicAccessConfigurationMetadataTypeDef",
     "PortRangeTypeDef",
-    "ScriptBootstrapActionConfigOutputTypeDef",
     "ScriptBootstrapActionConfigTypeDef",
     "CancelStepsInfoTypeDef",
     "CancelStepsInputRequestTypeDef",
     "MetricDimensionTypeDef",
     "ClusterStateChangeReasonTypeDef",
     "ClusterTimelineTypeDef",
     "ErrorDetailTypeDef",
     "Ec2InstanceAttributesTypeDef",
     "KerberosAttributesTypeDef",
     "PlacementGroupConfigTypeDef",
     "CommandTypeDef",
     "ComputeLimitsTypeDef",
-    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
-    "ConfigurationUnionTypeDef",
     "CreateSecurityConfigurationInputRequestTypeDef",
     "CreateStudioSessionMappingInputRequestTypeDef",
     "UsernamePasswordTypeDef",
     "DeleteSecurityConfigurationInputRequestTypeDef",
     "DeleteStudioInputRequestTypeDef",
     "DeleteStudioSessionMappingInputRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -121,21 +117,19 @@
     "OnDemandResizingSpecificationTypeDef",
     "SpotResizingSpecificationTypeDef",
     "InstanceFleetStateChangeReasonTypeDef",
     "InstanceFleetTimelineTypeDef",
     "InstanceGroupDetailTypeDef",
     "InstanceGroupStateChangeReasonTypeDef",
     "InstanceGroupTimelineTypeDef",
-    "InstanceResizePolicyOutputTypeDef",
     "InstanceResizePolicyTypeDef",
     "InstanceStateChangeReasonTypeDef",
     "InstanceTimelineTypeDef",
     "JobFlowExecutionStatusDetailTypeDef",
     "PlacementTypeTypeDef",
-    "PlacementTypeOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ListBootstrapActionsInputRequestTypeDef",
     "ListInstanceFleetsInputRequestTypeDef",
     "ListInstanceGroupsInputRequestTypeDef",
     "ListInstancesInputRequestTypeDef",
     "ReleaseLabelFilterTypeDef",
     "ListSecurityConfigurationsInputRequestTypeDef",
@@ -178,24 +172,20 @@
     "ListReleaseLabelsOutputTypeDef",
     "ModifyClusterOutputTypeDef",
     "RunJobFlowOutputTypeDef",
     "StartNotebookExecutionOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreateStudioInputRequestTypeDef",
     "StudioTypeDef",
-    "ApplicationUnionTypeDef",
     "AutoScalingPolicyStatusTypeDef",
     "GetAutoTerminationPolicyOutputTypeDef",
     "PutAutoTerminationPolicyInputRequestTypeDef",
-    "BlockPublicAccessConfigurationOutputTypeDef",
     "BlockPublicAccessConfigurationTypeDef",
-    "BootstrapActionConfigOutputTypeDef",
     "BootstrapActionConfigTypeDef",
     "CancelStepsOutputTypeDef",
-    "CloudWatchAlarmDefinitionOutputTypeDef",
     "CloudWatchAlarmDefinitionTypeDef",
     "ClusterStatusTypeDef",
     "ListBootstrapActionsOutputTypeDef",
     "ManagedScalingPolicyTypeDef",
     "CredentialsTypeDef",
     "DescribeClusterInputClusterRunningWaitTypeDef",
     "DescribeClusterInputClusterTerminatedWaitTypeDef",
@@ -203,20 +193,18 @@
     "DescribeJobFlowsInputRequestTypeDef",
     "ListClustersInputRequestTypeDef",
     "ListNotebookExecutionsInputRequestTypeDef",
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
-    "HadoopJarStepConfigOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
     "InstanceFleetResizingSpecificationsTypeDef",
     "InstanceFleetStatusTypeDef",
     "InstanceGroupStatusTypeDef",
-    "ShrinkPolicyOutputTypeDef",
     "ShrinkPolicyTypeDef",
     "InstanceStatusTypeDef",
     "JobFlowInstancesDetailTypeDef",
     "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     "ListClustersInputListClustersPaginateTypeDef",
     "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
     "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
@@ -235,55 +223,49 @@
     "NotebookExecutionTypeDef",
     "OnDemandProvisioningSpecificationTypeDef",
     "StartNotebookExecutionInputRequestTypeDef",
     "ScalingActionTypeDef",
     "StepStatusTypeDef",
     "DescribeStudioOutputTypeDef",
     "GetBlockPublicAccessConfigurationOutputTypeDef",
-    "BlockPublicAccessConfigurationUnionTypeDef",
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     "BootstrapActionDetailTypeDef",
-    "BootstrapActionConfigUnionTypeDef",
-    "ScalingTriggerOutputTypeDef",
     "ScalingTriggerTypeDef",
     "ClusterSummaryTypeDef",
     "ClusterTypeDef",
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
     "EbsConfigurationTypeDef",
     "InstanceTypeSpecificationTypeDef",
-    "StepConfigOutputTypeDef",
     "StepConfigTypeDef",
     "InstanceFleetModifyConfigTypeDef",
     "InstanceGroupModifyConfigTypeDef",
     "InstanceTypeDef",
     "ListNotebookExecutionsOutputTypeDef",
     "DescribeNotebookExecutionOutputTypeDef",
     "InstanceFleetProvisioningSpecificationsTypeDef",
     "StepSummaryTypeDef",
     "StepTypeDef",
-    "ScalingRuleOutputTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
     "InstanceTypeConfigTypeDef",
+    "AddJobFlowStepsInputRequestTypeDef",
     "StepDetailTypeDef",
-    "StepConfigUnionTypeDef",
     "ModifyInstanceFleetInputRequestTypeDef",
     "ModifyInstanceGroupsInputRequestTypeDef",
     "ListInstancesOutputTypeDef",
     "InstanceFleetTypeDef",
     "ListStepsOutputTypeDef",
     "DescribeStepOutputTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyTypeDef",
     "InstanceFleetConfigTypeDef",
     "JobFlowDetailTypeDef",
-    "AddJobFlowStepsInputRequestTypeDef",
     "ListInstanceFleetsOutputTypeDef",
     "InstanceGroupTypeDef",
     "PutAutoScalingPolicyOutputTypeDef",
     "InstanceGroupConfigTypeDef",
     "PutAutoScalingPolicyInputRequestTypeDef",
     "AddInstanceFleetInputRequestTypeDef",
     "DescribeJobFlowsOutputTypeDef",
@@ -309,32 +291,21 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ApplicationOutputTypeDef = TypedDict(
-    "ApplicationOutputTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-        "Args": List[str],
-        "AdditionalInfo": Dict[str, str],
-    },
-    total=False,
-)
-
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Name": str,
         "Version": str,
-        "Args": Sequence[str],
-        "AdditionalInfo": Mapping[str, str],
+        "Args": List[str],
+        "AdditionalInfo": Dict[str, str],
     },
     total=False,
 )
 
 ScalingConstraintsTypeDef = TypedDict(
     "ScalingConstraintsTypeDef",
     {
@@ -383,46 +354,24 @@
 )
 
 
 class PortRangeTypeDef(_RequiredPortRangeTypeDef, _OptionalPortRangeTypeDef):
     pass
 
 
-_RequiredScriptBootstrapActionConfigOutputTypeDef = TypedDict(
-    "_RequiredScriptBootstrapActionConfigOutputTypeDef",
-    {
-        "Path": str,
-    },
-)
-_OptionalScriptBootstrapActionConfigOutputTypeDef = TypedDict(
-    "_OptionalScriptBootstrapActionConfigOutputTypeDef",
-    {
-        "Args": List[str],
-    },
-    total=False,
-)
-
-
-class ScriptBootstrapActionConfigOutputTypeDef(
-    _RequiredScriptBootstrapActionConfigOutputTypeDef,
-    _OptionalScriptBootstrapActionConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredScriptBootstrapActionConfigTypeDef = TypedDict(
     "_RequiredScriptBootstrapActionConfigTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalScriptBootstrapActionConfigTypeDef = TypedDict(
     "_OptionalScriptBootstrapActionConfigTypeDef",
     {
-        "Args": Sequence[str],
+        "Args": List[str],
     },
     total=False,
 )
 
 
 class ScriptBootstrapActionConfigTypeDef(
     _RequiredScriptBootstrapActionConfigTypeDef, _OptionalScriptBootstrapActionConfigTypeDef
@@ -591,35 +540,24 @@
 )
 
 
 class ComputeLimitsTypeDef(_RequiredComputeLimitsTypeDef, _OptionalComputeLimitsTypeDef):
     pass
 
 
-ConfigurationOutputTypeDef = TypedDict(
-    "ConfigurationOutputTypeDef",
-    {
-        "Classification": str,
-        "Configurations": List[Dict[str, Any]],
-        "Properties": Dict[str, str],
-    },
-    total=False,
-)
-
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Classification": str,
         "Configurations": Sequence[Dict[str, Any]],
         "Properties": Mapping[str, str],
     },
     total=False,
 )
 
-ConfigurationUnionTypeDef = Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]
 CreateSecurityConfigurationInputRequestTypeDef = TypedDict(
     "CreateSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
         "SecurityConfiguration": str,
     },
 )
@@ -1019,29 +957,19 @@
         "CreationDateTime": datetime,
         "ReadyDateTime": datetime,
         "EndDateTime": datetime,
     },
     total=False,
 )
 
-InstanceResizePolicyOutputTypeDef = TypedDict(
-    "InstanceResizePolicyOutputTypeDef",
-    {
-        "InstancesToTerminate": List[str],
-        "InstancesToProtect": List[str],
-        "InstanceTerminationTimeout": int,
-    },
-    total=False,
-)
-
 InstanceResizePolicyTypeDef = TypedDict(
     "InstanceResizePolicyTypeDef",
     {
-        "InstancesToTerminate": Sequence[str],
-        "InstancesToProtect": Sequence[str],
+        "InstancesToTerminate": List[str],
+        "InstancesToProtect": List[str],
         "InstanceTerminationTimeout": int,
     },
     total=False,
 )
 
 InstanceStateChangeReasonTypeDef = TypedDict(
     "InstanceStateChangeReasonTypeDef",
@@ -1087,23 +1015,14 @@
     pass
 
 
 PlacementTypeTypeDef = TypedDict(
     "PlacementTypeTypeDef",
     {
         "AvailabilityZone": str,
-        "AvailabilityZones": Sequence[str],
-    },
-    total=False,
-)
-
-PlacementTypeOutputTypeDef = TypedDict(
-    "PlacementTypeOutputTypeDef",
-    {
-        "AvailabilityZone": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
@@ -1747,15 +1666,14 @@
         "IdpAuthUrl": str,
         "IdpRelayStateParameterName": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-ApplicationUnionTypeDef = Union[ApplicationTypeDef, ApplicationOutputTypeDef]
 AutoScalingPolicyStatusTypeDef = TypedDict(
     "AutoScalingPolicyStatusTypeDef",
     {
         "State": AutoScalingPolicyStateType,
         "StateChangeReason": AutoScalingPolicyStateChangeReasonTypeDef,
     },
     total=False,
@@ -1787,65 +1705,35 @@
 class PutAutoTerminationPolicyInputRequestTypeDef(
     _RequiredPutAutoTerminationPolicyInputRequestTypeDef,
     _OptionalPutAutoTerminationPolicyInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
-    "_RequiredBlockPublicAccessConfigurationOutputTypeDef",
-    {
-        "BlockPublicSecurityGroupRules": bool,
-    },
-)
-_OptionalBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
-    "_OptionalBlockPublicAccessConfigurationOutputTypeDef",
-    {
-        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeTypeDef],
-    },
-    total=False,
-)
-
-
-class BlockPublicAccessConfigurationOutputTypeDef(
-    _RequiredBlockPublicAccessConfigurationOutputTypeDef,
-    _OptionalBlockPublicAccessConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredBlockPublicAccessConfigurationTypeDef = TypedDict(
     "_RequiredBlockPublicAccessConfigurationTypeDef",
     {
         "BlockPublicSecurityGroupRules": bool,
     },
 )
 _OptionalBlockPublicAccessConfigurationTypeDef = TypedDict(
     "_OptionalBlockPublicAccessConfigurationTypeDef",
     {
-        "PermittedPublicSecurityGroupRuleRanges": Sequence[PortRangeTypeDef],
+        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeTypeDef],
     },
     total=False,
 )
 
 
 class BlockPublicAccessConfigurationTypeDef(
     _RequiredBlockPublicAccessConfigurationTypeDef, _OptionalBlockPublicAccessConfigurationTypeDef
 ):
     pass
 
 
-BootstrapActionConfigOutputTypeDef = TypedDict(
-    "BootstrapActionConfigOutputTypeDef",
-    {
-        "Name": str,
-        "ScriptBootstrapAction": ScriptBootstrapActionConfigOutputTypeDef,
-    },
-)
-
 BootstrapActionConfigTypeDef = TypedDict(
     "BootstrapActionConfigTypeDef",
     {
         "Name": str,
         "ScriptBootstrapAction": ScriptBootstrapActionConfigTypeDef,
     },
 )
@@ -1854,42 +1742,14 @@
     "CancelStepsOutputTypeDef",
     {
         "CancelStepsInfoList": List[CancelStepsInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
-    "_RequiredCloudWatchAlarmDefinitionOutputTypeDef",
-    {
-        "ComparisonOperator": ComparisonOperatorType,
-        "MetricName": str,
-        "Period": int,
-        "Threshold": float,
-    },
-)
-_OptionalCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
-    "_OptionalCloudWatchAlarmDefinitionOutputTypeDef",
-    {
-        "EvaluationPeriods": int,
-        "Namespace": str,
-        "Statistic": StatisticType,
-        "Unit": UnitType,
-        "Dimensions": List[MetricDimensionTypeDef],
-    },
-    total=False,
-)
-
-
-class CloudWatchAlarmDefinitionOutputTypeDef(
-    _RequiredCloudWatchAlarmDefinitionOutputTypeDef, _OptionalCloudWatchAlarmDefinitionOutputTypeDef
-):
-    pass
-
-
 _RequiredCloudWatchAlarmDefinitionTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmDefinitionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
         "MetricName": str,
         "Period": int,
         "Threshold": float,
@@ -2097,37 +1957,14 @@
     "GetStudioSessionMappingOutputTypeDef",
     {
         "SessionMapping": SessionMappingDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredHadoopJarStepConfigOutputTypeDef = TypedDict(
-    "_RequiredHadoopJarStepConfigOutputTypeDef",
-    {
-        "Jar": str,
-    },
-)
-_OptionalHadoopJarStepConfigOutputTypeDef = TypedDict(
-    "_OptionalHadoopJarStepConfigOutputTypeDef",
-    {
-        "Properties": List[KeyValueTypeDef],
-        "MainClass": str,
-        "Args": List[str],
-    },
-    total=False,
-)
-
-
-class HadoopJarStepConfigOutputTypeDef(
-    _RequiredHadoopJarStepConfigOutputTypeDef, _OptionalHadoopJarStepConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredHadoopJarStepConfigTypeDef = TypedDict(
     "_RequiredHadoopJarStepConfigTypeDef",
     {
         "Jar": str,
     },
 )
 _OptionalHadoopJarStepConfigTypeDef = TypedDict(
@@ -2172,23 +2009,14 @@
         "State": InstanceGroupStateType,
         "StateChangeReason": InstanceGroupStateChangeReasonTypeDef,
         "Timeline": InstanceGroupTimelineTypeDef,
     },
     total=False,
 )
 
-ShrinkPolicyOutputTypeDef = TypedDict(
-    "ShrinkPolicyOutputTypeDef",
-    {
-        "DecommissionTimeout": int,
-        "InstanceResizePolicy": InstanceResizePolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 ShrinkPolicyTypeDef = TypedDict(
     "ShrinkPolicyTypeDef",
     {
         "DecommissionTimeout": int,
         "InstanceResizePolicy": InstanceResizePolicyTypeDef,
     },
     total=False,
@@ -2217,15 +2045,15 @@
     {
         "MasterPublicDnsName": str,
         "MasterInstanceId": str,
         "InstanceGroups": List[InstanceGroupDetailTypeDef],
         "NormalizedInstanceHours": int,
         "Ec2KeyName": str,
         "Ec2SubnetId": str,
-        "Placement": PlacementTypeOutputTypeDef,
+        "Placement": PlacementTypeTypeDef,
         "KeepJobFlowAliveWhenNoSteps": bool,
         "TerminationProtected": bool,
         "HadoopVersion": str,
     },
     total=False,
 )
 
@@ -2578,48 +2406,35 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     {
-        "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationOutputTypeDef,
+        "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
         "BlockPublicAccessConfigurationMetadata": BlockPublicAccessConfigurationMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BlockPublicAccessConfigurationUnionTypeDef = Union[
-    BlockPublicAccessConfigurationTypeDef, BlockPublicAccessConfigurationOutputTypeDef
-]
 PutBlockPublicAccessConfigurationInputRequestTypeDef = TypedDict(
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
     },
 )
 
 BootstrapActionDetailTypeDef = TypedDict(
     "BootstrapActionDetailTypeDef",
     {
-        "BootstrapActionConfig": BootstrapActionConfigOutputTypeDef,
+        "BootstrapActionConfig": BootstrapActionConfigTypeDef,
     },
     total=False,
 )
 
-BootstrapActionConfigUnionTypeDef = Union[
-    BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef
-]
-ScalingTriggerOutputTypeDef = TypedDict(
-    "ScalingTriggerOutputTypeDef",
-    {
-        "CloudWatchAlarmDefinition": CloudWatchAlarmDefinitionOutputTypeDef,
-    },
-)
-
 ScalingTriggerTypeDef = TypedDict(
     "ScalingTriggerTypeDef",
     {
         "CloudWatchAlarmDefinition": CloudWatchAlarmDefinitionTypeDef,
     },
 )
 
@@ -2648,20 +2463,20 @@
         "LogEncryptionKmsKeyId": str,
         "RequestedAmiVersion": str,
         "RunningAmiVersion": str,
         "ReleaseLabel": str,
         "AutoTerminate": bool,
         "TerminationProtected": bool,
         "VisibleToAllUsers": bool,
-        "Applications": List[ApplicationOutputTypeDef],
+        "Applications": List[ApplicationTypeDef],
         "Tags": List[TagTypeDef],
         "ServiceRole": str,
         "NormalizedInstanceHours": int,
         "MasterPublicDnsName": str,
-        "Configurations": List["ConfigurationOutputTypeDef"],
+        "Configurations": List["ConfigurationTypeDef"],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
         "CustomAmiId": str,
         "EbsRootVolumeSize": int,
         "RepoUpgradeOnBoot": RepoUpgradeOnBootType,
         "KerberosAttributes": KerberosAttributesTypeDef,
@@ -2711,42 +2526,22 @@
 InstanceTypeSpecificationTypeDef = TypedDict(
     "InstanceTypeSpecificationTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": int,
         "BidPrice": str,
         "BidPriceAsPercentageOfOnDemandPrice": float,
-        "Configurations": List["ConfigurationOutputTypeDef"],
+        "Configurations": List["ConfigurationTypeDef"],
         "EbsBlockDevices": List[EbsBlockDeviceTypeDef],
         "EbsOptimized": bool,
         "CustomAmiId": str,
     },
     total=False,
 )
 
-_RequiredStepConfigOutputTypeDef = TypedDict(
-    "_RequiredStepConfigOutputTypeDef",
-    {
-        "Name": str,
-        "HadoopJarStep": HadoopJarStepConfigOutputTypeDef,
-    },
-)
-_OptionalStepConfigOutputTypeDef = TypedDict(
-    "_OptionalStepConfigOutputTypeDef",
-    {
-        "ActionOnFailure": ActionOnFailureType,
-    },
-    total=False,
-)
-
-
-class StepConfigOutputTypeDef(_RequiredStepConfigOutputTypeDef, _OptionalStepConfigOutputTypeDef):
-    pass
-
-
 _RequiredStepConfigTypeDef = TypedDict(
     "_RequiredStepConfigTypeDef",
     {
         "Name": str,
         "HadoopJarStep": HadoopJarStepConfigTypeDef,
     },
 )
@@ -2877,37 +2672,14 @@
         "ActionOnFailure": ActionOnFailureType,
         "Status": StepStatusTypeDef,
         "ExecutionRoleArn": str,
     },
     total=False,
 )
 
-_RequiredScalingRuleOutputTypeDef = TypedDict(
-    "_RequiredScalingRuleOutputTypeDef",
-    {
-        "Name": str,
-        "Action": ScalingActionTypeDef,
-        "Trigger": ScalingTriggerOutputTypeDef,
-    },
-)
-_OptionalScalingRuleOutputTypeDef = TypedDict(
-    "_OptionalScalingRuleOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class ScalingRuleOutputTypeDef(
-    _RequiredScalingRuleOutputTypeDef, _OptionalScalingRuleOutputTypeDef
-):
-    pass
-
-
 _RequiredScalingRuleTypeDef = TypedDict(
     "_RequiredScalingRuleTypeDef",
     {
         "Name": str,
         "Action": ScalingActionTypeDef,
         "Trigger": ScalingTriggerTypeDef,
     },
@@ -2964,23 +2736,44 @@
 
 class InstanceTypeConfigTypeDef(
     _RequiredInstanceTypeConfigTypeDef, _OptionalInstanceTypeConfigTypeDef
 ):
     pass
 
 
+_RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
+    "_RequiredAddJobFlowStepsInputRequestTypeDef",
+    {
+        "JobFlowId": str,
+        "Steps": Sequence[StepConfigTypeDef],
+    },
+)
+_OptionalAddJobFlowStepsInputRequestTypeDef = TypedDict(
+    "_OptionalAddJobFlowStepsInputRequestTypeDef",
+    {
+        "ExecutionRoleArn": str,
+    },
+    total=False,
+)
+
+
+class AddJobFlowStepsInputRequestTypeDef(
+    _RequiredAddJobFlowStepsInputRequestTypeDef, _OptionalAddJobFlowStepsInputRequestTypeDef
+):
+    pass
+
+
 StepDetailTypeDef = TypedDict(
     "StepDetailTypeDef",
     {
-        "StepConfig": StepConfigOutputTypeDef,
+        "StepConfig": StepConfigTypeDef,
         "ExecutionStatusDetail": StepExecutionStatusDetailTypeDef,
     },
 )
 
-StepConfigUnionTypeDef = Union[StepConfigTypeDef, StepConfigOutputTypeDef]
 ModifyInstanceFleetInputRequestTypeDef = TypedDict(
     "ModifyInstanceFleetInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceFleet": InstanceFleetModifyConfigTypeDef,
     },
 )
@@ -3039,15 +2832,15 @@
 )
 
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "Status": AutoScalingPolicyStatusTypeDef,
         "Constraints": ScalingConstraintsTypeDef,
-        "Rules": List[ScalingRuleOutputTypeDef],
+        "Rules": List[ScalingRuleTypeDef],
     },
     total=False,
 )
 
 AutoScalingPolicyTypeDef = TypedDict(
     "AutoScalingPolicyTypeDef",
     {
@@ -3110,36 +2903,14 @@
 )
 
 
 class JobFlowDetailTypeDef(_RequiredJobFlowDetailTypeDef, _OptionalJobFlowDetailTypeDef):
     pass
 
 
-_RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
-    "_RequiredAddJobFlowStepsInputRequestTypeDef",
-    {
-        "JobFlowId": str,
-        "Steps": Sequence[StepConfigUnionTypeDef],
-    },
-)
-_OptionalAddJobFlowStepsInputRequestTypeDef = TypedDict(
-    "_OptionalAddJobFlowStepsInputRequestTypeDef",
-    {
-        "ExecutionRoleArn": str,
-    },
-    total=False,
-)
-
-
-class AddJobFlowStepsInputRequestTypeDef(
-    _RequiredAddJobFlowStepsInputRequestTypeDef, _OptionalAddJobFlowStepsInputRequestTypeDef
-):
-    pass
-
-
 ListInstanceFleetsOutputTypeDef = TypedDict(
     "ListInstanceFleetsOutputTypeDef",
     {
         "InstanceFleets": List[InstanceFleetTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3153,21 +2924,21 @@
         "Market": MarketTypeType,
         "InstanceGroupType": InstanceGroupTypeType,
         "BidPrice": str,
         "InstanceType": str,
         "RequestedInstanceCount": int,
         "RunningInstanceCount": int,
         "Status": InstanceGroupStatusTypeDef,
-        "Configurations": List["ConfigurationOutputTypeDef"],
+        "Configurations": List["ConfigurationTypeDef"],
         "ConfigurationsVersion": int,
-        "LastSuccessfullyAppliedConfigurations": List["ConfigurationOutputTypeDef"],
+        "LastSuccessfullyAppliedConfigurations": List["ConfigurationTypeDef"],
         "LastSuccessfullyAppliedConfigurationsVersion": int,
         "EbsBlockDevices": List[EbsBlockDeviceTypeDef],
         "EbsOptimized": bool,
-        "ShrinkPolicy": ShrinkPolicyOutputTypeDef,
+        "ShrinkPolicy": ShrinkPolicyTypeDef,
         "AutoScalingPolicy": AutoScalingPolicyDescriptionTypeDef,
         "CustomAmiId": str,
     },
     total=False,
 )
 
 PutAutoScalingPolicyOutputTypeDef = TypedDict(
@@ -3287,20 +3058,20 @@
     "_OptionalRunJobFlowInputRequestTypeDef",
     {
         "LogUri": str,
         "LogEncryptionKmsKeyId": str,
         "AdditionalInfo": str,
         "AmiVersion": str,
         "ReleaseLabel": str,
-        "Steps": Sequence[StepConfigUnionTypeDef],
-        "BootstrapActions": Sequence[BootstrapActionConfigUnionTypeDef],
+        "Steps": Sequence[StepConfigTypeDef],
+        "BootstrapActions": Sequence[BootstrapActionConfigTypeDef],
         "SupportedProducts": Sequence[str],
         "NewSupportedProducts": Sequence[SupportedProductConfigTypeDef],
-        "Applications": Sequence[ApplicationUnionTypeDef],
-        "Configurations": Sequence[ConfigurationUnionTypeDef],
+        "Applications": Sequence[ApplicationTypeDef],
+        "Configurations": Sequence["ConfigurationTypeDef"],
         "VisibleToAllUsers": bool,
         "JobFlowRole": str,
         "ServiceRole": str,
         "Tags": Sequence[TagTypeDef],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
```

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/type_defs.pyi` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -62,37 +62,33 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "ApplicationOutputTypeDef",
     "ApplicationTypeDef",
     "ScalingConstraintsTypeDef",
     "AutoScalingPolicyStateChangeReasonTypeDef",
     "AutoTerminationPolicyTypeDef",
     "BlockPublicAccessConfigurationMetadataTypeDef",
     "PortRangeTypeDef",
-    "ScriptBootstrapActionConfigOutputTypeDef",
     "ScriptBootstrapActionConfigTypeDef",
     "CancelStepsInfoTypeDef",
     "CancelStepsInputRequestTypeDef",
     "MetricDimensionTypeDef",
     "ClusterStateChangeReasonTypeDef",
     "ClusterTimelineTypeDef",
     "ErrorDetailTypeDef",
     "Ec2InstanceAttributesTypeDef",
     "KerberosAttributesTypeDef",
     "PlacementGroupConfigTypeDef",
     "CommandTypeDef",
     "ComputeLimitsTypeDef",
-    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
-    "ConfigurationUnionTypeDef",
     "CreateSecurityConfigurationInputRequestTypeDef",
     "CreateStudioSessionMappingInputRequestTypeDef",
     "UsernamePasswordTypeDef",
     "DeleteSecurityConfigurationInputRequestTypeDef",
     "DeleteStudioInputRequestTypeDef",
     "DeleteStudioSessionMappingInputRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -120,21 +116,19 @@
     "OnDemandResizingSpecificationTypeDef",
     "SpotResizingSpecificationTypeDef",
     "InstanceFleetStateChangeReasonTypeDef",
     "InstanceFleetTimelineTypeDef",
     "InstanceGroupDetailTypeDef",
     "InstanceGroupStateChangeReasonTypeDef",
     "InstanceGroupTimelineTypeDef",
-    "InstanceResizePolicyOutputTypeDef",
     "InstanceResizePolicyTypeDef",
     "InstanceStateChangeReasonTypeDef",
     "InstanceTimelineTypeDef",
     "JobFlowExecutionStatusDetailTypeDef",
     "PlacementTypeTypeDef",
-    "PlacementTypeOutputTypeDef",
     "PaginatorConfigTypeDef",
     "ListBootstrapActionsInputRequestTypeDef",
     "ListInstanceFleetsInputRequestTypeDef",
     "ListInstanceGroupsInputRequestTypeDef",
     "ListInstancesInputRequestTypeDef",
     "ReleaseLabelFilterTypeDef",
     "ListSecurityConfigurationsInputRequestTypeDef",
@@ -177,24 +171,20 @@
     "ListReleaseLabelsOutputTypeDef",
     "ModifyClusterOutputTypeDef",
     "RunJobFlowOutputTypeDef",
     "StartNotebookExecutionOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreateStudioInputRequestTypeDef",
     "StudioTypeDef",
-    "ApplicationUnionTypeDef",
     "AutoScalingPolicyStatusTypeDef",
     "GetAutoTerminationPolicyOutputTypeDef",
     "PutAutoTerminationPolicyInputRequestTypeDef",
-    "BlockPublicAccessConfigurationOutputTypeDef",
     "BlockPublicAccessConfigurationTypeDef",
-    "BootstrapActionConfigOutputTypeDef",
     "BootstrapActionConfigTypeDef",
     "CancelStepsOutputTypeDef",
-    "CloudWatchAlarmDefinitionOutputTypeDef",
     "CloudWatchAlarmDefinitionTypeDef",
     "ClusterStatusTypeDef",
     "ListBootstrapActionsOutputTypeDef",
     "ManagedScalingPolicyTypeDef",
     "CredentialsTypeDef",
     "DescribeClusterInputClusterRunningWaitTypeDef",
     "DescribeClusterInputClusterTerminatedWaitTypeDef",
@@ -202,20 +192,18 @@
     "DescribeJobFlowsInputRequestTypeDef",
     "ListClustersInputRequestTypeDef",
     "ListNotebookExecutionsInputRequestTypeDef",
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
-    "HadoopJarStepConfigOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
     "InstanceFleetResizingSpecificationsTypeDef",
     "InstanceFleetStatusTypeDef",
     "InstanceGroupStatusTypeDef",
-    "ShrinkPolicyOutputTypeDef",
     "ShrinkPolicyTypeDef",
     "InstanceStatusTypeDef",
     "JobFlowInstancesDetailTypeDef",
     "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
     "ListClustersInputListClustersPaginateTypeDef",
     "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
     "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
@@ -234,55 +222,49 @@
     "NotebookExecutionTypeDef",
     "OnDemandProvisioningSpecificationTypeDef",
     "StartNotebookExecutionInputRequestTypeDef",
     "ScalingActionTypeDef",
     "StepStatusTypeDef",
     "DescribeStudioOutputTypeDef",
     "GetBlockPublicAccessConfigurationOutputTypeDef",
-    "BlockPublicAccessConfigurationUnionTypeDef",
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     "BootstrapActionDetailTypeDef",
-    "BootstrapActionConfigUnionTypeDef",
-    "ScalingTriggerOutputTypeDef",
     "ScalingTriggerTypeDef",
     "ClusterSummaryTypeDef",
     "ClusterTypeDef",
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
     "EbsConfigurationTypeDef",
     "InstanceTypeSpecificationTypeDef",
-    "StepConfigOutputTypeDef",
     "StepConfigTypeDef",
     "InstanceFleetModifyConfigTypeDef",
     "InstanceGroupModifyConfigTypeDef",
     "InstanceTypeDef",
     "ListNotebookExecutionsOutputTypeDef",
     "DescribeNotebookExecutionOutputTypeDef",
     "InstanceFleetProvisioningSpecificationsTypeDef",
     "StepSummaryTypeDef",
     "StepTypeDef",
-    "ScalingRuleOutputTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
     "InstanceTypeConfigTypeDef",
+    "AddJobFlowStepsInputRequestTypeDef",
     "StepDetailTypeDef",
-    "StepConfigUnionTypeDef",
     "ModifyInstanceFleetInputRequestTypeDef",
     "ModifyInstanceGroupsInputRequestTypeDef",
     "ListInstancesOutputTypeDef",
     "InstanceFleetTypeDef",
     "ListStepsOutputTypeDef",
     "DescribeStepOutputTypeDef",
     "AutoScalingPolicyDescriptionTypeDef",
     "AutoScalingPolicyTypeDef",
     "InstanceFleetConfigTypeDef",
     "JobFlowDetailTypeDef",
-    "AddJobFlowStepsInputRequestTypeDef",
     "ListInstanceFleetsOutputTypeDef",
     "InstanceGroupTypeDef",
     "PutAutoScalingPolicyOutputTypeDef",
     "InstanceGroupConfigTypeDef",
     "PutAutoScalingPolicyInputRequestTypeDef",
     "AddInstanceFleetInputRequestTypeDef",
     "DescribeJobFlowsOutputTypeDef",
@@ -308,32 +290,21 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-ApplicationOutputTypeDef = TypedDict(
-    "ApplicationOutputTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-        "Args": List[str],
-        "AdditionalInfo": Dict[str, str],
-    },
-    total=False,
-)
-
 ApplicationTypeDef = TypedDict(
     "ApplicationTypeDef",
     {
         "Name": str,
         "Version": str,
-        "Args": Sequence[str],
-        "AdditionalInfo": Mapping[str, str],
+        "Args": List[str],
+        "AdditionalInfo": Dict[str, str],
     },
     total=False,
 )
 
 ScalingConstraintsTypeDef = TypedDict(
     "ScalingConstraintsTypeDef",
     {
@@ -380,44 +351,24 @@
     },
     total=False,
 )
 
 class PortRangeTypeDef(_RequiredPortRangeTypeDef, _OptionalPortRangeTypeDef):
     pass
 
-_RequiredScriptBootstrapActionConfigOutputTypeDef = TypedDict(
-    "_RequiredScriptBootstrapActionConfigOutputTypeDef",
-    {
-        "Path": str,
-    },
-)
-_OptionalScriptBootstrapActionConfigOutputTypeDef = TypedDict(
-    "_OptionalScriptBootstrapActionConfigOutputTypeDef",
-    {
-        "Args": List[str],
-    },
-    total=False,
-)
-
-class ScriptBootstrapActionConfigOutputTypeDef(
-    _RequiredScriptBootstrapActionConfigOutputTypeDef,
-    _OptionalScriptBootstrapActionConfigOutputTypeDef,
-):
-    pass
-
 _RequiredScriptBootstrapActionConfigTypeDef = TypedDict(
     "_RequiredScriptBootstrapActionConfigTypeDef",
     {
         "Path": str,
     },
 )
 _OptionalScriptBootstrapActionConfigTypeDef = TypedDict(
     "_OptionalScriptBootstrapActionConfigTypeDef",
     {
-        "Args": Sequence[str],
+        "Args": List[str],
     },
     total=False,
 )
 
 class ScriptBootstrapActionConfigTypeDef(
     _RequiredScriptBootstrapActionConfigTypeDef, _OptionalScriptBootstrapActionConfigTypeDef
 ):
@@ -576,35 +527,24 @@
     },
     total=False,
 )
 
 class ComputeLimitsTypeDef(_RequiredComputeLimitsTypeDef, _OptionalComputeLimitsTypeDef):
     pass
 
-ConfigurationOutputTypeDef = TypedDict(
-    "ConfigurationOutputTypeDef",
-    {
-        "Classification": str,
-        "Configurations": List[Dict[str, Any]],
-        "Properties": Dict[str, str],
-    },
-    total=False,
-)
-
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Classification": str,
         "Configurations": Sequence[Dict[str, Any]],
         "Properties": Mapping[str, str],
     },
     total=False,
 )
 
-ConfigurationUnionTypeDef = Union["ConfigurationTypeDef", "ConfigurationOutputTypeDef"]
 CreateSecurityConfigurationInputRequestTypeDef = TypedDict(
     "CreateSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
         "SecurityConfiguration": str,
     },
 )
@@ -990,29 +930,19 @@
         "CreationDateTime": datetime,
         "ReadyDateTime": datetime,
         "EndDateTime": datetime,
     },
     total=False,
 )
 
-InstanceResizePolicyOutputTypeDef = TypedDict(
-    "InstanceResizePolicyOutputTypeDef",
-    {
-        "InstancesToTerminate": List[str],
-        "InstancesToProtect": List[str],
-        "InstanceTerminationTimeout": int,
-    },
-    total=False,
-)
-
 InstanceResizePolicyTypeDef = TypedDict(
     "InstanceResizePolicyTypeDef",
     {
-        "InstancesToTerminate": Sequence[str],
-        "InstancesToProtect": Sequence[str],
+        "InstancesToTerminate": List[str],
+        "InstancesToProtect": List[str],
         "InstanceTerminationTimeout": int,
     },
     total=False,
 )
 
 InstanceStateChangeReasonTypeDef = TypedDict(
     "InstanceStateChangeReasonTypeDef",
@@ -1056,23 +986,14 @@
 ):
     pass
 
 PlacementTypeTypeDef = TypedDict(
     "PlacementTypeTypeDef",
     {
         "AvailabilityZone": str,
-        "AvailabilityZones": Sequence[str],
-    },
-    total=False,
-)
-
-PlacementTypeOutputTypeDef = TypedDict(
-    "PlacementTypeOutputTypeDef",
-    {
-        "AvailabilityZone": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
@@ -1692,15 +1613,14 @@
         "IdpAuthUrl": str,
         "IdpRelayStateParameterName": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-ApplicationUnionTypeDef = Union[ApplicationTypeDef, ApplicationOutputTypeDef]
 AutoScalingPolicyStatusTypeDef = TypedDict(
     "AutoScalingPolicyStatusTypeDef",
     {
         "State": AutoScalingPolicyStateType,
         "StateChangeReason": AutoScalingPolicyStateChangeReasonTypeDef,
     },
     total=False,
@@ -1730,61 +1650,33 @@
 
 class PutAutoTerminationPolicyInputRequestTypeDef(
     _RequiredPutAutoTerminationPolicyInputRequestTypeDef,
     _OptionalPutAutoTerminationPolicyInputRequestTypeDef,
 ):
     pass
 
-_RequiredBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
-    "_RequiredBlockPublicAccessConfigurationOutputTypeDef",
-    {
-        "BlockPublicSecurityGroupRules": bool,
-    },
-)
-_OptionalBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
-    "_OptionalBlockPublicAccessConfigurationOutputTypeDef",
-    {
-        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeTypeDef],
-    },
-    total=False,
-)
-
-class BlockPublicAccessConfigurationOutputTypeDef(
-    _RequiredBlockPublicAccessConfigurationOutputTypeDef,
-    _OptionalBlockPublicAccessConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredBlockPublicAccessConfigurationTypeDef = TypedDict(
     "_RequiredBlockPublicAccessConfigurationTypeDef",
     {
         "BlockPublicSecurityGroupRules": bool,
     },
 )
 _OptionalBlockPublicAccessConfigurationTypeDef = TypedDict(
     "_OptionalBlockPublicAccessConfigurationTypeDef",
     {
-        "PermittedPublicSecurityGroupRuleRanges": Sequence[PortRangeTypeDef],
+        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeTypeDef],
     },
     total=False,
 )
 
 class BlockPublicAccessConfigurationTypeDef(
     _RequiredBlockPublicAccessConfigurationTypeDef, _OptionalBlockPublicAccessConfigurationTypeDef
 ):
     pass
 
-BootstrapActionConfigOutputTypeDef = TypedDict(
-    "BootstrapActionConfigOutputTypeDef",
-    {
-        "Name": str,
-        "ScriptBootstrapAction": ScriptBootstrapActionConfigOutputTypeDef,
-    },
-)
-
 BootstrapActionConfigTypeDef = TypedDict(
     "BootstrapActionConfigTypeDef",
     {
         "Name": str,
         "ScriptBootstrapAction": ScriptBootstrapActionConfigTypeDef,
     },
 )
@@ -1793,40 +1685,14 @@
     "CancelStepsOutputTypeDef",
     {
         "CancelStepsInfoList": List[CancelStepsInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
-    "_RequiredCloudWatchAlarmDefinitionOutputTypeDef",
-    {
-        "ComparisonOperator": ComparisonOperatorType,
-        "MetricName": str,
-        "Period": int,
-        "Threshold": float,
-    },
-)
-_OptionalCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
-    "_OptionalCloudWatchAlarmDefinitionOutputTypeDef",
-    {
-        "EvaluationPeriods": int,
-        "Namespace": str,
-        "Statistic": StatisticType,
-        "Unit": UnitType,
-        "Dimensions": List[MetricDimensionTypeDef],
-    },
-    total=False,
-)
-
-class CloudWatchAlarmDefinitionOutputTypeDef(
-    _RequiredCloudWatchAlarmDefinitionOutputTypeDef, _OptionalCloudWatchAlarmDefinitionOutputTypeDef
-):
-    pass
-
 _RequiredCloudWatchAlarmDefinitionTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmDefinitionTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
         "MetricName": str,
         "Period": int,
         "Threshold": float,
@@ -2024,35 +1890,14 @@
     "GetStudioSessionMappingOutputTypeDef",
     {
         "SessionMapping": SessionMappingDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredHadoopJarStepConfigOutputTypeDef = TypedDict(
-    "_RequiredHadoopJarStepConfigOutputTypeDef",
-    {
-        "Jar": str,
-    },
-)
-_OptionalHadoopJarStepConfigOutputTypeDef = TypedDict(
-    "_OptionalHadoopJarStepConfigOutputTypeDef",
-    {
-        "Properties": List[KeyValueTypeDef],
-        "MainClass": str,
-        "Args": List[str],
-    },
-    total=False,
-)
-
-class HadoopJarStepConfigOutputTypeDef(
-    _RequiredHadoopJarStepConfigOutputTypeDef, _OptionalHadoopJarStepConfigOutputTypeDef
-):
-    pass
-
 _RequiredHadoopJarStepConfigTypeDef = TypedDict(
     "_RequiredHadoopJarStepConfigTypeDef",
     {
         "Jar": str,
     },
 )
 _OptionalHadoopJarStepConfigTypeDef = TypedDict(
@@ -2095,23 +1940,14 @@
         "State": InstanceGroupStateType,
         "StateChangeReason": InstanceGroupStateChangeReasonTypeDef,
         "Timeline": InstanceGroupTimelineTypeDef,
     },
     total=False,
 )
 
-ShrinkPolicyOutputTypeDef = TypedDict(
-    "ShrinkPolicyOutputTypeDef",
-    {
-        "DecommissionTimeout": int,
-        "InstanceResizePolicy": InstanceResizePolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 ShrinkPolicyTypeDef = TypedDict(
     "ShrinkPolicyTypeDef",
     {
         "DecommissionTimeout": int,
         "InstanceResizePolicy": InstanceResizePolicyTypeDef,
     },
     total=False,
@@ -2140,15 +1976,15 @@
     {
         "MasterPublicDnsName": str,
         "MasterInstanceId": str,
         "InstanceGroups": List[InstanceGroupDetailTypeDef],
         "NormalizedInstanceHours": int,
         "Ec2KeyName": str,
         "Ec2SubnetId": str,
-        "Placement": PlacementTypeOutputTypeDef,
+        "Placement": PlacementTypeTypeDef,
         "KeepJobFlowAliveWhenNoSteps": bool,
         "TerminationProtected": bool,
         "HadoopVersion": str,
     },
     total=False,
 )
 
@@ -2483,48 +2319,35 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     {
-        "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationOutputTypeDef,
+        "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
         "BlockPublicAccessConfigurationMetadata": BlockPublicAccessConfigurationMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BlockPublicAccessConfigurationUnionTypeDef = Union[
-    BlockPublicAccessConfigurationTypeDef, BlockPublicAccessConfigurationOutputTypeDef
-]
 PutBlockPublicAccessConfigurationInputRequestTypeDef = TypedDict(
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
     },
 )
 
 BootstrapActionDetailTypeDef = TypedDict(
     "BootstrapActionDetailTypeDef",
     {
-        "BootstrapActionConfig": BootstrapActionConfigOutputTypeDef,
+        "BootstrapActionConfig": BootstrapActionConfigTypeDef,
     },
     total=False,
 )
 
-BootstrapActionConfigUnionTypeDef = Union[
-    BootstrapActionConfigTypeDef, BootstrapActionConfigOutputTypeDef
-]
-ScalingTriggerOutputTypeDef = TypedDict(
-    "ScalingTriggerOutputTypeDef",
-    {
-        "CloudWatchAlarmDefinition": CloudWatchAlarmDefinitionOutputTypeDef,
-    },
-)
-
 ScalingTriggerTypeDef = TypedDict(
     "ScalingTriggerTypeDef",
     {
         "CloudWatchAlarmDefinition": CloudWatchAlarmDefinitionTypeDef,
     },
 )
 
@@ -2553,20 +2376,20 @@
         "LogEncryptionKmsKeyId": str,
         "RequestedAmiVersion": str,
         "RunningAmiVersion": str,
         "ReleaseLabel": str,
         "AutoTerminate": bool,
         "TerminationProtected": bool,
         "VisibleToAllUsers": bool,
-        "Applications": List[ApplicationOutputTypeDef],
+        "Applications": List[ApplicationTypeDef],
         "Tags": List[TagTypeDef],
         "ServiceRole": str,
         "NormalizedInstanceHours": int,
         "MasterPublicDnsName": str,
-        "Configurations": List["ConfigurationOutputTypeDef"],
+        "Configurations": List["ConfigurationTypeDef"],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
         "CustomAmiId": str,
         "EbsRootVolumeSize": int,
         "RepoUpgradeOnBoot": RepoUpgradeOnBootType,
         "KerberosAttributes": KerberosAttributesTypeDef,
@@ -2616,40 +2439,22 @@
 InstanceTypeSpecificationTypeDef = TypedDict(
     "InstanceTypeSpecificationTypeDef",
     {
         "InstanceType": str,
         "WeightedCapacity": int,
         "BidPrice": str,
         "BidPriceAsPercentageOfOnDemandPrice": float,
-        "Configurations": List["ConfigurationOutputTypeDef"],
+        "Configurations": List["ConfigurationTypeDef"],
         "EbsBlockDevices": List[EbsBlockDeviceTypeDef],
         "EbsOptimized": bool,
         "CustomAmiId": str,
     },
     total=False,
 )
 
-_RequiredStepConfigOutputTypeDef = TypedDict(
-    "_RequiredStepConfigOutputTypeDef",
-    {
-        "Name": str,
-        "HadoopJarStep": HadoopJarStepConfigOutputTypeDef,
-    },
-)
-_OptionalStepConfigOutputTypeDef = TypedDict(
-    "_OptionalStepConfigOutputTypeDef",
-    {
-        "ActionOnFailure": ActionOnFailureType,
-    },
-    total=False,
-)
-
-class StepConfigOutputTypeDef(_RequiredStepConfigOutputTypeDef, _OptionalStepConfigOutputTypeDef):
-    pass
-
 _RequiredStepConfigTypeDef = TypedDict(
     "_RequiredStepConfigTypeDef",
     {
         "Name": str,
         "HadoopJarStep": HadoopJarStepConfigTypeDef,
     },
 )
@@ -2774,35 +2579,14 @@
         "ActionOnFailure": ActionOnFailureType,
         "Status": StepStatusTypeDef,
         "ExecutionRoleArn": str,
     },
     total=False,
 )
 
-_RequiredScalingRuleOutputTypeDef = TypedDict(
-    "_RequiredScalingRuleOutputTypeDef",
-    {
-        "Name": str,
-        "Action": ScalingActionTypeDef,
-        "Trigger": ScalingTriggerOutputTypeDef,
-    },
-)
-_OptionalScalingRuleOutputTypeDef = TypedDict(
-    "_OptionalScalingRuleOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class ScalingRuleOutputTypeDef(
-    _RequiredScalingRuleOutputTypeDef, _OptionalScalingRuleOutputTypeDef
-):
-    pass
-
 _RequiredScalingRuleTypeDef = TypedDict(
     "_RequiredScalingRuleTypeDef",
     {
         "Name": str,
         "Action": ScalingActionTypeDef,
         "Trigger": ScalingTriggerTypeDef,
     },
@@ -2855,23 +2639,42 @@
 )
 
 class InstanceTypeConfigTypeDef(
     _RequiredInstanceTypeConfigTypeDef, _OptionalInstanceTypeConfigTypeDef
 ):
     pass
 
+_RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
+    "_RequiredAddJobFlowStepsInputRequestTypeDef",
+    {
+        "JobFlowId": str,
+        "Steps": Sequence[StepConfigTypeDef],
+    },
+)
+_OptionalAddJobFlowStepsInputRequestTypeDef = TypedDict(
+    "_OptionalAddJobFlowStepsInputRequestTypeDef",
+    {
+        "ExecutionRoleArn": str,
+    },
+    total=False,
+)
+
+class AddJobFlowStepsInputRequestTypeDef(
+    _RequiredAddJobFlowStepsInputRequestTypeDef, _OptionalAddJobFlowStepsInputRequestTypeDef
+):
+    pass
+
 StepDetailTypeDef = TypedDict(
     "StepDetailTypeDef",
     {
-        "StepConfig": StepConfigOutputTypeDef,
+        "StepConfig": StepConfigTypeDef,
         "ExecutionStatusDetail": StepExecutionStatusDetailTypeDef,
     },
 )
 
-StepConfigUnionTypeDef = Union[StepConfigTypeDef, StepConfigOutputTypeDef]
 ModifyInstanceFleetInputRequestTypeDef = TypedDict(
     "ModifyInstanceFleetInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceFleet": InstanceFleetModifyConfigTypeDef,
     },
 )
@@ -2930,15 +2733,15 @@
 )
 
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "Status": AutoScalingPolicyStatusTypeDef,
         "Constraints": ScalingConstraintsTypeDef,
-        "Rules": List[ScalingRuleOutputTypeDef],
+        "Rules": List[ScalingRuleTypeDef],
     },
     total=False,
 )
 
 AutoScalingPolicyTypeDef = TypedDict(
     "AutoScalingPolicyTypeDef",
     {
@@ -2997,34 +2800,14 @@
     },
     total=False,
 )
 
 class JobFlowDetailTypeDef(_RequiredJobFlowDetailTypeDef, _OptionalJobFlowDetailTypeDef):
     pass
 
-_RequiredAddJobFlowStepsInputRequestTypeDef = TypedDict(
-    "_RequiredAddJobFlowStepsInputRequestTypeDef",
-    {
-        "JobFlowId": str,
-        "Steps": Sequence[StepConfigUnionTypeDef],
-    },
-)
-_OptionalAddJobFlowStepsInputRequestTypeDef = TypedDict(
-    "_OptionalAddJobFlowStepsInputRequestTypeDef",
-    {
-        "ExecutionRoleArn": str,
-    },
-    total=False,
-)
-
-class AddJobFlowStepsInputRequestTypeDef(
-    _RequiredAddJobFlowStepsInputRequestTypeDef, _OptionalAddJobFlowStepsInputRequestTypeDef
-):
-    pass
-
 ListInstanceFleetsOutputTypeDef = TypedDict(
     "ListInstanceFleetsOutputTypeDef",
     {
         "InstanceFleets": List[InstanceFleetTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -3038,21 +2821,21 @@
         "Market": MarketTypeType,
         "InstanceGroupType": InstanceGroupTypeType,
         "BidPrice": str,
         "InstanceType": str,
         "RequestedInstanceCount": int,
         "RunningInstanceCount": int,
         "Status": InstanceGroupStatusTypeDef,
-        "Configurations": List["ConfigurationOutputTypeDef"],
+        "Configurations": List["ConfigurationTypeDef"],
         "ConfigurationsVersion": int,
-        "LastSuccessfullyAppliedConfigurations": List["ConfigurationOutputTypeDef"],
+        "LastSuccessfullyAppliedConfigurations": List["ConfigurationTypeDef"],
         "LastSuccessfullyAppliedConfigurationsVersion": int,
         "EbsBlockDevices": List[EbsBlockDeviceTypeDef],
         "EbsOptimized": bool,
-        "ShrinkPolicy": ShrinkPolicyOutputTypeDef,
+        "ShrinkPolicy": ShrinkPolicyTypeDef,
         "AutoScalingPolicy": AutoScalingPolicyDescriptionTypeDef,
         "CustomAmiId": str,
     },
     total=False,
 )
 
 PutAutoScalingPolicyOutputTypeDef = TypedDict(
@@ -3170,20 +2953,20 @@
     "_OptionalRunJobFlowInputRequestTypeDef",
     {
         "LogUri": str,
         "LogEncryptionKmsKeyId": str,
         "AdditionalInfo": str,
         "AmiVersion": str,
         "ReleaseLabel": str,
-        "Steps": Sequence[StepConfigUnionTypeDef],
-        "BootstrapActions": Sequence[BootstrapActionConfigUnionTypeDef],
+        "Steps": Sequence[StepConfigTypeDef],
+        "BootstrapActions": Sequence[BootstrapActionConfigTypeDef],
         "SupportedProducts": Sequence[str],
         "NewSupportedProducts": Sequence[SupportedProductConfigTypeDef],
-        "Applications": Sequence[ApplicationUnionTypeDef],
-        "Configurations": Sequence[ConfigurationUnionTypeDef],
+        "Applications": Sequence[ApplicationTypeDef],
+        "Configurations": Sequence["ConfigurationTypeDef"],
         "VisibleToAllUsers": bool,
         "JobFlowRole": str,
         "ServiceRole": str,
         "Tags": Sequence[TagTypeDef],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
```

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/waiter.py` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr/waiter.pyi` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-emr-2.5.2.post1/types_aiobotocore_emr.egg-info/SOURCES.txt` & `types-aiobotocore-emr-2.5.2.post2/types_aiobotocore_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

