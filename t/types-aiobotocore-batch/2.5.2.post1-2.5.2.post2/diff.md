# Comparing `tmp/types-aiobotocore-batch-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-batch-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-batch-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-batch-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:28 2023, max compression
```

## Comparing `types-aiobotocore-batch-2.5.2.post1.tar` & `types-aiobotocore-batch-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.385648 types-aiobotocore-batch-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-08-02 14:51:55.385648 types-aiobotocore-batch-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17335 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.385648 types-aiobotocore-batch-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.385648 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22223 2023-08-02 14:33:48.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22185 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-08-02 14:33:48.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-08-02 14:33:48.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-08-02 14:33:48.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-08-02 14:33:48.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51766 2023-08-02 14:33:50.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51697 2023-08-02 14:33:49.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:47.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.385648 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18845 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:51:55.000000 types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.399229 types-aiobotocore-batch-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-08-04 12:00:28.391228 types-aiobotocore-batch-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:28.399229 types-aiobotocore-batch-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.391228 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22115 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-08-04 11:41:00.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-08-04 11:41:00.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-08-04 11:41:01.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43982 2023-08-04 11:41:00.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:59.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.391228 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2023-08-04 12:00:28.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-04 12:00:28.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:28.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:28.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:28.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 12:00:28.000000 types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-batch-2.5.2.post1/LICENSE` & `types-aiobotocore-batch-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post1/setup.py` & `types-aiobotocore-batch-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-batch",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_batch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Batch 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__init__.py` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__init__.pyi` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/__main__.py` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Batch 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Batch 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch\nOther"
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

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/client.py` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,40 +34,40 @@
     DescribeJobQueuesPaginator,
     ListJobsPaginator,
     ListSchedulingPoliciesPaginator,
 )
 from .type_defs import (
     ArrayPropertiesTypeDef,
     ComputeEnvironmentOrderTypeDef,
-    ComputeResourceUnionTypeDef,
+    ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
-    ContainerPropertiesUnionTypeDef,
+    ContainerPropertiesTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobQueuesResponseTypeDef,
     DescribeJobsResponseTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     EksConfigurationTypeDef,
     EksPropertiesOverrideTypeDef,
-    EksPropertiesUnionTypeDef,
-    FairsharePolicyUnionTypeDef,
+    EksPropertiesTypeDef,
+    FairsharePolicyTypeDef,
     JobDependencyTypeDef,
     JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     ListJobsResponseTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NodeOverridesTypeDef,
-    NodePropertiesUnionTypeDef,
+    NodePropertiesTypeDef,
     RegisterJobDefinitionResponseTypeDef,
-    RetryStrategyUnionTypeDef,
+    RetryStrategyTypeDef,
     SubmitJobResponseTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     UpdatePolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -137,15 +137,15 @@
     async def create_compute_environment(
         self,
         *,
         computeEnvironmentName: str,
         type: CETypeType,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
-        computeResources: ComputeResourceUnionTypeDef = ...,
+        computeResources: ComputeResourceTypeDef = ...,
         serviceRole: str = ...,
         tags: Mapping[str, str] = ...,
         eksConfiguration: EksConfigurationTypeDef = ...
     ) -> CreateComputeEnvironmentResponseTypeDef:
         """
         Creates an Batch compute environment.
 
@@ -170,15 +170,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_job_queue)
         """
 
     async def create_scheduling_policy(
         self,
         *,
         name: str,
-        fairsharePolicy: FairsharePolicyUnionTypeDef = ...,
+        fairsharePolicy: FairsharePolicyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSchedulingPolicyResponseTypeDef:
         """
         Creates an Batch scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_scheduling_policy)
@@ -329,22 +329,22 @@
     async def register_job_definition(
         self,
         *,
         jobDefinitionName: str,
         type: JobDefinitionTypeType,
         parameters: Mapping[str, str] = ...,
         schedulingPriority: int = ...,
-        containerProperties: ContainerPropertiesUnionTypeDef = ...,
-        nodeProperties: NodePropertiesUnionTypeDef = ...,
-        retryStrategy: RetryStrategyUnionTypeDef = ...,
+        containerProperties: ContainerPropertiesTypeDef = ...,
+        nodeProperties: NodePropertiesTypeDef = ...,
+        retryStrategy: RetryStrategyTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         platformCapabilities: Sequence[PlatformCapabilityType] = ...,
-        eksProperties: EksPropertiesUnionTypeDef = ...
+        eksProperties: EksPropertiesTypeDef = ...
     ) -> RegisterJobDefinitionResponseTypeDef:
         """
         Registers an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#register_job_definition)
         """
@@ -358,15 +358,15 @@
         shareIdentifier: str = ...,
         schedulingPriorityOverride: int = ...,
         arrayProperties: ArrayPropertiesTypeDef = ...,
         dependsOn: Sequence[JobDependencyTypeDef] = ...,
         parameters: Mapping[str, str] = ...,
         containerOverrides: ContainerOverridesTypeDef = ...,
         nodeOverrides: NodeOverridesTypeDef = ...,
-        retryStrategy: RetryStrategyUnionTypeDef = ...,
+        retryStrategy: RetryStrategyTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...
     ) -> SubmitJobResponseTypeDef:
         """
         Submits an Batch job from a job definition.
@@ -429,15 +429,15 @@
         Updates a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_job_queue)
         """
 
     async def update_scheduling_policy(
-        self, *, arn: str, fairsharePolicy: FairsharePolicyUnionTypeDef = ...
+        self, *, arn: str, fairsharePolicy: FairsharePolicyTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_scheduling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_scheduling_policy)
         """
```

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/client.pyi` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -34,40 +34,40 @@
     DescribeJobQueuesPaginator,
     ListJobsPaginator,
     ListSchedulingPoliciesPaginator,
 )
 from .type_defs import (
     ArrayPropertiesTypeDef,
     ComputeEnvironmentOrderTypeDef,
-    ComputeResourceUnionTypeDef,
+    ComputeResourceTypeDef,
     ComputeResourceUpdateTypeDef,
     ContainerOverridesTypeDef,
-    ContainerPropertiesUnionTypeDef,
+    ContainerPropertiesTypeDef,
     CreateComputeEnvironmentResponseTypeDef,
     CreateJobQueueResponseTypeDef,
     CreateSchedulingPolicyResponseTypeDef,
     DescribeComputeEnvironmentsResponseTypeDef,
     DescribeJobDefinitionsResponseTypeDef,
     DescribeJobQueuesResponseTypeDef,
     DescribeJobsResponseTypeDef,
     DescribeSchedulingPoliciesResponseTypeDef,
     EksConfigurationTypeDef,
     EksPropertiesOverrideTypeDef,
-    EksPropertiesUnionTypeDef,
-    FairsharePolicyUnionTypeDef,
+    EksPropertiesTypeDef,
+    FairsharePolicyTypeDef,
     JobDependencyTypeDef,
     JobTimeoutTypeDef,
     KeyValuesPairTypeDef,
     ListJobsResponseTypeDef,
     ListSchedulingPoliciesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NodeOverridesTypeDef,
-    NodePropertiesUnionTypeDef,
+    NodePropertiesTypeDef,
     RegisterJobDefinitionResponseTypeDef,
-    RetryStrategyUnionTypeDef,
+    RetryStrategyTypeDef,
     SubmitJobResponseTypeDef,
     UpdateComputeEnvironmentResponseTypeDef,
     UpdateJobQueueResponseTypeDef,
     UpdatePolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -129,15 +129,15 @@
     async def create_compute_environment(
         self,
         *,
         computeEnvironmentName: str,
         type: CETypeType,
         state: CEStateType = ...,
         unmanagedvCpus: int = ...,
-        computeResources: ComputeResourceUnionTypeDef = ...,
+        computeResources: ComputeResourceTypeDef = ...,
         serviceRole: str = ...,
         tags: Mapping[str, str] = ...,
         eksConfiguration: EksConfigurationTypeDef = ...
     ) -> CreateComputeEnvironmentResponseTypeDef:
         """
         Creates an Batch compute environment.
 
@@ -160,15 +160,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_job_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_job_queue)
         """
     async def create_scheduling_policy(
         self,
         *,
         name: str,
-        fairsharePolicy: FairsharePolicyUnionTypeDef = ...,
+        fairsharePolicy: FairsharePolicyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateSchedulingPolicyResponseTypeDef:
         """
         Creates an Batch scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#create_scheduling_policy)
@@ -305,22 +305,22 @@
     async def register_job_definition(
         self,
         *,
         jobDefinitionName: str,
         type: JobDefinitionTypeType,
         parameters: Mapping[str, str] = ...,
         schedulingPriority: int = ...,
-        containerProperties: ContainerPropertiesUnionTypeDef = ...,
-        nodeProperties: NodePropertiesUnionTypeDef = ...,
-        retryStrategy: RetryStrategyUnionTypeDef = ...,
+        containerProperties: ContainerPropertiesTypeDef = ...,
+        nodeProperties: NodePropertiesTypeDef = ...,
+        retryStrategy: RetryStrategyTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         platformCapabilities: Sequence[PlatformCapabilityType] = ...,
-        eksProperties: EksPropertiesUnionTypeDef = ...
+        eksProperties: EksPropertiesTypeDef = ...
     ) -> RegisterJobDefinitionResponseTypeDef:
         """
         Registers an Batch job definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#register_job_definition)
         """
@@ -333,15 +333,15 @@
         shareIdentifier: str = ...,
         schedulingPriorityOverride: int = ...,
         arrayProperties: ArrayPropertiesTypeDef = ...,
         dependsOn: Sequence[JobDependencyTypeDef] = ...,
         parameters: Mapping[str, str] = ...,
         containerOverrides: ContainerOverridesTypeDef = ...,
         nodeOverrides: NodeOverridesTypeDef = ...,
-        retryStrategy: RetryStrategyUnionTypeDef = ...,
+        retryStrategy: RetryStrategyTypeDef = ...,
         propagateTags: bool = ...,
         timeout: JobTimeoutTypeDef = ...,
         tags: Mapping[str, str] = ...,
         eksPropertiesOverride: EksPropertiesOverrideTypeDef = ...
     ) -> SubmitJobResponseTypeDef:
         """
         Submits an Batch job from a job definition.
@@ -398,15 +398,15 @@
         """
         Updates a job queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_job_queue)
         """
     async def update_scheduling_policy(
-        self, *, arn: str, fairsharePolicy: FairsharePolicyUnionTypeDef = ...
+        self, *, arn: str, fairsharePolicy: FairsharePolicyTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a scheduling policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_scheduling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_batch/client/#update_scheduling_policy)
         """
```

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/literals.py` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/literals.pyi` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/paginator.py` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/paginator.pyi` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/type_defs.py` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_batch.type_defs import ArrayPropertiesDetailTypeDef
 
     data: ArrayPropertiesDetailTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ArrayJobDependencyType,
     AssignPublicIpType,
     CEStateType,
     CEStatusType,
     CETypeType,
@@ -70,53 +70,47 @@
     "DeregisterJobDefinitionRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
     "DescribeJobDefinitionsRequestRequestTypeDef",
     "DescribeJobQueuesRequestRequestTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
-    "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EksAttemptContainerDetailTypeDef",
     "EksContainerEnvironmentVariableTypeDef",
-    "EksContainerResourceRequirementsOutputTypeDef",
+    "EksContainerResourceRequirementsTypeDef",
     "EksContainerSecurityContextTypeDef",
     "EksContainerVolumeMountTypeDef",
-    "EksContainerResourceRequirementsTypeDef",
     "EksEmptyDirTypeDef",
     "EksHostPathTypeDef",
-    "EksMetadataOutputTypeDef",
     "EksMetadataTypeDef",
     "EksSecretTypeDef",
     "EvaluateOnExitTypeDef",
     "ShareAttributesTypeDef",
     "HostTypeDef",
     "JobTimeoutTypeDef",
     "JobDependencyTypeDef",
     "NodeDetailsTypeDef",
     "NodePropertiesSummaryTypeDef",
     "KeyValuesPairTypeDef",
-    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
     "ListSchedulingPoliciesRequestRequestTypeDef",
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttemptContainerDetailTypeDef",
     "CreateJobQueueRequestRequestTypeDef",
     "JobQueueDetailTypeDef",
     "UpdateJobQueueRequestRequestTypeDef",
-    "ComputeResourceOutputTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
     "ContainerOverridesTypeDef",
-    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "CreateComputeEnvironmentResponseTypeDef",
     "CreateJobQueueResponseTypeDef",
     "CreateSchedulingPolicyResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RegisterJobDefinitionResponseTypeDef",
     "SubmitJobResponseTypeDef",
@@ -124,67 +118,52 @@
     "UpdateJobQueueResponseTypeDef",
     "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
     "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
     "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
     "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "EksAttemptDetailTypeDef",
-    "EksContainerDetailTypeDef",
-    "EksContainerOutputTypeDef",
     "EksContainerOverrideTypeDef",
+    "EksContainerDetailTypeDef",
     "EksContainerTypeDef",
     "EksVolumeTypeDef",
-    "RetryStrategyOutputTypeDef",
     "RetryStrategyTypeDef",
-    "FairsharePolicyOutputTypeDef",
     "FairsharePolicyTypeDef",
     "JobSummaryTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "ListSchedulingPoliciesResponseTypeDef",
     "AttemptDetailTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "ComputeEnvironmentDetailTypeDef",
-    "ComputeResourceUnionTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "NodePropertyOverrideTypeDef",
     "VolumeTypeDef",
     "EksPodPropertiesOverrideTypeDef",
     "EksPodPropertiesDetailTypeDef",
-    "EksPodPropertiesOutputTypeDef",
     "EksPodPropertiesTypeDef",
-    "RetryStrategyUnionTypeDef",
-    "SchedulingPolicyDetailTypeDef",
     "CreateSchedulingPolicyRequestRequestTypeDef",
-    "FairsharePolicyUnionTypeDef",
+    "SchedulingPolicyDetailTypeDef",
     "UpdateSchedulingPolicyRequestRequestTypeDef",
     "ListJobsResponseTypeDef",
     "DescribeComputeEnvironmentsResponseTypeDef",
     "NodeOverridesTypeDef",
     "ContainerDetailTypeDef",
-    "ContainerPropertiesOutputTypeDef",
     "ContainerPropertiesTypeDef",
     "EksPropertiesOverrideTypeDef",
     "EksPropertiesDetailTypeDef",
-    "EksPropertiesOutputTypeDef",
     "EksPropertiesTypeDef",
     "DescribeSchedulingPoliciesResponseTypeDef",
-    "NodeRangePropertyOutputTypeDef",
-    "ContainerPropertiesUnionTypeDef",
     "NodeRangePropertyTypeDef",
     "SubmitJobRequestRequestTypeDef",
-    "EksPropertiesUnionTypeDef",
-    "NodePropertiesOutputTypeDef",
     "NodePropertiesTypeDef",
     "JobDefinitionTypeDef",
     "JobDetailTypeDef",
-    "NodePropertiesUnionTypeDef",
     "RegisterJobDefinitionRequestRequestTypeDef",
     "DescribeJobDefinitionsResponseTypeDef",
     "DescribeJobsResponseTypeDef",
 )
 
 ArrayPropertiesDetailTypeDef = TypedDict(
     "ArrayPropertiesDetailTypeDef",
@@ -453,45 +432,25 @@
 DescribeSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
 )
 
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
@@ -532,16 +491,16 @@
 
 class EksContainerEnvironmentVariableTypeDef(
     _RequiredEksContainerEnvironmentVariableTypeDef, _OptionalEksContainerEnvironmentVariableTypeDef
 ):
     pass
 
 
-EksContainerResourceRequirementsOutputTypeDef = TypedDict(
-    "EksContainerResourceRequirementsOutputTypeDef",
+EksContainerResourceRequirementsTypeDef = TypedDict(
+    "EksContainerResourceRequirementsTypeDef",
     {
         "limits": Dict[str, str],
         "requests": Dict[str, str],
     },
     total=False,
 )
 
@@ -563,23 +522,14 @@
         "name": str,
         "mountPath": str,
         "readOnly": bool,
     },
     total=False,
 )
 
-EksContainerResourceRequirementsTypeDef = TypedDict(
-    "EksContainerResourceRequirementsTypeDef",
-    {
-        "limits": Mapping[str, str],
-        "requests": Mapping[str, str],
-    },
-    total=False,
-)
-
 EksEmptyDirTypeDef = TypedDict(
     "EksEmptyDirTypeDef",
     {
         "medium": str,
         "sizeLimit": str,
     },
     total=False,
@@ -589,26 +539,18 @@
     "EksHostPathTypeDef",
     {
         "path": str,
     },
     total=False,
 )
 
-EksMetadataOutputTypeDef = TypedDict(
-    "EksMetadataOutputTypeDef",
-    {
-        "labels": Dict[str, str],
-    },
-    total=False,
-)
-
 EksMetadataTypeDef = TypedDict(
     "EksMetadataTypeDef",
     {
-        "labels": Mapping[str, str],
+        "labels": Dict[str, str],
     },
     total=False,
 )
 
 _RequiredEksSecretTypeDef = TypedDict(
     "_RequiredEksSecretTypeDef",
     {
@@ -717,45 +659,25 @@
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
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
-    },
-    total=False,
-)
-
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
@@ -892,50 +814,14 @@
 
 class UpdateJobQueueRequestRequestTypeDef(
     _RequiredUpdateJobQueueRequestRequestTypeDef, _OptionalUpdateJobQueueRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredComputeResourceOutputTypeDef = TypedDict(
-    "_RequiredComputeResourceOutputTypeDef",
-    {
-        "type": CRTypeType,
-        "maxvCpus": int,
-        "subnets": List[str],
-    },
-)
-_OptionalComputeResourceOutputTypeDef = TypedDict(
-    "_OptionalComputeResourceOutputTypeDef",
-    {
-        "allocationStrategy": CRAllocationStrategyType,
-        "minvCpus": int,
-        "desiredvCpus": int,
-        "instanceTypes": List[str],
-        "imageId": str,
-        "securityGroupIds": List[str],
-        "ec2KeyPair": str,
-        "instanceRole": str,
-        "tags": Dict[str, str],
-        "placementGroup": str,
-        "bidPercentage": int,
-        "spotIamFleetRole": str,
-        "launchTemplate": LaunchTemplateSpecificationTypeDef,
-        "ec2Configuration": List[Ec2ConfigurationTypeDef],
-    },
-    total=False,
-)
-
-
-class ComputeResourceOutputTypeDef(
-    _RequiredComputeResourceOutputTypeDef, _OptionalComputeResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredComputeResourceTypeDef = TypedDict(
     "_RequiredComputeResourceTypeDef",
     {
         "type": CRTypeType,
         "maxvCpus": int,
         "subnets": Sequence[str],
     },
@@ -999,47 +885,25 @@
         "instanceType": str,
         "environment": Sequence[KeyValuePairTypeDef],
         "resourceRequirements": Sequence[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
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
     "_OptionalLogConfigurationTypeDef",
     {
-        "options": Mapping[str, str],
-        "secretOptions": Sequence[SecretTypeDef],
+        "options": Dict[str, str],
+        "secretOptions": List[SecretTypeDef],
     },
     total=False,
 )
 
 
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
@@ -1188,88 +1052,60 @@
         "startedAt": int,
         "stoppedAt": int,
         "statusReason": str,
     },
     total=False,
 )
 
-EksContainerDetailTypeDef = TypedDict(
-    "EksContainerDetailTypeDef",
+EksContainerOverrideTypeDef = TypedDict(
+    "EksContainerOverrideTypeDef",
     {
-        "name": str,
         "image": str,
-        "imagePullPolicy": str,
-        "command": List[str],
-        "args": List[str],
-        "env": List[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsOutputTypeDef,
-        "exitCode": int,
-        "reason": str,
-        "volumeMounts": List[EksContainerVolumeMountTypeDef],
-        "securityContext": EksContainerSecurityContextTypeDef,
+        "command": Sequence[str],
+        "args": Sequence[str],
+        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
+        "resources": EksContainerResourceRequirementsTypeDef,
     },
     total=False,
 )
 
-_RequiredEksContainerOutputTypeDef = TypedDict(
-    "_RequiredEksContainerOutputTypeDef",
-    {
-        "image": str,
-    },
-)
-_OptionalEksContainerOutputTypeDef = TypedDict(
-    "_OptionalEksContainerOutputTypeDef",
+EksContainerDetailTypeDef = TypedDict(
+    "EksContainerDetailTypeDef",
     {
         "name": str,
+        "image": str,
         "imagePullPolicy": str,
         "command": List[str],
         "args": List[str],
         "env": List[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsOutputTypeDef,
+        "resources": EksContainerResourceRequirementsTypeDef,
+        "exitCode": int,
+        "reason": str,
         "volumeMounts": List[EksContainerVolumeMountTypeDef],
         "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
-
-class EksContainerOutputTypeDef(
-    _RequiredEksContainerOutputTypeDef, _OptionalEksContainerOutputTypeDef
-):
-    pass
-
-
-EksContainerOverrideTypeDef = TypedDict(
-    "EksContainerOverrideTypeDef",
-    {
-        "image": str,
-        "command": Sequence[str],
-        "args": Sequence[str],
-        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredEksContainerTypeDef = TypedDict(
     "_RequiredEksContainerTypeDef",
     {
         "image": str,
     },
 )
 _OptionalEksContainerTypeDef = TypedDict(
     "_OptionalEksContainerTypeDef",
     {
         "name": str,
         "imagePullPolicy": str,
-        "command": Sequence[str],
-        "args": Sequence[str],
-        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
+        "command": List[str],
+        "args": List[str],
+        "env": List[EksContainerEnvironmentVariableTypeDef],
         "resources": EksContainerResourceRequirementsTypeDef,
-        "volumeMounts": Sequence[EksContainerVolumeMountTypeDef],
+        "volumeMounts": List[EksContainerVolumeMountTypeDef],
         "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
 
 class EksContainerTypeDef(_RequiredEksContainerTypeDef, _OptionalEksContainerTypeDef):
@@ -1293,38 +1129,19 @@
 )
 
 
 class EksVolumeTypeDef(_RequiredEksVolumeTypeDef, _OptionalEksVolumeTypeDef):
     pass
 
 
-RetryStrategyOutputTypeDef = TypedDict(
-    "RetryStrategyOutputTypeDef",
-    {
-        "attempts": int,
-        "evaluateOnExit": List[EvaluateOnExitTypeDef],
-    },
-    total=False,
-)
-
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
         "attempts": int,
-        "evaluateOnExit": Sequence[EvaluateOnExitTypeDef],
-    },
-    total=False,
-)
-
-FairsharePolicyOutputTypeDef = TypedDict(
-    "FairsharePolicyOutputTypeDef",
-    {
-        "shareDecaySeconds": int,
-        "computeReservation": int,
-        "shareDistribution": List[ShareAttributesTypeDef],
+        "evaluateOnExit": List[EvaluateOnExitTypeDef],
     },
     total=False,
 )
 
 FairsharePolicyTypeDef = TypedDict(
     "FairsharePolicyTypeDef",
     {
@@ -1387,34 +1204,21 @@
         "maxResults": int,
         "nextToken": str,
         "filters": Sequence[KeyValuesPairTypeDef],
     },
     total=False,
 )
 
-LinuxParametersOutputTypeDef = TypedDict(
-    "LinuxParametersOutputTypeDef",
-    {
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
 
 ListSchedulingPoliciesResponseTypeDef = TypedDict(
@@ -1459,15 +1263,15 @@
         "unmanagedvCpus": int,
         "ecsClusterArn": str,
         "tags": Dict[str, str],
         "type": CETypeType,
         "state": CEStateType,
         "status": CEStatusType,
         "statusReason": str,
-        "computeResources": ComputeResourceOutputTypeDef,
+        "computeResources": ComputeResourceTypeDef,
         "serviceRole": str,
         "updatePolicy": UpdatePolicyTypeDef,
         "eksConfiguration": EksConfigurationTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
         "uuid": str,
     },
     total=False,
@@ -1476,15 +1280,14 @@
 
 class ComputeEnvironmentDetailTypeDef(
     _RequiredComputeEnvironmentDetailTypeDef, _OptionalComputeEnvironmentDetailTypeDef
 ):
     pass
 
 
-ComputeResourceUnionTypeDef = Union[ComputeResourceTypeDef, ComputeResourceOutputTypeDef]
 _RequiredCreateComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironmentName": str,
         "type": CETypeType,
     },
 )
@@ -1581,93 +1384,78 @@
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerDetailTypeDef],
         "volumes": List[EksVolumeTypeDef],
         "podName": str,
         "nodeName": str,
-        "metadata": EksMetadataOutputTypeDef,
-    },
-    total=False,
-)
-
-EksPodPropertiesOutputTypeDef = TypedDict(
-    "EksPodPropertiesOutputTypeDef",
-    {
-        "serviceAccountName": str,
-        "hostNetwork": bool,
-        "dnsPolicy": str,
-        "containers": List[EksContainerOutputTypeDef],
-        "volumes": List[EksVolumeTypeDef],
-        "metadata": EksMetadataOutputTypeDef,
+        "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesTypeDef = TypedDict(
     "EksPodPropertiesTypeDef",
     {
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
-        "containers": Sequence[EksContainerTypeDef],
-        "volumes": Sequence[EksVolumeTypeDef],
+        "containers": List[EksContainerTypeDef],
+        "volumes": List[EksVolumeTypeDef],
         "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
-RetryStrategyUnionTypeDef = Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef]
-_RequiredSchedulingPolicyDetailTypeDef = TypedDict(
-    "_RequiredSchedulingPolicyDetailTypeDef",
+_RequiredCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSchedulingPolicyRequestRequestTypeDef",
     {
         "name": str,
-        "arn": str,
     },
 )
-_OptionalSchedulingPolicyDetailTypeDef = TypedDict(
-    "_OptionalSchedulingPolicyDetailTypeDef",
+_OptionalCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSchedulingPolicyRequestRequestTypeDef",
     {
-        "fairsharePolicy": FairsharePolicyOutputTypeDef,
-        "tags": Dict[str, str],
+        "fairsharePolicy": FairsharePolicyTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class SchedulingPolicyDetailTypeDef(
-    _RequiredSchedulingPolicyDetailTypeDef, _OptionalSchedulingPolicyDetailTypeDef
+class CreateSchedulingPolicyRequestRequestTypeDef(
+    _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
+    _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSchedulingPolicyRequestRequestTypeDef",
+_RequiredSchedulingPolicyDetailTypeDef = TypedDict(
+    "_RequiredSchedulingPolicyDetailTypeDef",
     {
         "name": str,
+        "arn": str,
     },
 )
-_OptionalCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSchedulingPolicyRequestRequestTypeDef",
+_OptionalSchedulingPolicyDetailTypeDef = TypedDict(
+    "_OptionalSchedulingPolicyDetailTypeDef",
     {
         "fairsharePolicy": FairsharePolicyTypeDef,
-        "tags": Mapping[str, str],
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class CreateSchedulingPolicyRequestRequestTypeDef(
-    _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
-    _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
+class SchedulingPolicyDetailTypeDef(
+    _RequiredSchedulingPolicyDetailTypeDef, _OptionalSchedulingPolicyDetailTypeDef
 ):
     pass
 
 
-FairsharePolicyUnionTypeDef = Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef]
 _RequiredUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchedulingPolicyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
@@ -1733,26 +1521,26 @@
         "reason": str,
         "containerInstanceArn": str,
         "taskArn": str,
         "logStreamName": str,
         "instanceType": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "resourceRequirements": List[ResourceRequirementTypeDef],
-        "linuxParameters": LinuxParametersOutputTypeDef,
-        "logConfiguration": LogConfigurationOutputTypeDef,
+        "linuxParameters": LinuxParametersTypeDef,
+        "logConfiguration": LogConfigurationTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
-ContainerPropertiesOutputTypeDef = TypedDict(
-    "ContainerPropertiesOutputTypeDef",
+ContainerPropertiesTypeDef = TypedDict(
+    "ContainerPropertiesTypeDef",
     {
         "image": str,
         "vcpus": int,
         "memory": int,
         "command": List[str],
         "jobRoleArn": str,
         "executionRoleArn": str,
@@ -1761,45 +1549,17 @@
         "mountPoints": List[MountPointTypeDef],
         "readonlyRootFilesystem": bool,
         "privileged": bool,
         "ulimits": List[UlimitTypeDef],
         "user": str,
         "instanceType": str,
         "resourceRequirements": List[ResourceRequirementTypeDef],
-        "linuxParameters": LinuxParametersOutputTypeDef,
-        "logConfiguration": LogConfigurationOutputTypeDef,
-        "secrets": List[SecretTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
-        "ephemeralStorage": EphemeralStorageTypeDef,
-    },
-    total=False,
-)
-
-ContainerPropertiesTypeDef = TypedDict(
-    "ContainerPropertiesTypeDef",
-    {
-        "image": str,
-        "vcpus": int,
-        "memory": int,
-        "command": Sequence[str],
-        "jobRoleArn": str,
-        "executionRoleArn": str,
-        "volumes": Sequence[VolumeTypeDef],
-        "environment": Sequence[KeyValuePairTypeDef],
-        "mountPoints": Sequence[MountPointTypeDef],
-        "readonlyRootFilesystem": bool,
-        "privileged": bool,
-        "ulimits": Sequence[UlimitTypeDef],
-        "user": str,
-        "instanceType": str,
-        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
-        "secrets": Sequence[SecretTypeDef],
+        "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
@@ -1815,22 +1575,14 @@
     "EksPropertiesDetailTypeDef",
     {
         "podProperties": EksPodPropertiesDetailTypeDef,
     },
     total=False,
 )
 
-EksPropertiesOutputTypeDef = TypedDict(
-    "EksPropertiesOutputTypeDef",
-    {
-        "podProperties": EksPodPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 EksPropertiesTypeDef = TypedDict(
     "EksPropertiesTypeDef",
     {
         "podProperties": EksPodPropertiesTypeDef,
     },
     total=False,
 )
@@ -1839,38 +1591,14 @@
     "DescribeSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredNodeRangePropertyOutputTypeDef = TypedDict(
-    "_RequiredNodeRangePropertyOutputTypeDef",
-    {
-        "targetNodes": str,
-    },
-)
-_OptionalNodeRangePropertyOutputTypeDef = TypedDict(
-    "_OptionalNodeRangePropertyOutputTypeDef",
-    {
-        "container": ContainerPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class NodeRangePropertyOutputTypeDef(
-    _RequiredNodeRangePropertyOutputTypeDef, _OptionalNodeRangePropertyOutputTypeDef
-):
-    pass
-
-
-ContainerPropertiesUnionTypeDef = Union[
-    ContainerPropertiesTypeDef, ContainerPropertiesOutputTypeDef
-]
 _RequiredNodeRangePropertyTypeDef = TypedDict(
     "_RequiredNodeRangePropertyTypeDef",
     {
         "targetNodes": str,
     },
 )
 _OptionalNodeRangePropertyTypeDef = TypedDict(
@@ -1918,30 +1646,20 @@
 
 class SubmitJobRequestRequestTypeDef(
     _RequiredSubmitJobRequestRequestTypeDef, _OptionalSubmitJobRequestRequestTypeDef
 ):
     pass
 
 
-EksPropertiesUnionTypeDef = Union[EksPropertiesTypeDef, EksPropertiesOutputTypeDef]
-NodePropertiesOutputTypeDef = TypedDict(
-    "NodePropertiesOutputTypeDef",
-    {
-        "numNodes": int,
-        "mainNode": int,
-        "nodeRangeProperties": List[NodeRangePropertyOutputTypeDef],
-    },
-)
-
 NodePropertiesTypeDef = TypedDict(
     "NodePropertiesTypeDef",
     {
         "numNodes": int,
         "mainNode": int,
-        "nodeRangeProperties": Sequence[NodeRangePropertyTypeDef],
+        "nodeRangeProperties": List[NodeRangePropertyTypeDef],
     },
 )
 
 _RequiredJobDefinitionTypeDef = TypedDict(
     "_RequiredJobDefinitionTypeDef",
     {
         "jobDefinitionName": str,
@@ -1952,22 +1670,22 @@
 )
 _OptionalJobDefinitionTypeDef = TypedDict(
     "_OptionalJobDefinitionTypeDef",
     {
         "status": str,
         "schedulingPriority": int,
         "parameters": Dict[str, str],
-        "retryStrategy": RetryStrategyOutputTypeDef,
-        "containerProperties": ContainerPropertiesOutputTypeDef,
+        "retryStrategy": RetryStrategyTypeDef,
+        "containerProperties": ContainerPropertiesTypeDef,
         "timeout": JobTimeoutTypeDef,
-        "nodeProperties": NodePropertiesOutputTypeDef,
+        "nodeProperties": NodePropertiesTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
-        "eksProperties": EksPropertiesOutputTypeDef,
+        "eksProperties": EksPropertiesTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
     },
     total=False,
 )
 
 
 class JobDefinitionTypeDef(_RequiredJobDefinitionTypeDef, _OptionalJobDefinitionTypeDef):
@@ -1990,21 +1708,21 @@
     {
         "jobArn": str,
         "shareIdentifier": str,
         "schedulingPriority": int,
         "attempts": List[AttemptDetailTypeDef],
         "statusReason": str,
         "createdAt": int,
-        "retryStrategy": RetryStrategyOutputTypeDef,
+        "retryStrategy": RetryStrategyTypeDef,
         "stoppedAt": int,
         "dependsOn": List[JobDependencyTypeDef],
         "parameters": Dict[str, str],
         "container": ContainerDetailTypeDef,
         "nodeDetails": NodeDetailsTypeDef,
-        "nodeProperties": NodePropertiesOutputTypeDef,
+        "nodeProperties": NodePropertiesTypeDef,
         "arrayProperties": ArrayPropertiesDetailTypeDef,
         "timeout": JobTimeoutTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
         "eksProperties": EksPropertiesDetailTypeDef,
         "eksAttempts": List[EksAttemptDetailTypeDef],
@@ -2015,15 +1733,14 @@
 )
 
 
 class JobDetailTypeDef(_RequiredJobDetailTypeDef, _OptionalJobDetailTypeDef):
     pass
 
 
-NodePropertiesUnionTypeDef = Union[NodePropertiesTypeDef, NodePropertiesOutputTypeDef]
 _RequiredRegisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinitionName": str,
         "type": JobDefinitionTypeType,
     },
 )
```

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch/type_defs.pyi` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_batch.type_defs import ArrayPropertiesDetailTypeDef
 
     data: ArrayPropertiesDetailTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ArrayJobDependencyType,
     AssignPublicIpType,
     CEStateType,
     CEStatusType,
     CETypeType,
@@ -69,53 +69,47 @@
     "DeregisterJobDefinitionRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeComputeEnvironmentsRequestRequestTypeDef",
     "DescribeJobDefinitionsRequestRequestTypeDef",
     "DescribeJobQueuesRequestRequestTypeDef",
     "DescribeJobsRequestRequestTypeDef",
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
-    "DeviceOutputTypeDef",
     "DeviceTypeDef",
     "EFSAuthorizationConfigTypeDef",
     "EksAttemptContainerDetailTypeDef",
     "EksContainerEnvironmentVariableTypeDef",
-    "EksContainerResourceRequirementsOutputTypeDef",
+    "EksContainerResourceRequirementsTypeDef",
     "EksContainerSecurityContextTypeDef",
     "EksContainerVolumeMountTypeDef",
-    "EksContainerResourceRequirementsTypeDef",
     "EksEmptyDirTypeDef",
     "EksHostPathTypeDef",
-    "EksMetadataOutputTypeDef",
     "EksMetadataTypeDef",
     "EksSecretTypeDef",
     "EvaluateOnExitTypeDef",
     "ShareAttributesTypeDef",
     "HostTypeDef",
     "JobTimeoutTypeDef",
     "JobDependencyTypeDef",
     "NodeDetailsTypeDef",
     "NodePropertiesSummaryTypeDef",
     "KeyValuesPairTypeDef",
-    "TmpfsOutputTypeDef",
     "TmpfsTypeDef",
     "ListSchedulingPoliciesRequestRequestTypeDef",
     "SchedulingPolicyListingDetailTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TerminateJobRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AttemptContainerDetailTypeDef",
     "CreateJobQueueRequestRequestTypeDef",
     "JobQueueDetailTypeDef",
     "UpdateJobQueueRequestRequestTypeDef",
-    "ComputeResourceOutputTypeDef",
     "ComputeResourceTypeDef",
     "ComputeResourceUpdateTypeDef",
     "ContainerOverridesTypeDef",
-    "LogConfigurationOutputTypeDef",
     "LogConfigurationTypeDef",
     "CreateComputeEnvironmentResponseTypeDef",
     "CreateJobQueueResponseTypeDef",
     "CreateSchedulingPolicyResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RegisterJobDefinitionResponseTypeDef",
     "SubmitJobResponseTypeDef",
@@ -123,67 +117,52 @@
     "UpdateJobQueueResponseTypeDef",
     "DescribeComputeEnvironmentsRequestDescribeComputeEnvironmentsPaginateTypeDef",
     "DescribeJobDefinitionsRequestDescribeJobDefinitionsPaginateTypeDef",
     "DescribeJobQueuesRequestDescribeJobQueuesPaginateTypeDef",
     "ListSchedulingPoliciesRequestListSchedulingPoliciesPaginateTypeDef",
     "EFSVolumeConfigurationTypeDef",
     "EksAttemptDetailTypeDef",
-    "EksContainerDetailTypeDef",
-    "EksContainerOutputTypeDef",
     "EksContainerOverrideTypeDef",
+    "EksContainerDetailTypeDef",
     "EksContainerTypeDef",
     "EksVolumeTypeDef",
-    "RetryStrategyOutputTypeDef",
     "RetryStrategyTypeDef",
-    "FairsharePolicyOutputTypeDef",
     "FairsharePolicyTypeDef",
     "JobSummaryTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "LinuxParametersOutputTypeDef",
     "LinuxParametersTypeDef",
     "ListSchedulingPoliciesResponseTypeDef",
     "AttemptDetailTypeDef",
     "DescribeJobQueuesResponseTypeDef",
     "ComputeEnvironmentDetailTypeDef",
-    "ComputeResourceUnionTypeDef",
     "CreateComputeEnvironmentRequestRequestTypeDef",
     "UpdateComputeEnvironmentRequestRequestTypeDef",
     "NodePropertyOverrideTypeDef",
     "VolumeTypeDef",
     "EksPodPropertiesOverrideTypeDef",
     "EksPodPropertiesDetailTypeDef",
-    "EksPodPropertiesOutputTypeDef",
     "EksPodPropertiesTypeDef",
-    "RetryStrategyUnionTypeDef",
-    "SchedulingPolicyDetailTypeDef",
     "CreateSchedulingPolicyRequestRequestTypeDef",
-    "FairsharePolicyUnionTypeDef",
+    "SchedulingPolicyDetailTypeDef",
     "UpdateSchedulingPolicyRequestRequestTypeDef",
     "ListJobsResponseTypeDef",
     "DescribeComputeEnvironmentsResponseTypeDef",
     "NodeOverridesTypeDef",
     "ContainerDetailTypeDef",
-    "ContainerPropertiesOutputTypeDef",
     "ContainerPropertiesTypeDef",
     "EksPropertiesOverrideTypeDef",
     "EksPropertiesDetailTypeDef",
-    "EksPropertiesOutputTypeDef",
     "EksPropertiesTypeDef",
     "DescribeSchedulingPoliciesResponseTypeDef",
-    "NodeRangePropertyOutputTypeDef",
-    "ContainerPropertiesUnionTypeDef",
     "NodeRangePropertyTypeDef",
     "SubmitJobRequestRequestTypeDef",
-    "EksPropertiesUnionTypeDef",
-    "NodePropertiesOutputTypeDef",
     "NodePropertiesTypeDef",
     "JobDefinitionTypeDef",
     "JobDetailTypeDef",
-    "NodePropertiesUnionTypeDef",
     "RegisterJobDefinitionRequestRequestTypeDef",
     "DescribeJobDefinitionsResponseTypeDef",
     "DescribeJobsResponseTypeDef",
 )
 
 ArrayPropertiesDetailTypeDef = TypedDict(
     "ArrayPropertiesDetailTypeDef",
@@ -450,43 +429,25 @@
 DescribeSchedulingPoliciesRequestRequestTypeDef = TypedDict(
     "DescribeSchedulingPoliciesRequestRequestTypeDef",
     {
         "arns": Sequence[str],
     },
 )
 
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
 
@@ -523,16 +484,16 @@
 )
 
 class EksContainerEnvironmentVariableTypeDef(
     _RequiredEksContainerEnvironmentVariableTypeDef, _OptionalEksContainerEnvironmentVariableTypeDef
 ):
     pass
 
-EksContainerResourceRequirementsOutputTypeDef = TypedDict(
-    "EksContainerResourceRequirementsOutputTypeDef",
+EksContainerResourceRequirementsTypeDef = TypedDict(
+    "EksContainerResourceRequirementsTypeDef",
     {
         "limits": Dict[str, str],
         "requests": Dict[str, str],
     },
     total=False,
 )
 
@@ -554,23 +515,14 @@
         "name": str,
         "mountPath": str,
         "readOnly": bool,
     },
     total=False,
 )
 
-EksContainerResourceRequirementsTypeDef = TypedDict(
-    "EksContainerResourceRequirementsTypeDef",
-    {
-        "limits": Mapping[str, str],
-        "requests": Mapping[str, str],
-    },
-    total=False,
-)
-
 EksEmptyDirTypeDef = TypedDict(
     "EksEmptyDirTypeDef",
     {
         "medium": str,
         "sizeLimit": str,
     },
     total=False,
@@ -580,26 +532,18 @@
     "EksHostPathTypeDef",
     {
         "path": str,
     },
     total=False,
 )
 
-EksMetadataOutputTypeDef = TypedDict(
-    "EksMetadataOutputTypeDef",
-    {
-        "labels": Dict[str, str],
-    },
-    total=False,
-)
-
 EksMetadataTypeDef = TypedDict(
     "EksMetadataTypeDef",
     {
-        "labels": Mapping[str, str],
+        "labels": Dict[str, str],
     },
     total=False,
 )
 
 _RequiredEksSecretTypeDef = TypedDict(
     "_RequiredEksSecretTypeDef",
     {
@@ -702,43 +646,25 @@
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
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
-    },
-    total=False,
-)
-
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
 
@@ -867,48 +793,14 @@
 )
 
 class UpdateJobQueueRequestRequestTypeDef(
     _RequiredUpdateJobQueueRequestRequestTypeDef, _OptionalUpdateJobQueueRequestRequestTypeDef
 ):
     pass
 
-_RequiredComputeResourceOutputTypeDef = TypedDict(
-    "_RequiredComputeResourceOutputTypeDef",
-    {
-        "type": CRTypeType,
-        "maxvCpus": int,
-        "subnets": List[str],
-    },
-)
-_OptionalComputeResourceOutputTypeDef = TypedDict(
-    "_OptionalComputeResourceOutputTypeDef",
-    {
-        "allocationStrategy": CRAllocationStrategyType,
-        "minvCpus": int,
-        "desiredvCpus": int,
-        "instanceTypes": List[str],
-        "imageId": str,
-        "securityGroupIds": List[str],
-        "ec2KeyPair": str,
-        "instanceRole": str,
-        "tags": Dict[str, str],
-        "placementGroup": str,
-        "bidPercentage": int,
-        "spotIamFleetRole": str,
-        "launchTemplate": LaunchTemplateSpecificationTypeDef,
-        "ec2Configuration": List[Ec2ConfigurationTypeDef],
-    },
-    total=False,
-)
-
-class ComputeResourceOutputTypeDef(
-    _RequiredComputeResourceOutputTypeDef, _OptionalComputeResourceOutputTypeDef
-):
-    pass
-
 _RequiredComputeResourceTypeDef = TypedDict(
     "_RequiredComputeResourceTypeDef",
     {
         "type": CRTypeType,
         "maxvCpus": int,
         "subnets": Sequence[str],
     },
@@ -970,45 +862,25 @@
         "instanceType": str,
         "environment": Sequence[KeyValuePairTypeDef],
         "resourceRequirements": Sequence[ResourceRequirementTypeDef],
     },
     total=False,
 )
 
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
     "_OptionalLogConfigurationTypeDef",
     {
-        "options": Mapping[str, str],
-        "secretOptions": Sequence[SecretTypeDef],
+        "options": Dict[str, str],
+        "secretOptions": List[SecretTypeDef],
     },
     total=False,
 )
 
 class LogConfigurationTypeDef(_RequiredLogConfigurationTypeDef, _OptionalLogConfigurationTypeDef):
     pass
 
@@ -1153,86 +1025,60 @@
         "startedAt": int,
         "stoppedAt": int,
         "statusReason": str,
     },
     total=False,
 )
 
-EksContainerDetailTypeDef = TypedDict(
-    "EksContainerDetailTypeDef",
+EksContainerOverrideTypeDef = TypedDict(
+    "EksContainerOverrideTypeDef",
     {
-        "name": str,
         "image": str,
-        "imagePullPolicy": str,
-        "command": List[str],
-        "args": List[str],
-        "env": List[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsOutputTypeDef,
-        "exitCode": int,
-        "reason": str,
-        "volumeMounts": List[EksContainerVolumeMountTypeDef],
-        "securityContext": EksContainerSecurityContextTypeDef,
+        "command": Sequence[str],
+        "args": Sequence[str],
+        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
+        "resources": EksContainerResourceRequirementsTypeDef,
     },
     total=False,
 )
 
-_RequiredEksContainerOutputTypeDef = TypedDict(
-    "_RequiredEksContainerOutputTypeDef",
-    {
-        "image": str,
-    },
-)
-_OptionalEksContainerOutputTypeDef = TypedDict(
-    "_OptionalEksContainerOutputTypeDef",
+EksContainerDetailTypeDef = TypedDict(
+    "EksContainerDetailTypeDef",
     {
         "name": str,
+        "image": str,
         "imagePullPolicy": str,
         "command": List[str],
         "args": List[str],
         "env": List[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsOutputTypeDef,
+        "resources": EksContainerResourceRequirementsTypeDef,
+        "exitCode": int,
+        "reason": str,
         "volumeMounts": List[EksContainerVolumeMountTypeDef],
         "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
-class EksContainerOutputTypeDef(
-    _RequiredEksContainerOutputTypeDef, _OptionalEksContainerOutputTypeDef
-):
-    pass
-
-EksContainerOverrideTypeDef = TypedDict(
-    "EksContainerOverrideTypeDef",
-    {
-        "image": str,
-        "command": Sequence[str],
-        "args": Sequence[str],
-        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
-        "resources": EksContainerResourceRequirementsTypeDef,
-    },
-    total=False,
-)
-
 _RequiredEksContainerTypeDef = TypedDict(
     "_RequiredEksContainerTypeDef",
     {
         "image": str,
     },
 )
 _OptionalEksContainerTypeDef = TypedDict(
     "_OptionalEksContainerTypeDef",
     {
         "name": str,
         "imagePullPolicy": str,
-        "command": Sequence[str],
-        "args": Sequence[str],
-        "env": Sequence[EksContainerEnvironmentVariableTypeDef],
+        "command": List[str],
+        "args": List[str],
+        "env": List[EksContainerEnvironmentVariableTypeDef],
         "resources": EksContainerResourceRequirementsTypeDef,
-        "volumeMounts": Sequence[EksContainerVolumeMountTypeDef],
+        "volumeMounts": List[EksContainerVolumeMountTypeDef],
         "securityContext": EksContainerSecurityContextTypeDef,
     },
     total=False,
 )
 
 class EksContainerTypeDef(_RequiredEksContainerTypeDef, _OptionalEksContainerTypeDef):
     pass
@@ -1252,38 +1098,19 @@
     },
     total=False,
 )
 
 class EksVolumeTypeDef(_RequiredEksVolumeTypeDef, _OptionalEksVolumeTypeDef):
     pass
 
-RetryStrategyOutputTypeDef = TypedDict(
-    "RetryStrategyOutputTypeDef",
-    {
-        "attempts": int,
-        "evaluateOnExit": List[EvaluateOnExitTypeDef],
-    },
-    total=False,
-)
-
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
         "attempts": int,
-        "evaluateOnExit": Sequence[EvaluateOnExitTypeDef],
-    },
-    total=False,
-)
-
-FairsharePolicyOutputTypeDef = TypedDict(
-    "FairsharePolicyOutputTypeDef",
-    {
-        "shareDecaySeconds": int,
-        "computeReservation": int,
-        "shareDistribution": List[ShareAttributesTypeDef],
+        "evaluateOnExit": List[EvaluateOnExitTypeDef],
     },
     total=False,
 )
 
 FairsharePolicyTypeDef = TypedDict(
     "FairsharePolicyTypeDef",
     {
@@ -1344,34 +1171,21 @@
         "maxResults": int,
         "nextToken": str,
         "filters": Sequence[KeyValuesPairTypeDef],
     },
     total=False,
 )
 
-LinuxParametersOutputTypeDef = TypedDict(
-    "LinuxParametersOutputTypeDef",
-    {
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
 
 ListSchedulingPoliciesResponseTypeDef = TypedDict(
@@ -1416,30 +1230,29 @@
         "unmanagedvCpus": int,
         "ecsClusterArn": str,
         "tags": Dict[str, str],
         "type": CETypeType,
         "state": CEStateType,
         "status": CEStatusType,
         "statusReason": str,
-        "computeResources": ComputeResourceOutputTypeDef,
+        "computeResources": ComputeResourceTypeDef,
         "serviceRole": str,
         "updatePolicy": UpdatePolicyTypeDef,
         "eksConfiguration": EksConfigurationTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
         "uuid": str,
     },
     total=False,
 )
 
 class ComputeEnvironmentDetailTypeDef(
     _RequiredComputeEnvironmentDetailTypeDef, _OptionalComputeEnvironmentDetailTypeDef
 ):
     pass
 
-ComputeResourceUnionTypeDef = Union[ComputeResourceTypeDef, ComputeResourceOutputTypeDef]
 _RequiredCreateComputeEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComputeEnvironmentRequestRequestTypeDef",
     {
         "computeEnvironmentName": str,
         "type": CETypeType,
     },
 )
@@ -1530,89 +1343,74 @@
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
         "containers": List[EksContainerDetailTypeDef],
         "volumes": List[EksVolumeTypeDef],
         "podName": str,
         "nodeName": str,
-        "metadata": EksMetadataOutputTypeDef,
-    },
-    total=False,
-)
-
-EksPodPropertiesOutputTypeDef = TypedDict(
-    "EksPodPropertiesOutputTypeDef",
-    {
-        "serviceAccountName": str,
-        "hostNetwork": bool,
-        "dnsPolicy": str,
-        "containers": List[EksContainerOutputTypeDef],
-        "volumes": List[EksVolumeTypeDef],
-        "metadata": EksMetadataOutputTypeDef,
+        "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
 EksPodPropertiesTypeDef = TypedDict(
     "EksPodPropertiesTypeDef",
     {
         "serviceAccountName": str,
         "hostNetwork": bool,
         "dnsPolicy": str,
-        "containers": Sequence[EksContainerTypeDef],
-        "volumes": Sequence[EksVolumeTypeDef],
+        "containers": List[EksContainerTypeDef],
+        "volumes": List[EksVolumeTypeDef],
         "metadata": EksMetadataTypeDef,
     },
     total=False,
 )
 
-RetryStrategyUnionTypeDef = Union[RetryStrategyTypeDef, RetryStrategyOutputTypeDef]
-_RequiredSchedulingPolicyDetailTypeDef = TypedDict(
-    "_RequiredSchedulingPolicyDetailTypeDef",
+_RequiredCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSchedulingPolicyRequestRequestTypeDef",
     {
         "name": str,
-        "arn": str,
     },
 )
-_OptionalSchedulingPolicyDetailTypeDef = TypedDict(
-    "_OptionalSchedulingPolicyDetailTypeDef",
+_OptionalCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSchedulingPolicyRequestRequestTypeDef",
     {
-        "fairsharePolicy": FairsharePolicyOutputTypeDef,
-        "tags": Dict[str, str],
+        "fairsharePolicy": FairsharePolicyTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class SchedulingPolicyDetailTypeDef(
-    _RequiredSchedulingPolicyDetailTypeDef, _OptionalSchedulingPolicyDetailTypeDef
+class CreateSchedulingPolicyRequestRequestTypeDef(
+    _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
+    _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSchedulingPolicyRequestRequestTypeDef",
+_RequiredSchedulingPolicyDetailTypeDef = TypedDict(
+    "_RequiredSchedulingPolicyDetailTypeDef",
     {
         "name": str,
+        "arn": str,
     },
 )
-_OptionalCreateSchedulingPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSchedulingPolicyRequestRequestTypeDef",
+_OptionalSchedulingPolicyDetailTypeDef = TypedDict(
+    "_OptionalSchedulingPolicyDetailTypeDef",
     {
         "fairsharePolicy": FairsharePolicyTypeDef,
-        "tags": Mapping[str, str],
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateSchedulingPolicyRequestRequestTypeDef(
-    _RequiredCreateSchedulingPolicyRequestRequestTypeDef,
-    _OptionalCreateSchedulingPolicyRequestRequestTypeDef,
+class SchedulingPolicyDetailTypeDef(
+    _RequiredSchedulingPolicyDetailTypeDef, _OptionalSchedulingPolicyDetailTypeDef
 ):
     pass
 
-FairsharePolicyUnionTypeDef = Union[FairsharePolicyTypeDef, FairsharePolicyOutputTypeDef]
 _RequiredUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchedulingPolicyRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 _OptionalUpdateSchedulingPolicyRequestRequestTypeDef = TypedDict(
@@ -1676,26 +1474,26 @@
         "reason": str,
         "containerInstanceArn": str,
         "taskArn": str,
         "logStreamName": str,
         "instanceType": str,
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "resourceRequirements": List[ResourceRequirementTypeDef],
-        "linuxParameters": LinuxParametersOutputTypeDef,
-        "logConfiguration": LogConfigurationOutputTypeDef,
+        "linuxParameters": LinuxParametersTypeDef,
+        "logConfiguration": LogConfigurationTypeDef,
         "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
-ContainerPropertiesOutputTypeDef = TypedDict(
-    "ContainerPropertiesOutputTypeDef",
+ContainerPropertiesTypeDef = TypedDict(
+    "ContainerPropertiesTypeDef",
     {
         "image": str,
         "vcpus": int,
         "memory": int,
         "command": List[str],
         "jobRoleArn": str,
         "executionRoleArn": str,
@@ -1704,45 +1502,17 @@
         "mountPoints": List[MountPointTypeDef],
         "readonlyRootFilesystem": bool,
         "privileged": bool,
         "ulimits": List[UlimitTypeDef],
         "user": str,
         "instanceType": str,
         "resourceRequirements": List[ResourceRequirementTypeDef],
-        "linuxParameters": LinuxParametersOutputTypeDef,
-        "logConfiguration": LogConfigurationOutputTypeDef,
-        "secrets": List[SecretTypeDef],
-        "networkConfiguration": NetworkConfigurationTypeDef,
-        "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
-        "ephemeralStorage": EphemeralStorageTypeDef,
-    },
-    total=False,
-)
-
-ContainerPropertiesTypeDef = TypedDict(
-    "ContainerPropertiesTypeDef",
-    {
-        "image": str,
-        "vcpus": int,
-        "memory": int,
-        "command": Sequence[str],
-        "jobRoleArn": str,
-        "executionRoleArn": str,
-        "volumes": Sequence[VolumeTypeDef],
-        "environment": Sequence[KeyValuePairTypeDef],
-        "mountPoints": Sequence[MountPointTypeDef],
-        "readonlyRootFilesystem": bool,
-        "privileged": bool,
-        "ulimits": Sequence[UlimitTypeDef],
-        "user": str,
-        "instanceType": str,
-        "resourceRequirements": Sequence[ResourceRequirementTypeDef],
         "linuxParameters": LinuxParametersTypeDef,
         "logConfiguration": LogConfigurationTypeDef,
-        "secrets": Sequence[SecretTypeDef],
+        "secrets": List[SecretTypeDef],
         "networkConfiguration": NetworkConfigurationTypeDef,
         "fargatePlatformConfiguration": FargatePlatformConfigurationTypeDef,
         "ephemeralStorage": EphemeralStorageTypeDef,
     },
     total=False,
 )
 
@@ -1758,22 +1528,14 @@
     "EksPropertiesDetailTypeDef",
     {
         "podProperties": EksPodPropertiesDetailTypeDef,
     },
     total=False,
 )
 
-EksPropertiesOutputTypeDef = TypedDict(
-    "EksPropertiesOutputTypeDef",
-    {
-        "podProperties": EksPodPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 EksPropertiesTypeDef = TypedDict(
     "EksPropertiesTypeDef",
     {
         "podProperties": EksPodPropertiesTypeDef,
     },
     total=False,
 )
@@ -1782,36 +1544,14 @@
     "DescribeSchedulingPoliciesResponseTypeDef",
     {
         "schedulingPolicies": List[SchedulingPolicyDetailTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredNodeRangePropertyOutputTypeDef = TypedDict(
-    "_RequiredNodeRangePropertyOutputTypeDef",
-    {
-        "targetNodes": str,
-    },
-)
-_OptionalNodeRangePropertyOutputTypeDef = TypedDict(
-    "_OptionalNodeRangePropertyOutputTypeDef",
-    {
-        "container": ContainerPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
-class NodeRangePropertyOutputTypeDef(
-    _RequiredNodeRangePropertyOutputTypeDef, _OptionalNodeRangePropertyOutputTypeDef
-):
-    pass
-
-ContainerPropertiesUnionTypeDef = Union[
-    ContainerPropertiesTypeDef, ContainerPropertiesOutputTypeDef
-]
 _RequiredNodeRangePropertyTypeDef = TypedDict(
     "_RequiredNodeRangePropertyTypeDef",
     {
         "targetNodes": str,
     },
 )
 _OptionalNodeRangePropertyTypeDef = TypedDict(
@@ -1855,30 +1595,20 @@
 )
 
 class SubmitJobRequestRequestTypeDef(
     _RequiredSubmitJobRequestRequestTypeDef, _OptionalSubmitJobRequestRequestTypeDef
 ):
     pass
 
-EksPropertiesUnionTypeDef = Union[EksPropertiesTypeDef, EksPropertiesOutputTypeDef]
-NodePropertiesOutputTypeDef = TypedDict(
-    "NodePropertiesOutputTypeDef",
-    {
-        "numNodes": int,
-        "mainNode": int,
-        "nodeRangeProperties": List[NodeRangePropertyOutputTypeDef],
-    },
-)
-
 NodePropertiesTypeDef = TypedDict(
     "NodePropertiesTypeDef",
     {
         "numNodes": int,
         "mainNode": int,
-        "nodeRangeProperties": Sequence[NodeRangePropertyTypeDef],
+        "nodeRangeProperties": List[NodeRangePropertyTypeDef],
     },
 )
 
 _RequiredJobDefinitionTypeDef = TypedDict(
     "_RequiredJobDefinitionTypeDef",
     {
         "jobDefinitionName": str,
@@ -1889,22 +1619,22 @@
 )
 _OptionalJobDefinitionTypeDef = TypedDict(
     "_OptionalJobDefinitionTypeDef",
     {
         "status": str,
         "schedulingPriority": int,
         "parameters": Dict[str, str],
-        "retryStrategy": RetryStrategyOutputTypeDef,
-        "containerProperties": ContainerPropertiesOutputTypeDef,
+        "retryStrategy": RetryStrategyTypeDef,
+        "containerProperties": ContainerPropertiesTypeDef,
         "timeout": JobTimeoutTypeDef,
-        "nodeProperties": NodePropertiesOutputTypeDef,
+        "nodeProperties": NodePropertiesTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
-        "eksProperties": EksPropertiesOutputTypeDef,
+        "eksProperties": EksPropertiesTypeDef,
         "containerOrchestrationType": OrchestrationTypeType,
     },
     total=False,
 )
 
 class JobDefinitionTypeDef(_RequiredJobDefinitionTypeDef, _OptionalJobDefinitionTypeDef):
     pass
@@ -1925,21 +1655,21 @@
     {
         "jobArn": str,
         "shareIdentifier": str,
         "schedulingPriority": int,
         "attempts": List[AttemptDetailTypeDef],
         "statusReason": str,
         "createdAt": int,
-        "retryStrategy": RetryStrategyOutputTypeDef,
+        "retryStrategy": RetryStrategyTypeDef,
         "stoppedAt": int,
         "dependsOn": List[JobDependencyTypeDef],
         "parameters": Dict[str, str],
         "container": ContainerDetailTypeDef,
         "nodeDetails": NodeDetailsTypeDef,
-        "nodeProperties": NodePropertiesOutputTypeDef,
+        "nodeProperties": NodePropertiesTypeDef,
         "arrayProperties": ArrayPropertiesDetailTypeDef,
         "timeout": JobTimeoutTypeDef,
         "tags": Dict[str, str],
         "propagateTags": bool,
         "platformCapabilities": List[PlatformCapabilityType],
         "eksProperties": EksPropertiesDetailTypeDef,
         "eksAttempts": List[EksAttemptDetailTypeDef],
@@ -1948,15 +1678,14 @@
     },
     total=False,
 )
 
 class JobDetailTypeDef(_RequiredJobDetailTypeDef, _OptionalJobDetailTypeDef):
     pass
 
-NodePropertiesUnionTypeDef = Union[NodePropertiesTypeDef, NodePropertiesOutputTypeDef]
 _RequiredRegisterJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterJobDefinitionRequestRequestTypeDef",
     {
         "jobDefinitionName": str,
         "type": JobDefinitionTypeType,
     },
 )
```

### Comparing `types-aiobotocore-batch-2.5.2.post1/types_aiobotocore_batch.egg-info/SOURCES.txt` & `types-aiobotocore-batch-2.5.2.post2/types_aiobotocore_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

