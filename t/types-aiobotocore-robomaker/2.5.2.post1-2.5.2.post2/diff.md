# Comparing `tmp/types-aiobotocore-robomaker-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-robomaker-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-robomaker-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-robomaker-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-robomaker-2.5.2.post1.tar` & `types-aiobotocore-robomaker-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:53.529479 types-aiobotocore-robomaker-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-08-02 14:52:53.521479 types-aiobotocore-robomaker-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:53.529479 types-aiobotocore-robomaker-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:53.521479 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44916 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44839 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13846 2023-08-02 14:47:58.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69711 2023-08-02 14:47:59.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69645 2023-08-02 14:47:58.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:57.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:53.521479 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:53.000000 types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.816643 types-aiobotocore-robomaker-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14624 2023-08-04 13:59:23.806643 types-aiobotocore-robomaker-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13098 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.816643 types-aiobotocore-robomaker-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.806643 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2867 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2866 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    44856 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    44779 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13941 2023-08-04 13:50:55.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13939 2023-08-04 13:50:55.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14005 2023-08-04 13:50:55.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13992 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    63517 2023-08-04 13:50:56.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    63462 2023-08-04 13:50:56.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:54.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.806643 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14624 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:23.000000 types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/LICENSE` & `types-aiobotocore-robomaker-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/setup.py` & `types-aiobotocore-robomaker-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-robomaker",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_robomaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.RoboMaker 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__init__.py` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__init__.pyi` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/__main__.py` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RoboMaker 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.RoboMaker 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker\nOther"
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

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/client.py` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     CreateRobotResponseTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     CreateSimulationJobResponseTypeDef,
     CreateWorldExportJobResponseTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     CreateWorldTemplateResponseTypeDef,
-    DataSourceConfigUnionTypeDef,
-    DeploymentApplicationConfigUnionTypeDef,
+    DataSourceConfigTypeDef,
+    DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     DescribeFleetResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
@@ -80,27 +80,27 @@
     ListWorldGenerationJobsResponseTypeDef,
     ListWorldsResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     RegisterRobotResponseTypeDef,
     RenderingEngineTypeDef,
-    RobotApplicationConfigUnionTypeDef,
+    RobotApplicationConfigTypeDef,
     RobotSoftwareSuiteTypeDef,
-    SimulationApplicationConfigUnionTypeDef,
-    SimulationJobRequestUnionTypeDef,
+    SimulationApplicationConfigTypeDef,
+    SimulationJobRequestTypeDef,
     SimulationSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     StartSimulationJobBatchResponseTypeDef,
     SyncDeploymentJobResponseTypeDef,
     TemplateLocationTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
-    VPCConfigUnionTypeDef,
+    VPCConfigTypeDef,
     WorldCountTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -224,15 +224,15 @@
         """
 
     async def create_deployment_job(
         self,
         *,
         clientRequestToken: str,
         fleet: str,
-        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigUnionTypeDef],
+        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigTypeDef],
         deploymentConfig: DeploymentConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeploymentJobResponseTypeDef:
         """
         Deploys a specific version of a robot application to robots in a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)
@@ -333,19 +333,19 @@
         *,
         maxJobDurationInSeconds: int,
         iamRole: str,
         clientRequestToken: str = ...,
         outputLocation: OutputLocationTypeDef = ...,
         loggingConfig: LoggingConfigTypeDef = ...,
         failureBehavior: FailureBehaviorType = ...,
-        robotApplications: Sequence[RobotApplicationConfigUnionTypeDef] = ...,
-        simulationApplications: Sequence[SimulationApplicationConfigUnionTypeDef] = ...,
-        dataSources: Sequence[DataSourceConfigUnionTypeDef] = ...,
+        robotApplications: Sequence[RobotApplicationConfigTypeDef] = ...,
+        simulationApplications: Sequence[SimulationApplicationConfigTypeDef] = ...,
+        dataSources: Sequence[DataSourceConfigTypeDef] = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfig: VPCConfigUnionTypeDef = ...,
+        vpcConfig: VPCConfigTypeDef = ...,
         compute: ComputeTypeDef = ...
     ) -> CreateSimulationJobResponseTypeDef:
         """
         Creates a simulation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_simulation_job)
@@ -718,15 +718,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.restart_simulation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#restart_simulation_job)
         """
 
     async def start_simulation_job_batch(
         self,
         *,
-        createSimulationJobRequests: Sequence[SimulationJobRequestUnionTypeDef],
+        createSimulationJobRequests: Sequence[SimulationJobRequestTypeDef],
         clientRequestToken: str = ...,
         batchPolicy: BatchPolicyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSimulationJobBatchResponseTypeDef:
         """
         Starts a new simulation job batch.
```

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/client.pyi` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -46,16 +46,16 @@
     CreateRobotResponseTypeDef,
     CreateSimulationApplicationResponseTypeDef,
     CreateSimulationApplicationVersionResponseTypeDef,
     CreateSimulationJobResponseTypeDef,
     CreateWorldExportJobResponseTypeDef,
     CreateWorldGenerationJobResponseTypeDef,
     CreateWorldTemplateResponseTypeDef,
-    DataSourceConfigUnionTypeDef,
-    DeploymentApplicationConfigUnionTypeDef,
+    DataSourceConfigTypeDef,
+    DeploymentApplicationConfigTypeDef,
     DeploymentConfigTypeDef,
     DeregisterRobotResponseTypeDef,
     DescribeDeploymentJobResponseTypeDef,
     DescribeFleetResponseTypeDef,
     DescribeRobotApplicationResponseTypeDef,
     DescribeRobotResponseTypeDef,
     DescribeSimulationApplicationResponseTypeDef,
@@ -80,27 +80,27 @@
     ListWorldGenerationJobsResponseTypeDef,
     ListWorldsResponseTypeDef,
     ListWorldTemplatesResponseTypeDef,
     LoggingConfigTypeDef,
     OutputLocationTypeDef,
     RegisterRobotResponseTypeDef,
     RenderingEngineTypeDef,
-    RobotApplicationConfigUnionTypeDef,
+    RobotApplicationConfigTypeDef,
     RobotSoftwareSuiteTypeDef,
-    SimulationApplicationConfigUnionTypeDef,
-    SimulationJobRequestUnionTypeDef,
+    SimulationApplicationConfigTypeDef,
+    SimulationJobRequestTypeDef,
     SimulationSoftwareSuiteTypeDef,
     SourceConfigTypeDef,
     StartSimulationJobBatchResponseTypeDef,
     SyncDeploymentJobResponseTypeDef,
     TemplateLocationTypeDef,
     UpdateRobotApplicationResponseTypeDef,
     UpdateSimulationApplicationResponseTypeDef,
     UpdateWorldTemplateResponseTypeDef,
-    VPCConfigUnionTypeDef,
+    VPCConfigTypeDef,
     WorldCountTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -210,15 +210,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#close)
         """
     async def create_deployment_job(
         self,
         *,
         clientRequestToken: str,
         fleet: str,
-        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigUnionTypeDef],
+        deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigTypeDef],
         deploymentConfig: DeploymentConfigTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDeploymentJobResponseTypeDef:
         """
         Deploys a specific version of a robot application to robots in a fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_deployment_job)
@@ -312,19 +312,19 @@
         *,
         maxJobDurationInSeconds: int,
         iamRole: str,
         clientRequestToken: str = ...,
         outputLocation: OutputLocationTypeDef = ...,
         loggingConfig: LoggingConfigTypeDef = ...,
         failureBehavior: FailureBehaviorType = ...,
-        robotApplications: Sequence[RobotApplicationConfigUnionTypeDef] = ...,
-        simulationApplications: Sequence[SimulationApplicationConfigUnionTypeDef] = ...,
-        dataSources: Sequence[DataSourceConfigUnionTypeDef] = ...,
+        robotApplications: Sequence[RobotApplicationConfigTypeDef] = ...,
+        simulationApplications: Sequence[SimulationApplicationConfigTypeDef] = ...,
+        dataSources: Sequence[DataSourceConfigTypeDef] = ...,
         tags: Mapping[str, str] = ...,
-        vpcConfig: VPCConfigUnionTypeDef = ...,
+        vpcConfig: VPCConfigTypeDef = ...,
         compute: ComputeTypeDef = ...
     ) -> CreateSimulationJobResponseTypeDef:
         """
         Creates a simulation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.create_simulation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#create_simulation_job)
@@ -660,15 +660,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client.restart_simulation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_robomaker/client/#restart_simulation_job)
         """
     async def start_simulation_job_batch(
         self,
         *,
-        createSimulationJobRequests: Sequence[SimulationJobRequestUnionTypeDef],
+        createSimulationJobRequests: Sequence[SimulationJobRequestTypeDef],
         clientRequestToken: str = ...,
         batchPolicy: BatchPolicyTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> StartSimulationJobBatchResponseTypeDef:
         """
         Starts a new simulation job batch.
```

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/literals.py` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,15 @@
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
@@ -317,14 +318,15 @@
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
@@ -403,26 +405,28 @@
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

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/literals.pyi` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
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
@@ -315,14 +316,15 @@
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
@@ -401,26 +403,28 @@
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

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/paginator.py` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/paginator.pyi` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/type_defs.py` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_robomaker.type_defs import BatchDeleteWorldsRequestRequestTypeDef
 
     data: BatchDeleteWorldsRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ArchitectureType,
     ComputeTypeType,
     DataSourceTypeType,
     DeploymentJobErrorCodeType,
     DeploymentStatusType,
@@ -66,29 +66,27 @@
     "SourceConfigTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
+    "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
     "TemplateLocationTypeDef",
-    "DataSourceConfigOutputTypeDef",
-    "DataSourceConfigTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
-    "DeploymentLaunchConfigOutputTypeDef",
     "DeploymentLaunchConfigTypeDef",
     "S3ObjectTypeDef",
     "DeregisterRobotRequestRequestTypeDef",
     "DescribeDeploymentJobRequestRequestTypeDef",
     "DescribeFleetRequestRequestTypeDef",
     "RobotTypeDef",
     "DescribeRobotApplicationRequestRequestTypeDef",
@@ -115,15 +113,14 @@
     "PortMappingTypeDef",
     "ProgressDetailTypeDef",
     "RegisterRobotRequestRequestTypeDef",
     "RestartSimulationJobRequestRequestTypeDef",
     "ToolTypeDef",
     "UploadConfigurationTypeDef",
     "WorldConfigTypeDef",
-    "VPCConfigOutputTypeDef",
     "SyncDeploymentJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchDeleteWorldsResponseTypeDef",
     "CreateFleetResponseTypeDef",
     "CreateRobotResponseTypeDef",
     "CreateWorldTemplateResponseTypeDef",
@@ -154,17 +151,15 @@
     "DescribeWorldExportJobResponseTypeDef",
     "WorldExportJobSummaryTypeDef",
     "CreateWorldGenerationJobRequestRequestTypeDef",
     "CreateWorldGenerationJobResponseTypeDef",
     "WorldGenerationJobSummaryTypeDef",
     "CreateWorldTemplateRequestRequestTypeDef",
     "UpdateWorldTemplateRequestRequestTypeDef",
-    "DataSourceConfigUnionTypeDef",
     "DataSourceTypeDef",
-    "DeploymentApplicationConfigOutputTypeDef",
     "DeploymentApplicationConfigTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
     "FailureSummaryTypeDef",
     "ListDeploymentJobsRequestRequestTypeDef",
@@ -188,51 +183,41 @@
     "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListSimulationJobBatchesResponseTypeDef",
     "ListWorldTemplatesResponseTypeDef",
     "ListWorldsResponseTypeDef",
-    "PortForwardingConfigOutputTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
-    "VPCConfigUnionTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
     "ListWorldExportJobsResponseTypeDef",
     "ListWorldGenerationJobsResponseTypeDef",
-    "DeploymentApplicationConfigUnionTypeDef",
+    "CreateDeploymentJobRequestRequestTypeDef",
     "CreateDeploymentJobResponseTypeDef",
     "DeploymentJobTypeDef",
     "SyncDeploymentJobResponseTypeDef",
     "FinishedWorldsSummaryTypeDef",
-    "LaunchConfigOutputTypeDef",
     "LaunchConfigTypeDef",
     "DescribeDeploymentJobResponseTypeDef",
-    "CreateDeploymentJobRequestRequestTypeDef",
     "ListDeploymentJobsResponseTypeDef",
     "DescribeWorldGenerationJobResponseTypeDef",
-    "RobotApplicationConfigOutputTypeDef",
-    "SimulationApplicationConfigOutputTypeDef",
     "RobotApplicationConfigTypeDef",
     "SimulationApplicationConfigTypeDef",
+    "CreateSimulationJobRequestRequestTypeDef",
     "CreateSimulationJobResponseTypeDef",
     "DescribeSimulationJobResponseTypeDef",
-    "SimulationJobRequestOutputTypeDef",
-    "SimulationJobTypeDef",
-    "RobotApplicationConfigUnionTypeDef",
-    "SimulationApplicationConfigUnionTypeDef",
     "SimulationJobRequestTypeDef",
+    "SimulationJobTypeDef",
     "FailedCreateSimulationJobRequestTypeDef",
+    "StartSimulationJobBatchRequestRequestTypeDef",
     "BatchDescribeSimulationJobResponseTypeDef",
-    "CreateSimulationJobRequestRequestTypeDef",
-    "SimulationJobRequestUnionTypeDef",
     "DescribeSimulationJobBatchResponseTypeDef",
     "StartSimulationJobBatchResponseTypeDef",
-    "StartSimulationJobBatchRequestRequestTypeDef",
 )
 
 BatchDeleteWorldsRequestRequestTypeDef = TypedDict(
     "BatchDeleteWorldsRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
     },
@@ -464,14 +449,36 @@
 class CreateSimulationApplicationVersionRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredDataSourceConfigTypeDef = TypedDict(
+    "_RequiredDataSourceConfigTypeDef",
+    {
+        "name": str,
+        "s3Bucket": str,
+        "s3Keys": Sequence[str],
+    },
+)
+_OptionalDataSourceConfigTypeDef = TypedDict(
+    "_OptionalDataSourceConfigTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+
+class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
+    pass
+
+
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "recordAllRosTopics": bool,
     },
     total=False,
 )
@@ -529,60 +536,14 @@
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
-_RequiredDataSourceConfigOutputTypeDef = TypedDict(
-    "_RequiredDataSourceConfigOutputTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": List[str],
-    },
-)
-_OptionalDataSourceConfigOutputTypeDef = TypedDict(
-    "_OptionalDataSourceConfigOutputTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-
-class DataSourceConfigOutputTypeDef(
-    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
-):
-    pass
-
-
-_RequiredDataSourceConfigTypeDef = TypedDict(
-    "_RequiredDataSourceConfigTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": Sequence[str],
-    },
-)
-_OptionalDataSourceConfigTypeDef = TypedDict(
-    "_OptionalDataSourceConfigTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-
-class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
-    pass
-
-
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
     total=False,
@@ -649,38 +610,14 @@
 DeleteWorldTemplateRequestRequestTypeDef = TypedDict(
     "DeleteWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
-_RequiredDeploymentLaunchConfigOutputTypeDef = TypedDict(
-    "_RequiredDeploymentLaunchConfigOutputTypeDef",
-    {
-        "packageName": str,
-        "launchFile": str,
-    },
-)
-_OptionalDeploymentLaunchConfigOutputTypeDef = TypedDict(
-    "_OptionalDeploymentLaunchConfigOutputTypeDef",
-    {
-        "preLaunchFile": str,
-        "postLaunchFile": str,
-        "environmentVariables": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class DeploymentLaunchConfigOutputTypeDef(
-    _RequiredDeploymentLaunchConfigOutputTypeDef, _OptionalDeploymentLaunchConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredDeploymentLaunchConfigTypeDef = TypedDict(
     "_RequiredDeploymentLaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
     },
 )
@@ -1062,34 +999,14 @@
     "WorldConfigTypeDef",
     {
         "world": str,
     },
     total=False,
 )
 
-_RequiredVPCConfigOutputTypeDef = TypedDict(
-    "_RequiredVPCConfigOutputTypeDef",
-    {
-        "subnets": List[str],
-    },
-)
-_OptionalVPCConfigOutputTypeDef = TypedDict(
-    "_OptionalVPCConfigOutputTypeDef",
-    {
-        "securityGroups": List[str],
-        "assignPublicIp": bool,
-    },
-    total=False,
-)
-
-
-class VPCConfigOutputTypeDef(_RequiredVPCConfigOutputTypeDef, _OptionalVPCConfigOutputTypeDef):
-    pass
-
-
 SyncDeploymentJobRequestRequestTypeDef = TypedDict(
     "SyncDeploymentJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "fleet": str,
     },
 )
@@ -1662,36 +1579,26 @@
 class UpdateWorldTemplateRequestRequestTypeDef(
     _RequiredUpdateWorldTemplateRequestRequestTypeDef,
     _OptionalUpdateWorldTemplateRequestRequestTypeDef,
 ):
     pass
 
 
-DataSourceConfigUnionTypeDef = Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "name": str,
         "s3Bucket": str,
         "s3Keys": List[S3KeyOutputTypeDef],
         "type": DataSourceTypeType,
         "destination": str,
     },
     total=False,
 )
 
-DeploymentApplicationConfigOutputTypeDef = TypedDict(
-    "DeploymentApplicationConfigOutputTypeDef",
-    {
-        "application": str,
-        "applicationVersion": str,
-        "launchConfig": DeploymentLaunchConfigOutputTypeDef,
-    },
-)
-
 DeploymentApplicationConfigTypeDef = TypedDict(
     "DeploymentApplicationConfigTypeDef",
     {
         "application": str,
         "applicationVersion": str,
         "launchConfig": DeploymentLaunchConfigTypeDef,
     },
@@ -1984,26 +1891,18 @@
     {
         "worldSummaries": List[WorldSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PortForwardingConfigOutputTypeDef = TypedDict(
-    "PortForwardingConfigOutputTypeDef",
-    {
-        "portMappings": List[PortMappingTypeDef],
-    },
-    total=False,
-)
-
 PortForwardingConfigTypeDef = TypedDict(
     "PortForwardingConfigTypeDef",
     {
-        "portMappings": Sequence[PortMappingTypeDef],
+        "portMappings": List[PortMappingTypeDef],
     },
     total=False,
 )
 
 RobotDeploymentTypeDef = TypedDict(
     "RobotDeploymentTypeDef",
     {
@@ -2014,15 +1913,14 @@
         "progressDetail": ProgressDetailTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
     },
     total=False,
 )
 
-VPCConfigUnionTypeDef = Union[VPCConfigTypeDef, VPCConfigOutputTypeDef]
 ListRobotApplicationsResponseTypeDef = TypedDict(
     "ListRobotApplicationsResponseTypeDef",
     {
         "robotApplicationSummaries": List[RobotApplicationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2051,24 +1949,46 @@
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeploymentApplicationConfigUnionTypeDef = Union[
-    DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef
-]
+_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "fleet": str,
+        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
+    },
+)
+_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "deploymentConfig": DeploymentConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDeploymentJobRequestRequestTypeDef(
+    _RequiredCreateDeploymentJobRequestRequestTypeDef,
+    _OptionalCreateDeploymentJobRequestRequestTypeDef,
+):
+    pass
+
+
 CreateDeploymentJobResponseTypeDef = TypedDict(
     "CreateDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "deploymentConfig": DeploymentConfigTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2076,15 +1996,15 @@
 
 DeploymentJobTypeDef = TypedDict(
     "DeploymentJobTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "deploymentConfig": DeploymentConfigTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
     },
     total=False,
 )
@@ -2092,15 +2012,15 @@
 SyncDeploymentJobResponseTypeDef = TypedDict(
     "SyncDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2110,82 +2030,44 @@
         "finishedCount": int,
         "succeededWorlds": List[str],
         "failureSummary": FailureSummaryTypeDef,
     },
     total=False,
 )
 
-LaunchConfigOutputTypeDef = TypedDict(
-    "LaunchConfigOutputTypeDef",
-    {
-        "packageName": str,
-        "launchFile": str,
-        "environmentVariables": Dict[str, str],
-        "portForwardingConfig": PortForwardingConfigOutputTypeDef,
-        "streamUI": bool,
-        "command": List[str],
-    },
-    total=False,
-)
-
 LaunchConfigTypeDef = TypedDict(
     "LaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
-        "environmentVariables": Mapping[str, str],
+        "environmentVariables": Dict[str, str],
         "portForwardingConfig": PortForwardingConfigTypeDef,
         "streamUI": bool,
-        "command": Sequence[str],
+        "command": List[str],
     },
     total=False,
 )
 
 DescribeDeploymentJobResponseTypeDef = TypedDict(
     "DescribeDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "fleet": str,
-        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigUnionTypeDef],
-    },
-)
-_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDeploymentJobRequestRequestTypeDef(
-    _RequiredCreateDeploymentJobRequestRequestTypeDef,
-    _OptionalCreateDeploymentJobRequestRequestTypeDef,
-):
-    pass
-
-
 ListDeploymentJobsResponseTypeDef = TypedDict(
     "ListDeploymentJobsResponseTypeDef",
     {
         "deploymentJobs": List[DeploymentJobTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2205,117 +2087,95 @@
         "finishedWorldsSummary": FinishedWorldsSummaryTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRobotApplicationConfigOutputTypeDef = TypedDict(
-    "_RequiredRobotApplicationConfigOutputTypeDef",
+_RequiredRobotApplicationConfigTypeDef = TypedDict(
+    "_RequiredRobotApplicationConfigTypeDef",
     {
         "application": str,
-        "launchConfig": LaunchConfigOutputTypeDef,
+        "launchConfig": LaunchConfigTypeDef,
     },
 )
-_OptionalRobotApplicationConfigOutputTypeDef = TypedDict(
-    "_OptionalRobotApplicationConfigOutputTypeDef",
+_OptionalRobotApplicationConfigTypeDef = TypedDict(
+    "_OptionalRobotApplicationConfigTypeDef",
     {
         "applicationVersion": str,
         "uploadConfigurations": List[UploadConfigurationTypeDef],
         "useDefaultUploadConfigurations": bool,
         "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 
-class RobotApplicationConfigOutputTypeDef(
-    _RequiredRobotApplicationConfigOutputTypeDef, _OptionalRobotApplicationConfigOutputTypeDef
+class RobotApplicationConfigTypeDef(
+    _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
 ):
     pass
 
 
-_RequiredSimulationApplicationConfigOutputTypeDef = TypedDict(
-    "_RequiredSimulationApplicationConfigOutputTypeDef",
+_RequiredSimulationApplicationConfigTypeDef = TypedDict(
+    "_RequiredSimulationApplicationConfigTypeDef",
     {
         "application": str,
-        "launchConfig": LaunchConfigOutputTypeDef,
+        "launchConfig": LaunchConfigTypeDef,
     },
 )
-_OptionalSimulationApplicationConfigOutputTypeDef = TypedDict(
-    "_OptionalSimulationApplicationConfigOutputTypeDef",
+_OptionalSimulationApplicationConfigTypeDef = TypedDict(
+    "_OptionalSimulationApplicationConfigTypeDef",
     {
         "applicationVersion": str,
         "uploadConfigurations": List[UploadConfigurationTypeDef],
         "worldConfigs": List[WorldConfigTypeDef],
         "useDefaultUploadConfigurations": bool,
         "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
 
-class SimulationApplicationConfigOutputTypeDef(
-    _RequiredSimulationApplicationConfigOutputTypeDef,
-    _OptionalSimulationApplicationConfigOutputTypeDef,
-):
-    pass
-
-
-_RequiredRobotApplicationConfigTypeDef = TypedDict(
-    "_RequiredRobotApplicationConfigTypeDef",
-    {
-        "application": str,
-        "launchConfig": LaunchConfigTypeDef,
-    },
-)
-_OptionalRobotApplicationConfigTypeDef = TypedDict(
-    "_OptionalRobotApplicationConfigTypeDef",
-    {
-        "applicationVersion": str,
-        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
-        "useDefaultUploadConfigurations": bool,
-        "tools": Sequence[ToolTypeDef],
-        "useDefaultTools": bool,
-    },
-    total=False,
-)
-
-
-class RobotApplicationConfigTypeDef(
-    _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
+class SimulationApplicationConfigTypeDef(
+    _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
 ):
     pass
 
 
-_RequiredSimulationApplicationConfigTypeDef = TypedDict(
-    "_RequiredSimulationApplicationConfigTypeDef",
+_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSimulationJobRequestRequestTypeDef",
     {
-        "application": str,
-        "launchConfig": LaunchConfigTypeDef,
+        "maxJobDurationInSeconds": int,
+        "iamRole": str,
     },
 )
-_OptionalSimulationApplicationConfigTypeDef = TypedDict(
-    "_OptionalSimulationApplicationConfigTypeDef",
+_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSimulationJobRequestRequestTypeDef",
     {
-        "applicationVersion": str,
-        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
-        "worldConfigs": Sequence[WorldConfigTypeDef],
-        "useDefaultUploadConfigurations": bool,
-        "tools": Sequence[ToolTypeDef],
-        "useDefaultTools": bool,
+        "clientRequestToken": str,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "failureBehavior": FailureBehaviorType,
+        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
+        "dataSources": Sequence[DataSourceConfigTypeDef],
+        "tags": Mapping[str, str],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
     },
     total=False,
 )
 
 
-class SimulationApplicationConfigTypeDef(
-    _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
+class CreateSimulationJobRequestRequestTypeDef(
+    _RequiredCreateSimulationJobRequestRequestTypeDef,
+    _OptionalCreateSimulationJobRequestRequestTypeDef,
 ):
     pass
 
 
 CreateSimulationJobResponseTypeDef = TypedDict(
     "CreateSimulationJobResponseTypeDef",
     {
@@ -2327,16 +2187,16 @@
         "failureCode": SimulationJobErrorCodeType,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
+        "robotApplications": List[RobotApplicationConfigTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "compute": ComputeResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2354,52 +2214,52 @@
         "failureReason": str,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
+        "robotApplications": List[RobotApplicationConfigTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSimulationJobRequestOutputTypeDef = TypedDict(
-    "_RequiredSimulationJobRequestOutputTypeDef",
+_RequiredSimulationJobRequestTypeDef = TypedDict(
+    "_RequiredSimulationJobRequestTypeDef",
     {
         "maxJobDurationInSeconds": int,
     },
 )
-_OptionalSimulationJobRequestOutputTypeDef = TypedDict(
-    "_OptionalSimulationJobRequestOutputTypeDef",
+_OptionalSimulationJobRequestTypeDef = TypedDict(
+    "_OptionalSimulationJobRequestTypeDef",
     {
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "iamRole": str,
         "failureBehavior": FailureBehaviorType,
         "useDefaultApplications": bool,
-        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
-        "dataSources": List[DataSourceConfigOutputTypeDef],
-        "vpcConfig": VPCConfigOutputTypeDef,
+        "robotApplications": List[RobotApplicationConfigTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "dataSources": List[DataSourceConfigTypeDef],
+        "vpcConfig": VPCConfigTypeDef,
         "compute": ComputeTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class SimulationJobRequestOutputTypeDef(
-    _RequiredSimulationJobRequestOutputTypeDef, _OptionalSimulationJobRequestOutputTypeDef
+class SimulationJobRequestTypeDef(
+    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
 ):
     pass
 
 
 SimulationJobTypeDef = TypedDict(
     "SimulationJobTypeDef",
     {
@@ -2413,130 +2273,82 @@
         "failureReason": str,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
+        "robotApplications": List[RobotApplicationConfigTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
     },
     total=False,
 )
 
-RobotApplicationConfigUnionTypeDef = Union[
-    RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef
-]
-SimulationApplicationConfigUnionTypeDef = Union[
-    SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef
-]
-_RequiredSimulationJobRequestTypeDef = TypedDict(
-    "_RequiredSimulationJobRequestTypeDef",
-    {
-        "maxJobDurationInSeconds": int,
-    },
-)
-_OptionalSimulationJobRequestTypeDef = TypedDict(
-    "_OptionalSimulationJobRequestTypeDef",
-    {
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
-        "iamRole": str,
-        "failureBehavior": FailureBehaviorType,
-        "useDefaultApplications": bool,
-        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
-        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
-        "dataSources": Sequence[DataSourceConfigTypeDef],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class SimulationJobRequestTypeDef(
-    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
-):
-    pass
-
-
 FailedCreateSimulationJobRequestTypeDef = TypedDict(
     "FailedCreateSimulationJobRequestTypeDef",
     {
-        "request": SimulationJobRequestOutputTypeDef,
+        "request": SimulationJobRequestTypeDef,
         "failureReason": str,
         "failureCode": SimulationJobErrorCodeType,
         "failedAt": datetime,
     },
     total=False,
 )
 
-BatchDescribeSimulationJobResponseTypeDef = TypedDict(
-    "BatchDescribeSimulationJobResponseTypeDef",
-    {
-        "jobs": List[SimulationJobTypeDef],
-        "unprocessedJobs": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSimulationJobRequestRequestTypeDef",
+_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
     {
-        "maxJobDurationInSeconds": int,
-        "iamRole": str,
+        "createSimulationJobRequests": Sequence[SimulationJobRequestTypeDef],
     },
 )
-_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSimulationJobRequestRequestTypeDef",
+_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
     {
         "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
-        "failureBehavior": FailureBehaviorType,
-        "robotApplications": Sequence[RobotApplicationConfigUnionTypeDef],
-        "simulationApplications": Sequence[SimulationApplicationConfigUnionTypeDef],
-        "dataSources": Sequence[DataSourceConfigUnionTypeDef],
+        "batchPolicy": BatchPolicyTypeDef,
         "tags": Mapping[str, str],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
     },
     total=False,
 )
 
 
-class CreateSimulationJobRequestRequestTypeDef(
-    _RequiredCreateSimulationJobRequestRequestTypeDef,
-    _OptionalCreateSimulationJobRequestRequestTypeDef,
+class StartSimulationJobBatchRequestRequestTypeDef(
+    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
+    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
 ):
     pass
 
 
-SimulationJobRequestUnionTypeDef = Union[
-    SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef
-]
+BatchDescribeSimulationJobResponseTypeDef = TypedDict(
+    "BatchDescribeSimulationJobResponseTypeDef",
+    {
+        "jobs": List[SimulationJobTypeDef],
+        "unprocessedJobs": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeSimulationJobBatchResponseTypeDef = TypedDict(
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "lastUpdatedAt": datetime,
         "createdAt": datetime,
         "clientRequestToken": str,
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
+        "pendingRequests": List[SimulationJobRequestTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSimulationJobBatchResponseTypeDef = TypedDict(
@@ -2546,36 +2358,13 @@
         "status": SimulationJobBatchStatusType,
         "createdAt": datetime,
         "clientRequestToken": str,
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
+        "pendingRequests": List[SimulationJobRequestTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
-    {
-        "createSimulationJobRequests": Sequence[SimulationJobRequestUnionTypeDef],
-    },
-)
-_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "batchPolicy": BatchPolicyTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class StartSimulationJobBatchRequestRequestTypeDef(
-    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
-    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker/type_defs.pyi` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_robomaker.type_defs import BatchDeleteWorldsRequestRequestTypeDef
 
     data: BatchDeleteWorldsRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     ArchitectureType,
     ComputeTypeType,
     DataSourceTypeType,
     DeploymentJobErrorCodeType,
     DeploymentStatusType,
@@ -65,29 +65,27 @@
     "SourceConfigTypeDef",
     "SourceTypeDef",
     "CreateRobotApplicationVersionRequestRequestTypeDef",
     "CreateRobotRequestRequestTypeDef",
     "RenderingEngineTypeDef",
     "SimulationSoftwareSuiteTypeDef",
     "CreateSimulationApplicationVersionRequestRequestTypeDef",
+    "DataSourceConfigTypeDef",
     "LoggingConfigTypeDef",
     "OutputLocationTypeDef",
     "VPCConfigTypeDef",
     "VPCConfigResponseTypeDef",
     "WorldCountTypeDef",
     "TemplateLocationTypeDef",
-    "DataSourceConfigOutputTypeDef",
-    "DataSourceConfigTypeDef",
     "S3KeyOutputTypeDef",
     "DeleteFleetRequestRequestTypeDef",
     "DeleteRobotApplicationRequestRequestTypeDef",
     "DeleteRobotRequestRequestTypeDef",
     "DeleteSimulationApplicationRequestRequestTypeDef",
     "DeleteWorldTemplateRequestRequestTypeDef",
-    "DeploymentLaunchConfigOutputTypeDef",
     "DeploymentLaunchConfigTypeDef",
     "S3ObjectTypeDef",
     "DeregisterRobotRequestRequestTypeDef",
     "DescribeDeploymentJobRequestRequestTypeDef",
     "DescribeFleetRequestRequestTypeDef",
     "RobotTypeDef",
     "DescribeRobotApplicationRequestRequestTypeDef",
@@ -114,15 +112,14 @@
     "PortMappingTypeDef",
     "ProgressDetailTypeDef",
     "RegisterRobotRequestRequestTypeDef",
     "RestartSimulationJobRequestRequestTypeDef",
     "ToolTypeDef",
     "UploadConfigurationTypeDef",
     "WorldConfigTypeDef",
-    "VPCConfigOutputTypeDef",
     "SyncDeploymentJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchDeleteWorldsResponseTypeDef",
     "CreateFleetResponseTypeDef",
     "CreateRobotResponseTypeDef",
     "CreateWorldTemplateResponseTypeDef",
@@ -153,17 +150,15 @@
     "DescribeWorldExportJobResponseTypeDef",
     "WorldExportJobSummaryTypeDef",
     "CreateWorldGenerationJobRequestRequestTypeDef",
     "CreateWorldGenerationJobResponseTypeDef",
     "WorldGenerationJobSummaryTypeDef",
     "CreateWorldTemplateRequestRequestTypeDef",
     "UpdateWorldTemplateRequestRequestTypeDef",
-    "DataSourceConfigUnionTypeDef",
     "DataSourceTypeDef",
-    "DeploymentApplicationConfigOutputTypeDef",
     "DeploymentApplicationConfigTypeDef",
     "DeploymentConfigTypeDef",
     "DescribeFleetResponseTypeDef",
     "ListRobotsResponseTypeDef",
     "ListSimulationJobsResponseTypeDef",
     "FailureSummaryTypeDef",
     "ListDeploymentJobsRequestRequestTypeDef",
@@ -187,51 +182,41 @@
     "ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef",
     "ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef",
     "ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef",
     "ListWorldsRequestListWorldsPaginateTypeDef",
     "ListSimulationJobBatchesResponseTypeDef",
     "ListWorldTemplatesResponseTypeDef",
     "ListWorldsResponseTypeDef",
-    "PortForwardingConfigOutputTypeDef",
     "PortForwardingConfigTypeDef",
     "RobotDeploymentTypeDef",
-    "VPCConfigUnionTypeDef",
     "ListRobotApplicationsResponseTypeDef",
     "ListSimulationApplicationsResponseTypeDef",
     "ListWorldExportJobsResponseTypeDef",
     "ListWorldGenerationJobsResponseTypeDef",
-    "DeploymentApplicationConfigUnionTypeDef",
+    "CreateDeploymentJobRequestRequestTypeDef",
     "CreateDeploymentJobResponseTypeDef",
     "DeploymentJobTypeDef",
     "SyncDeploymentJobResponseTypeDef",
     "FinishedWorldsSummaryTypeDef",
-    "LaunchConfigOutputTypeDef",
     "LaunchConfigTypeDef",
     "DescribeDeploymentJobResponseTypeDef",
-    "CreateDeploymentJobRequestRequestTypeDef",
     "ListDeploymentJobsResponseTypeDef",
     "DescribeWorldGenerationJobResponseTypeDef",
-    "RobotApplicationConfigOutputTypeDef",
-    "SimulationApplicationConfigOutputTypeDef",
     "RobotApplicationConfigTypeDef",
     "SimulationApplicationConfigTypeDef",
+    "CreateSimulationJobRequestRequestTypeDef",
     "CreateSimulationJobResponseTypeDef",
     "DescribeSimulationJobResponseTypeDef",
-    "SimulationJobRequestOutputTypeDef",
-    "SimulationJobTypeDef",
-    "RobotApplicationConfigUnionTypeDef",
-    "SimulationApplicationConfigUnionTypeDef",
     "SimulationJobRequestTypeDef",
+    "SimulationJobTypeDef",
     "FailedCreateSimulationJobRequestTypeDef",
+    "StartSimulationJobBatchRequestRequestTypeDef",
     "BatchDescribeSimulationJobResponseTypeDef",
-    "CreateSimulationJobRequestRequestTypeDef",
-    "SimulationJobRequestUnionTypeDef",
     "DescribeSimulationJobBatchResponseTypeDef",
     "StartSimulationJobBatchResponseTypeDef",
-    "StartSimulationJobBatchRequestRequestTypeDef",
 )
 
 BatchDeleteWorldsRequestRequestTypeDef = TypedDict(
     "BatchDeleteWorldsRequestRequestTypeDef",
     {
         "worlds": Sequence[str],
     },
@@ -455,14 +440,34 @@
 
 class CreateSimulationApplicationVersionRequestRequestTypeDef(
     _RequiredCreateSimulationApplicationVersionRequestRequestTypeDef,
     _OptionalCreateSimulationApplicationVersionRequestRequestTypeDef,
 ):
     pass
 
+_RequiredDataSourceConfigTypeDef = TypedDict(
+    "_RequiredDataSourceConfigTypeDef",
+    {
+        "name": str,
+        "s3Bucket": str,
+        "s3Keys": Sequence[str],
+    },
+)
+_OptionalDataSourceConfigTypeDef = TypedDict(
+    "_OptionalDataSourceConfigTypeDef",
+    {
+        "type": DataSourceTypeType,
+        "destination": str,
+    },
+    total=False,
+)
+
+class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
+    pass
+
 LoggingConfigTypeDef = TypedDict(
     "LoggingConfigTypeDef",
     {
         "recordAllRosTopics": bool,
     },
     total=False,
 )
@@ -518,56 +523,14 @@
     "TemplateLocationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
     },
 )
 
-_RequiredDataSourceConfigOutputTypeDef = TypedDict(
-    "_RequiredDataSourceConfigOutputTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": List[str],
-    },
-)
-_OptionalDataSourceConfigOutputTypeDef = TypedDict(
-    "_OptionalDataSourceConfigOutputTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-class DataSourceConfigOutputTypeDef(
-    _RequiredDataSourceConfigOutputTypeDef, _OptionalDataSourceConfigOutputTypeDef
-):
-    pass
-
-_RequiredDataSourceConfigTypeDef = TypedDict(
-    "_RequiredDataSourceConfigTypeDef",
-    {
-        "name": str,
-        "s3Bucket": str,
-        "s3Keys": Sequence[str],
-    },
-)
-_OptionalDataSourceConfigTypeDef = TypedDict(
-    "_OptionalDataSourceConfigTypeDef",
-    {
-        "type": DataSourceTypeType,
-        "destination": str,
-    },
-    total=False,
-)
-
-class DataSourceConfigTypeDef(_RequiredDataSourceConfigTypeDef, _OptionalDataSourceConfigTypeDef):
-    pass
-
 S3KeyOutputTypeDef = TypedDict(
     "S3KeyOutputTypeDef",
     {
         "s3Key": str,
         "etag": str,
     },
     total=False,
@@ -630,36 +593,14 @@
 DeleteWorldTemplateRequestRequestTypeDef = TypedDict(
     "DeleteWorldTemplateRequestRequestTypeDef",
     {
         "template": str,
     },
 )
 
-_RequiredDeploymentLaunchConfigOutputTypeDef = TypedDict(
-    "_RequiredDeploymentLaunchConfigOutputTypeDef",
-    {
-        "packageName": str,
-        "launchFile": str,
-    },
-)
-_OptionalDeploymentLaunchConfigOutputTypeDef = TypedDict(
-    "_OptionalDeploymentLaunchConfigOutputTypeDef",
-    {
-        "preLaunchFile": str,
-        "postLaunchFile": str,
-        "environmentVariables": Dict[str, str],
-    },
-    total=False,
-)
-
-class DeploymentLaunchConfigOutputTypeDef(
-    _RequiredDeploymentLaunchConfigOutputTypeDef, _OptionalDeploymentLaunchConfigOutputTypeDef
-):
-    pass
-
 _RequiredDeploymentLaunchConfigTypeDef = TypedDict(
     "_RequiredDeploymentLaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
     },
 )
@@ -1029,32 +970,14 @@
     "WorldConfigTypeDef",
     {
         "world": str,
     },
     total=False,
 )
 
-_RequiredVPCConfigOutputTypeDef = TypedDict(
-    "_RequiredVPCConfigOutputTypeDef",
-    {
-        "subnets": List[str],
-    },
-)
-_OptionalVPCConfigOutputTypeDef = TypedDict(
-    "_OptionalVPCConfigOutputTypeDef",
-    {
-        "securityGroups": List[str],
-        "assignPublicIp": bool,
-    },
-    total=False,
-)
-
-class VPCConfigOutputTypeDef(_RequiredVPCConfigOutputTypeDef, _OptionalVPCConfigOutputTypeDef):
-    pass
-
 SyncDeploymentJobRequestRequestTypeDef = TypedDict(
     "SyncDeploymentJobRequestRequestTypeDef",
     {
         "clientRequestToken": str,
         "fleet": str,
     },
 )
@@ -1613,36 +1536,26 @@
 
 class UpdateWorldTemplateRequestRequestTypeDef(
     _RequiredUpdateWorldTemplateRequestRequestTypeDef,
     _OptionalUpdateWorldTemplateRequestRequestTypeDef,
 ):
     pass
 
-DataSourceConfigUnionTypeDef = Union[DataSourceConfigTypeDef, DataSourceConfigOutputTypeDef]
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "name": str,
         "s3Bucket": str,
         "s3Keys": List[S3KeyOutputTypeDef],
         "type": DataSourceTypeType,
         "destination": str,
     },
     total=False,
 )
 
-DeploymentApplicationConfigOutputTypeDef = TypedDict(
-    "DeploymentApplicationConfigOutputTypeDef",
-    {
-        "application": str,
-        "applicationVersion": str,
-        "launchConfig": DeploymentLaunchConfigOutputTypeDef,
-    },
-)
-
 DeploymentApplicationConfigTypeDef = TypedDict(
     "DeploymentApplicationConfigTypeDef",
     {
         "application": str,
         "applicationVersion": str,
         "launchConfig": DeploymentLaunchConfigTypeDef,
     },
@@ -1935,26 +1848,18 @@
     {
         "worldSummaries": List[WorldSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PortForwardingConfigOutputTypeDef = TypedDict(
-    "PortForwardingConfigOutputTypeDef",
-    {
-        "portMappings": List[PortMappingTypeDef],
-    },
-    total=False,
-)
-
 PortForwardingConfigTypeDef = TypedDict(
     "PortForwardingConfigTypeDef",
     {
-        "portMappings": Sequence[PortMappingTypeDef],
+        "portMappings": List[PortMappingTypeDef],
     },
     total=False,
 )
 
 RobotDeploymentTypeDef = TypedDict(
     "RobotDeploymentTypeDef",
     {
@@ -1965,15 +1870,14 @@
         "progressDetail": ProgressDetailTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
     },
     total=False,
 )
 
-VPCConfigUnionTypeDef = Union[VPCConfigTypeDef, VPCConfigOutputTypeDef]
 ListRobotApplicationsResponseTypeDef = TypedDict(
     "ListRobotApplicationsResponseTypeDef",
     {
         "robotApplicationSummaries": List[RobotApplicationSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2002,24 +1906,44 @@
     {
         "worldGenerationJobSummaries": List[WorldGenerationJobSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeploymentApplicationConfigUnionTypeDef = Union[
-    DeploymentApplicationConfigTypeDef, DeploymentApplicationConfigOutputTypeDef
-]
+_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "clientRequestToken": str,
+        "fleet": str,
+        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigTypeDef],
+    },
+)
+_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
+    {
+        "deploymentConfig": DeploymentConfigTypeDef,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDeploymentJobRequestRequestTypeDef(
+    _RequiredCreateDeploymentJobRequestRequestTypeDef,
+    _OptionalCreateDeploymentJobRequestRequestTypeDef,
+):
+    pass
+
 CreateDeploymentJobResponseTypeDef = TypedDict(
     "CreateDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "deploymentConfig": DeploymentConfigTypeDef,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2027,15 +1951,15 @@
 
 DeploymentJobTypeDef = TypedDict(
     "DeploymentJobTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "deploymentConfig": DeploymentConfigTypeDef,
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
     },
     total=False,
 )
@@ -2043,15 +1967,15 @@
 SyncDeploymentJobResponseTypeDef = TypedDict(
     "SyncDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2061,80 +1985,44 @@
         "finishedCount": int,
         "succeededWorlds": List[str],
         "failureSummary": FailureSummaryTypeDef,
     },
     total=False,
 )
 
-LaunchConfigOutputTypeDef = TypedDict(
-    "LaunchConfigOutputTypeDef",
-    {
-        "packageName": str,
-        "launchFile": str,
-        "environmentVariables": Dict[str, str],
-        "portForwardingConfig": PortForwardingConfigOutputTypeDef,
-        "streamUI": bool,
-        "command": List[str],
-    },
-    total=False,
-)
-
 LaunchConfigTypeDef = TypedDict(
     "LaunchConfigTypeDef",
     {
         "packageName": str,
         "launchFile": str,
-        "environmentVariables": Mapping[str, str],
+        "environmentVariables": Dict[str, str],
         "portForwardingConfig": PortForwardingConfigTypeDef,
         "streamUI": bool,
-        "command": Sequence[str],
+        "command": List[str],
     },
     total=False,
 )
 
 DescribeDeploymentJobResponseTypeDef = TypedDict(
     "DescribeDeploymentJobResponseTypeDef",
     {
         "arn": str,
         "fleet": str,
         "status": DeploymentStatusType,
         "deploymentConfig": DeploymentConfigTypeDef,
-        "deploymentApplicationConfigs": List[DeploymentApplicationConfigOutputTypeDef],
+        "deploymentApplicationConfigs": List[DeploymentApplicationConfigTypeDef],
         "failureReason": str,
         "failureCode": DeploymentJobErrorCodeType,
         "createdAt": datetime,
         "robotDeploymentSummary": List[RobotDeploymentTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "fleet": str,
-        "deploymentApplicationConfigs": Sequence[DeploymentApplicationConfigUnionTypeDef],
-    },
-)
-_OptionalCreateDeploymentJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDeploymentJobRequestRequestTypeDef",
-    {
-        "deploymentConfig": DeploymentConfigTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDeploymentJobRequestRequestTypeDef(
-    _RequiredCreateDeploymentJobRequestRequestTypeDef,
-    _OptionalCreateDeploymentJobRequestRequestTypeDef,
-):
-    pass
-
 ListDeploymentJobsResponseTypeDef = TypedDict(
     "ListDeploymentJobsResponseTypeDef",
     {
         "deploymentJobs": List[DeploymentJobTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2154,110 +2042,90 @@
         "finishedWorldsSummary": FinishedWorldsSummaryTypeDef,
         "tags": Dict[str, str],
         "worldTags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredRobotApplicationConfigOutputTypeDef = TypedDict(
-    "_RequiredRobotApplicationConfigOutputTypeDef",
+_RequiredRobotApplicationConfigTypeDef = TypedDict(
+    "_RequiredRobotApplicationConfigTypeDef",
     {
         "application": str,
-        "launchConfig": LaunchConfigOutputTypeDef,
+        "launchConfig": LaunchConfigTypeDef,
     },
 )
-_OptionalRobotApplicationConfigOutputTypeDef = TypedDict(
-    "_OptionalRobotApplicationConfigOutputTypeDef",
+_OptionalRobotApplicationConfigTypeDef = TypedDict(
+    "_OptionalRobotApplicationConfigTypeDef",
     {
         "applicationVersion": str,
         "uploadConfigurations": List[UploadConfigurationTypeDef],
         "useDefaultUploadConfigurations": bool,
         "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
-class RobotApplicationConfigOutputTypeDef(
-    _RequiredRobotApplicationConfigOutputTypeDef, _OptionalRobotApplicationConfigOutputTypeDef
+class RobotApplicationConfigTypeDef(
+    _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
 ):
     pass
 
-_RequiredSimulationApplicationConfigOutputTypeDef = TypedDict(
-    "_RequiredSimulationApplicationConfigOutputTypeDef",
+_RequiredSimulationApplicationConfigTypeDef = TypedDict(
+    "_RequiredSimulationApplicationConfigTypeDef",
     {
         "application": str,
-        "launchConfig": LaunchConfigOutputTypeDef,
+        "launchConfig": LaunchConfigTypeDef,
     },
 )
-_OptionalSimulationApplicationConfigOutputTypeDef = TypedDict(
-    "_OptionalSimulationApplicationConfigOutputTypeDef",
+_OptionalSimulationApplicationConfigTypeDef = TypedDict(
+    "_OptionalSimulationApplicationConfigTypeDef",
     {
         "applicationVersion": str,
         "uploadConfigurations": List[UploadConfigurationTypeDef],
         "worldConfigs": List[WorldConfigTypeDef],
         "useDefaultUploadConfigurations": bool,
         "tools": List[ToolTypeDef],
         "useDefaultTools": bool,
     },
     total=False,
 )
 
-class SimulationApplicationConfigOutputTypeDef(
-    _RequiredSimulationApplicationConfigOutputTypeDef,
-    _OptionalSimulationApplicationConfigOutputTypeDef,
-):
-    pass
-
-_RequiredRobotApplicationConfigTypeDef = TypedDict(
-    "_RequiredRobotApplicationConfigTypeDef",
-    {
-        "application": str,
-        "launchConfig": LaunchConfigTypeDef,
-    },
-)
-_OptionalRobotApplicationConfigTypeDef = TypedDict(
-    "_OptionalRobotApplicationConfigTypeDef",
-    {
-        "applicationVersion": str,
-        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
-        "useDefaultUploadConfigurations": bool,
-        "tools": Sequence[ToolTypeDef],
-        "useDefaultTools": bool,
-    },
-    total=False,
-)
-
-class RobotApplicationConfigTypeDef(
-    _RequiredRobotApplicationConfigTypeDef, _OptionalRobotApplicationConfigTypeDef
+class SimulationApplicationConfigTypeDef(
+    _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
 ):
     pass
 
-_RequiredSimulationApplicationConfigTypeDef = TypedDict(
-    "_RequiredSimulationApplicationConfigTypeDef",
+_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSimulationJobRequestRequestTypeDef",
     {
-        "application": str,
-        "launchConfig": LaunchConfigTypeDef,
+        "maxJobDurationInSeconds": int,
+        "iamRole": str,
     },
 )
-_OptionalSimulationApplicationConfigTypeDef = TypedDict(
-    "_OptionalSimulationApplicationConfigTypeDef",
+_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSimulationJobRequestRequestTypeDef",
     {
-        "applicationVersion": str,
-        "uploadConfigurations": Sequence[UploadConfigurationTypeDef],
-        "worldConfigs": Sequence[WorldConfigTypeDef],
-        "useDefaultUploadConfigurations": bool,
-        "tools": Sequence[ToolTypeDef],
-        "useDefaultTools": bool,
+        "clientRequestToken": str,
+        "outputLocation": OutputLocationTypeDef,
+        "loggingConfig": LoggingConfigTypeDef,
+        "failureBehavior": FailureBehaviorType,
+        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
+        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
+        "dataSources": Sequence[DataSourceConfigTypeDef],
+        "tags": Mapping[str, str],
+        "vpcConfig": VPCConfigTypeDef,
+        "compute": ComputeTypeDef,
     },
     total=False,
 )
 
-class SimulationApplicationConfigTypeDef(
-    _RequiredSimulationApplicationConfigTypeDef, _OptionalSimulationApplicationConfigTypeDef
+class CreateSimulationJobRequestRequestTypeDef(
+    _RequiredCreateSimulationJobRequestRequestTypeDef,
+    _OptionalCreateSimulationJobRequestRequestTypeDef,
 ):
     pass
 
 CreateSimulationJobResponseTypeDef = TypedDict(
     "CreateSimulationJobResponseTypeDef",
     {
         "arn": str,
@@ -2268,16 +2136,16 @@
         "failureCode": SimulationJobErrorCodeType,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
+        "robotApplications": List[RobotApplicationConfigTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "compute": ComputeResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2295,51 +2163,51 @@
         "failureReason": str,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
+        "robotApplications": List[RobotApplicationConfigTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredSimulationJobRequestOutputTypeDef = TypedDict(
-    "_RequiredSimulationJobRequestOutputTypeDef",
+_RequiredSimulationJobRequestTypeDef = TypedDict(
+    "_RequiredSimulationJobRequestTypeDef",
     {
         "maxJobDurationInSeconds": int,
     },
 )
-_OptionalSimulationJobRequestOutputTypeDef = TypedDict(
-    "_OptionalSimulationJobRequestOutputTypeDef",
+_OptionalSimulationJobRequestTypeDef = TypedDict(
+    "_OptionalSimulationJobRequestTypeDef",
     {
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "iamRole": str,
         "failureBehavior": FailureBehaviorType,
         "useDefaultApplications": bool,
-        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
-        "dataSources": List[DataSourceConfigOutputTypeDef],
-        "vpcConfig": VPCConfigOutputTypeDef,
+        "robotApplications": List[RobotApplicationConfigTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigTypeDef],
+        "dataSources": List[DataSourceConfigTypeDef],
+        "vpcConfig": VPCConfigTypeDef,
         "compute": ComputeTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-class SimulationJobRequestOutputTypeDef(
-    _RequiredSimulationJobRequestOutputTypeDef, _OptionalSimulationJobRequestOutputTypeDef
+class SimulationJobRequestTypeDef(
+    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
 ):
     pass
 
 SimulationJobTypeDef = TypedDict(
     "SimulationJobTypeDef",
     {
         "arn": str,
@@ -2352,126 +2220,80 @@
         "failureReason": str,
         "clientRequestToken": str,
         "outputLocation": OutputLocationTypeDef,
         "loggingConfig": LoggingConfigTypeDef,
         "maxJobDurationInSeconds": int,
         "simulationTimeMillis": int,
         "iamRole": str,
-        "robotApplications": List[RobotApplicationConfigOutputTypeDef],
-        "simulationApplications": List[SimulationApplicationConfigOutputTypeDef],
+        "robotApplications": List[RobotApplicationConfigTypeDef],
+        "simulationApplications": List[SimulationApplicationConfigTypeDef],
         "dataSources": List[DataSourceTypeDef],
         "tags": Dict[str, str],
         "vpcConfig": VPCConfigResponseTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "compute": ComputeResponseTypeDef,
     },
     total=False,
 )
 
-RobotApplicationConfigUnionTypeDef = Union[
-    RobotApplicationConfigTypeDef, RobotApplicationConfigOutputTypeDef
-]
-SimulationApplicationConfigUnionTypeDef = Union[
-    SimulationApplicationConfigTypeDef, SimulationApplicationConfigOutputTypeDef
-]
-_RequiredSimulationJobRequestTypeDef = TypedDict(
-    "_RequiredSimulationJobRequestTypeDef",
-    {
-        "maxJobDurationInSeconds": int,
-    },
-)
-_OptionalSimulationJobRequestTypeDef = TypedDict(
-    "_OptionalSimulationJobRequestTypeDef",
-    {
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
-        "iamRole": str,
-        "failureBehavior": FailureBehaviorType,
-        "useDefaultApplications": bool,
-        "robotApplications": Sequence[RobotApplicationConfigTypeDef],
-        "simulationApplications": Sequence[SimulationApplicationConfigTypeDef],
-        "dataSources": Sequence[DataSourceConfigTypeDef],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class SimulationJobRequestTypeDef(
-    _RequiredSimulationJobRequestTypeDef, _OptionalSimulationJobRequestTypeDef
-):
-    pass
-
 FailedCreateSimulationJobRequestTypeDef = TypedDict(
     "FailedCreateSimulationJobRequestTypeDef",
     {
-        "request": SimulationJobRequestOutputTypeDef,
+        "request": SimulationJobRequestTypeDef,
         "failureReason": str,
         "failureCode": SimulationJobErrorCodeType,
         "failedAt": datetime,
     },
     total=False,
 )
 
-BatchDescribeSimulationJobResponseTypeDef = TypedDict(
-    "BatchDescribeSimulationJobResponseTypeDef",
-    {
-        "jobs": List[SimulationJobTypeDef],
-        "unprocessedJobs": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSimulationJobRequestRequestTypeDef",
+_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
     {
-        "maxJobDurationInSeconds": int,
-        "iamRole": str,
+        "createSimulationJobRequests": Sequence[SimulationJobRequestTypeDef],
     },
 )
-_OptionalCreateSimulationJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSimulationJobRequestRequestTypeDef",
+_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
+    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
     {
         "clientRequestToken": str,
-        "outputLocation": OutputLocationTypeDef,
-        "loggingConfig": LoggingConfigTypeDef,
-        "failureBehavior": FailureBehaviorType,
-        "robotApplications": Sequence[RobotApplicationConfigUnionTypeDef],
-        "simulationApplications": Sequence[SimulationApplicationConfigUnionTypeDef],
-        "dataSources": Sequence[DataSourceConfigUnionTypeDef],
+        "batchPolicy": BatchPolicyTypeDef,
         "tags": Mapping[str, str],
-        "vpcConfig": VPCConfigTypeDef,
-        "compute": ComputeTypeDef,
     },
     total=False,
 )
 
-class CreateSimulationJobRequestRequestTypeDef(
-    _RequiredCreateSimulationJobRequestRequestTypeDef,
-    _OptionalCreateSimulationJobRequestRequestTypeDef,
+class StartSimulationJobBatchRequestRequestTypeDef(
+    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
+    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
 ):
     pass
 
-SimulationJobRequestUnionTypeDef = Union[
-    SimulationJobRequestTypeDef, SimulationJobRequestOutputTypeDef
-]
+BatchDescribeSimulationJobResponseTypeDef = TypedDict(
+    "BatchDescribeSimulationJobResponseTypeDef",
+    {
+        "jobs": List[SimulationJobTypeDef],
+        "unprocessedJobs": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeSimulationJobBatchResponseTypeDef = TypedDict(
     "DescribeSimulationJobBatchResponseTypeDef",
     {
         "arn": str,
         "status": SimulationJobBatchStatusType,
         "lastUpdatedAt": datetime,
         "createdAt": datetime,
         "clientRequestToken": str,
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
+        "pendingRequests": List[SimulationJobRequestTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSimulationJobBatchResponseTypeDef = TypedDict(
@@ -2481,35 +2303,13 @@
         "status": SimulationJobBatchStatusType,
         "createdAt": datetime,
         "clientRequestToken": str,
         "batchPolicy": BatchPolicyTypeDef,
         "failureCode": Literal["InternalServiceError"],
         "failureReason": str,
         "failedRequests": List[FailedCreateSimulationJobRequestTypeDef],
-        "pendingRequests": List[SimulationJobRequestOutputTypeDef],
+        "pendingRequests": List[SimulationJobRequestTypeDef],
         "createdRequests": List[SimulationJobSummaryTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_RequiredStartSimulationJobBatchRequestRequestTypeDef",
-    {
-        "createSimulationJobRequests": Sequence[SimulationJobRequestUnionTypeDef],
-    },
-)
-_OptionalStartSimulationJobBatchRequestRequestTypeDef = TypedDict(
-    "_OptionalStartSimulationJobBatchRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-        "batchPolicy": BatchPolicyTypeDef,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class StartSimulationJobBatchRequestRequestTypeDef(
-    _RequiredStartSimulationJobBatchRequestRequestTypeDef,
-    _OptionalStartSimulationJobBatchRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-robomaker-2.5.2.post1/types_aiobotocore_robomaker.egg-info/SOURCES.txt` & `types-aiobotocore-robomaker-2.5.2.post2/types_aiobotocore_robomaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

