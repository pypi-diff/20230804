# Comparing `tmp/types-aiobotocore-sagemaker-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sagemaker-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-2.5.2.post1.tar` & `types-aiobotocore-sagemaker-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.513468 types-aiobotocore-sagemaker-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:38.000000 types-aiobotocore-sagemaker-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    88265 2023-08-02 14:52:57.513468 types-aiobotocore-sagemaker-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    86739 2023-08-02 14:48:38.000000 types-aiobotocore-sagemaker-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:57.513468 types-aiobotocore-sagemaker-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:48:38.000000 types-aiobotocore-sagemaker-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.509467 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-08-02 14:48:38.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18581 2023-08-02 14:48:38.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:48:38.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   272360 2023-08-02 14:48:40.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   271968 2023-08-02 14:48:39.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    56576 2023-08-02 14:48:45.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    56574 2023-08-02 14:48:44.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   100004 2023-08-02 14:48:41.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    99933 2023-08-02 14:48:41.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:38.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   552288 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   551571 2023-08-02 14:48:50.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:38.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14121 2023-08-02 14:48:41.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-02 14:48:41.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.513468 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    88265 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.086643 types-aiobotocore-sagemaker-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26500 2023-08-04 13:59:25.086643 types-aiobotocore-sagemaker-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24974 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.086643 types-aiobotocore-sagemaker-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.076643 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18810 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18809 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   274298 2023-08-04 13:52:02.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   273903 2023-08-04 13:52:01.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    58126 2023-08-04 13:52:05.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    58124 2023-08-04 13:52:04.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   101540 2023-08-04 13:52:03.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   101468 2023-08-04 13:52:03.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   500242 2023-08-04 13:52:22.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   499609 2023-08-04 13:52:13.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:56.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14121 2023-08-04 13:52:03.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14108 2023-08-04 13:52:03.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.086643 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26500 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:59:25.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/LICENSE` & `types-aiobotocore-sagemaker-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/setup.py` & `types-aiobotocore-sagemaker-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sagemaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SageMaker 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/__init__.py` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         ListNotebookInstanceLifecycleConfigsPaginator,
         ListNotebookInstancesPaginator,
         ListPipelineExecutionStepsPaginator,
         ListPipelineExecutionsPaginator,
         ListPipelineParametersForExecutionPaginator,
         ListPipelinesPaginator,
         ListProcessingJobsPaginator,
+        ListResourceCatalogsPaginator,
         ListSpacesPaginator,
         ListStageDevicesPaginator,
         ListStudioLifecycleConfigsPaginator,
         ListSubscribedWorkteamsPaginator,
         ListTagsPaginator,
         ListTrainingJobsForHyperParameterTuningJobPaginator,
         ListTrainingJobsPaginator,
@@ -161,14 +162,15 @@
     list_notebook_instance_lifecycle_configs_paginator: ListNotebookInstanceLifecycleConfigsPaginator = client.get_paginator("list_notebook_instance_lifecycle_configs")
     list_notebook_instances_paginator: ListNotebookInstancesPaginator = client.get_paginator("list_notebook_instances")
     list_pipeline_execution_steps_paginator: ListPipelineExecutionStepsPaginator = client.get_paginator("list_pipeline_execution_steps")
     list_pipeline_executions_paginator: ListPipelineExecutionsPaginator = client.get_paginator("list_pipeline_executions")
     list_pipeline_parameters_for_execution_paginator: ListPipelineParametersForExecutionPaginator = client.get_paginator("list_pipeline_parameters_for_execution")
     list_pipelines_paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
     list_processing_jobs_paginator: ListProcessingJobsPaginator = client.get_paginator("list_processing_jobs")
+    list_resource_catalogs_paginator: ListResourceCatalogsPaginator = client.get_paginator("list_resource_catalogs")
     list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
     list_stage_devices_paginator: ListStageDevicesPaginator = client.get_paginator("list_stage_devices")
     list_studio_lifecycle_configs_paginator: ListStudioLifecycleConfigsPaginator = client.get_paginator("list_studio_lifecycle_configs")
     list_subscribed_workteams_paginator: ListSubscribedWorkteamsPaginator = client.get_paginator("list_subscribed_workteams")
     list_tags_paginator: ListTagsPaginator = client.get_paginator("list_tags")
     list_training_jobs_paginator: ListTrainingJobsPaginator = client.get_paginator("list_training_jobs")
     list_training_jobs_for_hyper_parameter_tuning_job_paginator: ListTrainingJobsForHyperParameterTuningJobPaginator = client.get_paginator("list_training_jobs_for_hyper_parameter_tuning_job")
@@ -233,14 +235,15 @@
     ListNotebookInstanceLifecycleConfigsPaginator,
     ListNotebookInstancesPaginator,
     ListPipelineExecutionsPaginator,
     ListPipelineExecutionStepsPaginator,
     ListPipelineParametersForExecutionPaginator,
     ListPipelinesPaginator,
     ListProcessingJobsPaginator,
+    ListResourceCatalogsPaginator,
     ListSpacesPaginator,
     ListStageDevicesPaginator,
     ListStudioLifecycleConfigsPaginator,
     ListSubscribedWorkteamsPaginator,
     ListTagsPaginator,
     ListTrainingJobsForHyperParameterTuningJobPaginator,
     ListTrainingJobsPaginator,
@@ -330,14 +333,15 @@
     "ListNotebookInstanceLifecycleConfigsPaginator",
     "ListNotebookInstancesPaginator",
     "ListPipelineExecutionStepsPaginator",
     "ListPipelineExecutionsPaginator",
     "ListPipelineParametersForExecutionPaginator",
     "ListPipelinesPaginator",
     "ListProcessingJobsPaginator",
+    "ListResourceCatalogsPaginator",
     "ListSpacesPaginator",
     "ListStageDevicesPaginator",
     "ListStudioLifecycleConfigsPaginator",
     "ListSubscribedWorkteamsPaginator",
     "ListTagsPaginator",
     "ListTrainingJobsForHyperParameterTuningJobPaginator",
     "ListTrainingJobsPaginator",
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/__init__.pyi` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
         ListNotebookInstanceLifecycleConfigsPaginator,
         ListNotebookInstancesPaginator,
         ListPipelineExecutionStepsPaginator,
         ListPipelineExecutionsPaginator,
         ListPipelineParametersForExecutionPaginator,
         ListPipelinesPaginator,
         ListProcessingJobsPaginator,
+        ListResourceCatalogsPaginator,
         ListSpacesPaginator,
         ListStageDevicesPaginator,
         ListStudioLifecycleConfigsPaginator,
         ListSubscribedWorkteamsPaginator,
         ListTagsPaginator,
         ListTrainingJobsForHyperParameterTuningJobPaginator,
         ListTrainingJobsPaginator,
@@ -161,14 +162,15 @@
     list_notebook_instance_lifecycle_configs_paginator: ListNotebookInstanceLifecycleConfigsPaginator = client.get_paginator("list_notebook_instance_lifecycle_configs")
     list_notebook_instances_paginator: ListNotebookInstancesPaginator = client.get_paginator("list_notebook_instances")
     list_pipeline_execution_steps_paginator: ListPipelineExecutionStepsPaginator = client.get_paginator("list_pipeline_execution_steps")
     list_pipeline_executions_paginator: ListPipelineExecutionsPaginator = client.get_paginator("list_pipeline_executions")
     list_pipeline_parameters_for_execution_paginator: ListPipelineParametersForExecutionPaginator = client.get_paginator("list_pipeline_parameters_for_execution")
     list_pipelines_paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
     list_processing_jobs_paginator: ListProcessingJobsPaginator = client.get_paginator("list_processing_jobs")
+    list_resource_catalogs_paginator: ListResourceCatalogsPaginator = client.get_paginator("list_resource_catalogs")
     list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
     list_stage_devices_paginator: ListStageDevicesPaginator = client.get_paginator("list_stage_devices")
     list_studio_lifecycle_configs_paginator: ListStudioLifecycleConfigsPaginator = client.get_paginator("list_studio_lifecycle_configs")
     list_subscribed_workteams_paginator: ListSubscribedWorkteamsPaginator = client.get_paginator("list_subscribed_workteams")
     list_tags_paginator: ListTagsPaginator = client.get_paginator("list_tags")
     list_training_jobs_paginator: ListTrainingJobsPaginator = client.get_paginator("list_training_jobs")
     list_training_jobs_for_hyper_parameter_tuning_job_paginator: ListTrainingJobsForHyperParameterTuningJobPaginator = client.get_paginator("list_training_jobs_for_hyper_parameter_tuning_job")
@@ -233,14 +235,15 @@
     ListNotebookInstanceLifecycleConfigsPaginator,
     ListNotebookInstancesPaginator,
     ListPipelineExecutionsPaginator,
     ListPipelineExecutionStepsPaginator,
     ListPipelineParametersForExecutionPaginator,
     ListPipelinesPaginator,
     ListProcessingJobsPaginator,
+    ListResourceCatalogsPaginator,
     ListSpacesPaginator,
     ListStageDevicesPaginator,
     ListStudioLifecycleConfigsPaginator,
     ListSubscribedWorkteamsPaginator,
     ListTagsPaginator,
     ListTrainingJobsForHyperParameterTuningJobPaginator,
     ListTrainingJobsPaginator,
@@ -329,14 +332,15 @@
     "ListNotebookInstanceLifecycleConfigsPaginator",
     "ListNotebookInstancesPaginator",
     "ListPipelineExecutionStepsPaginator",
     "ListPipelineExecutionsPaginator",
     "ListPipelineParametersForExecutionPaginator",
     "ListPipelinesPaginator",
     "ListProcessingJobsPaginator",
+    "ListResourceCatalogsPaginator",
     "ListSpacesPaginator",
     "ListStageDevicesPaginator",
     "ListStudioLifecycleConfigsPaginator",
     "ListSubscribedWorkteamsPaginator",
     "ListTagsPaginator",
     "ListTrainingJobsForHyperParameterTuningJobPaginator",
     "ListTrainingJobsPaginator",
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/__main__.py` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SageMaker 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SageMaker 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker\nOther"
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

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/client.py` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     AutoMLSortOrderType,
     BatchStrategyType,
     CandidateSortByType,
     CandidateStatusType,
     CodeRepositorySortByType,
     CodeRepositorySortOrderType,
     CompilationJobStatusType,
+    CrossAccountFilterOptionType,
     DirectInternetAccessType,
     DirectionType,
     EdgePackagingJobStatusType,
     EndpointConfigSortKeyType,
     EndpointSortKeyType,
     EndpointStatusType,
     ExecutionStatusType,
@@ -98,14 +99,15 @@
     ProblemTypeType,
     ProcessingJobStatusType,
     ProcessorType,
     ProjectSortByType,
     ProjectSortOrderType,
     RecommendationJobStatusType,
     RecommendationJobTypeType,
+    ResourceCatalogSortOrderType,
     ResourceTypeType,
     RootAccessType,
     ScheduleStatusType,
     SearchSortOrderType,
     SortActionsByType,
     SortAssociationsByType,
     SortByType,
@@ -179,14 +181,15 @@
     ListNotebookInstanceLifecycleConfigsPaginator,
     ListNotebookInstancesPaginator,
     ListPipelineExecutionsPaginator,
     ListPipelineExecutionStepsPaginator,
     ListPipelineParametersForExecutionPaginator,
     ListPipelinesPaginator,
     ListProcessingJobsPaginator,
+    ListResourceCatalogsPaginator,
     ListSpacesPaginator,
     ListStageDevicesPaginator,
     ListStudioLifecycleConfigsPaginator,
     ListSubscribedWorkteamsPaginator,
     ListTagsPaginator,
     ListTrainingJobsForHyperParameterTuningJobPaginator,
     ListTrainingJobsPaginator,
@@ -197,37 +200,37 @@
     ListWorkforcesPaginator,
     ListWorkteamsPaginator,
     SearchPaginator,
 )
 from .type_defs import (
     ActionSourceTypeDef,
     AddAssociationResponseTypeDef,
-    AdditionalInferenceSpecificationDefinitionUnionTypeDef,
+    AdditionalInferenceSpecificationDefinitionTypeDef,
     AddTagsOutputTypeDef,
-    AlgorithmSpecificationUnionTypeDef,
-    AlgorithmValidationSpecificationUnionTypeDef,
-    AppSpecificationUnionTypeDef,
-    ArtifactSourceUnionTypeDef,
+    AlgorithmSpecificationTypeDef,
+    AlgorithmValidationSpecificationTypeDef,
+    AppSpecificationTypeDef,
+    ArtifactSourceTypeDef,
     AssociateTrialComponentResponseTypeDef,
-    AsyncInferenceConfigUnionTypeDef,
+    AsyncInferenceConfigTypeDef,
     AutoMLChannelTypeDef,
     AutoMLDataSplitConfigTypeDef,
     AutoMLJobChannelTypeDef,
-    AutoMLJobConfigUnionTypeDef,
+    AutoMLJobConfigTypeDef,
     AutoMLJobObjectiveTypeDef,
     AutoMLOutputDataConfigTypeDef,
-    AutoMLProblemTypeConfigUnionTypeDef,
-    AutoMLSecurityConfigUnionTypeDef,
+    AutoMLProblemTypeConfigTypeDef,
+    AutoMLSecurityConfigTypeDef,
     AutotuneTypeDef,
     BatchDataCaptureConfigTypeDef,
     BatchDescribeModelPackageOutputTypeDef,
-    ChannelUnionTypeDef,
+    ChannelTypeDef,
     CheckpointConfigTypeDef,
     CognitoConfigTypeDef,
-    ContainerDefinitionUnionTypeDef,
+    ContainerDefinitionTypeDef,
     ContextSourceTypeDef,
     CreateActionResponseTypeDef,
     CreateAlgorithmOutputTypeDef,
     CreateAppImageConfigResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateArtifactResponseTypeDef,
     CreateAutoMLJobResponseTypeDef,
@@ -272,33 +275,33 @@
     CreateTrainingJobResponseTypeDef,
     CreateTransformJobResponseTypeDef,
     CreateTrialComponentResponseTypeDef,
     CreateTrialResponseTypeDef,
     CreateUserProfileResponseTypeDef,
     CreateWorkforceResponseTypeDef,
     CreateWorkteamResponseTypeDef,
-    DataCaptureConfigUnionTypeDef,
+    DataCaptureConfigTypeDef,
     DataProcessingTypeDef,
-    DataQualityAppSpecificationUnionTypeDef,
+    DataQualityAppSpecificationTypeDef,
     DataQualityBaselineConfigTypeDef,
-    DataQualityJobInputUnionTypeDef,
-    DebugHookConfigUnionTypeDef,
-    DebugRuleConfigurationUnionTypeDef,
-    DefaultSpaceSettingsUnionTypeDef,
+    DataQualityJobInputTypeDef,
+    DebugHookConfigTypeDef,
+    DebugRuleConfigurationTypeDef,
+    DefaultSpaceSettingsTypeDef,
     DeleteActionResponseTypeDef,
     DeleteArtifactResponseTypeDef,
     DeleteAssociationResponseTypeDef,
     DeleteContextResponseTypeDef,
     DeleteExperimentResponseTypeDef,
     DeleteInferenceExperimentResponseTypeDef,
     DeletePipelineResponseTypeDef,
     DeleteTrialComponentResponseTypeDef,
     DeleteTrialResponseTypeDef,
     DeleteWorkteamResponseTypeDef,
-    DeploymentConfigUnionTypeDef,
+    DeploymentConfigTypeDef,
     DeploymentStageTypeDef,
     DescribeActionResponseTypeDef,
     DescribeAlgorithmOutputTypeDef,
     DescribeAppImageConfigResponseTypeDef,
     DescribeAppResponseTypeDef,
     DescribeArtifactResponseTypeDef,
     DescribeAutoMLJobResponseTypeDef,
@@ -354,49 +357,50 @@
     DescribeUserProfileResponseTypeDef,
     DescribeWorkforceResponseTypeDef,
     DescribeWorkteamResponseTypeDef,
     DesiredWeightAndCapacityTypeDef,
     DeviceTypeDef,
     DisassociateTrialComponentResponseTypeDef,
     DomainSettingsForUpdateTypeDef,
-    DomainSettingsUnionTypeDef,
+    DomainSettingsTypeDef,
     DriftCheckBaselinesTypeDef,
     EdgeDeploymentModelConfigTypeDef,
     EdgeOutputConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     ExperimentConfigTypeDef,
-    ExplainerConfigUnionTypeDef,
+    ExplainerConfigTypeDef,
     FeatureDefinitionTypeDef,
     FeatureParameterTypeDef,
     FlowDefinitionOutputConfigTypeDef,
     GetDeviceFleetReportResponseTypeDef,
     GetLineageGroupPolicyResponseTypeDef,
     GetModelPackageGroupPolicyOutputTypeDef,
     GetSagemakerServicecatalogPortfolioStatusOutputTypeDef,
+    GetScalingConfigurationRecommendationResponseTypeDef,
     GetSearchSuggestionsResponseTypeDef,
     GitConfigForUpdateTypeDef,
     GitConfigTypeDef,
     HubS3StorageConfigTypeDef,
     HumanLoopActivationConfigTypeDef,
-    HumanLoopConfigUnionTypeDef,
+    HumanLoopConfigTypeDef,
     HumanLoopRequestSourceTypeDef,
-    HumanTaskConfigUnionTypeDef,
-    HyperParameterTrainingJobDefinitionUnionTypeDef,
-    HyperParameterTuningJobConfigUnionTypeDef,
-    HyperParameterTuningJobWarmStartConfigUnionTypeDef,
+    HumanTaskConfigTypeDef,
+    HyperParameterTrainingJobDefinitionTypeDef,
+    HyperParameterTuningJobConfigTypeDef,
+    HyperParameterTuningJobWarmStartConfigTypeDef,
     ImportHubContentResponseTypeDef,
     InferenceExecutionConfigTypeDef,
-    InferenceExperimentDataStorageConfigUnionTypeDef,
-    InferenceExperimentScheduleUnionTypeDef,
-    InferenceSpecificationUnionTypeDef,
+    InferenceExperimentDataStorageConfigTypeDef,
+    InferenceExperimentScheduleTypeDef,
+    InferenceSpecificationTypeDef,
     InputConfigTypeDef,
     InstanceMetadataServiceConfigurationTypeDef,
-    KernelGatewayImageConfigUnionTypeDef,
-    LabelingJobAlgorithmsConfigUnionTypeDef,
-    LabelingJobInputConfigUnionTypeDef,
+    KernelGatewayImageConfigTypeDef,
+    LabelingJobAlgorithmsConfigTypeDef,
+    LabelingJobInputConfigTypeDef,
     LabelingJobOutputConfigTypeDef,
     LabelingJobStoppingConditionsTypeDef,
     ListActionsResponseTypeDef,
     ListAlgorithmsOutputTypeDef,
     ListAliasesResponseTypeDef,
     ListAppImageConfigsResponseTypeDef,
     ListAppsResponseTypeDef,
@@ -449,107 +453,110 @@
     ListNotebookInstancesOutputTypeDef,
     ListPipelineExecutionsResponseTypeDef,
     ListPipelineExecutionStepsResponseTypeDef,
     ListPipelineParametersForExecutionResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListProcessingJobsResponseTypeDef,
     ListProjectsOutputTypeDef,
+    ListResourceCatalogsResponseTypeDef,
     ListSpacesResponseTypeDef,
     ListStageDevicesResponseTypeDef,
     ListStudioLifecycleConfigsResponseTypeDef,
     ListSubscribedWorkteamsResponseTypeDef,
     ListTagsOutputTypeDef,
     ListTrainingJobsForHyperParameterTuningJobResponseTypeDef,
     ListTrainingJobsResponseTypeDef,
     ListTransformJobsResponseTypeDef,
     ListTrialComponentsResponseTypeDef,
     ListTrialsResponseTypeDef,
     ListUserProfilesResponseTypeDef,
     ListWorkforcesResponseTypeDef,
     ListWorkteamsResponseTypeDef,
-    MemberDefinitionUnionTypeDef,
+    MemberDefinitionTypeDef,
     MetadataPropertiesTypeDef,
-    ModelBiasAppSpecificationUnionTypeDef,
+    ModelBiasAppSpecificationTypeDef,
     ModelBiasBaselineConfigTypeDef,
-    ModelBiasJobInputUnionTypeDef,
+    ModelBiasJobInputTypeDef,
     ModelCardExportOutputConfigTypeDef,
     ModelCardSecurityConfigTypeDef,
     ModelClientConfigTypeDef,
     ModelDeployConfigTypeDef,
-    ModelExplainabilityAppSpecificationUnionTypeDef,
+    ModelExplainabilityAppSpecificationTypeDef,
     ModelExplainabilityBaselineConfigTypeDef,
-    ModelExplainabilityJobInputUnionTypeDef,
+    ModelExplainabilityJobInputTypeDef,
     ModelMetadataSearchExpressionTypeDef,
     ModelMetricsTypeDef,
-    ModelPackageValidationSpecificationUnionTypeDef,
-    ModelQualityAppSpecificationUnionTypeDef,
+    ModelPackageValidationSpecificationTypeDef,
+    ModelQualityAppSpecificationTypeDef,
     ModelQualityBaselineConfigTypeDef,
-    ModelQualityJobInputUnionTypeDef,
+    ModelQualityJobInputTypeDef,
     ModelVariantConfigTypeDef,
-    MonitoringNetworkConfigUnionTypeDef,
-    MonitoringOutputConfigUnionTypeDef,
+    MonitoringNetworkConfigTypeDef,
+    MonitoringOutputConfigTypeDef,
     MonitoringResourcesTypeDef,
-    MonitoringScheduleConfigUnionTypeDef,
+    MonitoringScheduleConfigTypeDef,
     MonitoringStoppingConditionTypeDef,
-    NeoVpcConfigUnionTypeDef,
-    NetworkConfigUnionTypeDef,
+    NeoVpcConfigTypeDef,
+    NetworkConfigTypeDef,
     NotebookInstanceLifecycleHookTypeDef,
     NotificationConfigurationTypeDef,
     OfflineStoreConfigTypeDef,
     OidcConfigTypeDef,
     OnlineStoreConfigTypeDef,
+    OnlineStoreConfigUpdateTypeDef,
     OutputConfigTypeDef,
     OutputDataConfigTypeDef,
     OutputParameterTypeDef,
     ParallelismConfigurationTypeDef,
     ParameterTypeDef,
     PipelineDefinitionS3LocationTypeDef,
     ProcessingInputTypeDef,
-    ProcessingOutputConfigUnionTypeDef,
+    ProcessingOutputConfigTypeDef,
     ProcessingResourcesTypeDef,
     ProcessingStoppingConditionTypeDef,
     ProductionVariantTypeDef,
     ProfilerConfigForUpdateTypeDef,
-    ProfilerConfigUnionTypeDef,
-    ProfilerRuleConfigurationUnionTypeDef,
+    ProfilerConfigTypeDef,
+    ProfilerRuleConfigurationTypeDef,
     PutModelPackageGroupPolicyOutputTypeDef,
     QueryFiltersTypeDef,
     QueryLineageResponseTypeDef,
-    RecommendationJobInputConfigUnionTypeDef,
+    RecommendationJobInputConfigTypeDef,
     RecommendationJobOutputConfigTypeDef,
-    RecommendationJobStoppingConditionsUnionTypeDef,
+    RecommendationJobStoppingConditionsTypeDef,
     RenderableTaskTypeDef,
     RenderUiTemplateResponseTypeDef,
     ResourceConfigForUpdateTypeDef,
-    ResourceConfigUnionTypeDef,
+    ResourceConfigTypeDef,
     ResourceSpecTypeDef,
     RetentionPolicyTypeDef,
     RetryPipelineExecutionResponseTypeDef,
     RetryStrategyTypeDef,
+    ScalingPolicyObjectiveTypeDef,
     SearchExpressionTypeDef,
     SearchResponseTypeDef,
-    SelectiveExecutionConfigUnionTypeDef,
+    SelectiveExecutionConfigTypeDef,
     SendPipelineExecutionStepFailureResponseTypeDef,
     SendPipelineExecutionStepSuccessResponseTypeDef,
-    ServiceCatalogProvisioningDetailsUnionTypeDef,
+    ServiceCatalogProvisioningDetailsTypeDef,
     ServiceCatalogProvisioningUpdateDetailsTypeDef,
-    ShadowModeConfigUnionTypeDef,
-    SourceAlgorithmSpecificationUnionTypeDef,
-    SourceIpConfigUnionTypeDef,
-    SpaceSettingsUnionTypeDef,
+    ShadowModeConfigTypeDef,
+    SourceAlgorithmSpecificationTypeDef,
+    SourceIpConfigTypeDef,
+    SpaceSettingsTypeDef,
     StartInferenceExperimentResponseTypeDef,
     StartPipelineExecutionResponseTypeDef,
     StopInferenceExperimentResponseTypeDef,
     StoppingConditionTypeDef,
     StopPipelineExecutionResponseTypeDef,
     SuggestionQueryTypeDef,
     TagTypeDef,
     TensorBoardOutputConfigTypeDef,
     TimestampTypeDef,
-    TrainingSpecificationUnionTypeDef,
+    TrainingSpecificationTypeDef,
     TransformInputTypeDef,
     TransformOutputTypeDef,
     TransformResourcesTypeDef,
     TrialComponentArtifactTypeDef,
     TrialComponentParameterValueTypeDef,
     TrialComponentStatusTypeDef,
     UiTemplateTypeDef,
@@ -577,17 +584,17 @@
     UpdateSpaceResponseTypeDef,
     UpdateTrainingJobResponseTypeDef,
     UpdateTrialComponentResponseTypeDef,
     UpdateTrialResponseTypeDef,
     UpdateUserProfileResponseTypeDef,
     UpdateWorkforceResponseTypeDef,
     UpdateWorkteamResponseTypeDef,
-    UserSettingsUnionTypeDef,
+    UserSettingsTypeDef,
     VariantPropertyTypeDef,
-    VpcConfigUnionTypeDef,
+    VpcConfigTypeDef,
     WorkforceVpcConfigRequestTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     EndpointInServiceWaiter,
     ImageCreatedWaiter,
     ImageDeletedWaiter,
@@ -721,18 +728,18 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_action)
         """
 
     async def create_algorithm(
         self,
         *,
         AlgorithmName: str,
-        TrainingSpecification: TrainingSpecificationUnionTypeDef,
+        TrainingSpecification: TrainingSpecificationTypeDef,
         AlgorithmDescription: str = ...,
-        InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,
-        ValidationSpecification: AlgorithmValidationSpecificationUnionTypeDef = ...,
+        InferenceSpecification: InferenceSpecificationTypeDef = ...,
+        ValidationSpecification: AlgorithmValidationSpecificationTypeDef = ...,
         CertifyForMarketplace: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateAlgorithmOutputTypeDef:
         """
         Create a machine learning algorithm that you can use in SageMaker and list in
         the Amazon Web Services Marketplace.
 
@@ -759,27 +766,27 @@
         """
 
     async def create_app_image_config(
         self,
         *,
         AppImageConfigName: str,
         Tags: Sequence[TagTypeDef] = ...,
-        KernelGatewayImageConfig: KernelGatewayImageConfigUnionTypeDef = ...
+        KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...
     ) -> CreateAppImageConfigResponseTypeDef:
         """
         Creates a configuration for running a SageMaker image as a KernelGateway app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_app_image_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_app_image_config)
         """
 
     async def create_artifact(
         self,
         *,
-        Source: ArtifactSourceUnionTypeDef,
+        Source: ArtifactSourceTypeDef,
         ArtifactType: str,
         ArtifactName: str = ...,
         Properties: Mapping[str, str] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateArtifactResponseTypeDef:
         """
@@ -794,15 +801,15 @@
         *,
         AutoMLJobName: str,
         InputDataConfig: Sequence[AutoMLChannelTypeDef],
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
         RoleArn: str,
         ProblemType: ProblemTypeType = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
-        AutoMLJobConfig: AutoMLJobConfigUnionTypeDef = ...,
+        AutoMLJobConfig: AutoMLJobConfigTypeDef = ...,
         GenerateCandidateDefinitionsOnly: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ModelDeployConfig: ModelDeployConfigTypeDef = ...
     ) -> CreateAutoMLJobResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job.
 
@@ -812,18 +819,18 @@
 
     async def create_auto_ml_job_v2(
         self,
         *,
         AutoMLJobName: str,
         AutoMLJobInputDataConfig: Sequence[AutoMLJobChannelTypeDef],
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
-        AutoMLProblemTypeConfig: AutoMLProblemTypeConfigUnionTypeDef,
+        AutoMLProblemTypeConfig: AutoMLProblemTypeConfigTypeDef,
         RoleArn: str,
         Tags: Sequence[TagTypeDef] = ...,
-        SecurityConfig: AutoMLSecurityConfigUnionTypeDef = ...,
+        SecurityConfig: AutoMLSecurityConfigTypeDef = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
         ModelDeployConfig: ModelDeployConfigTypeDef = ...,
         DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...
     ) -> CreateAutoMLJobV2ResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job
         V2.
@@ -851,15 +858,15 @@
         *,
         CompilationJobName: str,
         RoleArn: str,
         OutputConfig: OutputConfigTypeDef,
         StoppingCondition: StoppingConditionTypeDef,
         ModelPackageVersionArn: str = ...,
         InputConfig: InputConfigTypeDef = ...,
-        VpcConfig: NeoVpcConfigUnionTypeDef = ...,
+        VpcConfig: NeoVpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateCompilationJobResponseTypeDef:
         """
         Starts a model compilation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_compilation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_compilation_job)
@@ -882,21 +889,21 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_context)
         """
 
     async def create_data_quality_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        DataQualityAppSpecification: DataQualityAppSpecificationUnionTypeDef,
-        DataQualityJobInput: DataQualityJobInputUnionTypeDef,
-        DataQualityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
+        DataQualityAppSpecification: DataQualityAppSpecificationTypeDef,
+        DataQualityJobInput: DataQualityJobInputTypeDef,
+        DataQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         DataQualityBaselineConfig: DataQualityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors data quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_data_quality_job_definition)
@@ -921,24 +928,24 @@
         """
 
     async def create_domain(
         self,
         *,
         DomainName: str,
         AuthMode: AuthModeType,
-        DefaultUserSettings: UserSettingsUnionTypeDef,
+        DefaultUserSettings: UserSettingsTypeDef,
         SubnetIds: Sequence[str],
         VpcId: str,
         Tags: Sequence[TagTypeDef] = ...,
         AppNetworkAccessType: AppNetworkAccessTypeType = ...,
         HomeEfsFileSystemKmsKeyId: str = ...,
         KmsKeyId: str = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,
-        DomainSettings: DomainSettingsUnionTypeDef = ...,
-        DefaultSpaceSettings: DefaultSpaceSettingsUnionTypeDef = ...
+        DomainSettings: DomainSettingsTypeDef = ...,
+        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a `Domain` used by Amazon SageMaker Studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_domain)
         """
@@ -989,34 +996,34 @@
         """
 
     async def create_endpoint(
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
-        DeploymentConfig: DeploymentConfigUnionTypeDef = ...,
+        DeploymentConfig: DeploymentConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateEndpointOutputTypeDef:
         """
         Creates an endpoint using the endpoint configuration specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_endpoint)
         """
 
     async def create_endpoint_config(
         self,
         *,
         EndpointConfigName: str,
         ProductionVariants: Sequence[ProductionVariantTypeDef],
-        DataCaptureConfig: DataCaptureConfigUnionTypeDef = ...,
+        DataCaptureConfig: DataCaptureConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
-        AsyncInferenceConfig: AsyncInferenceConfigUnionTypeDef = ...,
-        ExplainerConfig: ExplainerConfigUnionTypeDef = ...,
+        AsyncInferenceConfig: AsyncInferenceConfigTypeDef = ...,
+        ExplainerConfig: ExplainerConfigTypeDef = ...,
         ShadowProductionVariants: Sequence[ProductionVariantTypeDef] = ...
     ) -> CreateEndpointConfigOutputTypeDef:
         """
         Creates an endpoint configuration that SageMaker hosting services uses to deploy
         models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint_config)
@@ -1058,15 +1065,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_feature_group)
         """
 
     async def create_flow_definition(
         self,
         *,
         FlowDefinitionName: str,
-        HumanLoopConfig: HumanLoopConfigUnionTypeDef,
+        HumanLoopConfig: HumanLoopConfigTypeDef,
         OutputConfig: FlowDefinitionOutputConfigTypeDef,
         RoleArn: str,
         HumanLoopRequestSource: HumanLoopRequestSourceTypeDef = ...,
         HumanLoopActivationConfig: HumanLoopActivationConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFlowDefinitionResponseTypeDef:
         """
@@ -1107,18 +1114,18 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_human_task_ui)
         """
 
     async def create_hyper_parameter_tuning_job(
         self,
         *,
         HyperParameterTuningJobName: str,
-        HyperParameterTuningJobConfig: HyperParameterTuningJobConfigUnionTypeDef,
-        TrainingJobDefinition: HyperParameterTrainingJobDefinitionUnionTypeDef = ...,
-        TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionUnionTypeDef] = ...,
-        WarmStartConfig: HyperParameterTuningJobWarmStartConfigUnionTypeDef = ...,
+        HyperParameterTuningJobConfig: HyperParameterTuningJobConfigTypeDef,
+        TrainingJobDefinition: HyperParameterTrainingJobDefinitionTypeDef = ...,
+        TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionTypeDef] = ...,
+        WarmStartConfig: HyperParameterTuningJobWarmStartConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Autotune: AutotuneTypeDef = ...
     ) -> CreateHyperParameterTuningJobResponseTypeDef:
         """
         Starts a hyperparameter tuning job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_hyper_parameter_tuning_job)
@@ -1167,18 +1174,18 @@
         self,
         *,
         Name: str,
         Type: Literal["ShadowMode"],
         RoleArn: str,
         EndpointName: str,
         ModelVariants: Sequence[ModelVariantConfigTypeDef],
-        ShadowModeConfig: ShadowModeConfigUnionTypeDef,
-        Schedule: InferenceExperimentScheduleUnionTypeDef = ...,
+        ShadowModeConfig: ShadowModeConfigTypeDef,
+        Schedule: InferenceExperimentScheduleTypeDef = ...,
         Description: str = ...,
-        DataStorageConfig: InferenceExperimentDataStorageConfigUnionTypeDef = ...,
+        DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
         KmsKey: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateInferenceExperimentResponseTypeDef:
         """
         Creates an inference experiment using the configurations specified in the
         request.
 
@@ -1188,17 +1195,17 @@
 
     async def create_inference_recommendations_job(
         self,
         *,
         JobName: str,
         JobType: RecommendationJobTypeType,
         RoleArn: str,
-        InputConfig: RecommendationJobInputConfigUnionTypeDef,
+        InputConfig: RecommendationJobInputConfigTypeDef,
         JobDescription: str = ...,
-        StoppingConditions: RecommendationJobStoppingConditionsUnionTypeDef = ...,
+        StoppingConditions: RecommendationJobStoppingConditionsTypeDef = ...,
         OutputConfig: RecommendationJobOutputConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateInferenceRecommendationsJobResponseTypeDef:
         """
         Starts a recommendation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_recommendations_job)
@@ -1206,60 +1213,60 @@
         """
 
     async def create_labeling_job(
         self,
         *,
         LabelingJobName: str,
         LabelAttributeName: str,
-        InputConfig: LabelingJobInputConfigUnionTypeDef,
+        InputConfig: LabelingJobInputConfigTypeDef,
         OutputConfig: LabelingJobOutputConfigTypeDef,
         RoleArn: str,
-        HumanTaskConfig: HumanTaskConfigUnionTypeDef,
+        HumanTaskConfig: HumanTaskConfigTypeDef,
         LabelCategoryConfigS3Uri: str = ...,
         StoppingConditions: LabelingJobStoppingConditionsTypeDef = ...,
-        LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigUnionTypeDef = ...,
+        LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateLabelingJobResponseTypeDef:
         """
         Creates a job that uses workers to label the data objects in your input dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_labeling_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_labeling_job)
         """
 
     async def create_model(
         self,
         *,
         ModelName: str,
         ExecutionRoleArn: str,
-        PrimaryContainer: ContainerDefinitionUnionTypeDef = ...,
-        Containers: Sequence[ContainerDefinitionUnionTypeDef] = ...,
+        PrimaryContainer: ContainerDefinitionTypeDef = ...,
+        Containers: Sequence[ContainerDefinitionTypeDef] = ...,
         InferenceExecutionConfig: InferenceExecutionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         EnableNetworkIsolation: bool = ...
     ) -> CreateModelOutputTypeDef:
         """
         Creates a model in SageMaker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model)
         """
 
     async def create_model_bias_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelBiasAppSpecification: ModelBiasAppSpecificationUnionTypeDef,
-        ModelBiasJobInput: ModelBiasJobInputUnionTypeDef,
-        ModelBiasJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
+        ModelBiasAppSpecification: ModelBiasAppSpecificationTypeDef,
+        ModelBiasJobInput: ModelBiasJobInputTypeDef,
+        ModelBiasJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelBiasBaselineConfig: ModelBiasBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelBiasJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model bias job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_bias_job_definition)
@@ -1297,21 +1304,21 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_card_export_job)
         """
 
     async def create_model_explainability_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationUnionTypeDef,
-        ModelExplainabilityJobInput: ModelExplainabilityJobInputUnionTypeDef,
-        ModelExplainabilityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
+        ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationTypeDef,
+        ModelExplainabilityJobInput: ModelExplainabilityJobInputTypeDef,
+        ModelExplainabilityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelExplainabilityBaselineConfig: ModelExplainabilityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelExplainabilityJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model explainability job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_explainability_job_definition)
@@ -1320,30 +1327,30 @@
 
     async def create_model_package(
         self,
         *,
         ModelPackageName: str = ...,
         ModelPackageGroupName: str = ...,
         ModelPackageDescription: str = ...,
-        InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,
-        ValidationSpecification: ModelPackageValidationSpecificationUnionTypeDef = ...,
-        SourceAlgorithmSpecification: SourceAlgorithmSpecificationUnionTypeDef = ...,
+        InferenceSpecification: InferenceSpecificationTypeDef = ...,
+        ValidationSpecification: ModelPackageValidationSpecificationTypeDef = ...,
+        SourceAlgorithmSpecification: SourceAlgorithmSpecificationTypeDef = ...,
         CertifyForMarketplace: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
         ModelMetrics: ModelMetricsTypeDef = ...,
         ClientToken: str = ...,
         CustomerMetadataProperties: Mapping[str, str] = ...,
         DriftCheckBaselines: DriftCheckBaselinesTypeDef = ...,
         Domain: str = ...,
         Task: str = ...,
         SamplePayloadUrl: str = ...,
         AdditionalInferenceSpecifications: Sequence[
-            AdditionalInferenceSpecificationDefinitionUnionTypeDef
+            AdditionalInferenceSpecificationDefinitionTypeDef
         ] = ...
     ) -> CreateModelPackageOutputTypeDef:
         """
         Creates a model package that you can use to create SageMaker models or list on
         Amazon Web Services Marketplace, or a versioned model that is part of a model
         group.
 
@@ -1365,36 +1372,36 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_package_group)
         """
 
     async def create_model_quality_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelQualityAppSpecification: ModelQualityAppSpecificationUnionTypeDef,
-        ModelQualityJobInput: ModelQualityJobInputUnionTypeDef,
-        ModelQualityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
+        ModelQualityAppSpecification: ModelQualityAppSpecificationTypeDef,
+        ModelQualityJobInput: ModelQualityJobInputTypeDef,
+        ModelQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelQualityBaselineConfig: ModelQualityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors model quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_quality_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_quality_job_definition)
         """
 
     async def create_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
-        MonitoringScheduleConfig: MonitoringScheduleConfigUnionTypeDef,
+        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMonitoringScheduleResponseTypeDef:
         """
         Creates a schedule that regularly starts Amazon SageMaker Processing Jobs to
         monitor the data captured for an Amazon SageMaker Endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_monitoring_schedule)
@@ -1491,36 +1498,36 @@
         """
 
     async def create_processing_job(
         self,
         *,
         ProcessingJobName: str,
         ProcessingResources: ProcessingResourcesTypeDef,
-        AppSpecification: AppSpecificationUnionTypeDef,
+        AppSpecification: AppSpecificationTypeDef,
         RoleArn: str,
         ProcessingInputs: Sequence[ProcessingInputTypeDef] = ...,
-        ProcessingOutputConfig: ProcessingOutputConfigUnionTypeDef = ...,
+        ProcessingOutputConfig: ProcessingOutputConfigTypeDef = ...,
         StoppingCondition: ProcessingStoppingConditionTypeDef = ...,
         Environment: Mapping[str, str] = ...,
-        NetworkConfig: NetworkConfigUnionTypeDef = ...,
+        NetworkConfig: NetworkConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ExperimentConfig: ExperimentConfigTypeDef = ...
     ) -> CreateProcessingJobResponseTypeDef:
         """
         Creates a processing job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_processing_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_processing_job)
         """
 
     async def create_project(
         self,
         *,
         ProjectName: str,
-        ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsUnionTypeDef,
+        ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsTypeDef,
         ProjectDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a machine learning (ML) project that can contain one or more templates
         that set up an ML pipeline from training to deploying an approved model.
 
@@ -1530,15 +1537,15 @@
 
     async def create_space(
         self,
         *,
         DomainId: str,
         SpaceName: str,
         Tags: Sequence[TagTypeDef] = ...,
-        SpaceSettings: SpaceSettingsUnionTypeDef = ...
+        SpaceSettings: SpaceSettingsTypeDef = ...
     ) -> CreateSpaceResponseTypeDef:
         """
         Creates a space used for real time collaboration in a Domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_space)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_space)
         """
@@ -1558,33 +1565,33 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_studio_lifecycle_config)
         """
 
     async def create_training_job(
         self,
         *,
         TrainingJobName: str,
-        AlgorithmSpecification: AlgorithmSpecificationUnionTypeDef,
+        AlgorithmSpecification: AlgorithmSpecificationTypeDef,
         RoleArn: str,
         OutputDataConfig: OutputDataConfigTypeDef,
-        ResourceConfig: ResourceConfigUnionTypeDef,
+        ResourceConfig: ResourceConfigTypeDef,
         StoppingCondition: StoppingConditionTypeDef,
         HyperParameters: Mapping[str, str] = ...,
-        InputDataConfig: Sequence[ChannelUnionTypeDef] = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        InputDataConfig: Sequence[ChannelTypeDef] = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EnableNetworkIsolation: bool = ...,
         EnableInterContainerTrafficEncryption: bool = ...,
         EnableManagedSpotTraining: bool = ...,
         CheckpointConfig: CheckpointConfigTypeDef = ...,
-        DebugHookConfig: DebugHookConfigUnionTypeDef = ...,
-        DebugRuleConfigurations: Sequence[DebugRuleConfigurationUnionTypeDef] = ...,
+        DebugHookConfig: DebugHookConfigTypeDef = ...,
+        DebugRuleConfigurations: Sequence[DebugRuleConfigurationTypeDef] = ...,
         TensorBoardOutputConfig: TensorBoardOutputConfigTypeDef = ...,
         ExperimentConfig: ExperimentConfigTypeDef = ...,
-        ProfilerConfig: ProfilerConfigUnionTypeDef = ...,
-        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationUnionTypeDef] = ...,
+        ProfilerConfig: ProfilerConfigTypeDef = ...,
+        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
         Environment: Mapping[str, str] = ...,
         RetryStrategy: RetryStrategyTypeDef = ...
     ) -> CreateTrainingJobResponseTypeDef:
         """
         Starts a model training job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_training_job)
@@ -1657,45 +1664,45 @@
         self,
         *,
         DomainId: str,
         UserProfileName: str,
         SingleSignOnUserIdentifier: str = ...,
         SingleSignOnUserValue: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        UserSettings: UserSettingsUnionTypeDef = ...
+        UserSettings: UserSettingsTypeDef = ...
     ) -> CreateUserProfileResponseTypeDef:
         """
         Creates a user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_user_profile)
         """
 
     async def create_workforce(
         self,
         *,
         WorkforceName: str,
         CognitoConfig: CognitoConfigTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
-        SourceIpConfig: SourceIpConfigUnionTypeDef = ...,
+        SourceIpConfig: SourceIpConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...
     ) -> CreateWorkforceResponseTypeDef:
         """
         Use this operation to create a workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_workforce)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_workforce)
         """
 
     async def create_workteam(
         self,
         *,
         WorkteamName: str,
-        MemberDefinitions: Sequence[MemberDefinitionUnionTypeDef],
+        MemberDefinitions: Sequence[MemberDefinitionTypeDef],
         Description: str,
         WorkforceName: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWorkteamResponseTypeDef:
         """
         Creates a new work team for labeling your data.
@@ -1743,15 +1750,15 @@
         Deletes an AppImageConfig.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_app_image_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#delete_app_image_config)
         """
 
     async def delete_artifact(
-        self, *, ArtifactArn: str = ..., Source: ArtifactSourceUnionTypeDef = ...
+        self, *, ArtifactArn: str = ..., Source: ArtifactSourceTypeDef = ...
     ) -> DeleteArtifactResponseTypeDef:
         """
         Deletes an artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#delete_artifact)
         """
@@ -2786,14 +2793,30 @@
         """
         Gets the status of Service Catalog in SageMaker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_sagemaker_servicecatalog_portfolio_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_sagemaker_servicecatalog_portfolio_status)
         """
 
+    async def get_scaling_configuration_recommendation(
+        self,
+        *,
+        InferenceRecommendationsJobName: str,
+        RecommendationId: str = ...,
+        EndpointName: str = ...,
+        TargetCpuUtilizationPerCore: int = ...,
+        ScalingPolicyObjective: ScalingPolicyObjectiveTypeDef = ...
+    ) -> GetScalingConfigurationRecommendationResponseTypeDef:
+        """
+        Starts an Amazon SageMaker Inference Recommender autoscaling recommendation job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_scaling_configuration_recommendation)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_scaling_configuration_recommendation)
+        """
+
     async def get_search_suggestions(
         self, *, Resource: ResourceTypeType, SuggestionQuery: SuggestionQueryTypeDef = ...
     ) -> GetSearchSuggestionsResponseTypeDef:
         """
         An auto-complete API for the search functionality in the SageMaker console.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_search_suggestions)
@@ -3924,14 +3947,32 @@
         """
         Gets a list of the projects in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_projects)
         """
 
+    async def list_resource_catalogs(
+        self,
+        *,
+        NameContains: str = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
+        SortOrder: ResourceCatalogSortOrderType = ...,
+        SortBy: Literal["CreationTime"] = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> ListResourceCatalogsResponseTypeDef:
+        """
+        Lists Amazon SageMaker Catalogs based on given filters and orders.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_resource_catalogs)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_resource_catalogs)
+        """
+
     async def list_spaces(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortOrder: SortOrderType = ...,
         SortBy: SpaceSortKeyType = ...,
@@ -4232,15 +4273,16 @@
         self,
         *,
         Resource: ResourceTypeType,
         SearchExpression: "SearchExpressionTypeDef" = ...,
         SortBy: str = ...,
         SortOrder: SearchSortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
+        CrossAccountFilterOption: CrossAccountFilterOptionType = ...
     ) -> SearchResponseTypeDef:
         """
         Finds SageMaker resources that match a search query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#search)
         """
@@ -4317,15 +4359,15 @@
         *,
         PipelineName: str,
         ClientRequestToken: str,
         PipelineExecutionDisplayName: str = ...,
         PipelineParameters: Sequence[ParameterTypeDef] = ...,
         PipelineExecutionDescription: str = ...,
         ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
-        SelectiveExecutionConfig: SelectiveExecutionConfigUnionTypeDef = ...
+        SelectiveExecutionConfig: SelectiveExecutionConfigTypeDef = ...
     ) -> StartPipelineExecutionResponseTypeDef:
         """
         Starts a pipeline execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.start_pipeline_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#start_pipeline_execution)
         """
@@ -4483,15 +4525,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_action)
         """
 
     async def update_app_image_config(
         self,
         *,
         AppImageConfigName: str,
-        KernelGatewayImageConfig: KernelGatewayImageConfigUnionTypeDef = ...
+        KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...
     ) -> UpdateAppImageConfigResponseTypeDef:
         """
         Updates the properties of an AppImageConfig.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_app_image_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_app_image_config)
         """
@@ -4562,17 +4604,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_devices)
         """
 
     async def update_domain(
         self,
         *,
         DomainId: str,
-        DefaultUserSettings: UserSettingsUnionTypeDef = ...,
+        DefaultUserSettings: UserSettingsTypeDef = ...,
         DomainSettingsForUpdate: DomainSettingsForUpdateTypeDef = ...,
-        DefaultSpaceSettings: DefaultSpaceSettingsUnionTypeDef = ...,
+        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the default settings for new user profiles in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_domain)
@@ -4581,15 +4623,15 @@
     async def update_endpoint(
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
         RetainAllVariantProperties: bool = ...,
         ExcludeRetainedVariantProperties: Sequence[VariantPropertyTypeDef] = ...,
-        DeploymentConfig: DeploymentConfigUnionTypeDef = ...,
+        DeploymentConfig: DeploymentConfigTypeDef = ...,
         RetainDeploymentConfig: bool = ...
     ) -> UpdateEndpointOutputTypeDef:
         """
         Deploys the new `EndpointConfig` specified in the request, switches to using
         newly created endpoint, and then deletes resources provisioned for the endpoint
         using the previous `EndpointConfig` (there is no availability loss).
 
@@ -4618,18 +4660,23 @@
         Adds, updates, or removes the description of an experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_experiment)
         """
 
     async def update_feature_group(
-        self, *, FeatureGroupName: str, FeatureAdditions: Sequence[FeatureDefinitionTypeDef] = ...
+        self,
+        *,
+        FeatureGroupName: str,
+        FeatureAdditions: Sequence[FeatureDefinitionTypeDef] = ...,
+        OnlineStoreConfig: OnlineStoreConfigUpdateTypeDef = ...
     ) -> UpdateFeatureGroupResponseTypeDef:
         """
-        Updates the feature group.
+        Updates the feature group by either adding features or updating the online store
+        configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_feature_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_feature_group)
         """
 
     async def update_feature_metadata(
         self,
@@ -4701,19 +4748,19 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_image_version)
         """
 
     async def update_inference_experiment(
         self,
         *,
         Name: str,
-        Schedule: InferenceExperimentScheduleUnionTypeDef = ...,
+        Schedule: InferenceExperimentScheduleTypeDef = ...,
         Description: str = ...,
         ModelVariants: Sequence[ModelVariantConfigTypeDef] = ...,
-        DataStorageConfig: InferenceExperimentDataStorageConfigUnionTypeDef = ...,
-        ShadowModeConfig: ShadowModeConfigUnionTypeDef = ...
+        DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
+        ShadowModeConfig: ShadowModeConfigTypeDef = ...
     ) -> UpdateInferenceExperimentResponseTypeDef:
         """
         Updates an inference experiment that you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_inference_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_inference_experiment)
         """
@@ -4733,15 +4780,15 @@
         *,
         ModelPackageArn: str,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         ApprovalDescription: str = ...,
         CustomerMetadataProperties: Mapping[str, str] = ...,
         CustomerMetadataPropertiesToRemove: Sequence[str] = ...,
         AdditionalInferenceSpecificationsToAdd: Sequence[
-            AdditionalInferenceSpecificationDefinitionUnionTypeDef
+            AdditionalInferenceSpecificationDefinitionTypeDef
         ] = ...
     ) -> UpdateModelPackageOutputTypeDef:
         """
         Updates a versioned model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_model_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_model_package)
@@ -4762,15 +4809,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_monitoring_alert)
         """
 
     async def update_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
-        MonitoringScheduleConfig: MonitoringScheduleConfigUnionTypeDef
+        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef
     ) -> UpdateMonitoringScheduleResponseTypeDef:
         """
         Updates a previously created schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_monitoring_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_monitoring_schedule)
         """
@@ -4862,29 +4909,29 @@
         sets up an ML pipeline from training to deploying an approved model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_project)
         """
 
     async def update_space(
-        self, *, DomainId: str, SpaceName: str, SpaceSettings: SpaceSettingsUnionTypeDef = ...
+        self, *, DomainId: str, SpaceName: str, SpaceSettings: SpaceSettingsTypeDef = ...
     ) -> UpdateSpaceResponseTypeDef:
         """
         Updates the settings of a space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_space)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_space)
         """
 
     async def update_training_job(
         self,
         *,
         TrainingJobName: str,
         ProfilerConfig: ProfilerConfigForUpdateTypeDef = ...,
-        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationUnionTypeDef] = ...,
+        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
         ResourceConfig: ResourceConfigForUpdateTypeDef = ...
     ) -> UpdateTrainingJobResponseTypeDef:
         """
         Update a model training job to request a new Debugger profiling configuration or
         to change warm pool retention length.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_training_job)
@@ -4920,43 +4967,43 @@
         Updates one or more properties of a trial component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_trial_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_trial_component)
         """
 
     async def update_user_profile(
-        self, *, DomainId: str, UserProfileName: str, UserSettings: UserSettingsUnionTypeDef = ...
+        self, *, DomainId: str, UserProfileName: str, UserSettings: UserSettingsTypeDef = ...
     ) -> UpdateUserProfileResponseTypeDef:
         """
         Updates a user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_user_profile)
         """
 
     async def update_workforce(
         self,
         *,
         WorkforceName: str,
-        SourceIpConfig: SourceIpConfigUnionTypeDef = ...,
+        SourceIpConfig: SourceIpConfigTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
         WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...
     ) -> UpdateWorkforceResponseTypeDef:
         """
         Use this operation to update your workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workforce)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_workforce)
         """
 
     async def update_workteam(
         self,
         *,
         WorkteamName: str,
-        MemberDefinitions: Sequence[MemberDefinitionUnionTypeDef] = ...,
+        MemberDefinitions: Sequence[MemberDefinitionTypeDef] = ...,
         Description: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...
     ) -> UpdateWorkteamResponseTypeDef:
         """
         Updates an existing work team with new member definitions or description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workteam)
@@ -5420,14 +5467,23 @@
     ) -> ListProcessingJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_resource_catalogs"]
+    ) -> ListResourceCatalogsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_spaces"]) -> ListSpacesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_paginator)
         """
 
     @overload
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/client.pyi` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     AutoMLSortOrderType,
     BatchStrategyType,
     CandidateSortByType,
     CandidateStatusType,
     CodeRepositorySortByType,
     CodeRepositorySortOrderType,
     CompilationJobStatusType,
+    CrossAccountFilterOptionType,
     DirectInternetAccessType,
     DirectionType,
     EdgePackagingJobStatusType,
     EndpointConfigSortKeyType,
     EndpointSortKeyType,
     EndpointStatusType,
     ExecutionStatusType,
@@ -98,14 +99,15 @@
     ProblemTypeType,
     ProcessingJobStatusType,
     ProcessorType,
     ProjectSortByType,
     ProjectSortOrderType,
     RecommendationJobStatusType,
     RecommendationJobTypeType,
+    ResourceCatalogSortOrderType,
     ResourceTypeType,
     RootAccessType,
     ScheduleStatusType,
     SearchSortOrderType,
     SortActionsByType,
     SortAssociationsByType,
     SortByType,
@@ -179,14 +181,15 @@
     ListNotebookInstanceLifecycleConfigsPaginator,
     ListNotebookInstancesPaginator,
     ListPipelineExecutionsPaginator,
     ListPipelineExecutionStepsPaginator,
     ListPipelineParametersForExecutionPaginator,
     ListPipelinesPaginator,
     ListProcessingJobsPaginator,
+    ListResourceCatalogsPaginator,
     ListSpacesPaginator,
     ListStageDevicesPaginator,
     ListStudioLifecycleConfigsPaginator,
     ListSubscribedWorkteamsPaginator,
     ListTagsPaginator,
     ListTrainingJobsForHyperParameterTuningJobPaginator,
     ListTrainingJobsPaginator,
@@ -197,37 +200,37 @@
     ListWorkforcesPaginator,
     ListWorkteamsPaginator,
     SearchPaginator,
 )
 from .type_defs import (
     ActionSourceTypeDef,
     AddAssociationResponseTypeDef,
-    AdditionalInferenceSpecificationDefinitionUnionTypeDef,
+    AdditionalInferenceSpecificationDefinitionTypeDef,
     AddTagsOutputTypeDef,
-    AlgorithmSpecificationUnionTypeDef,
-    AlgorithmValidationSpecificationUnionTypeDef,
-    AppSpecificationUnionTypeDef,
-    ArtifactSourceUnionTypeDef,
+    AlgorithmSpecificationTypeDef,
+    AlgorithmValidationSpecificationTypeDef,
+    AppSpecificationTypeDef,
+    ArtifactSourceTypeDef,
     AssociateTrialComponentResponseTypeDef,
-    AsyncInferenceConfigUnionTypeDef,
+    AsyncInferenceConfigTypeDef,
     AutoMLChannelTypeDef,
     AutoMLDataSplitConfigTypeDef,
     AutoMLJobChannelTypeDef,
-    AutoMLJobConfigUnionTypeDef,
+    AutoMLJobConfigTypeDef,
     AutoMLJobObjectiveTypeDef,
     AutoMLOutputDataConfigTypeDef,
-    AutoMLProblemTypeConfigUnionTypeDef,
-    AutoMLSecurityConfigUnionTypeDef,
+    AutoMLProblemTypeConfigTypeDef,
+    AutoMLSecurityConfigTypeDef,
     AutotuneTypeDef,
     BatchDataCaptureConfigTypeDef,
     BatchDescribeModelPackageOutputTypeDef,
-    ChannelUnionTypeDef,
+    ChannelTypeDef,
     CheckpointConfigTypeDef,
     CognitoConfigTypeDef,
-    ContainerDefinitionUnionTypeDef,
+    ContainerDefinitionTypeDef,
     ContextSourceTypeDef,
     CreateActionResponseTypeDef,
     CreateAlgorithmOutputTypeDef,
     CreateAppImageConfigResponseTypeDef,
     CreateAppResponseTypeDef,
     CreateArtifactResponseTypeDef,
     CreateAutoMLJobResponseTypeDef,
@@ -272,33 +275,33 @@
     CreateTrainingJobResponseTypeDef,
     CreateTransformJobResponseTypeDef,
     CreateTrialComponentResponseTypeDef,
     CreateTrialResponseTypeDef,
     CreateUserProfileResponseTypeDef,
     CreateWorkforceResponseTypeDef,
     CreateWorkteamResponseTypeDef,
-    DataCaptureConfigUnionTypeDef,
+    DataCaptureConfigTypeDef,
     DataProcessingTypeDef,
-    DataQualityAppSpecificationUnionTypeDef,
+    DataQualityAppSpecificationTypeDef,
     DataQualityBaselineConfigTypeDef,
-    DataQualityJobInputUnionTypeDef,
-    DebugHookConfigUnionTypeDef,
-    DebugRuleConfigurationUnionTypeDef,
-    DefaultSpaceSettingsUnionTypeDef,
+    DataQualityJobInputTypeDef,
+    DebugHookConfigTypeDef,
+    DebugRuleConfigurationTypeDef,
+    DefaultSpaceSettingsTypeDef,
     DeleteActionResponseTypeDef,
     DeleteArtifactResponseTypeDef,
     DeleteAssociationResponseTypeDef,
     DeleteContextResponseTypeDef,
     DeleteExperimentResponseTypeDef,
     DeleteInferenceExperimentResponseTypeDef,
     DeletePipelineResponseTypeDef,
     DeleteTrialComponentResponseTypeDef,
     DeleteTrialResponseTypeDef,
     DeleteWorkteamResponseTypeDef,
-    DeploymentConfigUnionTypeDef,
+    DeploymentConfigTypeDef,
     DeploymentStageTypeDef,
     DescribeActionResponseTypeDef,
     DescribeAlgorithmOutputTypeDef,
     DescribeAppImageConfigResponseTypeDef,
     DescribeAppResponseTypeDef,
     DescribeArtifactResponseTypeDef,
     DescribeAutoMLJobResponseTypeDef,
@@ -354,49 +357,50 @@
     DescribeUserProfileResponseTypeDef,
     DescribeWorkforceResponseTypeDef,
     DescribeWorkteamResponseTypeDef,
     DesiredWeightAndCapacityTypeDef,
     DeviceTypeDef,
     DisassociateTrialComponentResponseTypeDef,
     DomainSettingsForUpdateTypeDef,
-    DomainSettingsUnionTypeDef,
+    DomainSettingsTypeDef,
     DriftCheckBaselinesTypeDef,
     EdgeDeploymentModelConfigTypeDef,
     EdgeOutputConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     ExperimentConfigTypeDef,
-    ExplainerConfigUnionTypeDef,
+    ExplainerConfigTypeDef,
     FeatureDefinitionTypeDef,
     FeatureParameterTypeDef,
     FlowDefinitionOutputConfigTypeDef,
     GetDeviceFleetReportResponseTypeDef,
     GetLineageGroupPolicyResponseTypeDef,
     GetModelPackageGroupPolicyOutputTypeDef,
     GetSagemakerServicecatalogPortfolioStatusOutputTypeDef,
+    GetScalingConfigurationRecommendationResponseTypeDef,
     GetSearchSuggestionsResponseTypeDef,
     GitConfigForUpdateTypeDef,
     GitConfigTypeDef,
     HubS3StorageConfigTypeDef,
     HumanLoopActivationConfigTypeDef,
-    HumanLoopConfigUnionTypeDef,
+    HumanLoopConfigTypeDef,
     HumanLoopRequestSourceTypeDef,
-    HumanTaskConfigUnionTypeDef,
-    HyperParameterTrainingJobDefinitionUnionTypeDef,
-    HyperParameterTuningJobConfigUnionTypeDef,
-    HyperParameterTuningJobWarmStartConfigUnionTypeDef,
+    HumanTaskConfigTypeDef,
+    HyperParameterTrainingJobDefinitionTypeDef,
+    HyperParameterTuningJobConfigTypeDef,
+    HyperParameterTuningJobWarmStartConfigTypeDef,
     ImportHubContentResponseTypeDef,
     InferenceExecutionConfigTypeDef,
-    InferenceExperimentDataStorageConfigUnionTypeDef,
-    InferenceExperimentScheduleUnionTypeDef,
-    InferenceSpecificationUnionTypeDef,
+    InferenceExperimentDataStorageConfigTypeDef,
+    InferenceExperimentScheduleTypeDef,
+    InferenceSpecificationTypeDef,
     InputConfigTypeDef,
     InstanceMetadataServiceConfigurationTypeDef,
-    KernelGatewayImageConfigUnionTypeDef,
-    LabelingJobAlgorithmsConfigUnionTypeDef,
-    LabelingJobInputConfigUnionTypeDef,
+    KernelGatewayImageConfigTypeDef,
+    LabelingJobAlgorithmsConfigTypeDef,
+    LabelingJobInputConfigTypeDef,
     LabelingJobOutputConfigTypeDef,
     LabelingJobStoppingConditionsTypeDef,
     ListActionsResponseTypeDef,
     ListAlgorithmsOutputTypeDef,
     ListAliasesResponseTypeDef,
     ListAppImageConfigsResponseTypeDef,
     ListAppsResponseTypeDef,
@@ -449,107 +453,110 @@
     ListNotebookInstancesOutputTypeDef,
     ListPipelineExecutionsResponseTypeDef,
     ListPipelineExecutionStepsResponseTypeDef,
     ListPipelineParametersForExecutionResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListProcessingJobsResponseTypeDef,
     ListProjectsOutputTypeDef,
+    ListResourceCatalogsResponseTypeDef,
     ListSpacesResponseTypeDef,
     ListStageDevicesResponseTypeDef,
     ListStudioLifecycleConfigsResponseTypeDef,
     ListSubscribedWorkteamsResponseTypeDef,
     ListTagsOutputTypeDef,
     ListTrainingJobsForHyperParameterTuningJobResponseTypeDef,
     ListTrainingJobsResponseTypeDef,
     ListTransformJobsResponseTypeDef,
     ListTrialComponentsResponseTypeDef,
     ListTrialsResponseTypeDef,
     ListUserProfilesResponseTypeDef,
     ListWorkforcesResponseTypeDef,
     ListWorkteamsResponseTypeDef,
-    MemberDefinitionUnionTypeDef,
+    MemberDefinitionTypeDef,
     MetadataPropertiesTypeDef,
-    ModelBiasAppSpecificationUnionTypeDef,
+    ModelBiasAppSpecificationTypeDef,
     ModelBiasBaselineConfigTypeDef,
-    ModelBiasJobInputUnionTypeDef,
+    ModelBiasJobInputTypeDef,
     ModelCardExportOutputConfigTypeDef,
     ModelCardSecurityConfigTypeDef,
     ModelClientConfigTypeDef,
     ModelDeployConfigTypeDef,
-    ModelExplainabilityAppSpecificationUnionTypeDef,
+    ModelExplainabilityAppSpecificationTypeDef,
     ModelExplainabilityBaselineConfigTypeDef,
-    ModelExplainabilityJobInputUnionTypeDef,
+    ModelExplainabilityJobInputTypeDef,
     ModelMetadataSearchExpressionTypeDef,
     ModelMetricsTypeDef,
-    ModelPackageValidationSpecificationUnionTypeDef,
-    ModelQualityAppSpecificationUnionTypeDef,
+    ModelPackageValidationSpecificationTypeDef,
+    ModelQualityAppSpecificationTypeDef,
     ModelQualityBaselineConfigTypeDef,
-    ModelQualityJobInputUnionTypeDef,
+    ModelQualityJobInputTypeDef,
     ModelVariantConfigTypeDef,
-    MonitoringNetworkConfigUnionTypeDef,
-    MonitoringOutputConfigUnionTypeDef,
+    MonitoringNetworkConfigTypeDef,
+    MonitoringOutputConfigTypeDef,
     MonitoringResourcesTypeDef,
-    MonitoringScheduleConfigUnionTypeDef,
+    MonitoringScheduleConfigTypeDef,
     MonitoringStoppingConditionTypeDef,
-    NeoVpcConfigUnionTypeDef,
-    NetworkConfigUnionTypeDef,
+    NeoVpcConfigTypeDef,
+    NetworkConfigTypeDef,
     NotebookInstanceLifecycleHookTypeDef,
     NotificationConfigurationTypeDef,
     OfflineStoreConfigTypeDef,
     OidcConfigTypeDef,
     OnlineStoreConfigTypeDef,
+    OnlineStoreConfigUpdateTypeDef,
     OutputConfigTypeDef,
     OutputDataConfigTypeDef,
     OutputParameterTypeDef,
     ParallelismConfigurationTypeDef,
     ParameterTypeDef,
     PipelineDefinitionS3LocationTypeDef,
     ProcessingInputTypeDef,
-    ProcessingOutputConfigUnionTypeDef,
+    ProcessingOutputConfigTypeDef,
     ProcessingResourcesTypeDef,
     ProcessingStoppingConditionTypeDef,
     ProductionVariantTypeDef,
     ProfilerConfigForUpdateTypeDef,
-    ProfilerConfigUnionTypeDef,
-    ProfilerRuleConfigurationUnionTypeDef,
+    ProfilerConfigTypeDef,
+    ProfilerRuleConfigurationTypeDef,
     PutModelPackageGroupPolicyOutputTypeDef,
     QueryFiltersTypeDef,
     QueryLineageResponseTypeDef,
-    RecommendationJobInputConfigUnionTypeDef,
+    RecommendationJobInputConfigTypeDef,
     RecommendationJobOutputConfigTypeDef,
-    RecommendationJobStoppingConditionsUnionTypeDef,
+    RecommendationJobStoppingConditionsTypeDef,
     RenderableTaskTypeDef,
     RenderUiTemplateResponseTypeDef,
     ResourceConfigForUpdateTypeDef,
-    ResourceConfigUnionTypeDef,
+    ResourceConfigTypeDef,
     ResourceSpecTypeDef,
     RetentionPolicyTypeDef,
     RetryPipelineExecutionResponseTypeDef,
     RetryStrategyTypeDef,
+    ScalingPolicyObjectiveTypeDef,
     SearchExpressionTypeDef,
     SearchResponseTypeDef,
-    SelectiveExecutionConfigUnionTypeDef,
+    SelectiveExecutionConfigTypeDef,
     SendPipelineExecutionStepFailureResponseTypeDef,
     SendPipelineExecutionStepSuccessResponseTypeDef,
-    ServiceCatalogProvisioningDetailsUnionTypeDef,
+    ServiceCatalogProvisioningDetailsTypeDef,
     ServiceCatalogProvisioningUpdateDetailsTypeDef,
-    ShadowModeConfigUnionTypeDef,
-    SourceAlgorithmSpecificationUnionTypeDef,
-    SourceIpConfigUnionTypeDef,
-    SpaceSettingsUnionTypeDef,
+    ShadowModeConfigTypeDef,
+    SourceAlgorithmSpecificationTypeDef,
+    SourceIpConfigTypeDef,
+    SpaceSettingsTypeDef,
     StartInferenceExperimentResponseTypeDef,
     StartPipelineExecutionResponseTypeDef,
     StopInferenceExperimentResponseTypeDef,
     StoppingConditionTypeDef,
     StopPipelineExecutionResponseTypeDef,
     SuggestionQueryTypeDef,
     TagTypeDef,
     TensorBoardOutputConfigTypeDef,
     TimestampTypeDef,
-    TrainingSpecificationUnionTypeDef,
+    TrainingSpecificationTypeDef,
     TransformInputTypeDef,
     TransformOutputTypeDef,
     TransformResourcesTypeDef,
     TrialComponentArtifactTypeDef,
     TrialComponentParameterValueTypeDef,
     TrialComponentStatusTypeDef,
     UiTemplateTypeDef,
@@ -577,17 +584,17 @@
     UpdateSpaceResponseTypeDef,
     UpdateTrainingJobResponseTypeDef,
     UpdateTrialComponentResponseTypeDef,
     UpdateTrialResponseTypeDef,
     UpdateUserProfileResponseTypeDef,
     UpdateWorkforceResponseTypeDef,
     UpdateWorkteamResponseTypeDef,
-    UserSettingsUnionTypeDef,
+    UserSettingsTypeDef,
     VariantPropertyTypeDef,
-    VpcConfigUnionTypeDef,
+    VpcConfigTypeDef,
     WorkforceVpcConfigRequestTypeDef,
 )
 from .waiter import (
     EndpointDeletedWaiter,
     EndpointInServiceWaiter,
     ImageCreatedWaiter,
     ImageDeletedWaiter,
@@ -709,18 +716,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_action)
         """
     async def create_algorithm(
         self,
         *,
         AlgorithmName: str,
-        TrainingSpecification: TrainingSpecificationUnionTypeDef,
+        TrainingSpecification: TrainingSpecificationTypeDef,
         AlgorithmDescription: str = ...,
-        InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,
-        ValidationSpecification: AlgorithmValidationSpecificationUnionTypeDef = ...,
+        InferenceSpecification: InferenceSpecificationTypeDef = ...,
+        ValidationSpecification: AlgorithmValidationSpecificationTypeDef = ...,
         CertifyForMarketplace: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateAlgorithmOutputTypeDef:
         """
         Create a machine learning algorithm that you can use in SageMaker and list in
         the Amazon Web Services Marketplace.
 
@@ -745,26 +752,26 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_app)
         """
     async def create_app_image_config(
         self,
         *,
         AppImageConfigName: str,
         Tags: Sequence[TagTypeDef] = ...,
-        KernelGatewayImageConfig: KernelGatewayImageConfigUnionTypeDef = ...
+        KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...
     ) -> CreateAppImageConfigResponseTypeDef:
         """
         Creates a configuration for running a SageMaker image as a KernelGateway app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_app_image_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_app_image_config)
         """
     async def create_artifact(
         self,
         *,
-        Source: ArtifactSourceUnionTypeDef,
+        Source: ArtifactSourceTypeDef,
         ArtifactType: str,
         ArtifactName: str = ...,
         Properties: Mapping[str, str] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateArtifactResponseTypeDef:
         """
@@ -778,15 +785,15 @@
         *,
         AutoMLJobName: str,
         InputDataConfig: Sequence[AutoMLChannelTypeDef],
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
         RoleArn: str,
         ProblemType: ProblemTypeType = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
-        AutoMLJobConfig: AutoMLJobConfigUnionTypeDef = ...,
+        AutoMLJobConfig: AutoMLJobConfigTypeDef = ...,
         GenerateCandidateDefinitionsOnly: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ModelDeployConfig: ModelDeployConfigTypeDef = ...
     ) -> CreateAutoMLJobResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job.
 
@@ -795,18 +802,18 @@
         """
     async def create_auto_ml_job_v2(
         self,
         *,
         AutoMLJobName: str,
         AutoMLJobInputDataConfig: Sequence[AutoMLJobChannelTypeDef],
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
-        AutoMLProblemTypeConfig: AutoMLProblemTypeConfigUnionTypeDef,
+        AutoMLProblemTypeConfig: AutoMLProblemTypeConfigTypeDef,
         RoleArn: str,
         Tags: Sequence[TagTypeDef] = ...,
-        SecurityConfig: AutoMLSecurityConfigUnionTypeDef = ...,
+        SecurityConfig: AutoMLSecurityConfigTypeDef = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
         ModelDeployConfig: ModelDeployConfigTypeDef = ...,
         DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...
     ) -> CreateAutoMLJobV2ResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job
         V2.
@@ -832,15 +839,15 @@
         *,
         CompilationJobName: str,
         RoleArn: str,
         OutputConfig: OutputConfigTypeDef,
         StoppingCondition: StoppingConditionTypeDef,
         ModelPackageVersionArn: str = ...,
         InputConfig: InputConfigTypeDef = ...,
-        VpcConfig: NeoVpcConfigUnionTypeDef = ...,
+        VpcConfig: NeoVpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateCompilationJobResponseTypeDef:
         """
         Starts a model compilation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_compilation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_compilation_job)
@@ -861,21 +868,21 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_context)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_context)
         """
     async def create_data_quality_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        DataQualityAppSpecification: DataQualityAppSpecificationUnionTypeDef,
-        DataQualityJobInput: DataQualityJobInputUnionTypeDef,
-        DataQualityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
+        DataQualityAppSpecification: DataQualityAppSpecificationTypeDef,
+        DataQualityJobInput: DataQualityJobInputTypeDef,
+        DataQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         DataQualityBaselineConfig: DataQualityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDataQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors data quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_data_quality_job_definition)
@@ -898,24 +905,24 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_device_fleet)
         """
     async def create_domain(
         self,
         *,
         DomainName: str,
         AuthMode: AuthModeType,
-        DefaultUserSettings: UserSettingsUnionTypeDef,
+        DefaultUserSettings: UserSettingsTypeDef,
         SubnetIds: Sequence[str],
         VpcId: str,
         Tags: Sequence[TagTypeDef] = ...,
         AppNetworkAccessType: AppNetworkAccessTypeType = ...,
         HomeEfsFileSystemKmsKeyId: str = ...,
         KmsKeyId: str = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,
-        DomainSettings: DomainSettingsUnionTypeDef = ...,
-        DefaultSpaceSettings: DefaultSpaceSettingsUnionTypeDef = ...
+        DomainSettings: DomainSettingsTypeDef = ...,
+        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a `Domain` used by Amazon SageMaker Studio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_domain)
         """
@@ -962,33 +969,33 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_edge_packaging_job)
         """
     async def create_endpoint(
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
-        DeploymentConfig: DeploymentConfigUnionTypeDef = ...,
+        DeploymentConfig: DeploymentConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateEndpointOutputTypeDef:
         """
         Creates an endpoint using the endpoint configuration specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_endpoint)
         """
     async def create_endpoint_config(
         self,
         *,
         EndpointConfigName: str,
         ProductionVariants: Sequence[ProductionVariantTypeDef],
-        DataCaptureConfig: DataCaptureConfigUnionTypeDef = ...,
+        DataCaptureConfig: DataCaptureConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
-        AsyncInferenceConfig: AsyncInferenceConfigUnionTypeDef = ...,
-        ExplainerConfig: ExplainerConfigUnionTypeDef = ...,
+        AsyncInferenceConfig: AsyncInferenceConfigTypeDef = ...,
+        ExplainerConfig: ExplainerConfigTypeDef = ...,
         ShadowProductionVariants: Sequence[ProductionVariantTypeDef] = ...
     ) -> CreateEndpointConfigOutputTypeDef:
         """
         Creates an endpoint configuration that SageMaker hosting services uses to deploy
         models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint_config)
@@ -1027,15 +1034,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_feature_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_feature_group)
         """
     async def create_flow_definition(
         self,
         *,
         FlowDefinitionName: str,
-        HumanLoopConfig: HumanLoopConfigUnionTypeDef,
+        HumanLoopConfig: HumanLoopConfigTypeDef,
         OutputConfig: FlowDefinitionOutputConfigTypeDef,
         RoleArn: str,
         HumanLoopRequestSource: HumanLoopRequestSourceTypeDef = ...,
         HumanLoopActivationConfig: HumanLoopActivationConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFlowDefinitionResponseTypeDef:
         """
@@ -1073,18 +1080,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_human_task_ui)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_human_task_ui)
         """
     async def create_hyper_parameter_tuning_job(
         self,
         *,
         HyperParameterTuningJobName: str,
-        HyperParameterTuningJobConfig: HyperParameterTuningJobConfigUnionTypeDef,
-        TrainingJobDefinition: HyperParameterTrainingJobDefinitionUnionTypeDef = ...,
-        TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionUnionTypeDef] = ...,
-        WarmStartConfig: HyperParameterTuningJobWarmStartConfigUnionTypeDef = ...,
+        HyperParameterTuningJobConfig: HyperParameterTuningJobConfigTypeDef,
+        TrainingJobDefinition: HyperParameterTrainingJobDefinitionTypeDef = ...,
+        TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionTypeDef] = ...,
+        WarmStartConfig: HyperParameterTuningJobWarmStartConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Autotune: AutotuneTypeDef = ...
     ) -> CreateHyperParameterTuningJobResponseTypeDef:
         """
         Starts a hyperparameter tuning job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_hyper_parameter_tuning_job)
@@ -1130,18 +1137,18 @@
         self,
         *,
         Name: str,
         Type: Literal["ShadowMode"],
         RoleArn: str,
         EndpointName: str,
         ModelVariants: Sequence[ModelVariantConfigTypeDef],
-        ShadowModeConfig: ShadowModeConfigUnionTypeDef,
-        Schedule: InferenceExperimentScheduleUnionTypeDef = ...,
+        ShadowModeConfig: ShadowModeConfigTypeDef,
+        Schedule: InferenceExperimentScheduleTypeDef = ...,
         Description: str = ...,
-        DataStorageConfig: InferenceExperimentDataStorageConfigUnionTypeDef = ...,
+        DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
         KmsKey: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateInferenceExperimentResponseTypeDef:
         """
         Creates an inference experiment using the configurations specified in the
         request.
 
@@ -1150,75 +1157,75 @@
         """
     async def create_inference_recommendations_job(
         self,
         *,
         JobName: str,
         JobType: RecommendationJobTypeType,
         RoleArn: str,
-        InputConfig: RecommendationJobInputConfigUnionTypeDef,
+        InputConfig: RecommendationJobInputConfigTypeDef,
         JobDescription: str = ...,
-        StoppingConditions: RecommendationJobStoppingConditionsUnionTypeDef = ...,
+        StoppingConditions: RecommendationJobStoppingConditionsTypeDef = ...,
         OutputConfig: RecommendationJobOutputConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateInferenceRecommendationsJobResponseTypeDef:
         """
         Starts a recommendation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_recommendations_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_inference_recommendations_job)
         """
     async def create_labeling_job(
         self,
         *,
         LabelingJobName: str,
         LabelAttributeName: str,
-        InputConfig: LabelingJobInputConfigUnionTypeDef,
+        InputConfig: LabelingJobInputConfigTypeDef,
         OutputConfig: LabelingJobOutputConfigTypeDef,
         RoleArn: str,
-        HumanTaskConfig: HumanTaskConfigUnionTypeDef,
+        HumanTaskConfig: HumanTaskConfigTypeDef,
         LabelCategoryConfigS3Uri: str = ...,
         StoppingConditions: LabelingJobStoppingConditionsTypeDef = ...,
-        LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigUnionTypeDef = ...,
+        LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateLabelingJobResponseTypeDef:
         """
         Creates a job that uses workers to label the data objects in your input dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_labeling_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_labeling_job)
         """
     async def create_model(
         self,
         *,
         ModelName: str,
         ExecutionRoleArn: str,
-        PrimaryContainer: ContainerDefinitionUnionTypeDef = ...,
-        Containers: Sequence[ContainerDefinitionUnionTypeDef] = ...,
+        PrimaryContainer: ContainerDefinitionTypeDef = ...,
+        Containers: Sequence[ContainerDefinitionTypeDef] = ...,
         InferenceExecutionConfig: InferenceExecutionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         EnableNetworkIsolation: bool = ...
     ) -> CreateModelOutputTypeDef:
         """
         Creates a model in SageMaker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model)
         """
     async def create_model_bias_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelBiasAppSpecification: ModelBiasAppSpecificationUnionTypeDef,
-        ModelBiasJobInput: ModelBiasJobInputUnionTypeDef,
-        ModelBiasJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
+        ModelBiasAppSpecification: ModelBiasAppSpecificationTypeDef,
+        ModelBiasJobInput: ModelBiasJobInputTypeDef,
+        ModelBiasJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelBiasBaselineConfig: ModelBiasBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelBiasJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model bias job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_bias_job_definition)
@@ -1253,21 +1260,21 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_card_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_card_export_job)
         """
     async def create_model_explainability_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationUnionTypeDef,
-        ModelExplainabilityJobInput: ModelExplainabilityJobInputUnionTypeDef,
-        ModelExplainabilityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
+        ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationTypeDef,
+        ModelExplainabilityJobInput: ModelExplainabilityJobInputTypeDef,
+        ModelExplainabilityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelExplainabilityBaselineConfig: ModelExplainabilityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelExplainabilityJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model explainability job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_explainability_job_definition)
@@ -1275,30 +1282,30 @@
         """
     async def create_model_package(
         self,
         *,
         ModelPackageName: str = ...,
         ModelPackageGroupName: str = ...,
         ModelPackageDescription: str = ...,
-        InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,
-        ValidationSpecification: ModelPackageValidationSpecificationUnionTypeDef = ...,
-        SourceAlgorithmSpecification: SourceAlgorithmSpecificationUnionTypeDef = ...,
+        InferenceSpecification: InferenceSpecificationTypeDef = ...,
+        ValidationSpecification: ModelPackageValidationSpecificationTypeDef = ...,
+        SourceAlgorithmSpecification: SourceAlgorithmSpecificationTypeDef = ...,
         CertifyForMarketplace: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
         ModelMetrics: ModelMetricsTypeDef = ...,
         ClientToken: str = ...,
         CustomerMetadataProperties: Mapping[str, str] = ...,
         DriftCheckBaselines: DriftCheckBaselinesTypeDef = ...,
         Domain: str = ...,
         Task: str = ...,
         SamplePayloadUrl: str = ...,
         AdditionalInferenceSpecifications: Sequence[
-            AdditionalInferenceSpecificationDefinitionUnionTypeDef
+            AdditionalInferenceSpecificationDefinitionTypeDef
         ] = ...
     ) -> CreateModelPackageOutputTypeDef:
         """
         Creates a model package that you can use to create SageMaker models or list on
         Amazon Web Services Marketplace, or a versioned model that is part of a model
         group.
 
@@ -1318,35 +1325,35 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_package_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_package_group)
         """
     async def create_model_quality_job_definition(
         self,
         *,
         JobDefinitionName: str,
-        ModelQualityAppSpecification: ModelQualityAppSpecificationUnionTypeDef,
-        ModelQualityJobInput: ModelQualityJobInputUnionTypeDef,
-        ModelQualityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,
+        ModelQualityAppSpecification: ModelQualityAppSpecificationTypeDef,
+        ModelQualityJobInput: ModelQualityJobInputTypeDef,
+        ModelQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelQualityBaselineConfig: ModelQualityBaselineConfigTypeDef = ...,
-        NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,
+        NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateModelQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors model quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_quality_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_quality_job_definition)
         """
     async def create_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
-        MonitoringScheduleConfig: MonitoringScheduleConfigUnionTypeDef,
+        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMonitoringScheduleResponseTypeDef:
         """
         Creates a schedule that regularly starts Amazon SageMaker Processing Jobs to
         monitor the data captured for an Amazon SageMaker Endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_monitoring_schedule)
@@ -1437,35 +1444,35 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_presigned_notebook_instance_url)
         """
     async def create_processing_job(
         self,
         *,
         ProcessingJobName: str,
         ProcessingResources: ProcessingResourcesTypeDef,
-        AppSpecification: AppSpecificationUnionTypeDef,
+        AppSpecification: AppSpecificationTypeDef,
         RoleArn: str,
         ProcessingInputs: Sequence[ProcessingInputTypeDef] = ...,
-        ProcessingOutputConfig: ProcessingOutputConfigUnionTypeDef = ...,
+        ProcessingOutputConfig: ProcessingOutputConfigTypeDef = ...,
         StoppingCondition: ProcessingStoppingConditionTypeDef = ...,
         Environment: Mapping[str, str] = ...,
-        NetworkConfig: NetworkConfigUnionTypeDef = ...,
+        NetworkConfig: NetworkConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ExperimentConfig: ExperimentConfigTypeDef = ...
     ) -> CreateProcessingJobResponseTypeDef:
         """
         Creates a processing job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_processing_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_processing_job)
         """
     async def create_project(
         self,
         *,
         ProjectName: str,
-        ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsUnionTypeDef,
+        ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsTypeDef,
         ProjectDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a machine learning (ML) project that can contain one or more templates
         that set up an ML pipeline from training to deploying an approved model.
 
@@ -1474,15 +1481,15 @@
         """
     async def create_space(
         self,
         *,
         DomainId: str,
         SpaceName: str,
         Tags: Sequence[TagTypeDef] = ...,
-        SpaceSettings: SpaceSettingsUnionTypeDef = ...
+        SpaceSettings: SpaceSettingsTypeDef = ...
     ) -> CreateSpaceResponseTypeDef:
         """
         Creates a space used for real time collaboration in a Domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_space)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_space)
         """
@@ -1500,33 +1507,33 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_studio_lifecycle_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_studio_lifecycle_config)
         """
     async def create_training_job(
         self,
         *,
         TrainingJobName: str,
-        AlgorithmSpecification: AlgorithmSpecificationUnionTypeDef,
+        AlgorithmSpecification: AlgorithmSpecificationTypeDef,
         RoleArn: str,
         OutputDataConfig: OutputDataConfigTypeDef,
-        ResourceConfig: ResourceConfigUnionTypeDef,
+        ResourceConfig: ResourceConfigTypeDef,
         StoppingCondition: StoppingConditionTypeDef,
         HyperParameters: Mapping[str, str] = ...,
-        InputDataConfig: Sequence[ChannelUnionTypeDef] = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        InputDataConfig: Sequence[ChannelTypeDef] = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         EnableNetworkIsolation: bool = ...,
         EnableInterContainerTrafficEncryption: bool = ...,
         EnableManagedSpotTraining: bool = ...,
         CheckpointConfig: CheckpointConfigTypeDef = ...,
-        DebugHookConfig: DebugHookConfigUnionTypeDef = ...,
-        DebugRuleConfigurations: Sequence[DebugRuleConfigurationUnionTypeDef] = ...,
+        DebugHookConfig: DebugHookConfigTypeDef = ...,
+        DebugRuleConfigurations: Sequence[DebugRuleConfigurationTypeDef] = ...,
         TensorBoardOutputConfig: TensorBoardOutputConfigTypeDef = ...,
         ExperimentConfig: ExperimentConfigTypeDef = ...,
-        ProfilerConfig: ProfilerConfigUnionTypeDef = ...,
-        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationUnionTypeDef] = ...,
+        ProfilerConfig: ProfilerConfigTypeDef = ...,
+        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
         Environment: Mapping[str, str] = ...,
         RetryStrategy: RetryStrategyTypeDef = ...
     ) -> CreateTrainingJobResponseTypeDef:
         """
         Starts a model training job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_training_job)
@@ -1595,43 +1602,43 @@
         self,
         *,
         DomainId: str,
         UserProfileName: str,
         SingleSignOnUserIdentifier: str = ...,
         SingleSignOnUserValue: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        UserSettings: UserSettingsUnionTypeDef = ...
+        UserSettings: UserSettingsTypeDef = ...
     ) -> CreateUserProfileResponseTypeDef:
         """
         Creates a user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_user_profile)
         """
     async def create_workforce(
         self,
         *,
         WorkforceName: str,
         CognitoConfig: CognitoConfigTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
-        SourceIpConfig: SourceIpConfigUnionTypeDef = ...,
+        SourceIpConfig: SourceIpConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...
     ) -> CreateWorkforceResponseTypeDef:
         """
         Use this operation to create a workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_workforce)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_workforce)
         """
     async def create_workteam(
         self,
         *,
         WorkteamName: str,
-        MemberDefinitions: Sequence[MemberDefinitionUnionTypeDef],
+        MemberDefinitions: Sequence[MemberDefinitionTypeDef],
         Description: str,
         WorkforceName: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWorkteamResponseTypeDef:
         """
         Creates a new work team for labeling your data.
@@ -1674,15 +1681,15 @@
         """
         Deletes an AppImageConfig.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_app_image_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#delete_app_image_config)
         """
     async def delete_artifact(
-        self, *, ArtifactArn: str = ..., Source: ArtifactSourceUnionTypeDef = ...
+        self, *, ArtifactArn: str = ..., Source: ArtifactSourceTypeDef = ...
     ) -> DeleteArtifactResponseTypeDef:
         """
         Deletes an artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#delete_artifact)
         """
@@ -2609,14 +2616,29 @@
     ) -> GetSagemakerServicecatalogPortfolioStatusOutputTypeDef:
         """
         Gets the status of Service Catalog in SageMaker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_sagemaker_servicecatalog_portfolio_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_sagemaker_servicecatalog_portfolio_status)
         """
+    async def get_scaling_configuration_recommendation(
+        self,
+        *,
+        InferenceRecommendationsJobName: str,
+        RecommendationId: str = ...,
+        EndpointName: str = ...,
+        TargetCpuUtilizationPerCore: int = ...,
+        ScalingPolicyObjective: ScalingPolicyObjectiveTypeDef = ...
+    ) -> GetScalingConfigurationRecommendationResponseTypeDef:
+        """
+        Starts an Amazon SageMaker Inference Recommender autoscaling recommendation job.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_scaling_configuration_recommendation)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_scaling_configuration_recommendation)
+        """
     async def get_search_suggestions(
         self, *, Resource: ResourceTypeType, SuggestionQuery: SuggestionQueryTypeDef = ...
     ) -> GetSearchSuggestionsResponseTypeDef:
         """
         An auto-complete API for the search functionality in the SageMaker console.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_search_suggestions)
@@ -3687,14 +3709,31 @@
     ) -> ListProjectsOutputTypeDef:
         """
         Gets a list of the projects in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_projects)
         """
+    async def list_resource_catalogs(
+        self,
+        *,
+        NameContains: str = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
+        SortOrder: ResourceCatalogSortOrderType = ...,
+        SortBy: Literal["CreationTime"] = ...,
+        MaxResults: int = ...,
+        NextToken: str = ...
+    ) -> ListResourceCatalogsResponseTypeDef:
+        """
+        Lists Amazon SageMaker Catalogs based on given filters and orders.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_resource_catalogs)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_resource_catalogs)
+        """
     async def list_spaces(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortOrder: SortOrderType = ...,
         SortBy: SpaceSortKeyType = ...,
@@ -3977,15 +4016,16 @@
         self,
         *,
         Resource: ResourceTypeType,
         SearchExpression: "SearchExpressionTypeDef" = ...,
         SortBy: str = ...,
         SortOrder: SearchSortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
+        CrossAccountFilterOption: CrossAccountFilterOptionType = ...
     ) -> SearchResponseTypeDef:
         """
         Finds SageMaker resources that match a search query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#search)
         """
@@ -4055,15 +4095,15 @@
         *,
         PipelineName: str,
         ClientRequestToken: str,
         PipelineExecutionDisplayName: str = ...,
         PipelineParameters: Sequence[ParameterTypeDef] = ...,
         PipelineExecutionDescription: str = ...,
         ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
-        SelectiveExecutionConfig: SelectiveExecutionConfigUnionTypeDef = ...
+        SelectiveExecutionConfig: SelectiveExecutionConfigTypeDef = ...
     ) -> StartPipelineExecutionResponseTypeDef:
         """
         Starts a pipeline execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.start_pipeline_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#start_pipeline_execution)
         """
@@ -4205,15 +4245,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_action)
         """
     async def update_app_image_config(
         self,
         *,
         AppImageConfigName: str,
-        KernelGatewayImageConfig: KernelGatewayImageConfigUnionTypeDef = ...
+        KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...
     ) -> UpdateAppImageConfigResponseTypeDef:
         """
         Updates the properties of an AppImageConfig.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_app_image_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_app_image_config)
         """
@@ -4278,17 +4318,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_devices)
         """
     async def update_domain(
         self,
         *,
         DomainId: str,
-        DefaultUserSettings: UserSettingsUnionTypeDef = ...,
+        DefaultUserSettings: UserSettingsTypeDef = ...,
         DomainSettingsForUpdate: DomainSettingsForUpdateTypeDef = ...,
-        DefaultSpaceSettings: DefaultSpaceSettingsUnionTypeDef = ...,
+        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the default settings for new user profiles in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_domain)
@@ -4296,15 +4336,15 @@
     async def update_endpoint(
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
         RetainAllVariantProperties: bool = ...,
         ExcludeRetainedVariantProperties: Sequence[VariantPropertyTypeDef] = ...,
-        DeploymentConfig: DeploymentConfigUnionTypeDef = ...,
+        DeploymentConfig: DeploymentConfigTypeDef = ...,
         RetainDeploymentConfig: bool = ...
     ) -> UpdateEndpointOutputTypeDef:
         """
         Deploys the new `EndpointConfig` specified in the request, switches to using
         newly created endpoint, and then deletes resources provisioned for the endpoint
         using the previous `EndpointConfig` (there is no availability loss).
 
@@ -4330,18 +4370,23 @@
         """
         Adds, updates, or removes the description of an experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_experiment)
         """
     async def update_feature_group(
-        self, *, FeatureGroupName: str, FeatureAdditions: Sequence[FeatureDefinitionTypeDef] = ...
+        self,
+        *,
+        FeatureGroupName: str,
+        FeatureAdditions: Sequence[FeatureDefinitionTypeDef] = ...,
+        OnlineStoreConfig: OnlineStoreConfigUpdateTypeDef = ...
     ) -> UpdateFeatureGroupResponseTypeDef:
         """
-        Updates the feature group.
+        Updates the feature group by either adding features or updating the online store
+        configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_feature_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_feature_group)
         """
     async def update_feature_metadata(
         self,
         *,
@@ -4408,19 +4453,19 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_image_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_image_version)
         """
     async def update_inference_experiment(
         self,
         *,
         Name: str,
-        Schedule: InferenceExperimentScheduleUnionTypeDef = ...,
+        Schedule: InferenceExperimentScheduleTypeDef = ...,
         Description: str = ...,
         ModelVariants: Sequence[ModelVariantConfigTypeDef] = ...,
-        DataStorageConfig: InferenceExperimentDataStorageConfigUnionTypeDef = ...,
-        ShadowModeConfig: ShadowModeConfigUnionTypeDef = ...
+        DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
+        ShadowModeConfig: ShadowModeConfigTypeDef = ...
     ) -> UpdateInferenceExperimentResponseTypeDef:
         """
         Updates an inference experiment that you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_inference_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_inference_experiment)
         """
@@ -4438,15 +4483,15 @@
         *,
         ModelPackageArn: str,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         ApprovalDescription: str = ...,
         CustomerMetadataProperties: Mapping[str, str] = ...,
         CustomerMetadataPropertiesToRemove: Sequence[str] = ...,
         AdditionalInferenceSpecificationsToAdd: Sequence[
-            AdditionalInferenceSpecificationDefinitionUnionTypeDef
+            AdditionalInferenceSpecificationDefinitionTypeDef
         ] = ...
     ) -> UpdateModelPackageOutputTypeDef:
         """
         Updates a versioned model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_model_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_model_package)
@@ -4465,15 +4510,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_monitoring_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_monitoring_alert)
         """
     async def update_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
-        MonitoringScheduleConfig: MonitoringScheduleConfigUnionTypeDef
+        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef
     ) -> UpdateMonitoringScheduleResponseTypeDef:
         """
         Updates a previously created schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_monitoring_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_monitoring_schedule)
         """
@@ -4559,28 +4604,28 @@
         Updates a machine learning (ML) project that is created from a template that
         sets up an ML pipeline from training to deploying an approved model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_project)
         """
     async def update_space(
-        self, *, DomainId: str, SpaceName: str, SpaceSettings: SpaceSettingsUnionTypeDef = ...
+        self, *, DomainId: str, SpaceName: str, SpaceSettings: SpaceSettingsTypeDef = ...
     ) -> UpdateSpaceResponseTypeDef:
         """
         Updates the settings of a space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_space)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_space)
         """
     async def update_training_job(
         self,
         *,
         TrainingJobName: str,
         ProfilerConfig: ProfilerConfigForUpdateTypeDef = ...,
-        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationUnionTypeDef] = ...,
+        ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
         ResourceConfig: ResourceConfigForUpdateTypeDef = ...
     ) -> UpdateTrainingJobResponseTypeDef:
         """
         Update a model training job to request a new Debugger profiling configuration or
         to change warm pool retention length.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_training_job)
@@ -4613,41 +4658,41 @@
         """
         Updates one or more properties of a trial component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_trial_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_trial_component)
         """
     async def update_user_profile(
-        self, *, DomainId: str, UserProfileName: str, UserSettings: UserSettingsUnionTypeDef = ...
+        self, *, DomainId: str, UserProfileName: str, UserSettings: UserSettingsTypeDef = ...
     ) -> UpdateUserProfileResponseTypeDef:
         """
         Updates a user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_user_profile)
         """
     async def update_workforce(
         self,
         *,
         WorkforceName: str,
-        SourceIpConfig: SourceIpConfigUnionTypeDef = ...,
+        SourceIpConfig: SourceIpConfigTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
         WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...
     ) -> UpdateWorkforceResponseTypeDef:
         """
         Use this operation to update your workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workforce)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_workforce)
         """
     async def update_workteam(
         self,
         *,
         WorkteamName: str,
-        MemberDefinitions: Sequence[MemberDefinitionUnionTypeDef] = ...,
+        MemberDefinitions: Sequence[MemberDefinitionTypeDef] = ...,
         Description: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...
     ) -> UpdateWorkteamResponseTypeDef:
         """
         Updates an existing work team with new member definitions or description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workteam)
@@ -5056,14 +5101,22 @@
         self, operation_name: Literal["list_processing_jobs"]
     ) -> ListProcessingJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_paginator)
         """
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_resource_catalogs"]
+    ) -> ListResourceCatalogsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_paginator)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_paginator)
+        """
+    @overload
     def get_paginator(self, operation_name: Literal["list_spaces"]) -> ListSpacesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_paginator)
         """
     @overload
     def get_paginator(
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/literals.py` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "ActionStatusType",
+    "AggregationTransformationValueType",
     "AlgorithmSortByType",
     "AlgorithmStatusType",
     "AppImageConfigSortKeyType",
     "AppInstanceTypeType",
     "AppNetworkAccessTypeType",
     "AppSecurityGroupManagementType",
     "AppSortKeyType",
@@ -67,14 +68,15 @@
     "CodeRepositorySortOrderType",
     "CompilationJobStatusType",
     "CompleteOnConvergenceType",
     "CompressionTypeType",
     "ConditionOutcomeType",
     "ContainerModeType",
     "ContentClassifierType",
+    "CrossAccountFilterOptionType",
     "DataDistributionTypeType",
     "DetailedAlgorithmStatusType",
     "DetailedModelPackageStatusType",
     "DeviceDeploymentStatusType",
     "DeviceSubsetTypeType",
     "DirectInternetAccessType",
     "DirectionType",
@@ -93,14 +95,16 @@
     "FeatureGroupSortByType",
     "FeatureGroupSortOrderType",
     "FeatureGroupStatusType",
     "FeatureStatusType",
     "FeatureTypeType",
     "FileSystemAccessModeType",
     "FileSystemTypeType",
+    "FillingTypeType",
+    "FlatInvocationsType",
     "FlowDefinitionStatusType",
     "FrameworkType",
     "HubContentSortByType",
     "HubContentStatusType",
     "HubContentTypeType",
     "HubSortByType",
     "HubStatusType",
@@ -190,14 +194,15 @@
     "ListNotebookInstanceLifecycleConfigsPaginatorName",
     "ListNotebookInstancesPaginatorName",
     "ListPipelineExecutionStepsPaginatorName",
     "ListPipelineExecutionsPaginatorName",
     "ListPipelineParametersForExecutionPaginatorName",
     "ListPipelinesPaginatorName",
     "ListProcessingJobsPaginatorName",
+    "ListResourceCatalogsPaginatorName",
     "ListSpacesPaginatorName",
     "ListStageDevicesPaginatorName",
     "ListStudioLifecycleConfigsPaginatorName",
     "ListSubscribedWorkteamsPaginatorName",
     "ListTagsPaginatorName",
     "ListTrainingJobsForHyperParameterTuningJobPaginatorName",
     "ListTrainingJobsPaginatorName",
@@ -271,21 +276,24 @@
     "ProfilingStatusType",
     "ProjectSortByType",
     "ProjectSortOrderType",
     "ProjectStatusType",
     "RStudioServerProAccessStatusType",
     "RStudioServerProUserGroupType",
     "RecommendationJobStatusType",
+    "RecommendationJobSupportedEndpointTypeType",
     "RecommendationJobTypeType",
     "RecommendationStatusType",
     "RecommendationStepTypeType",
     "RecordWrapperType",
     "RedshiftResultCompressionTypeType",
     "RedshiftResultFormatType",
     "RepositoryAccessModeType",
+    "ResourceCatalogSortByType",
+    "ResourceCatalogSortOrderType",
     "ResourceTypeType",
     "RetentionTypeType",
     "RootAccessType",
     "RuleEvaluationStatusType",
     "S3DataDistributionType",
     "S3DataTypeType",
     "S3ModelDataTypeType",
@@ -307,14 +315,15 @@
     "SortPipelinesByType",
     "SortTrialComponentsByType",
     "SortTrialsByType",
     "SpaceSortKeyType",
     "SpaceStatusType",
     "SplitTypeType",
     "StageStatusType",
+    "StatisticType",
     "StepStatusType",
     "StudioLifecycleConfigAppTypeType",
     "StudioLifecycleConfigSortKeyType",
     "TableFormatType",
     "TargetDeviceType",
     "TargetPlatformAcceleratorType",
     "TargetPlatformArchType",
@@ -328,14 +337,15 @@
     "TrainingJobSortByOptionsType",
     "TrainingJobStatusType",
     "TrainingRepositoryAccessModeType",
     "TransformInstanceTypeType",
     "TransformJobCompletedOrStoppedWaiterName",
     "TransformJobStatusType",
     "TrialComponentPrimaryStatusType",
+    "TtlDurationUnitType",
     "UserProfileSortKeyType",
     "UserProfileStatusType",
     "VariantPropertyTypeType",
     "VariantStatusType",
     "VendorGuidanceType",
     "WarmPoolResourceStatusType",
     "WorkforceStatusType",
@@ -345,14 +355,15 @@
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
 
 ActionStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping", "Unknown"]
+AggregationTransformationValueType = Literal["avg", "first", "max", "min", "sum"]
 AlgorithmSortByType = Literal["CreationTime", "Name"]
 AlgorithmStatusType = Literal["Completed", "Deleting", "Failed", "InProgress", "Pending"]
 AppImageConfigSortKeyType = Literal["CreationTime", "LastModifiedTime", "Name"]
 AppInstanceTypeType = Literal[
     "ml.c5.12xlarge",
     "ml.c5.18xlarge",
     "ml.c5.24xlarge",
@@ -452,54 +463,65 @@
     "GeneratingExplainabilityReport",
     "GeneratingModelInsightsReport",
     "MaxAutoMLJobRuntimeReached",
     "MaxCandidatesReached",
     "ModelDeploymentError",
     "ModelInsightsError",
     "ModelTuning",
+    "PreTraining",
     "Starting",
     "Stopped",
     "Stopping",
     "TrainingModels",
 ]
 AutoMLJobStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping"]
 AutoMLMetricEnumType = Literal[
     "AUC",
     "Accuracy",
+    "AverageWeightedQuantileLoss",
     "BalancedAccuracy",
     "F1",
     "F1macro",
     "MAE",
+    "MAPE",
+    "MASE",
     "MSE",
     "Precision",
     "PrecisionMacro",
     "R2",
     "RMSE",
     "Recall",
     "RecallMacro",
+    "WAPE",
 ]
 AutoMLMetricExtendedEnumType = Literal[
     "AUC",
     "Accuracy",
+    "AverageWeightedQuantileLoss",
     "BalancedAccuracy",
     "F1",
     "F1macro",
     "InferenceLatency",
     "LogLoss",
     "MAE",
+    "MAPE",
+    "MASE",
     "MSE",
     "Precision",
     "PrecisionMacro",
     "R2",
     "RMSE",
     "Recall",
     "RecallMacro",
+    "WAPE",
 ]
 AutoMLModeType = Literal["AUTO", "ENSEMBLING", "HYPERPARAMETER_TUNING"]
-AutoMLProblemTypeConfigNameType = Literal["ImageClassification", "Tabular", "TextClassification"]
+AutoMLProblemTypeConfigNameType = Literal[
+    "ImageClassification", "Tabular", "TextClassification", "TimeSeriesForecasting"
+]
 AutoMLProcessingUnitType = Literal["CPU", "GPU"]
 AutoMLS3DataTypeType = Literal["AugmentedManifestFile", "ManifestFile", "S3Prefix"]
 AutoMLSortByType = Literal["CreationTime", "Name", "Status"]
 AutoMLSortOrderType = Literal["Ascending", "Descending"]
 AutotuneModeType = Literal["Enabled"]
 AwsManagedHumanLoopRequestSourceType = Literal[
     "AWS/Rekognition/DetectModerationLabels/Image/V3", "AWS/Textract/AnalyzeDocument/Forms/V1"
@@ -584,14 +606,15 @@
     "COMPLETED", "FAILED", "INPROGRESS", "STARTING", "STOPPED", "STOPPING"
 ]
 CompleteOnConvergenceType = Literal["Disabled", "Enabled"]
 CompressionTypeType = Literal["Gzip", "None"]
 ConditionOutcomeType = Literal["False", "True"]
 ContainerModeType = Literal["MultiModel", "SingleModel"]
 ContentClassifierType = Literal["FreeOfAdultContent", "FreeOfPersonallyIdentifiableInformation"]
+CrossAccountFilterOptionType = Literal["CrossAccount", "SameAccount"]
 DataDistributionTypeType = Literal["FullyReplicated", "ShardedByS3Key"]
 DetailedAlgorithmStatusType = Literal["Completed", "Failed", "InProgress", "NotStarted"]
 DetailedModelPackageStatusType = Literal["Completed", "Failed", "InProgress", "NotStarted"]
 DeviceDeploymentStatusType = Literal[
     "DEPLOYED", "FAILED", "INPROGRESS", "READYTODEPLOY", "STOPPED", "STOPPING"
 ]
 DeviceSubsetTypeType = Literal["NAMECONTAINS", "PERCENTAGE", "SELECTION"]
@@ -613,28 +636,40 @@
     "Creating",
     "Deleting",
     "Failed",
     "InService",
     "OutOfService",
     "RollingBack",
     "SystemUpdating",
+    "UpdateRollbackFailed",
     "Updating",
 ]
 ExecutionRoleIdentityConfigType = Literal["DISABLED", "USER_PROFILE_NAME"]
 ExecutionStatusType = Literal[
     "Completed", "CompletedWithViolations", "Failed", "InProgress", "Pending", "Stopped", "Stopping"
 ]
 FailureHandlingPolicyType = Literal["DO_NOTHING", "ROLLBACK_ON_FAILURE"]
 FeatureGroupSortByType = Literal["CreationTime", "FeatureGroupStatus", "Name", "OfflineStoreStatus"]
 FeatureGroupSortOrderType = Literal["Ascending", "Descending"]
 FeatureGroupStatusType = Literal["CreateFailed", "Created", "Creating", "DeleteFailed", "Deleting"]
 FeatureStatusType = Literal["DISABLED", "ENABLED"]
 FeatureTypeType = Literal["Fractional", "Integral", "String"]
 FileSystemAccessModeType = Literal["ro", "rw"]
 FileSystemTypeType = Literal["EFS", "FSxLustre"]
+FillingTypeType = Literal[
+    "backfill",
+    "backfill_value",
+    "frontfill",
+    "frontfill_value",
+    "futurefill",
+    "futurefill_value",
+    "middlefill",
+    "middlefill_value",
+]
+FlatInvocationsType = Literal["Continue", "Stop"]
 FlowDefinitionStatusType = Literal["Active", "Deleting", "Failed", "Initializing"]
 FrameworkType = Literal[
     "DARKNET", "KERAS", "MXNET", "ONNX", "PYTORCH", "SKLEARN", "TENSORFLOW", "TFLITE", "XGBOOST"
 ]
 HubContentSortByType = Literal["CreationTime", "HubContentName", "HubContentStatus"]
 HubContentStatusType = Literal["Available", "DeleteFailed", "Deleting", "ImportFailed", "Importing"]
 HubContentTypeType = Literal["Model", "Notebook"]
@@ -824,14 +859,15 @@
 ]
 ListNotebookInstancesPaginatorName = Literal["list_notebook_instances"]
 ListPipelineExecutionStepsPaginatorName = Literal["list_pipeline_execution_steps"]
 ListPipelineExecutionsPaginatorName = Literal["list_pipeline_executions"]
 ListPipelineParametersForExecutionPaginatorName = Literal["list_pipeline_parameters_for_execution"]
 ListPipelinesPaginatorName = Literal["list_pipelines"]
 ListProcessingJobsPaginatorName = Literal["list_processing_jobs"]
+ListResourceCatalogsPaginatorName = Literal["list_resource_catalogs"]
 ListSpacesPaginatorName = Literal["list_spaces"]
 ListStageDevicesPaginatorName = Literal["list_stage_devices"]
 ListStudioLifecycleConfigsPaginatorName = Literal["list_studio_lifecycle_configs"]
 ListSubscribedWorkteamsPaginatorName = Literal["list_subscribed_workteams"]
 ListTagsPaginatorName = Literal["list_tags"]
 ListTrainingJobsForHyperParameterTuningJobPaginatorName = Literal[
     "list_training_jobs_for_hyper_parameter_tuning_job"
@@ -1151,21 +1187,24 @@
     "UpdateInProgress",
 ]
 RStudioServerProAccessStatusType = Literal["DISABLED", "ENABLED"]
 RStudioServerProUserGroupType = Literal["R_STUDIO_ADMIN", "R_STUDIO_USER"]
 RecommendationJobStatusType = Literal[
     "COMPLETED", "FAILED", "IN_PROGRESS", "PENDING", "STOPPED", "STOPPING"
 ]
+RecommendationJobSupportedEndpointTypeType = Literal["RealTime", "Serverless"]
 RecommendationJobTypeType = Literal["Advanced", "Default"]
 RecommendationStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "NOT_APPLICABLE"]
 RecommendationStepTypeType = Literal["BENCHMARK"]
 RecordWrapperType = Literal["None", "RecordIO"]
 RedshiftResultCompressionTypeType = Literal["BZIP2", "GZIP", "None", "SNAPPY", "ZSTD"]
 RedshiftResultFormatType = Literal["CSV", "PARQUET"]
 RepositoryAccessModeType = Literal["Platform", "Vpc"]
+ResourceCatalogSortByType = Literal["CreationTime"]
+ResourceCatalogSortOrderType = Literal["Ascending", "Descending"]
 ResourceTypeType = Literal[
     "Endpoint",
     "Experiment",
     "ExperimentTrial",
     "ExperimentTrialComponent",
     "FeatureGroup",
     "FeatureMetadata",
@@ -1235,14 +1274,15 @@
     "FAILED",
     "INPROGRESS",
     "READYTODEPLOY",
     "STARTING",
     "STOPPED",
     "STOPPING",
 ]
+StatisticType = Literal["Average", "Maximum", "Minimum", "SampleCount", "Sum"]
 StepStatusType = Literal["Executing", "Failed", "Starting", "Stopped", "Stopping", "Succeeded"]
 StudioLifecycleConfigAppTypeType = Literal["JupyterServer", "KernelGateway"]
 StudioLifecycleConfigSortKeyType = Literal["CreationTime", "LastModifiedTime", "Name"]
 TableFormatType = Literal["Glue", "Iceberg"]
 TargetDeviceType = Literal[
     "aisage",
     "amba_cv2",
@@ -1279,15 +1319,15 @@
     "x86_win32",
     "x86_win64",
 ]
 TargetPlatformAcceleratorType = Literal["INTEL_GRAPHICS", "MALI", "NNA", "NVIDIA"]
 TargetPlatformArchType = Literal["ARM64", "ARM_EABI", "ARM_EABIHF", "X86", "X86_64"]
 TargetPlatformOsType = Literal["ANDROID", "LINUX"]
 TrafficRoutingConfigTypeType = Literal["ALL_AT_ONCE", "CANARY", "LINEAR"]
-TrafficTypeType = Literal["PHASES"]
+TrafficTypeType = Literal["PHASES", "STAIRS"]
 TrainingInputModeType = Literal["FastFile", "File", "Pipe"]
 TrainingInstanceTypeType = Literal[
     "ml.c4.2xlarge",
     "ml.c4.4xlarge",
     "ml.c4.8xlarge",
     "ml.c4.xlarge",
     "ml.c5.18xlarge",
@@ -1329,14 +1369,15 @@
     "ml.p2.8xlarge",
     "ml.p2.xlarge",
     "ml.p3.16xlarge",
     "ml.p3.2xlarge",
     "ml.p3.8xlarge",
     "ml.p3dn.24xlarge",
     "ml.p4d.24xlarge",
+    "ml.p5.48xlarge",
     "ml.trn1.2xlarge",
     "ml.trn1.32xlarge",
     "ml.trn1n.32xlarge",
 ]
 TrainingJobCompletedOrStoppedWaiterName = Literal["training_job_completed_or_stopped"]
 TrainingJobEarlyStoppingTypeType = Literal["Auto", "Off"]
 TrainingJobSortByOptionsType = Literal[
@@ -1379,14 +1420,15 @@
     "ml.p3.8xlarge",
 ]
 TransformJobCompletedOrStoppedWaiterName = Literal["transform_job_completed_or_stopped"]
 TransformJobStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping"]
 TrialComponentPrimaryStatusType = Literal[
     "Completed", "Failed", "InProgress", "Stopped", "Stopping"
 ]
+TtlDurationUnitType = Literal["Days", "Hours", "Minutes", "Seconds", "Weeks"]
 UserProfileSortKeyType = Literal["CreationTime", "LastModifiedTime"]
 UserProfileStatusType = Literal[
     "Delete_Failed", "Deleting", "Failed", "InService", "Pending", "Update_Failed", "Updating"
 ]
 VariantPropertyTypeType = Literal["DataCaptureConfig", "DesiredInstanceCount", "DesiredWeight"]
 VariantStatusType = Literal["ActivatingTraffic", "Baking", "Creating", "Deleting", "Updating"]
 VendorGuidanceType = Literal["ARCHIVED", "NOT_PROVIDED", "STABLE", "TO_BE_ARCHIVED"]
@@ -1404,14 +1446,15 @@
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
@@ -1507,14 +1550,15 @@
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
@@ -1593,26 +1637,28 @@
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
@@ -1807,14 +1853,15 @@
     "list_notebook_instance_lifecycle_configs",
     "list_notebook_instances",
     "list_pipeline_execution_steps",
     "list_pipeline_executions",
     "list_pipeline_parameters_for_execution",
     "list_pipelines",
     "list_processing_jobs",
+    "list_resource_catalogs",
     "list_spaces",
     "list_stage_devices",
     "list_studio_lifecycle_configs",
     "list_subscribed_workteams",
     "list_tags",
     "list_training_jobs",
     "list_training_jobs_for_hyper_parameter_tuning_job",
@@ -1858,14 +1905,15 @@
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

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/literals.pyi` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "ActionStatusType",
+    "AggregationTransformationValueType",
     "AlgorithmSortByType",
     "AlgorithmStatusType",
     "AppImageConfigSortKeyType",
     "AppInstanceTypeType",
     "AppNetworkAccessTypeType",
     "AppSecurityGroupManagementType",
     "AppSortKeyType",
@@ -66,14 +67,15 @@
     "CodeRepositorySortOrderType",
     "CompilationJobStatusType",
     "CompleteOnConvergenceType",
     "CompressionTypeType",
     "ConditionOutcomeType",
     "ContainerModeType",
     "ContentClassifierType",
+    "CrossAccountFilterOptionType",
     "DataDistributionTypeType",
     "DetailedAlgorithmStatusType",
     "DetailedModelPackageStatusType",
     "DeviceDeploymentStatusType",
     "DeviceSubsetTypeType",
     "DirectInternetAccessType",
     "DirectionType",
@@ -92,14 +94,16 @@
     "FeatureGroupSortByType",
     "FeatureGroupSortOrderType",
     "FeatureGroupStatusType",
     "FeatureStatusType",
     "FeatureTypeType",
     "FileSystemAccessModeType",
     "FileSystemTypeType",
+    "FillingTypeType",
+    "FlatInvocationsType",
     "FlowDefinitionStatusType",
     "FrameworkType",
     "HubContentSortByType",
     "HubContentStatusType",
     "HubContentTypeType",
     "HubSortByType",
     "HubStatusType",
@@ -189,14 +193,15 @@
     "ListNotebookInstanceLifecycleConfigsPaginatorName",
     "ListNotebookInstancesPaginatorName",
     "ListPipelineExecutionStepsPaginatorName",
     "ListPipelineExecutionsPaginatorName",
     "ListPipelineParametersForExecutionPaginatorName",
     "ListPipelinesPaginatorName",
     "ListProcessingJobsPaginatorName",
+    "ListResourceCatalogsPaginatorName",
     "ListSpacesPaginatorName",
     "ListStageDevicesPaginatorName",
     "ListStudioLifecycleConfigsPaginatorName",
     "ListSubscribedWorkteamsPaginatorName",
     "ListTagsPaginatorName",
     "ListTrainingJobsForHyperParameterTuningJobPaginatorName",
     "ListTrainingJobsPaginatorName",
@@ -270,21 +275,24 @@
     "ProfilingStatusType",
     "ProjectSortByType",
     "ProjectSortOrderType",
     "ProjectStatusType",
     "RStudioServerProAccessStatusType",
     "RStudioServerProUserGroupType",
     "RecommendationJobStatusType",
+    "RecommendationJobSupportedEndpointTypeType",
     "RecommendationJobTypeType",
     "RecommendationStatusType",
     "RecommendationStepTypeType",
     "RecordWrapperType",
     "RedshiftResultCompressionTypeType",
     "RedshiftResultFormatType",
     "RepositoryAccessModeType",
+    "ResourceCatalogSortByType",
+    "ResourceCatalogSortOrderType",
     "ResourceTypeType",
     "RetentionTypeType",
     "RootAccessType",
     "RuleEvaluationStatusType",
     "S3DataDistributionType",
     "S3DataTypeType",
     "S3ModelDataTypeType",
@@ -306,14 +314,15 @@
     "SortPipelinesByType",
     "SortTrialComponentsByType",
     "SortTrialsByType",
     "SpaceSortKeyType",
     "SpaceStatusType",
     "SplitTypeType",
     "StageStatusType",
+    "StatisticType",
     "StepStatusType",
     "StudioLifecycleConfigAppTypeType",
     "StudioLifecycleConfigSortKeyType",
     "TableFormatType",
     "TargetDeviceType",
     "TargetPlatformAcceleratorType",
     "TargetPlatformArchType",
@@ -327,14 +336,15 @@
     "TrainingJobSortByOptionsType",
     "TrainingJobStatusType",
     "TrainingRepositoryAccessModeType",
     "TransformInstanceTypeType",
     "TransformJobCompletedOrStoppedWaiterName",
     "TransformJobStatusType",
     "TrialComponentPrimaryStatusType",
+    "TtlDurationUnitType",
     "UserProfileSortKeyType",
     "UserProfileStatusType",
     "VariantPropertyTypeType",
     "VariantStatusType",
     "VendorGuidanceType",
     "WarmPoolResourceStatusType",
     "WorkforceStatusType",
@@ -343,14 +353,15 @@
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
 ActionStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping", "Unknown"]
+AggregationTransformationValueType = Literal["avg", "first", "max", "min", "sum"]
 AlgorithmSortByType = Literal["CreationTime", "Name"]
 AlgorithmStatusType = Literal["Completed", "Deleting", "Failed", "InProgress", "Pending"]
 AppImageConfigSortKeyType = Literal["CreationTime", "LastModifiedTime", "Name"]
 AppInstanceTypeType = Literal[
     "ml.c5.12xlarge",
     "ml.c5.18xlarge",
     "ml.c5.24xlarge",
@@ -450,54 +461,65 @@
     "GeneratingExplainabilityReport",
     "GeneratingModelInsightsReport",
     "MaxAutoMLJobRuntimeReached",
     "MaxCandidatesReached",
     "ModelDeploymentError",
     "ModelInsightsError",
     "ModelTuning",
+    "PreTraining",
     "Starting",
     "Stopped",
     "Stopping",
     "TrainingModels",
 ]
 AutoMLJobStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping"]
 AutoMLMetricEnumType = Literal[
     "AUC",
     "Accuracy",
+    "AverageWeightedQuantileLoss",
     "BalancedAccuracy",
     "F1",
     "F1macro",
     "MAE",
+    "MAPE",
+    "MASE",
     "MSE",
     "Precision",
     "PrecisionMacro",
     "R2",
     "RMSE",
     "Recall",
     "RecallMacro",
+    "WAPE",
 ]
 AutoMLMetricExtendedEnumType = Literal[
     "AUC",
     "Accuracy",
+    "AverageWeightedQuantileLoss",
     "BalancedAccuracy",
     "F1",
     "F1macro",
     "InferenceLatency",
     "LogLoss",
     "MAE",
+    "MAPE",
+    "MASE",
     "MSE",
     "Precision",
     "PrecisionMacro",
     "R2",
     "RMSE",
     "Recall",
     "RecallMacro",
+    "WAPE",
 ]
 AutoMLModeType = Literal["AUTO", "ENSEMBLING", "HYPERPARAMETER_TUNING"]
-AutoMLProblemTypeConfigNameType = Literal["ImageClassification", "Tabular", "TextClassification"]
+AutoMLProblemTypeConfigNameType = Literal[
+    "ImageClassification", "Tabular", "TextClassification", "TimeSeriesForecasting"
+]
 AutoMLProcessingUnitType = Literal["CPU", "GPU"]
 AutoMLS3DataTypeType = Literal["AugmentedManifestFile", "ManifestFile", "S3Prefix"]
 AutoMLSortByType = Literal["CreationTime", "Name", "Status"]
 AutoMLSortOrderType = Literal["Ascending", "Descending"]
 AutotuneModeType = Literal["Enabled"]
 AwsManagedHumanLoopRequestSourceType = Literal[
     "AWS/Rekognition/DetectModerationLabels/Image/V3", "AWS/Textract/AnalyzeDocument/Forms/V1"
@@ -582,14 +604,15 @@
     "COMPLETED", "FAILED", "INPROGRESS", "STARTING", "STOPPED", "STOPPING"
 ]
 CompleteOnConvergenceType = Literal["Disabled", "Enabled"]
 CompressionTypeType = Literal["Gzip", "None"]
 ConditionOutcomeType = Literal["False", "True"]
 ContainerModeType = Literal["MultiModel", "SingleModel"]
 ContentClassifierType = Literal["FreeOfAdultContent", "FreeOfPersonallyIdentifiableInformation"]
+CrossAccountFilterOptionType = Literal["CrossAccount", "SameAccount"]
 DataDistributionTypeType = Literal["FullyReplicated", "ShardedByS3Key"]
 DetailedAlgorithmStatusType = Literal["Completed", "Failed", "InProgress", "NotStarted"]
 DetailedModelPackageStatusType = Literal["Completed", "Failed", "InProgress", "NotStarted"]
 DeviceDeploymentStatusType = Literal[
     "DEPLOYED", "FAILED", "INPROGRESS", "READYTODEPLOY", "STOPPED", "STOPPING"
 ]
 DeviceSubsetTypeType = Literal["NAMECONTAINS", "PERCENTAGE", "SELECTION"]
@@ -611,28 +634,40 @@
     "Creating",
     "Deleting",
     "Failed",
     "InService",
     "OutOfService",
     "RollingBack",
     "SystemUpdating",
+    "UpdateRollbackFailed",
     "Updating",
 ]
 ExecutionRoleIdentityConfigType = Literal["DISABLED", "USER_PROFILE_NAME"]
 ExecutionStatusType = Literal[
     "Completed", "CompletedWithViolations", "Failed", "InProgress", "Pending", "Stopped", "Stopping"
 ]
 FailureHandlingPolicyType = Literal["DO_NOTHING", "ROLLBACK_ON_FAILURE"]
 FeatureGroupSortByType = Literal["CreationTime", "FeatureGroupStatus", "Name", "OfflineStoreStatus"]
 FeatureGroupSortOrderType = Literal["Ascending", "Descending"]
 FeatureGroupStatusType = Literal["CreateFailed", "Created", "Creating", "DeleteFailed", "Deleting"]
 FeatureStatusType = Literal["DISABLED", "ENABLED"]
 FeatureTypeType = Literal["Fractional", "Integral", "String"]
 FileSystemAccessModeType = Literal["ro", "rw"]
 FileSystemTypeType = Literal["EFS", "FSxLustre"]
+FillingTypeType = Literal[
+    "backfill",
+    "backfill_value",
+    "frontfill",
+    "frontfill_value",
+    "futurefill",
+    "futurefill_value",
+    "middlefill",
+    "middlefill_value",
+]
+FlatInvocationsType = Literal["Continue", "Stop"]
 FlowDefinitionStatusType = Literal["Active", "Deleting", "Failed", "Initializing"]
 FrameworkType = Literal[
     "DARKNET", "KERAS", "MXNET", "ONNX", "PYTORCH", "SKLEARN", "TENSORFLOW", "TFLITE", "XGBOOST"
 ]
 HubContentSortByType = Literal["CreationTime", "HubContentName", "HubContentStatus"]
 HubContentStatusType = Literal["Available", "DeleteFailed", "Deleting", "ImportFailed", "Importing"]
 HubContentTypeType = Literal["Model", "Notebook"]
@@ -822,14 +857,15 @@
 ]
 ListNotebookInstancesPaginatorName = Literal["list_notebook_instances"]
 ListPipelineExecutionStepsPaginatorName = Literal["list_pipeline_execution_steps"]
 ListPipelineExecutionsPaginatorName = Literal["list_pipeline_executions"]
 ListPipelineParametersForExecutionPaginatorName = Literal["list_pipeline_parameters_for_execution"]
 ListPipelinesPaginatorName = Literal["list_pipelines"]
 ListProcessingJobsPaginatorName = Literal["list_processing_jobs"]
+ListResourceCatalogsPaginatorName = Literal["list_resource_catalogs"]
 ListSpacesPaginatorName = Literal["list_spaces"]
 ListStageDevicesPaginatorName = Literal["list_stage_devices"]
 ListStudioLifecycleConfigsPaginatorName = Literal["list_studio_lifecycle_configs"]
 ListSubscribedWorkteamsPaginatorName = Literal["list_subscribed_workteams"]
 ListTagsPaginatorName = Literal["list_tags"]
 ListTrainingJobsForHyperParameterTuningJobPaginatorName = Literal[
     "list_training_jobs_for_hyper_parameter_tuning_job"
@@ -1149,21 +1185,24 @@
     "UpdateInProgress",
 ]
 RStudioServerProAccessStatusType = Literal["DISABLED", "ENABLED"]
 RStudioServerProUserGroupType = Literal["R_STUDIO_ADMIN", "R_STUDIO_USER"]
 RecommendationJobStatusType = Literal[
     "COMPLETED", "FAILED", "IN_PROGRESS", "PENDING", "STOPPED", "STOPPING"
 ]
+RecommendationJobSupportedEndpointTypeType = Literal["RealTime", "Serverless"]
 RecommendationJobTypeType = Literal["Advanced", "Default"]
 RecommendationStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "NOT_APPLICABLE"]
 RecommendationStepTypeType = Literal["BENCHMARK"]
 RecordWrapperType = Literal["None", "RecordIO"]
 RedshiftResultCompressionTypeType = Literal["BZIP2", "GZIP", "None", "SNAPPY", "ZSTD"]
 RedshiftResultFormatType = Literal["CSV", "PARQUET"]
 RepositoryAccessModeType = Literal["Platform", "Vpc"]
+ResourceCatalogSortByType = Literal["CreationTime"]
+ResourceCatalogSortOrderType = Literal["Ascending", "Descending"]
 ResourceTypeType = Literal[
     "Endpoint",
     "Experiment",
     "ExperimentTrial",
     "ExperimentTrialComponent",
     "FeatureGroup",
     "FeatureMetadata",
@@ -1233,14 +1272,15 @@
     "FAILED",
     "INPROGRESS",
     "READYTODEPLOY",
     "STARTING",
     "STOPPED",
     "STOPPING",
 ]
+StatisticType = Literal["Average", "Maximum", "Minimum", "SampleCount", "Sum"]
 StepStatusType = Literal["Executing", "Failed", "Starting", "Stopped", "Stopping", "Succeeded"]
 StudioLifecycleConfigAppTypeType = Literal["JupyterServer", "KernelGateway"]
 StudioLifecycleConfigSortKeyType = Literal["CreationTime", "LastModifiedTime", "Name"]
 TableFormatType = Literal["Glue", "Iceberg"]
 TargetDeviceType = Literal[
     "aisage",
     "amba_cv2",
@@ -1277,15 +1317,15 @@
     "x86_win32",
     "x86_win64",
 ]
 TargetPlatformAcceleratorType = Literal["INTEL_GRAPHICS", "MALI", "NNA", "NVIDIA"]
 TargetPlatformArchType = Literal["ARM64", "ARM_EABI", "ARM_EABIHF", "X86", "X86_64"]
 TargetPlatformOsType = Literal["ANDROID", "LINUX"]
 TrafficRoutingConfigTypeType = Literal["ALL_AT_ONCE", "CANARY", "LINEAR"]
-TrafficTypeType = Literal["PHASES"]
+TrafficTypeType = Literal["PHASES", "STAIRS"]
 TrainingInputModeType = Literal["FastFile", "File", "Pipe"]
 TrainingInstanceTypeType = Literal[
     "ml.c4.2xlarge",
     "ml.c4.4xlarge",
     "ml.c4.8xlarge",
     "ml.c4.xlarge",
     "ml.c5.18xlarge",
@@ -1327,14 +1367,15 @@
     "ml.p2.8xlarge",
     "ml.p2.xlarge",
     "ml.p3.16xlarge",
     "ml.p3.2xlarge",
     "ml.p3.8xlarge",
     "ml.p3dn.24xlarge",
     "ml.p4d.24xlarge",
+    "ml.p5.48xlarge",
     "ml.trn1.2xlarge",
     "ml.trn1.32xlarge",
     "ml.trn1n.32xlarge",
 ]
 TrainingJobCompletedOrStoppedWaiterName = Literal["training_job_completed_or_stopped"]
 TrainingJobEarlyStoppingTypeType = Literal["Auto", "Off"]
 TrainingJobSortByOptionsType = Literal[
@@ -1377,14 +1418,15 @@
     "ml.p3.8xlarge",
 ]
 TransformJobCompletedOrStoppedWaiterName = Literal["transform_job_completed_or_stopped"]
 TransformJobStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping"]
 TrialComponentPrimaryStatusType = Literal[
     "Completed", "Failed", "InProgress", "Stopped", "Stopping"
 ]
+TtlDurationUnitType = Literal["Days", "Hours", "Minutes", "Seconds", "Weeks"]
 UserProfileSortKeyType = Literal["CreationTime", "LastModifiedTime"]
 UserProfileStatusType = Literal[
     "Delete_Failed", "Deleting", "Failed", "InService", "Pending", "Update_Failed", "Updating"
 ]
 VariantPropertyTypeType = Literal["DataCaptureConfig", "DesiredInstanceCount", "DesiredWeight"]
 VariantStatusType = Literal["ActivatingTraffic", "Baking", "Creating", "Deleting", "Updating"]
 VendorGuidanceType = Literal["ARCHIVED", "NOT_PROVIDED", "STABLE", "TO_BE_ARCHIVED"]
@@ -1402,14 +1444,15 @@
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
@@ -1505,14 +1548,15 @@
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
@@ -1591,26 +1635,28 @@
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
@@ -1805,14 +1851,15 @@
     "list_notebook_instance_lifecycle_configs",
     "list_notebook_instances",
     "list_pipeline_execution_steps",
     "list_pipeline_executions",
     "list_pipeline_parameters_for_execution",
     "list_pipelines",
     "list_processing_jobs",
+    "list_resource_catalogs",
     "list_spaces",
     "list_stage_devices",
     "list_studio_lifecycle_configs",
     "list_subscribed_workteams",
     "list_tags",
     "list_training_jobs",
     "list_training_jobs_for_hyper_parameter_tuning_job",
@@ -1856,14 +1903,15 @@
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

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/paginator.py` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         ListNotebookInstanceLifecycleConfigsPaginator,
         ListNotebookInstancesPaginator,
         ListPipelineExecutionStepsPaginator,
         ListPipelineExecutionsPaginator,
         ListPipelineParametersForExecutionPaginator,
         ListPipelinesPaginator,
         ListProcessingJobsPaginator,
+        ListResourceCatalogsPaginator,
         ListSpacesPaginator,
         ListStageDevicesPaginator,
         ListStudioLifecycleConfigsPaginator,
         ListSubscribedWorkteamsPaginator,
         ListTagsPaginator,
         ListTrainingJobsPaginator,
         ListTrainingJobsForHyperParameterTuningJobPaginator,
@@ -134,14 +135,15 @@
         list_notebook_instance_lifecycle_configs_paginator: ListNotebookInstanceLifecycleConfigsPaginator = client.get_paginator("list_notebook_instance_lifecycle_configs")
         list_notebook_instances_paginator: ListNotebookInstancesPaginator = client.get_paginator("list_notebook_instances")
         list_pipeline_execution_steps_paginator: ListPipelineExecutionStepsPaginator = client.get_paginator("list_pipeline_execution_steps")
         list_pipeline_executions_paginator: ListPipelineExecutionsPaginator = client.get_paginator("list_pipeline_executions")
         list_pipeline_parameters_for_execution_paginator: ListPipelineParametersForExecutionPaginator = client.get_paginator("list_pipeline_parameters_for_execution")
         list_pipelines_paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
         list_processing_jobs_paginator: ListProcessingJobsPaginator = client.get_paginator("list_processing_jobs")
+        list_resource_catalogs_paginator: ListResourceCatalogsPaginator = client.get_paginator("list_resource_catalogs")
         list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
         list_stage_devices_paginator: ListStageDevicesPaginator = client.get_paginator("list_stage_devices")
         list_studio_lifecycle_configs_paginator: ListStudioLifecycleConfigsPaginator = client.get_paginator("list_studio_lifecycle_configs")
         list_subscribed_workteams_paginator: ListSubscribedWorkteamsPaginator = client.get_paginator("list_subscribed_workteams")
         list_tags_paginator: ListTagsPaginator = client.get_paginator("list_tags")
         list_training_jobs_paginator: ListTrainingJobsPaginator = client.get_paginator("list_training_jobs")
         list_training_jobs_for_hyper_parameter_tuning_job_paginator: ListTrainingJobsForHyperParameterTuningJobPaginator = client.get_paginator("list_training_jobs_for_hyper_parameter_tuning_job")
@@ -168,14 +170,15 @@
     AutoMLSortByType,
     AutoMLSortOrderType,
     CandidateSortByType,
     CandidateStatusType,
     CodeRepositorySortByType,
     CodeRepositorySortOrderType,
     CompilationJobStatusType,
+    CrossAccountFilterOptionType,
     EdgePackagingJobStatusType,
     EndpointConfigSortKeyType,
     EndpointSortKeyType,
     EndpointStatusType,
     ExecutionStatusType,
     FeatureGroupSortByType,
     FeatureGroupSortOrderType,
@@ -217,14 +220,15 @@
     NotebookInstanceSortKeyType,
     NotebookInstanceSortOrderType,
     NotebookInstanceStatusType,
     OfflineStoreStatusValueType,
     OrderKeyType,
     ProcessingJobStatusType,
     RecommendationJobStatusType,
+    ResourceCatalogSortOrderType,
     ResourceTypeType,
     ScheduleStatusType,
     SearchSortOrderType,
     SortActionsByType,
     SortAssociationsByType,
     SortByType,
     SortContextsByType,
@@ -296,14 +300,15 @@
     ListNotebookInstanceLifecycleConfigsOutputTypeDef,
     ListNotebookInstancesOutputTypeDef,
     ListPipelineExecutionsResponseTypeDef,
     ListPipelineExecutionStepsResponseTypeDef,
     ListPipelineParametersForExecutionResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListProcessingJobsResponseTypeDef,
+    ListResourceCatalogsResponseTypeDef,
     ListSpacesResponseTypeDef,
     ListStageDevicesResponseTypeDef,
     ListStudioLifecycleConfigsResponseTypeDef,
     ListSubscribedWorkteamsResponseTypeDef,
     ListTagsOutputTypeDef,
     ListTrainingJobsForHyperParameterTuningJobResponseTypeDef,
     ListTrainingJobsResponseTypeDef,
@@ -377,14 +382,15 @@
     "ListNotebookInstanceLifecycleConfigsPaginator",
     "ListNotebookInstancesPaginator",
     "ListPipelineExecutionStepsPaginator",
     "ListPipelineExecutionsPaginator",
     "ListPipelineParametersForExecutionPaginator",
     "ListPipelinesPaginator",
     "ListProcessingJobsPaginator",
+    "ListResourceCatalogsPaginator",
     "ListSpacesPaginator",
     "ListStageDevicesPaginator",
     "ListStudioLifecycleConfigsPaginator",
     "ListSubscribedWorkteamsPaginator",
     "ListTagsPaginator",
     "ListTrainingJobsPaginator",
     "ListTrainingJobsForHyperParameterTuningJobPaginator",
@@ -1642,14 +1648,36 @@
     ) -> AsyncIterator[ListProcessingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListProcessingJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listprocessingjobspaginator)
         """
 
 
+class ListResourceCatalogsPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListResourceCatalogs)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listresourcecatalogspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        NameContains: str = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
+        SortOrder: ResourceCatalogSortOrderType = ...,
+        SortBy: Literal["CreationTime"] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListResourceCatalogsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListResourceCatalogs.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listresourcecatalogspaginator)
+        """
+
+
 class ListSpacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListSpaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listspacespaginator)
     """
 
     def paginate(
@@ -1931,13 +1959,14 @@
     def paginate(
         self,
         *,
         Resource: ResourceTypeType,
         SearchExpression: "SearchExpressionTypeDef" = ...,
         SortBy: str = ...,
         SortOrder: SearchSortOrderType = ...,
+        CrossAccountFilterOption: CrossAccountFilterOptionType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.Search.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#searchpaginator)
         """
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/paginator.pyi` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         ListNotebookInstanceLifecycleConfigsPaginator,
         ListNotebookInstancesPaginator,
         ListPipelineExecutionStepsPaginator,
         ListPipelineExecutionsPaginator,
         ListPipelineParametersForExecutionPaginator,
         ListPipelinesPaginator,
         ListProcessingJobsPaginator,
+        ListResourceCatalogsPaginator,
         ListSpacesPaginator,
         ListStageDevicesPaginator,
         ListStudioLifecycleConfigsPaginator,
         ListSubscribedWorkteamsPaginator,
         ListTagsPaginator,
         ListTrainingJobsPaginator,
         ListTrainingJobsForHyperParameterTuningJobPaginator,
@@ -134,14 +135,15 @@
         list_notebook_instance_lifecycle_configs_paginator: ListNotebookInstanceLifecycleConfigsPaginator = client.get_paginator("list_notebook_instance_lifecycle_configs")
         list_notebook_instances_paginator: ListNotebookInstancesPaginator = client.get_paginator("list_notebook_instances")
         list_pipeline_execution_steps_paginator: ListPipelineExecutionStepsPaginator = client.get_paginator("list_pipeline_execution_steps")
         list_pipeline_executions_paginator: ListPipelineExecutionsPaginator = client.get_paginator("list_pipeline_executions")
         list_pipeline_parameters_for_execution_paginator: ListPipelineParametersForExecutionPaginator = client.get_paginator("list_pipeline_parameters_for_execution")
         list_pipelines_paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
         list_processing_jobs_paginator: ListProcessingJobsPaginator = client.get_paginator("list_processing_jobs")
+        list_resource_catalogs_paginator: ListResourceCatalogsPaginator = client.get_paginator("list_resource_catalogs")
         list_spaces_paginator: ListSpacesPaginator = client.get_paginator("list_spaces")
         list_stage_devices_paginator: ListStageDevicesPaginator = client.get_paginator("list_stage_devices")
         list_studio_lifecycle_configs_paginator: ListStudioLifecycleConfigsPaginator = client.get_paginator("list_studio_lifecycle_configs")
         list_subscribed_workteams_paginator: ListSubscribedWorkteamsPaginator = client.get_paginator("list_subscribed_workteams")
         list_tags_paginator: ListTagsPaginator = client.get_paginator("list_tags")
         list_training_jobs_paginator: ListTrainingJobsPaginator = client.get_paginator("list_training_jobs")
         list_training_jobs_for_hyper_parameter_tuning_job_paginator: ListTrainingJobsForHyperParameterTuningJobPaginator = client.get_paginator("list_training_jobs_for_hyper_parameter_tuning_job")
@@ -168,14 +170,15 @@
     AutoMLSortByType,
     AutoMLSortOrderType,
     CandidateSortByType,
     CandidateStatusType,
     CodeRepositorySortByType,
     CodeRepositorySortOrderType,
     CompilationJobStatusType,
+    CrossAccountFilterOptionType,
     EdgePackagingJobStatusType,
     EndpointConfigSortKeyType,
     EndpointSortKeyType,
     EndpointStatusType,
     ExecutionStatusType,
     FeatureGroupSortByType,
     FeatureGroupSortOrderType,
@@ -217,14 +220,15 @@
     NotebookInstanceSortKeyType,
     NotebookInstanceSortOrderType,
     NotebookInstanceStatusType,
     OfflineStoreStatusValueType,
     OrderKeyType,
     ProcessingJobStatusType,
     RecommendationJobStatusType,
+    ResourceCatalogSortOrderType,
     ResourceTypeType,
     ScheduleStatusType,
     SearchSortOrderType,
     SortActionsByType,
     SortAssociationsByType,
     SortByType,
     SortContextsByType,
@@ -296,14 +300,15 @@
     ListNotebookInstanceLifecycleConfigsOutputTypeDef,
     ListNotebookInstancesOutputTypeDef,
     ListPipelineExecutionsResponseTypeDef,
     ListPipelineExecutionStepsResponseTypeDef,
     ListPipelineParametersForExecutionResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListProcessingJobsResponseTypeDef,
+    ListResourceCatalogsResponseTypeDef,
     ListSpacesResponseTypeDef,
     ListStageDevicesResponseTypeDef,
     ListStudioLifecycleConfigsResponseTypeDef,
     ListSubscribedWorkteamsResponseTypeDef,
     ListTagsOutputTypeDef,
     ListTrainingJobsForHyperParameterTuningJobResponseTypeDef,
     ListTrainingJobsResponseTypeDef,
@@ -376,14 +381,15 @@
     "ListNotebookInstanceLifecycleConfigsPaginator",
     "ListNotebookInstancesPaginator",
     "ListPipelineExecutionStepsPaginator",
     "ListPipelineExecutionsPaginator",
     "ListPipelineParametersForExecutionPaginator",
     "ListPipelinesPaginator",
     "ListProcessingJobsPaginator",
+    "ListResourceCatalogsPaginator",
     "ListSpacesPaginator",
     "ListStageDevicesPaginator",
     "ListStudioLifecycleConfigsPaginator",
     "ListSubscribedWorkteamsPaginator",
     "ListTagsPaginator",
     "ListTrainingJobsPaginator",
     "ListTrainingJobsForHyperParameterTuningJobPaginator",
@@ -1584,14 +1590,35 @@
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProcessingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListProcessingJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listprocessingjobspaginator)
         """
 
+class ListResourceCatalogsPaginator(AioPaginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListResourceCatalogs)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listresourcecatalogspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        NameContains: str = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
+        SortOrder: ResourceCatalogSortOrderType = ...,
+        SortBy: Literal["CreationTime"] = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> AsyncIterator[ListResourceCatalogsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListResourceCatalogs.paginate)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listresourcecatalogspaginator)
+        """
+
 class ListSpacesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListSpaces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listspacespaginator)
     """
 
     def paginate(
@@ -1860,13 +1887,14 @@
     def paginate(
         self,
         *,
         Resource: ResourceTypeType,
         SearchExpression: "SearchExpressionTypeDef" = ...,
         SortBy: str = ...,
         SortOrder: SearchSortOrderType = ...,
+        CrossAccountFilterOption: CrossAccountFilterOptionType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.Search.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#searchpaginator)
         """
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/type_defs.py` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ActionStatusType,
+    AggregationTransformationValueType,
     AlgorithmSortByType,
     AlgorithmStatusType,
     AppImageConfigSortKeyType,
     AppInstanceTypeType,
     AppNetworkAccessTypeType,
     AppSecurityGroupManagementType,
     AppStatusType,
@@ -61,14 +62,15 @@
     CodeRepositorySortOrderType,
     CompilationJobStatusType,
     CompleteOnConvergenceType,
     CompressionTypeType,
     ConditionOutcomeType,
     ContainerModeType,
     ContentClassifierType,
+    CrossAccountFilterOptionType,
     DataDistributionTypeType,
     DetailedAlgorithmStatusType,
     DetailedModelPackageStatusType,
     DeviceDeploymentStatusType,
     DeviceSubsetTypeType,
     DirectInternetAccessType,
     DirectionType,
@@ -84,14 +86,16 @@
     FeatureGroupSortByType,
     FeatureGroupSortOrderType,
     FeatureGroupStatusType,
     FeatureStatusType,
     FeatureTypeType,
     FileSystemAccessModeType,
     FileSystemTypeType,
+    FillingTypeType,
+    FlatInvocationsType,
     FlowDefinitionStatusType,
     FrameworkType,
     HubContentSortByType,
     HubContentStatusType,
     HubContentTypeType,
     HubSortByType,
     HubStatusType,
@@ -178,20 +182,22 @@
     ProductionVariantAcceleratorTypeType,
     ProductionVariantInstanceTypeType,
     ProfilingStatusType,
     ProjectSortByType,
     ProjectSortOrderType,
     ProjectStatusType,
     RecommendationJobStatusType,
+    RecommendationJobSupportedEndpointTypeType,
     RecommendationJobTypeType,
     RecommendationStatusType,
     RecordWrapperType,
     RedshiftResultCompressionTypeType,
     RedshiftResultFormatType,
     RepositoryAccessModeType,
+    ResourceCatalogSortOrderType,
     ResourceTypeType,
     RetentionTypeType,
     RootAccessType,
     RStudioServerProAccessStatusType,
     RStudioServerProUserGroupType,
     RuleEvaluationStatusType,
     S3DataDistributionType,
@@ -213,32 +219,35 @@
     SortPipelinesByType,
     SortTrialComponentsByType,
     SortTrialsByType,
     SpaceSortKeyType,
     SpaceStatusType,
     SplitTypeType,
     StageStatusType,
+    StatisticType,
     StepStatusType,
     StudioLifecycleConfigAppTypeType,
     StudioLifecycleConfigSortKeyType,
     TableFormatType,
     TargetDeviceType,
     TargetPlatformAcceleratorType,
     TargetPlatformArchType,
     TargetPlatformOsType,
     TrafficRoutingConfigTypeType,
+    TrafficTypeType,
     TrainingInputModeType,
     TrainingInstanceTypeType,
     TrainingJobEarlyStoppingTypeType,
     TrainingJobSortByOptionsType,
     TrainingJobStatusType,
     TrainingRepositoryAccessModeType,
     TransformInstanceTypeType,
     TransformJobStatusType,
     TrialComponentPrimaryStatusType,
+    TtlDurationUnitType,
     UserProfileSortKeyType,
     UserProfileStatusType,
     VariantPropertyTypeType,
     VariantStatusType,
     VendorGuidanceType,
     WarmPoolResourceStatusType,
     WorkforceStatusType,
@@ -262,75 +271,65 @@
     "AgentVersionTypeDef",
     "AlarmTypeDef",
     "MetricDefinitionTypeDef",
     "AlgorithmStatusItemTypeDef",
     "AlgorithmSummaryTypeDef",
     "AnnotationConsolidationConfigTypeDef",
     "AppDetailsTypeDef",
-    "AppSpecificationOutputTypeDef",
     "AppSpecificationTypeDef",
     "ArtifactSourceTypeTypeDef",
     "AssociateTrialComponentRequestRequestTypeDef",
     "AsyncInferenceClientConfigTypeDef",
-    "AsyncInferenceNotificationConfigOutputTypeDef",
     "AsyncInferenceNotificationConfigTypeDef",
     "AthenaDatasetDefinitionTypeDef",
-    "AutoMLAlgorithmConfigOutputTypeDef",
     "AutoMLAlgorithmConfigTypeDef",
     "AutoMLCandidateStepTypeDef",
     "AutoMLContainerDefinitionTypeDef",
     "FinalAutoMLJobObjectiveMetricTypeDef",
     "AutoMLS3DataSourceTypeDef",
     "AutoMLDataSplitConfigTypeDef",
     "AutoMLJobArtifactsTypeDef",
     "AutoMLJobCompletionCriteriaTypeDef",
     "AutoMLJobObjectiveTypeDef",
     "AutoMLJobStepMetadataTypeDef",
     "AutoMLPartialFailureReasonTypeDef",
     "AutoMLOutputDataConfigTypeDef",
     "TabularResolvedAttributesTypeDef",
-    "VpcConfigOutputTypeDef",
     "VpcConfigTypeDef",
     "AutoParameterTypeDef",
     "AutotuneTypeDef",
     "BatchDataCaptureConfigTypeDef",
     "BatchDescribeModelPackageErrorTypeDef",
     "BatchDescribeModelPackageInputRequestTypeDef",
     "BestObjectiveNotImprovingTypeDef",
     "MetricsSourceTypeDef",
     "CacheHitResultTypeDef",
     "OutputParameterTypeDef",
     "CandidateArtifactLocationsTypeDef",
     "MetricDatumTypeDef",
     "ModelRegisterSettingsTypeDef",
     "TimeSeriesForecastingSettingsTypeDef",
+    "WorkspaceSettingsTypeDef",
     "CapacitySizeTypeDef",
-    "CaptureContentTypeHeaderOutputTypeDef",
     "CaptureContentTypeHeaderTypeDef",
     "CaptureOptionTypeDef",
-    "CategoricalParameterOutputTypeDef",
-    "CategoricalParameterRangeOutputTypeDef",
-    "CategoricalParameterRangeSpecificationOutputTypeDef",
     "CategoricalParameterRangeSpecificationTypeDef",
     "CategoricalParameterRangeTypeDef",
     "CategoricalParameterTypeDef",
-    "ShuffleConfigTypeDef",
-    "ChannelSpecificationOutputTypeDef",
     "ChannelSpecificationTypeDef",
+    "ShuffleConfigTypeDef",
     "CheckpointConfigTypeDef",
     "ClarifyCheckStepMetadataTypeDef",
-    "ClarifyInferenceConfigOutputTypeDef",
     "ClarifyInferenceConfigTypeDef",
     "ClarifyShapBaselineConfigTypeDef",
     "ClarifyTextConfigTypeDef",
     "GitConfigTypeDef",
     "CodeRepositoryTypeDef",
     "CognitoConfigTypeDef",
     "CognitoMemberDefinitionTypeDef",
-    "CollectionConfigurationOutputTypeDef",
     "CollectionConfigurationTypeDef",
     "CompilationJobSummaryTypeDef",
     "ConditionStepMetadataTypeDef",
     "MultiModelConfigTypeDef",
     "ContextSourceTypeDef",
     "ContinuousParameterRangeSpecificationTypeDef",
     "ContinuousParameterRangeTypeDef",
@@ -363,16 +362,18 @@
     "NotebookInstanceLifecycleHookTypeDef",
     "ParallelismConfigurationTypeDef",
     "PipelineDefinitionS3LocationTypeDef",
     "CreatePresignedDomainUrlRequestRequestTypeDef",
     "CreatePresignedNotebookInstanceUrlInputRequestTypeDef",
     "ExperimentConfigTypeDef",
     "ProcessingStoppingConditionTypeDef",
+    "DebugRuleConfigurationTypeDef",
     "OutputDataConfigTypeDef",
     "ProfilerConfigTypeDef",
+    "ProfilerRuleConfigurationTypeDef",
     "RetryStrategyTypeDef",
     "TensorBoardOutputConfigTypeDef",
     "DataProcessingTypeDef",
     "ModelClientConfigTypeDef",
     "TransformOutputTypeDef",
     "TransformResourcesTypeDef",
     "TimestampTypeDef",
@@ -380,26 +381,23 @@
     "TrialComponentParameterValueTypeDef",
     "TrialComponentStatusTypeDef",
     "OidcConfigTypeDef",
     "SourceIpConfigTypeDef",
     "WorkforceVpcConfigRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "CustomImageTypeDef",
+    "CustomizedMetricSpecificationTypeDef",
     "DataCaptureConfigSummaryTypeDef",
     "DataCatalogConfigTypeDef",
-    "DataQualityAppSpecificationOutputTypeDef",
     "MonitoringConstraintsResourceTypeDef",
     "MonitoringStatisticsResourceTypeDef",
     "EndpointInputTypeDef",
     "FileSystemDataSourceTypeDef",
-    "S3DataSourceOutputTypeDef",
     "S3DataSourceTypeDef",
     "RedshiftDatasetDefinitionTypeDef",
-    "DebugRuleConfigurationOutputTypeDef",
-    "DebugRuleConfigurationTypeDef",
     "DebugRuleEvaluationStatusTypeDef",
     "DeleteActionRequestRequestTypeDef",
     "DeleteAlgorithmInputRequestTypeDef",
     "DeleteAppImageConfigRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteCodeRepositoryInputRequestTypeDef",
@@ -439,32 +437,30 @@
     "DeleteTrialComponentRequestRequestTypeDef",
     "DeleteTrialRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
     "DeleteWorkforceRequestRequestTypeDef",
     "DeleteWorkteamRequestRequestTypeDef",
     "DeployedImageTypeDef",
     "RealTimeInferenceRecommendationTypeDef",
-    "DeviceSelectionConfigOutputTypeDef",
+    "DeviceSelectionConfigTypeDef",
     "EdgeDeploymentConfigTypeDef",
     "EdgeDeploymentStatusTypeDef",
-    "DeviceSelectionConfigTypeDef",
     "DeregisterDevicesRequestRequestTypeDef",
     "DescribeActionRequestRequestTypeDef",
     "DescribeAlgorithmInputRequestTypeDef",
     "DescribeAppImageConfigRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeArtifactRequestRequestTypeDef",
     "DescribeAutoMLJobRequestRequestTypeDef",
     "ModelDeployResultTypeDef",
     "DescribeAutoMLJobV2RequestRequestTypeDef",
     "DescribeCodeRepositoryInputRequestTypeDef",
     "DescribeCompilationJobRequestRequestTypeDef",
     "ModelArtifactsTypeDef",
     "ModelDigestsTypeDef",
-    "NeoVpcConfigOutputTypeDef",
     "DescribeContextRequestRequestTypeDef",
     "DescribeDataQualityJobDefinitionRequestRequestTypeDef",
     "DescribeDeviceFleetRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "EdgeModelTypeDef",
     "DescribeDomainRequestRequestTypeDef",
     "DescribeEdgeDeploymentPlanRequestRequestTypeDef",
@@ -491,32 +487,28 @@
     "HyperParameterTuningJobConsumedResourcesTypeDef",
     "ObjectiveStatusCountersTypeDef",
     "TrainingJobStatusCountersTypeDef",
     "DescribeImageRequestRequestTypeDef",
     "DescribeImageVersionRequestRequestTypeDef",
     "DescribeInferenceExperimentRequestRequestTypeDef",
     "EndpointMetadataTypeDef",
-    "InferenceExperimentScheduleOutputTypeDef",
     "DescribeInferenceRecommendationsJobRequestRequestTypeDef",
     "DescribeLabelingJobRequestRequestTypeDef",
     "LabelCountersTypeDef",
     "LabelingJobOutputTypeDef",
     "DescribeLineageGroupRequestRequestTypeDef",
     "DescribeModelBiasJobDefinitionRequestRequestTypeDef",
-    "ModelBiasAppSpecificationOutputTypeDef",
     "DescribeModelCardExportJobRequestRequestTypeDef",
     "ModelCardExportArtifactsTypeDef",
     "DescribeModelCardRequestRequestTypeDef",
     "DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef",
-    "ModelExplainabilityAppSpecificationOutputTypeDef",
     "DescribeModelInputRequestTypeDef",
     "DescribeModelPackageGroupInputRequestTypeDef",
     "DescribeModelPackageInputRequestTypeDef",
     "DescribeModelQualityJobDefinitionRequestRequestTypeDef",
-    "ModelQualityAppSpecificationOutputTypeDef",
     "DescribeMonitoringScheduleRequestRequestTypeDef",
     "MonitoringExecutionSummaryTypeDef",
     "DescribeNotebookInstanceInputRequestTypeDef",
     "DescribeNotebookInstanceLifecycleConfigInputRequestTypeDef",
     "DescribePipelineDefinitionForExecutionRequestRequestTypeDef",
     "DescribePipelineExecutionRequestRequestTypeDef",
     "PipelineExperimentConfigTypeDef",
@@ -526,16 +518,14 @@
     "ServiceCatalogProvisionedProductDetailsTypeDef",
     "DescribeSpaceRequestRequestTypeDef",
     "DescribeStudioLifecycleConfigRequestRequestTypeDef",
     "DescribeSubscribedWorkteamRequestRequestTypeDef",
     "SubscribedWorkteamTypeDef",
     "DescribeTrainingJobRequestRequestTypeDef",
     "MetricDataTypeDef",
-    "ProfilerConfigOutputTypeDef",
-    "ProfilerRuleConfigurationOutputTypeDef",
     "ProfilerRuleEvaluationStatusTypeDef",
     "SecondaryStatusTransitionTypeDef",
     "WarmPoolStatusTypeDef",
     "DescribeTransformJobRequestRequestTypeDef",
     "DescribeTrialComponentRequestRequestTypeDef",
     "TrialComponentMetricSummaryTypeDef",
     "TrialComponentSourceTypeDef",
@@ -556,26 +546,28 @@
     "EMRStepMetadataTypeDef",
     "EdgeDeploymentPlanSummaryTypeDef",
     "EdgeModelStatTypeDef",
     "EdgePackagingJobSummaryTypeDef",
     "EdgeTypeDef",
     "EndpointConfigSummaryTypeDef",
     "EndpointInfoTypeDef",
-    "EndpointOutputConfigurationTypeDef",
+    "ProductionVariantServerlessConfigTypeDef",
     "InferenceMetricsTypeDef",
     "EndpointSummaryTypeDef",
     "EnvironmentParameterTypeDef",
     "FailStepMetadataTypeDef",
     "FileSystemConfigTypeDef",
     "FilterTypeDef",
     "FinalHyperParameterTuningJobObjectiveMetricTypeDef",
     "FlowDefinitionSummaryTypeDef",
     "GetDeviceFleetReportRequestRequestTypeDef",
     "GetLineageGroupPolicyRequestRequestTypeDef",
     "GetModelPackageGroupPolicyInputRequestTypeDef",
+    "ScalingPolicyObjectiveTypeDef",
+    "ScalingPolicyMetricTypeDef",
     "PropertyNameSuggestionTypeDef",
     "GitConfigForUpdateTypeDef",
     "HubContentInfoTypeDef",
     "HubInfoTypeDef",
     "HumanLoopActivationConditionsConfigTypeDef",
     "UiConfigTypeDef",
     "HumanTaskUiSummaryTypeDef",
@@ -591,15 +583,14 @@
     "RecommendationMetricsTypeDef",
     "InferenceRecommendationsJobTypeDef",
     "InstanceGroupTypeDef",
     "IntegerParameterRangeSpecificationTypeDef",
     "IntegerParameterRangeTypeDef",
     "KernelSpecTypeDef",
     "LabelCountersForWorkteamTypeDef",
-    "LabelingJobDataAttributesOutputTypeDef",
     "LabelingJobDataAttributesTypeDef",
     "LabelingJobS3DataSourceTypeDef",
     "LabelingJobSnsDataSourceTypeDef",
     "LineageGroupSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
@@ -622,51 +613,51 @@
     "ListPipelineExecutionStepsRequestRequestTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "ListPipelineParametersForExecutionRequestRequestTypeDef",
     "ParameterTypeDef",
     "PipelineSummaryTypeDef",
     "ProcessingJobSummaryTypeDef",
     "ProjectSummaryTypeDef",
+    "ResourceCatalogTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceDetailsTypeDef",
     "ListStageDevicesRequestRequestTypeDef",
     "StudioLifecycleConfigDetailsTypeDef",
     "ListSubscribedWorkteamsRequestRequestTypeDef",
     "ListTagsInputRequestTypeDef",
     "ListTrainingJobsForHyperParameterTuningJobRequestRequestTypeDef",
     "TransformJobSummaryTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileDetailsTypeDef",
     "ListWorkforcesRequestRequestTypeDef",
     "ListWorkteamsRequestRequestTypeDef",
-    "OidcMemberDefinitionOutputTypeDef",
     "OidcMemberDefinitionTypeDef",
+    "PredefinedMetricSpecificationTypeDef",
     "MonitoringGroundTruthS3InputTypeDef",
     "ModelDashboardEndpointTypeDef",
     "ModelDashboardIndicatorActionTypeDef",
     "S3ModelDataSourceTypeDef",
     "RealTimeInferenceConfigTypeDef",
     "ModelInputTypeDef",
     "ModelLatencyThresholdTypeDef",
     "ModelMetadataFilterTypeDef",
     "ModelPackageStatusItemTypeDef",
     "ModelStepMetadataTypeDef",
-    "MonitoringAppSpecificationOutputTypeDef",
     "MonitoringAppSpecificationTypeDef",
     "MonitoringClusterConfigTypeDef",
     "MonitoringCsvDatasetFormatTypeDef",
     "MonitoringJsonDatasetFormatTypeDef",
     "MonitoringS3OutputTypeDef",
     "ScheduleConfigTypeDef",
     "S3StorageConfigTypeDef",
     "OidcConfigForResponseTypeDef",
     "OnlineStoreSecurityConfigTypeDef",
+    "TtlDurationTypeDef",
     "TargetPlatformTypeDef",
     "ParentTypeDef",
-    "ProductionVariantServerlessConfigTypeDef",
     "ProductionVariantStatusTypeDef",
     "PhaseTypeDef",
     "ProcessingJobStepMetadataTypeDef",
     "QualityCheckStepMetadataTypeDef",
     "RegisterModelStepMetadataTypeDef",
     "TrainingJobStepMetadataTypeDef",
     "TransformJobStepMetadataTypeDef",
@@ -674,37 +665,34 @@
     "SelectiveExecutionResultTypeDef",
     "ProcessingClusterConfigTypeDef",
     "ProcessingFeatureStoreOutputTypeDef",
     "ProcessingS3InputTypeDef",
     "ProcessingS3OutputTypeDef",
     "ProductionVariantCoreDumpConfigTypeDef",
     "ProfilerConfigForUpdateTypeDef",
-    "ProfilerRuleConfigurationTypeDef",
     "PropertyNameQueryTypeDef",
     "ProvisioningParameterTypeDef",
     "USDTypeDef",
     "PutModelPackageGroupPolicyInputRequestTypeDef",
     "VertexTypeDef",
     "RStudioServerProAppSettingsTypeDef",
     "RecommendationJobCompiledOutputConfigTypeDef",
-    "RecommendationJobPayloadConfigOutputTypeDef",
     "RecommendationJobPayloadConfigTypeDef",
     "RecommendationJobResourceLimitTypeDef",
-    "RecommendationJobVpcConfigOutputTypeDef",
     "RecommendationJobVpcConfigTypeDef",
     "RenderableTaskTypeDef",
     "RenderingErrorTypeDef",
     "ResourceConfigForUpdateTypeDef",
     "SearchRequestRequestTypeDef",
     "SelectedStepTypeDef",
     "SendPipelineExecutionStepFailureRequestRequestTypeDef",
     "ShadowModelVariantConfigTypeDef",
     "SharingSettingsTypeDef",
     "SourceAlgorithmTypeDef",
-    "SourceIpConfigOutputTypeDef",
+    "StairsTypeDef",
     "StartEdgeDeploymentStageRequestRequestTypeDef",
     "StartInferenceExperimentRequestRequestTypeDef",
     "StartMonitoringScheduleRequestRequestTypeDef",
     "StartNotebookInstanceInputRequestTypeDef",
     "StopAutoMLJobRequestRequestTypeDef",
     "StopCompilationJobRequestRequestTypeDef",
     "StopEdgeDeploymentStageRequestRequestTypeDef",
@@ -714,14 +702,16 @@
     "StopLabelingJobRequestRequestTypeDef",
     "StopMonitoringScheduleRequestRequestTypeDef",
     "StopNotebookInstanceInputRequestTypeDef",
     "StopPipelineExecutionRequestRequestTypeDef",
     "StopProcessingJobRequestRequestTypeDef",
     "StopTrainingJobRequestRequestTypeDef",
     "StopTransformJobRequestRequestTypeDef",
+    "TimeSeriesConfigTypeDef",
+    "TimeSeriesTransformationsTypeDef",
     "TrainingRepositoryAuthConfigTypeDef",
     "TransformS3DataSourceTypeDef",
     "UpdateActionRequestRequestTypeDef",
     "UpdateArtifactRequestRequestTypeDef",
     "UpdateContextRequestRequestTypeDef",
     "VariantPropertyTypeDef",
     "UpdateExperimentRequestRequestTypeDef",
@@ -845,87 +835,70 @@
     "AddTagsOutputTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
     "CreateModelPackageGroupInputRequestTypeDef",
     "CreateStudioLifecycleConfigRequestRequestTypeDef",
     "ImportHubContentRequestRequestTypeDef",
     "ListTagsOutputTypeDef",
-    "AutoRollbackConfigOutputTypeDef",
     "AutoRollbackConfigTypeDef",
-    "HyperParameterAlgorithmSpecificationOutputTypeDef",
     "HyperParameterAlgorithmSpecificationTypeDef",
     "AlgorithmStatusDetailsTypeDef",
     "ListAlgorithmsOutputTypeDef",
     "ListAppsResponseTypeDef",
-    "AppSpecificationUnionTypeDef",
-    "ArtifactSourceOutputTypeDef",
     "ArtifactSourceTypeDef",
-    "AsyncInferenceOutputConfigOutputTypeDef",
     "AsyncInferenceOutputConfigTypeDef",
-    "AutoMLCandidateGenerationConfigOutputTypeDef",
-    "CandidateGenerationConfigOutputTypeDef",
     "AutoMLCandidateGenerationConfigTypeDef",
     "CandidateGenerationConfigTypeDef",
     "AutoMLDataSourceTypeDef",
     "ImageClassificationJobConfigTypeDef",
     "TextClassificationJobConfigTypeDef",
     "ResolvedAttributesTypeDef",
     "AutoMLJobSummaryTypeDef",
     "AutoMLProblemTypeResolvedAttributesTypeDef",
-    "AutoMLSecurityConfigOutputTypeDef",
-    "LabelingJobResourceConfigOutputTypeDef",
-    "MonitoringNetworkConfigOutputTypeDef",
-    "NetworkConfigOutputTypeDef",
     "AutoMLSecurityConfigTypeDef",
     "LabelingJobResourceConfigTypeDef",
     "MonitoringNetworkConfigTypeDef",
     "NetworkConfigTypeDef",
-    "VpcConfigUnionTypeDef",
     "BiasTypeDef",
     "DriftCheckModelDataQualityTypeDef",
     "DriftCheckModelQualityTypeDef",
     "ExplainabilityTypeDef",
     "ModelDataQualityTypeDef",
     "ModelQualityTypeDef",
     "CallbackStepMetadataTypeDef",
     "LambdaStepMetadataTypeDef",
     "SendPipelineExecutionStepSuccessRequestRequestTypeDef",
     "CandidatePropertiesTypeDef",
     "CanvasAppSettingsTypeDef",
+    "RollingUpdatePolicyTypeDef",
     "TrafficRoutingConfigTypeDef",
-    "InferenceExperimentDataStorageConfigOutputTypeDef",
     "InferenceExperimentDataStorageConfigTypeDef",
-    "DataCaptureConfigOutputTypeDef",
     "DataCaptureConfigTypeDef",
-    "EnvironmentParameterRangesOutputTypeDef",
     "EnvironmentParameterRangesTypeDef",
     "ClarifyShapConfigTypeDef",
     "CodeRepositorySummaryTypeDef",
     "CreateCodeRepositoryInputRequestTypeDef",
     "DescribeCodeRepositoryOutputTypeDef",
-    "DebugHookConfigOutputTypeDef",
     "DebugHookConfigTypeDef",
     "ListCompilationJobsResponseTypeDef",
     "ContextSummaryTypeDef",
     "CreateContextRequestRequestTypeDef",
     "TuningJobCompletionCriteriaTypeDef",
     "CreateActionRequestRequestTypeDef",
     "CreateTrialRequestRequestTypeDef",
     "CreateAppRequestRequestTypeDef",
     "DescribeAppResponseTypeDef",
-    "JupyterServerAppSettingsOutputTypeDef",
     "JupyterServerAppSettingsTypeDef",
     "RStudioServerProDomainSettingsForUpdateTypeDef",
     "RStudioServerProDomainSettingsTypeDef",
     "TensorBoardAppSettingsTypeDef",
     "CreateDeviceFleetRequestRequestTypeDef",
     "CreateEdgePackagingJobRequestRequestTypeDef",
     "DescribeDeviceFleetResponseTypeDef",
     "UpdateDeviceFleetRequestRequestTypeDef",
-    "UpdateFeatureGroupRequestRequestTypeDef",
     "CreateHubRequestRequestTypeDef",
     "DescribeHubResponseTypeDef",
     "CreateHumanTaskUiRequestRequestTypeDef",
     "CreateModelCardExportJobRequestRequestTypeDef",
     "CreateModelCardRequestRequestTypeDef",
     "CreateNotebookInstanceInputRequestTypeDef",
     "DescribeNotebookInstanceOutputTypeDef",
@@ -983,43 +956,38 @@
     "ListMonitoringSchedulesRequestRequestTypeDef",
     "ListNotebookInstanceLifecycleConfigsInputRequestTypeDef",
     "ListNotebookInstancesInputRequestTypeDef",
     "ListPipelineExecutionsRequestRequestTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListProcessingJobsRequestRequestTypeDef",
     "ListProjectsInputRequestTypeDef",
+    "ListResourceCatalogsRequestRequestTypeDef",
     "ListStudioLifecycleConfigsRequestRequestTypeDef",
     "ListTrainingJobsRequestRequestTypeDef",
     "ListTransformJobsRequestRequestTypeDef",
     "ListTrialComponentsRequestRequestTypeDef",
     "ListTrialsRequestRequestTypeDef",
     "QueryFiltersTypeDef",
     "CreateTrialComponentRequestRequestTypeDef",
     "UpdateTrialComponentRequestRequestTypeDef",
     "CreateWorkforceRequestRequestTypeDef",
     "UpdateWorkforceRequestRequestTypeDef",
-    "KernelGatewayAppSettingsOutputTypeDef",
     "KernelGatewayAppSettingsTypeDef",
-    "RSessionAppSettingsOutputTypeDef",
     "RSessionAppSettingsTypeDef",
-    "DataQualityAppSpecificationUnionTypeDef",
     "ModelBiasBaselineConfigTypeDef",
     "ModelExplainabilityBaselineConfigTypeDef",
     "ModelQualityBaselineConfigTypeDef",
     "DataQualityBaselineConfigTypeDef",
     "MonitoringBaselineConfigTypeDef",
-    "DataSourceOutputTypeDef",
     "DataSourceTypeDef",
     "DatasetDefinitionTypeDef",
-    "DebugRuleConfigurationUnionTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeploymentRecommendationTypeDef",
-    "DeploymentStageStatusSummaryTypeDef",
     "DeploymentStageTypeDef",
-    "NeoVpcConfigUnionTypeDef",
+    "DeploymentStageStatusSummaryTypeDef",
     "DescribeDeviceResponseTypeDef",
     "DescribeEdgePackagingJobResponseTypeDef",
     "DescribeEndpointInputEndpointDeletedWaitTypeDef",
     "DescribeEndpointInputEndpointInServiceWaitTypeDef",
     "DescribeImageRequestImageCreatedWaitTypeDef",
     "DescribeImageRequestImageDeletedWaitTypeDef",
     "DescribeImageRequestImageUpdatedWaitTypeDef",
@@ -1034,23 +1002,18 @@
     "ExperimentSummaryTypeDef",
     "FeatureGroupSummaryTypeDef",
     "DescribeFeatureMetadataResponseTypeDef",
     "FeatureMetadataTypeDef",
     "UpdateFeatureMetadataRequestRequestTypeDef",
     "DescribeHubContentResponseTypeDef",
     "DescribeHumanTaskUiResponseTypeDef",
-    "InferenceExperimentSummaryTypeDef",
-    "ModelBiasAppSpecificationUnionTypeDef",
     "DescribeModelCardExportJobResponseTypeDef",
-    "ModelExplainabilityAppSpecificationUnionTypeDef",
-    "ModelQualityAppSpecificationUnionTypeDef",
     "ListMonitoringExecutionsResponseTypeDef",
     "DescribeSubscribedWorkteamResponseTypeDef",
     "ListSubscribedWorkteamsResponseTypeDef",
-    "ProfilerConfigUnionTypeDef",
     "TrainingJobSummaryTypeDef",
     "TrialSummaryTypeDef",
     "DesiredWeightAndCapacityTypeDef",
     "ListStageDevicesResponseTypeDef",
     "ListDeviceFleetsResponseTypeDef",
     "DeviceSummaryTypeDef",
     "RegisterDevicesRequestRequestTypeDef",
@@ -1058,45 +1021,41 @@
     "ListDomainsResponseTypeDef",
     "DriftCheckBiasTypeDef",
     "DriftCheckExplainabilityTypeDef",
     "ListEdgeDeploymentPlansResponseTypeDef",
     "GetDeviceFleetReportResponseTypeDef",
     "ListEdgePackagingJobsResponseTypeDef",
     "ListEndpointConfigsOutputTypeDef",
+    "EndpointOutputConfigurationTypeDef",
     "EndpointPerformanceTypeDef",
     "ListEndpointsOutputTypeDef",
     "ModelConfigurationTypeDef",
     "NestedFiltersTypeDef",
     "HyperParameterTrainingJobSummaryTypeDef",
     "ListFlowDefinitionsResponseTypeDef",
+    "GetScalingConfigurationRecommendationRequestRequestTypeDef",
     "GetSearchSuggestionsResponseTypeDef",
     "UpdateCodeRepositoryInputRequestTypeDef",
     "ListHubContentVersionsResponseTypeDef",
     "ListHubContentsResponseTypeDef",
     "ListHubsResponseTypeDef",
     "HumanLoopActivationConfigTypeDef",
     "ListHumanTaskUisResponseTypeDef",
-    "HyperParameterTuningResourceConfigOutputTypeDef",
     "HyperParameterTuningResourceConfigTypeDef",
     "HyperParameterTuningJobSummaryTypeDef",
     "HyperParameterTuningJobStrategyConfigTypeDef",
-    "HyperParameterTuningJobWarmStartConfigOutputTypeDef",
     "HyperParameterTuningJobWarmStartConfigTypeDef",
     "UserContextTypeDef",
     "ImageConfigTypeDef",
     "ListImagesResponseTypeDef",
     "ListImageVersionsResponseTypeDef",
     "ListInferenceRecommendationsJobsResponseTypeDef",
-    "ResourceConfigOutputTypeDef",
     "ResourceConfigTypeDef",
-    "ParameterRangeOutputTypeDef",
     "ParameterRangeTypeDef",
-    "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
-    "KernelGatewayImageConfigOutputTypeDef",
     "KernelGatewayImageConfigTypeDef",
     "LabelingJobForWorkteamSummaryTypeDef",
     "LabelingJobDataSourceTypeDef",
     "ListLineageGroupsResponseTypeDef",
     "ListActionsRequestListActionsPaginateTypeDef",
     "ListAlgorithmsInputListAlgorithmsPaginateTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
@@ -1146,14 +1105,15 @@
     "ListNotebookInstanceLifecycleConfigsInputListNotebookInstanceLifecycleConfigsPaginateTypeDef",
     "ListNotebookInstancesInputListNotebookInstancesPaginateTypeDef",
     "ListPipelineExecutionStepsRequestListPipelineExecutionStepsPaginateTypeDef",
     "ListPipelineExecutionsRequestListPipelineExecutionsPaginateTypeDef",
     "ListPipelineParametersForExecutionRequestListPipelineParametersForExecutionPaginateTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListProcessingJobsRequestListProcessingJobsPaginateTypeDef",
+    "ListResourceCatalogsRequestListResourceCatalogsPaginateTypeDef",
     "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListStageDevicesRequestListStageDevicesPaginateTypeDef",
     "ListStudioLifecycleConfigsRequestListStudioLifecycleConfigsPaginateTypeDef",
     "ListSubscribedWorkteamsRequestListSubscribedWorkteamsPaginateTypeDef",
     "ListTagsInputListTagsPaginateTypeDef",
     "ListTrainingJobsForHyperParameterTuningJobRequestListTrainingJobsForHyperParameterTuningJobPaginateTypeDef",
     "ListTrainingJobsRequestListTrainingJobsPaginateTypeDef",
@@ -1180,129 +1140,102 @@
     "ListNotebookInstanceLifecycleConfigsOutputTypeDef",
     "ListNotebookInstancesOutputTypeDef",
     "ListPipelineExecutionsResponseTypeDef",
     "ListPipelineParametersForExecutionResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ListProcessingJobsResponseTypeDef",
     "ListProjectsOutputTypeDef",
+    "ListResourceCatalogsResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "ListStudioLifecycleConfigsResponseTypeDef",
     "ListTransformJobsResponseTypeDef",
     "ListUserProfilesResponseTypeDef",
-    "MemberDefinitionOutputTypeDef",
     "MemberDefinitionTypeDef",
+    "MetricSpecificationTypeDef",
     "MonitoringAlertActionsTypeDef",
     "ModelDataSourceTypeDef",
     "ModelInfrastructureConfigTypeDef",
-    "ModelPackageContainerDefinitionOutputTypeDef",
     "ModelPackageContainerDefinitionTypeDef",
-    "RecommendationJobStoppingConditionsOutputTypeDef",
     "RecommendationJobStoppingConditionsTypeDef",
     "ModelMetadataSearchExpressionTypeDef",
     "ModelPackageStatusDetailsTypeDef",
     "MonitoringResourcesTypeDef",
-    "MonitoringDatasetFormatOutputTypeDef",
     "MonitoringDatasetFormatTypeDef",
     "MonitoringOutputTypeDef",
     "OfflineStoreConfigTypeDef",
     "OnlineStoreConfigTypeDef",
+    "OnlineStoreConfigUpdateTypeDef",
     "OutputConfigTypeDef",
     "PendingProductionVariantSummaryTypeDef",
     "ProductionVariantSummaryTypeDef",
-    "TrafficPatternOutputTypeDef",
-    "TrafficPatternTypeDef",
     "ProcessingResourcesTypeDef",
     "ProcessingOutputTypeDef",
     "ProductionVariantTypeDef",
-    "ProfilerRuleConfigurationUnionTypeDef",
     "SuggestionQueryTypeDef",
-    "ServiceCatalogProvisioningDetailsOutputTypeDef",
     "ServiceCatalogProvisioningDetailsTypeDef",
     "ServiceCatalogProvisioningUpdateDetailsTypeDef",
     "PublicWorkforceTaskPriceTypeDef",
     "QueryLineageResponseTypeDef",
     "RecommendationJobOutputConfigTypeDef",
-    "RecommendationJobContainerConfigOutputTypeDef",
     "RecommendationJobContainerConfigTypeDef",
     "RenderUiTemplateRequestRequestTypeDef",
     "RenderUiTemplateResponseTypeDef",
-    "SelectiveExecutionConfigOutputTypeDef",
+    "UpdateTrainingJobRequestRequestTypeDef",
     "SelectiveExecutionConfigTypeDef",
-    "ShadowModeConfigOutputTypeDef",
     "ShadowModeConfigTypeDef",
-    "SourceAlgorithmSpecificationOutputTypeDef",
     "SourceAlgorithmSpecificationTypeDef",
-    "SourceIpConfigUnionTypeDef",
+    "TrafficPatternTypeDef",
+    "TimeSeriesForecastingJobConfigTypeDef",
     "TrainingImageConfigTypeDef",
     "TransformDataSourceTypeDef",
     "WorkforceTypeDef",
     "ListActionsResponseTypeDef",
     "ArtifactSummaryTypeDef",
-    "ArtifactSourceUnionTypeDef",
     "CreateArtifactRequestRequestTypeDef",
     "DeleteArtifactRequestRequestTypeDef",
-    "AsyncInferenceConfigOutputTypeDef",
     "AsyncInferenceConfigTypeDef",
-    "TabularJobConfigOutputTypeDef",
     "TabularJobConfigTypeDef",
     "AutoMLChannelTypeDef",
     "AutoMLJobChannelTypeDef",
     "ListAutoMLJobsResponseTypeDef",
     "AutoMLResolvedAttributesTypeDef",
-    "AutoMLJobConfigOutputTypeDef",
-    "LabelingJobAlgorithmsConfigOutputTypeDef",
     "AutoMLJobConfigTypeDef",
-    "AutoMLSecurityConfigUnionTypeDef",
     "LabelingJobAlgorithmsConfigTypeDef",
-    "MonitoringNetworkConfigUnionTypeDef",
-    "NetworkConfigUnionTypeDef",
     "ModelMetricsTypeDef",
     "PipelineExecutionStepMetadataTypeDef",
     "AutoMLCandidateTypeDef",
     "BlueGreenUpdatePolicyTypeDef",
-    "InferenceExperimentDataStorageConfigUnionTypeDef",
-    "DataCaptureConfigUnionTypeDef",
-    "EndpointInputConfigurationOutputTypeDef",
     "EndpointInputConfigurationTypeDef",
-    "ClarifyExplainerConfigOutputTypeDef",
     "ClarifyExplainerConfigTypeDef",
     "ListCodeRepositoriesOutputTypeDef",
-    "DebugHookConfigUnionTypeDef",
     "ListContextsResponseTypeDef",
     "DomainSettingsForUpdateTypeDef",
-    "DomainSettingsOutputTypeDef",
     "DomainSettingsTypeDef",
-    "InferenceExperimentScheduleUnionTypeDef",
+    "InferenceExperimentSummaryTypeDef",
     "QueryLineageRequestRequestTypeDef",
-    "DefaultSpaceSettingsOutputTypeDef",
-    "SpaceSettingsOutputTypeDef",
     "DefaultSpaceSettingsTypeDef",
     "SpaceSettingsTypeDef",
-    "UserSettingsOutputTypeDef",
     "UserSettingsTypeDef",
-    "ChannelOutputTypeDef",
     "ChannelTypeDef",
     "ProcessingInputTypeDef",
-    "DescribeEdgeDeploymentPlanResponseTypeDef",
     "CreateEdgeDeploymentPlanRequestRequestTypeDef",
     "CreateEdgeDeploymentStageRequestRequestTypeDef",
+    "DescribeEdgeDeploymentPlanResponseTypeDef",
     "ListExperimentsResponseTypeDef",
     "ListFeatureGroupsResponseTypeDef",
-    "ListInferenceExperimentsResponseTypeDef",
     "ListTrainingJobsResponseTypeDef",
     "ListTrialsResponseTypeDef",
     "UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef",
     "ListDevicesResponseTypeDef",
     "DriftCheckBaselinesTypeDef",
     "InferenceRecommendationTypeDef",
     "RecommendationJobInferenceBenchmarkTypeDef",
     "SearchExpressionTypeDef",
     "ListTrainingJobsForHyperParameterTuningJobResponseTypeDef",
     "ListHyperParameterTuningJobsResponseTypeDef",
-    "HyperParameterTuningJobWarmStartConfigUnionTypeDef",
     "AssociationSummaryTypeDef",
     "DescribeActionResponseTypeDef",
     "DescribeArtifactResponseTypeDef",
     "DescribeContextResponseTypeDef",
     "DescribeExperimentResponseTypeDef",
     "DescribeLineageGroupResponseTypeDef",
     "DescribeModelCardResponseTypeDef",
@@ -1313,229 +1246,164 @@
     "ExperimentTypeDef",
     "ModelCardTypeDef",
     "ModelDashboardModelCardTypeDef",
     "ModelPackageGroupTypeDef",
     "PipelineTypeDef",
     "TrialComponentSimpleSummaryTypeDef",
     "TrialComponentSummaryTypeDef",
-    "ResourceConfigUnionTypeDef",
-    "HyperParameterSpecificationOutputTypeDef",
     "HyperParameterSpecificationTypeDef",
-    "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "AppImageConfigDetailsTypeDef",
-    "DescribeAppImageConfigResponseTypeDef",
     "CreateAppImageConfigRequestRequestTypeDef",
-    "KernelGatewayImageConfigUnionTypeDef",
+    "DescribeAppImageConfigResponseTypeDef",
     "UpdateAppImageConfigRequestRequestTypeDef",
     "ListLabelingJobsForWorkteamResponseTypeDef",
-    "LabelingJobInputConfigOutputTypeDef",
     "LabelingJobInputConfigTypeDef",
+    "CreateWorkteamRequestRequestTypeDef",
+    "UpdateWorkteamRequestRequestTypeDef",
     "WorkteamTypeDef",
-    "MemberDefinitionUnionTypeDef",
+    "TargetTrackingScalingPolicyConfigurationTypeDef",
     "MonitoringAlertSummaryTypeDef",
-    "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
     "ModelVariantConfigSummaryTypeDef",
     "ModelVariantConfigTypeDef",
-    "AdditionalInferenceSpecificationDefinitionOutputTypeDef",
-    "InferenceSpecificationOutputTypeDef",
     "AdditionalInferenceSpecificationDefinitionTypeDef",
     "InferenceSpecificationTypeDef",
-    "RecommendationJobStoppingConditionsUnionTypeDef",
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
     "ListModelMetadataRequestRequestTypeDef",
-    "BatchTransformInputOutputTypeDef",
     "BatchTransformInputTypeDef",
-    "MonitoringOutputConfigOutputTypeDef",
     "MonitoringOutputConfigTypeDef",
     "CreateFeatureGroupRequestRequestTypeDef",
     "DescribeFeatureGroupResponseTypeDef",
     "FeatureGroupTypeDef",
+    "UpdateFeatureGroupRequestRequestTypeDef",
     "CreateCompilationJobRequestRequestTypeDef",
     "DescribeCompilationJobResponseTypeDef",
     "PendingDeploymentSummaryTypeDef",
-    "ProcessingOutputConfigOutputTypeDef",
     "ProcessingOutputConfigTypeDef",
-    "UpdateTrainingJobRequestRequestTypeDef",
     "GetSearchSuggestionsRequestRequestTypeDef",
+    "CreateProjectInputRequestTypeDef",
     "DescribeProjectOutputTypeDef",
     "ProjectTypeDef",
-    "CreateProjectInputRequestTypeDef",
-    "ServiceCatalogProvisioningDetailsUnionTypeDef",
     "UpdateProjectInputRequestTypeDef",
-    "HumanLoopConfigOutputTypeDef",
     "HumanLoopConfigTypeDef",
-    "HumanTaskConfigOutputTypeDef",
     "HumanTaskConfigTypeDef",
     "DescribePipelineExecutionResponseTypeDef",
     "PipelineExecutionTypeDef",
-    "SelectiveExecutionConfigUnionTypeDef",
     "StartPipelineExecutionRequestRequestTypeDef",
-    "ShadowModeConfigUnionTypeDef",
-    "SourceAlgorithmSpecificationUnionTypeDef",
-    "AlgorithmSpecificationOutputTypeDef",
     "AlgorithmSpecificationTypeDef",
     "TransformInputTypeDef",
     "DescribeWorkforceResponseTypeDef",
     "ListWorkforcesResponseTypeDef",
     "UpdateWorkforceResponseTypeDef",
     "ListArtifactsResponseTypeDef",
-    "AsyncInferenceConfigUnionTypeDef",
-    "AutoMLProblemTypeConfigOutputTypeDef",
     "AutoMLProblemTypeConfigTypeDef",
-    "AutoMLJobConfigUnionTypeDef",
     "CreateAutoMLJobRequestRequestTypeDef",
-    "LabelingJobAlgorithmsConfigUnionTypeDef",
     "PipelineExecutionStepTypeDef",
     "DescribeAutoMLJobResponseTypeDef",
     "ListCandidatesForAutoMLJobResponseTypeDef",
-    "DeploymentConfigOutputTypeDef",
     "DeploymentConfigTypeDef",
-    "RecommendationJobInputConfigOutputTypeDef",
     "RecommendationJobInputConfigTypeDef",
-    "ExplainerConfigOutputTypeDef",
     "ExplainerConfigTypeDef",
-    "DomainSettingsUnionTypeDef",
-    "DescribeSpaceResponseTypeDef",
-    "DefaultSpaceSettingsUnionTypeDef",
+    "ListInferenceExperimentsResponseTypeDef",
     "CreateSpaceRequestRequestTypeDef",
-    "SpaceSettingsUnionTypeDef",
+    "DescribeSpaceResponseTypeDef",
     "UpdateSpaceRequestRequestTypeDef",
-    "DescribeDomainResponseTypeDef",
-    "DescribeUserProfileResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
+    "DescribeDomainResponseTypeDef",
+    "DescribeUserProfileResponseTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
-    "UserSettingsUnionTypeDef",
-    "HyperParameterTrainingJobDefinitionOutputTypeDef",
-    "TrainingJobDefinitionOutputTypeDef",
-    "ChannelUnionTypeDef",
     "HyperParameterTrainingJobDefinitionTypeDef",
     "TrainingJobDefinitionTypeDef",
     "InferenceRecommendationsJobStepTypeDef",
     "ListAssociationsResponseTypeDef",
     "TrialTypeDef",
     "ListTrialComponentsResponseTypeDef",
-    "TrainingSpecificationOutputTypeDef",
     "TrainingSpecificationTypeDef",
-    "HyperParameterTuningJobConfigUnionTypeDef",
     "ListAppImageConfigsResponseTypeDef",
     "LabelingJobSummaryTypeDef",
-    "LabelingJobInputConfigUnionTypeDef",
     "DescribeWorkteamResponseTypeDef",
     "ListWorkteamsResponseTypeDef",
     "UpdateWorkteamResponseTypeDef",
-    "CreateWorkteamRequestRequestTypeDef",
-    "UpdateWorkteamRequestRequestTypeDef",
+    "ScalingPolicyTypeDef",
     "ListMonitoringAlertsResponseTypeDef",
+    "CreateModelInputRequestTypeDef",
     "DescribeModelOutputTypeDef",
     "ModelTypeDef",
-    "ContainerDefinitionUnionTypeDef",
     "DescribeInferenceExperimentResponseTypeDef",
     "CreateInferenceExperimentRequestRequestTypeDef",
     "StopInferenceExperimentRequestRequestTypeDef",
     "UpdateInferenceExperimentRequestRequestTypeDef",
+    "UpdateModelPackageInputRequestTypeDef",
     "BatchDescribeModelPackageSummaryTypeDef",
-    "AdditionalInferenceSpecificationDefinitionUnionTypeDef",
-    "InferenceSpecificationUnionTypeDef",
-    "DataQualityJobInputOutputTypeDef",
-    "ModelBiasJobInputOutputTypeDef",
-    "ModelExplainabilityJobInputOutputTypeDef",
-    "ModelQualityJobInputOutputTypeDef",
-    "MonitoringInputOutputTypeDef",
     "DataQualityJobInputTypeDef",
     "ModelBiasJobInputTypeDef",
     "ModelExplainabilityJobInputTypeDef",
     "ModelQualityJobInputTypeDef",
     "MonitoringInputTypeDef",
-    "MonitoringOutputConfigUnionTypeDef",
+    "CreateProcessingJobRequestRequestTypeDef",
     "DescribeProcessingJobResponseTypeDef",
     "ProcessingJobTypeDef",
-    "CreateProcessingJobRequestRequestTypeDef",
-    "ProcessingOutputConfigUnionTypeDef",
-    "DescribeFlowDefinitionResponseTypeDef",
     "CreateFlowDefinitionRequestRequestTypeDef",
-    "HumanLoopConfigUnionTypeDef",
-    "DescribeLabelingJobResponseTypeDef",
+    "DescribeFlowDefinitionResponseTypeDef",
     "CreateLabelingJobRequestRequestTypeDef",
-    "HumanTaskConfigUnionTypeDef",
+    "DescribeLabelingJobResponseTypeDef",
+    "CreateTrainingJobRequestRequestTypeDef",
     "DescribeTrainingJobResponseTypeDef",
     "TrainingJobTypeDef",
-    "AlgorithmSpecificationUnionTypeDef",
     "CreateTransformJobRequestRequestTypeDef",
     "DescribeTransformJobResponseTypeDef",
-    "TransformJobDefinitionOutputTypeDef",
     "TransformJobDefinitionTypeDef",
     "TransformJobTypeDef",
-    "DescribeAutoMLJobV2ResponseTypeDef",
-    "AutoMLProblemTypeConfigUnionTypeDef",
     "CreateAutoMLJobV2RequestRequestTypeDef",
+    "DescribeAutoMLJobV2ResponseTypeDef",
     "ListPipelineExecutionStepsResponseTypeDef",
     "CreateEndpointInputRequestTypeDef",
-    "DeploymentConfigUnionTypeDef",
     "UpdateEndpointInputRequestTypeDef",
-    "DescribeInferenceRecommendationsJobResponseTypeDef",
     "CreateInferenceRecommendationsJobRequestRequestTypeDef",
-    "RecommendationJobInputConfigUnionTypeDef",
+    "DescribeInferenceRecommendationsJobResponseTypeDef",
+    "CreateEndpointConfigInputRequestTypeDef",
     "DescribeEndpointConfigOutputTypeDef",
     "DescribeEndpointOutputTypeDef",
-    "CreateEndpointConfigInputRequestTypeDef",
-    "ExplainerConfigUnionTypeDef",
+    "CreateHyperParameterTuningJobRequestRequestTypeDef",
     "DescribeHyperParameterTuningJobResponseTypeDef",
     "HyperParameterTuningJobSearchEntityTypeDef",
-    "CreateTrainingJobRequestRequestTypeDef",
-    "HyperParameterTrainingJobDefinitionUnionTypeDef",
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
-    "TrainingSpecificationUnionTypeDef",
     "ListLabelingJobsResponseTypeDef",
-    "CreateModelInputRequestTypeDef",
+    "DynamicScalingConfigurationTypeDef",
     "BatchDescribeModelPackageOutputTypeDef",
-    "UpdateModelPackageInputRequestTypeDef",
-    "DescribeDataQualityJobDefinitionResponseTypeDef",
-    "DescribeModelBiasJobDefinitionResponseTypeDef",
-    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
-    "DescribeModelQualityJobDefinitionResponseTypeDef",
-    "MonitoringJobDefinitionOutputTypeDef",
     "CreateDataQualityJobDefinitionRequestRequestTypeDef",
-    "DataQualityJobInputUnionTypeDef",
+    "DescribeDataQualityJobDefinitionResponseTypeDef",
     "CreateModelBiasJobDefinitionRequestRequestTypeDef",
-    "ModelBiasJobInputUnionTypeDef",
+    "DescribeModelBiasJobDefinitionResponseTypeDef",
     "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
-    "ModelExplainabilityJobInputUnionTypeDef",
+    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
     "CreateModelQualityJobDefinitionRequestRequestTypeDef",
-    "ModelQualityJobInputUnionTypeDef",
+    "DescribeModelQualityJobDefinitionResponseTypeDef",
     "MonitoringJobDefinitionTypeDef",
-    "AlgorithmValidationProfileOutputTypeDef",
-    "ModelPackageValidationProfileOutputTypeDef",
     "AlgorithmValidationProfileTypeDef",
     "ModelPackageValidationProfileTypeDef",
     "TrialComponentSourceDetailTypeDef",
-    "CreateHyperParameterTuningJobRequestRequestTypeDef",
-    "MonitoringScheduleConfigOutputTypeDef",
+    "GetScalingConfigurationRecommendationResponseTypeDef",
     "MonitoringScheduleConfigTypeDef",
-    "AlgorithmValidationSpecificationOutputTypeDef",
-    "ModelPackageValidationSpecificationOutputTypeDef",
     "AlgorithmValidationSpecificationTypeDef",
     "ModelPackageValidationSpecificationTypeDef",
     "TrialComponentTypeDef",
+    "CreateMonitoringScheduleRequestRequestTypeDef",
     "DescribeMonitoringScheduleResponseTypeDef",
     "ModelDashboardMonitoringScheduleTypeDef",
     "MonitoringScheduleTypeDef",
-    "CreateMonitoringScheduleRequestRequestTypeDef",
-    "MonitoringScheduleConfigUnionTypeDef",
     "UpdateMonitoringScheduleRequestRequestTypeDef",
+    "CreateAlgorithmInputRequestTypeDef",
     "DescribeAlgorithmOutputTypeDef",
+    "CreateModelPackageInputRequestTypeDef",
     "DescribeModelPackageOutputTypeDef",
     "ModelPackageTypeDef",
-    "AlgorithmValidationSpecificationUnionTypeDef",
-    "CreateAlgorithmInputRequestTypeDef",
-    "CreateModelPackageInputRequestTypeDef",
-    "ModelPackageValidationSpecificationUnionTypeDef",
     "ModelDashboardModelTypeDef",
     "EndpointTypeDef",
     "SearchRecordTypeDef",
     "SearchResponseTypeDef",
 )
 
 _RequiredActionSourceTypeDef = TypedDict(
@@ -1684,36 +1552,14 @@
         "Status": AppStatusType,
         "CreationTime": datetime,
         "SpaceName": str,
     },
     total=False,
 )
 
-_RequiredAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-    },
-)
-_OptionalAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalAppSpecificationOutputTypeDef",
-    {
-        "ContainerEntrypoint": List[str],
-        "ContainerArguments": List[str],
-    },
-    total=False,
-)
-
-
-class AppSpecificationOutputTypeDef(
-    _RequiredAppSpecificationOutputTypeDef, _OptionalAppSpecificationOutputTypeDef
-):
-    pass
-
-
 _RequiredAppSpecificationTypeDef = TypedDict(
     "_RequiredAppSpecificationTypeDef",
     {
         "ImageUri": str,
     },
 )
 _OptionalAppSpecificationTypeDef = TypedDict(
@@ -1750,24 +1596,14 @@
     "AsyncInferenceClientConfigTypeDef",
     {
         "MaxConcurrentInvocationsPerInstance": int,
     },
     total=False,
 )
 
-AsyncInferenceNotificationConfigOutputTypeDef = TypedDict(
-    "AsyncInferenceNotificationConfigOutputTypeDef",
-    {
-        "SuccessTopic": str,
-        "ErrorTopic": str,
-        "IncludeInferenceResponseIn": List[AsyncNotificationTopicTypesType],
-    },
-    total=False,
-)
-
 AsyncInferenceNotificationConfigTypeDef = TypedDict(
     "AsyncInferenceNotificationConfigTypeDef",
     {
         "SuccessTopic": str,
         "ErrorTopic": str,
         "IncludeInferenceResponseIn": Sequence[AsyncNotificationTopicTypesType],
     },
@@ -1797,21 +1633,14 @@
 
 class AthenaDatasetDefinitionTypeDef(
     _RequiredAthenaDatasetDefinitionTypeDef, _OptionalAthenaDatasetDefinitionTypeDef
 ):
     pass
 
 
-AutoMLAlgorithmConfigOutputTypeDef = TypedDict(
-    "AutoMLAlgorithmConfigOutputTypeDef",
-    {
-        "AutoMLAlgorithms": List[AutoMLAlgorithmType],
-    },
-)
-
 AutoMLAlgorithmConfigTypeDef = TypedDict(
     "AutoMLAlgorithmConfigTypeDef",
     {
         "AutoMLAlgorithms": Sequence[AutoMLAlgorithmType],
     },
 )
 
@@ -1952,22 +1781,14 @@
     "TabularResolvedAttributesTypeDef",
     {
         "ProblemType": ProblemTypeType,
     },
     total=False,
 )
 
-VpcConfigOutputTypeDef = TypedDict(
-    "VpcConfigOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "Subnets": List[str],
-    },
-)
-
 VpcConfigTypeDef = TypedDict(
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
@@ -2074,14 +1895,15 @@
         "Explainability": str,
     },
 )
 _OptionalCandidateArtifactLocationsTypeDef = TypedDict(
     "_OptionalCandidateArtifactLocationsTypeDef",
     {
         "ModelInsights": str,
+        "BacktestResults": str,
     },
     total=False,
 )
 
 
 class CandidateArtifactLocationsTypeDef(
     _RequiredCandidateArtifactLocationsTypeDef, _OptionalCandidateArtifactLocationsTypeDef
@@ -2114,29 +1936,29 @@
     {
         "Status": FeatureStatusType,
         "AmazonForecastRoleArn": str,
     },
     total=False,
 )
 
-CapacitySizeTypeDef = TypedDict(
-    "CapacitySizeTypeDef",
+WorkspaceSettingsTypeDef = TypedDict(
+    "WorkspaceSettingsTypeDef",
     {
-        "Type": CapacitySizeTypeType,
-        "Value": int,
+        "S3ArtifactPath": str,
+        "S3KmsKeyId": str,
     },
+    total=False,
 )
 
-CaptureContentTypeHeaderOutputTypeDef = TypedDict(
-    "CaptureContentTypeHeaderOutputTypeDef",
+CapacitySizeTypeDef = TypedDict(
+    "CapacitySizeTypeDef",
     {
-        "CsvContentTypes": List[str],
-        "JsonContentTypes": List[str],
+        "Type": CapacitySizeTypeType,
+        "Value": int,
     },
-    total=False,
 )
 
 CaptureContentTypeHeaderTypeDef = TypedDict(
     "CaptureContentTypeHeaderTypeDef",
     {
         "CsvContentTypes": Sequence[str],
         "JsonContentTypes": Sequence[str],
@@ -2147,37 +1969,14 @@
 CaptureOptionTypeDef = TypedDict(
     "CaptureOptionTypeDef",
     {
         "CaptureMode": CaptureModeType,
     },
 )
 
-CategoricalParameterOutputTypeDef = TypedDict(
-    "CategoricalParameterOutputTypeDef",
-    {
-        "Name": str,
-        "Value": List[str],
-    },
-)
-
-CategoricalParameterRangeOutputTypeDef = TypedDict(
-    "CategoricalParameterRangeOutputTypeDef",
-    {
-        "Name": str,
-        "Values": List[str],
-    },
-)
-
-CategoricalParameterRangeSpecificationOutputTypeDef = TypedDict(
-    "CategoricalParameterRangeSpecificationOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-)
-
 CategoricalParameterRangeSpecificationTypeDef = TypedDict(
     "CategoricalParameterRangeSpecificationTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
@@ -2193,46 +1992,14 @@
     "CategoricalParameterTypeDef",
     {
         "Name": str,
         "Value": Sequence[str],
     },
 )
 
-ShuffleConfigTypeDef = TypedDict(
-    "ShuffleConfigTypeDef",
-    {
-        "Seed": int,
-    },
-)
-
-_RequiredChannelSpecificationOutputTypeDef = TypedDict(
-    "_RequiredChannelSpecificationOutputTypeDef",
-    {
-        "Name": str,
-        "SupportedContentTypes": List[str],
-        "SupportedInputModes": List[TrainingInputModeType],
-    },
-)
-_OptionalChannelSpecificationOutputTypeDef = TypedDict(
-    "_OptionalChannelSpecificationOutputTypeDef",
-    {
-        "Description": str,
-        "IsRequired": bool,
-        "SupportedCompressionTypes": List[CompressionTypeType],
-    },
-    total=False,
-)
-
-
-class ChannelSpecificationOutputTypeDef(
-    _RequiredChannelSpecificationOutputTypeDef, _OptionalChannelSpecificationOutputTypeDef
-):
-    pass
-
-
 _RequiredChannelSpecificationTypeDef = TypedDict(
     "_RequiredChannelSpecificationTypeDef",
     {
         "Name": str,
         "SupportedContentTypes": Sequence[str],
         "SupportedInputModes": Sequence[TrainingInputModeType],
     },
@@ -2250,14 +2017,21 @@
 
 class ChannelSpecificationTypeDef(
     _RequiredChannelSpecificationTypeDef, _OptionalChannelSpecificationTypeDef
 ):
     pass
 
 
+ShuffleConfigTypeDef = TypedDict(
+    "ShuffleConfigTypeDef",
+    {
+        "Seed": int,
+    },
+)
+
 _RequiredCheckpointConfigTypeDef = TypedDict(
     "_RequiredCheckpointConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalCheckpointConfigTypeDef = TypedDict(
@@ -2284,32 +2058,14 @@
         "CheckJobArn": str,
         "SkipCheck": bool,
         "RegisterNewBaseline": bool,
     },
     total=False,
 )
 
-ClarifyInferenceConfigOutputTypeDef = TypedDict(
-    "ClarifyInferenceConfigOutputTypeDef",
-    {
-        "FeaturesAttribute": str,
-        "ContentTemplate": str,
-        "MaxRecordCount": int,
-        "MaxPayloadInMB": int,
-        "ProbabilityIndex": int,
-        "LabelIndex": int,
-        "ProbabilityAttribute": str,
-        "LabelAttribute": str,
-        "LabelHeaders": List[str],
-        "FeatureHeaders": List[str],
-        "FeatureTypes": List[ClarifyFeatureTypeType],
-    },
-    total=False,
-)
-
 ClarifyInferenceConfigTypeDef = TypedDict(
     "ClarifyInferenceConfigTypeDef",
     {
         "FeaturesAttribute": str,
         "ContentTemplate": str,
         "MaxRecordCount": int,
         "MaxPayloadInMB": int,
@@ -2382,23 +2138,14 @@
     {
         "UserPool": str,
         "UserGroup": str,
         "ClientId": str,
     },
 )
 
-CollectionConfigurationOutputTypeDef = TypedDict(
-    "CollectionConfigurationOutputTypeDef",
-    {
-        "CollectionName": str,
-        "CollectionParameters": Dict[str, str],
-    },
-    total=False,
-)
-
 CollectionConfigurationTypeDef = TypedDict(
     "CollectionConfigurationTypeDef",
     {
         "CollectionName": str,
         "CollectionParameters": Mapping[str, str],
     },
     total=False,
@@ -2951,14 +2698,40 @@
 ProcessingStoppingConditionTypeDef = TypedDict(
     "ProcessingStoppingConditionTypeDef",
     {
         "MaxRuntimeInSeconds": int,
     },
 )
 
+_RequiredDebugRuleConfigurationTypeDef = TypedDict(
+    "_RequiredDebugRuleConfigurationTypeDef",
+    {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+    },
+)
+_OptionalDebugRuleConfigurationTypeDef = TypedDict(
+    "_OptionalDebugRuleConfigurationTypeDef",
+    {
+        "LocalPath": str,
+        "S3OutputPath": str,
+        "InstanceType": ProcessingInstanceTypeType,
+        "VolumeSizeInGB": int,
+        "RuleParameters": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class DebugRuleConfigurationTypeDef(
+    _RequiredDebugRuleConfigurationTypeDef, _OptionalDebugRuleConfigurationTypeDef
+):
+    pass
+
+
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3OutputPath": str,
     },
 )
 _OptionalOutputDataConfigTypeDef = TypedDict(
@@ -2982,14 +2755,40 @@
         "ProfilingIntervalInMilliseconds": int,
         "ProfilingParameters": Mapping[str, str],
         "DisableProfiler": bool,
     },
     total=False,
 )
 
+_RequiredProfilerRuleConfigurationTypeDef = TypedDict(
+    "_RequiredProfilerRuleConfigurationTypeDef",
+    {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+    },
+)
+_OptionalProfilerRuleConfigurationTypeDef = TypedDict(
+    "_OptionalProfilerRuleConfigurationTypeDef",
+    {
+        "LocalPath": str,
+        "S3OutputPath": str,
+        "InstanceType": ProcessingInstanceTypeType,
+        "VolumeSizeInGB": int,
+        "RuleParameters": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class ProfilerRuleConfigurationTypeDef(
+    _RequiredProfilerRuleConfigurationTypeDef, _OptionalProfilerRuleConfigurationTypeDef
+):
+    pass
+
+
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
         "MaximumRetryAttempts": int,
     },
 )
 
@@ -3171,14 +2970,24 @@
 )
 
 
 class CustomImageTypeDef(_RequiredCustomImageTypeDef, _OptionalCustomImageTypeDef):
     pass
 
 
+CustomizedMetricSpecificationTypeDef = TypedDict(
+    "CustomizedMetricSpecificationTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": StatisticType,
+    },
+    total=False,
+)
+
 DataCaptureConfigSummaryTypeDef = TypedDict(
     "DataCaptureConfigSummaryTypeDef",
     {
         "EnableCapture": bool,
         "CaptureStatus": CaptureStatusType,
         "CurrentSamplingPercentage": int,
         "DestinationS3Uri": str,
@@ -3191,40 +3000,14 @@
     {
         "TableName": str,
         "Catalog": str,
         "Database": str,
     },
 )
 
-_RequiredDataQualityAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredDataQualityAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-    },
-)
-_OptionalDataQualityAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalDataQualityAppSpecificationOutputTypeDef",
-    {
-        "ContainerEntrypoint": List[str],
-        "ContainerArguments": List[str],
-        "RecordPreprocessorSourceUri": str,
-        "PostAnalyticsProcessorSourceUri": str,
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class DataQualityAppSpecificationOutputTypeDef(
-    _RequiredDataQualityAppSpecificationOutputTypeDef,
-    _OptionalDataQualityAppSpecificationOutputTypeDef,
-):
-    pass
-
-
 MonitoringConstraintsResourceTypeDef = TypedDict(
     "MonitoringConstraintsResourceTypeDef",
     {
         "S3Uri": str,
     },
     total=False,
 )
@@ -3270,38 +3053,14 @@
         "FileSystemId": str,
         "FileSystemAccessMode": FileSystemAccessModeType,
         "FileSystemType": FileSystemTypeType,
         "DirectoryPath": str,
     },
 )
 
-_RequiredS3DataSourceOutputTypeDef = TypedDict(
-    "_RequiredS3DataSourceOutputTypeDef",
-    {
-        "S3DataType": S3DataTypeType,
-        "S3Uri": str,
-    },
-)
-_OptionalS3DataSourceOutputTypeDef = TypedDict(
-    "_OptionalS3DataSourceOutputTypeDef",
-    {
-        "S3DataDistributionType": S3DataDistributionType,
-        "AttributeNames": List[str],
-        "InstanceGroupNames": List[str],
-    },
-    total=False,
-)
-
-
-class S3DataSourceOutputTypeDef(
-    _RequiredS3DataSourceOutputTypeDef, _OptionalS3DataSourceOutputTypeDef
-):
-    pass
-
-
 _RequiredS3DataSourceTypeDef = TypedDict(
     "_RequiredS3DataSourceTypeDef",
     {
         "S3DataType": S3DataTypeType,
         "S3Uri": str,
     },
 )
@@ -3344,66 +3103,14 @@
 
 class RedshiftDatasetDefinitionTypeDef(
     _RequiredRedshiftDatasetDefinitionTypeDef, _OptionalRedshiftDatasetDefinitionTypeDef
 ):
     pass
 
 
-_RequiredDebugRuleConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDebugRuleConfigurationOutputTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-    },
-)
-_OptionalDebugRuleConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDebugRuleConfigurationOutputTypeDef",
-    {
-        "LocalPath": str,
-        "S3OutputPath": str,
-        "InstanceType": ProcessingInstanceTypeType,
-        "VolumeSizeInGB": int,
-        "RuleParameters": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class DebugRuleConfigurationOutputTypeDef(
-    _RequiredDebugRuleConfigurationOutputTypeDef, _OptionalDebugRuleConfigurationOutputTypeDef
-):
-    pass
-
-
-_RequiredDebugRuleConfigurationTypeDef = TypedDict(
-    "_RequiredDebugRuleConfigurationTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-    },
-)
-_OptionalDebugRuleConfigurationTypeDef = TypedDict(
-    "_OptionalDebugRuleConfigurationTypeDef",
-    {
-        "LocalPath": str,
-        "S3OutputPath": str,
-        "InstanceType": ProcessingInstanceTypeType,
-        "VolumeSizeInGB": int,
-        "RuleParameters": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class DebugRuleConfigurationTypeDef(
-    _RequiredDebugRuleConfigurationTypeDef, _OptionalDebugRuleConfigurationTypeDef
-):
-    pass
-
-
 DebugRuleEvaluationStatusTypeDef = TypedDict(
     "DebugRuleEvaluationStatusTypeDef",
     {
         "RuleConfigurationName": str,
         "RuleEvaluationJobArn": str,
         "RuleEvaluationStatus": RuleEvaluationStatusType,
         "StatusDetails": str,
@@ -3791,33 +3498,33 @@
 
 class RealTimeInferenceRecommendationTypeDef(
     _RequiredRealTimeInferenceRecommendationTypeDef, _OptionalRealTimeInferenceRecommendationTypeDef
 ):
     pass
 
 
-_RequiredDeviceSelectionConfigOutputTypeDef = TypedDict(
-    "_RequiredDeviceSelectionConfigOutputTypeDef",
+_RequiredDeviceSelectionConfigTypeDef = TypedDict(
+    "_RequiredDeviceSelectionConfigTypeDef",
     {
         "DeviceSubsetType": DeviceSubsetTypeType,
     },
 )
-_OptionalDeviceSelectionConfigOutputTypeDef = TypedDict(
-    "_OptionalDeviceSelectionConfigOutputTypeDef",
+_OptionalDeviceSelectionConfigTypeDef = TypedDict(
+    "_OptionalDeviceSelectionConfigTypeDef",
     {
         "Percentage": int,
-        "DeviceNames": List[str],
+        "DeviceNames": Sequence[str],
         "DeviceNameContains": str,
     },
     total=False,
 )
 
 
-class DeviceSelectionConfigOutputTypeDef(
-    _RequiredDeviceSelectionConfigOutputTypeDef, _OptionalDeviceSelectionConfigOutputTypeDef
+class DeviceSelectionConfigTypeDef(
+    _RequiredDeviceSelectionConfigTypeDef, _OptionalDeviceSelectionConfigTypeDef
 ):
     pass
 
 
 EdgeDeploymentConfigTypeDef = TypedDict(
     "EdgeDeploymentConfigTypeDef",
     {
@@ -3846,37 +3553,14 @@
 
 class EdgeDeploymentStatusTypeDef(
     _RequiredEdgeDeploymentStatusTypeDef, _OptionalEdgeDeploymentStatusTypeDef
 ):
     pass
 
 
-_RequiredDeviceSelectionConfigTypeDef = TypedDict(
-    "_RequiredDeviceSelectionConfigTypeDef",
-    {
-        "DeviceSubsetType": DeviceSubsetTypeType,
-    },
-)
-_OptionalDeviceSelectionConfigTypeDef = TypedDict(
-    "_OptionalDeviceSelectionConfigTypeDef",
-    {
-        "Percentage": int,
-        "DeviceNames": Sequence[str],
-        "DeviceNameContains": str,
-    },
-    total=False,
-)
-
-
-class DeviceSelectionConfigTypeDef(
-    _RequiredDeviceSelectionConfigTypeDef, _OptionalDeviceSelectionConfigTypeDef
-):
-    pass
-
-
 DeregisterDevicesRequestRequestTypeDef = TypedDict(
     "DeregisterDevicesRequestRequestTypeDef",
     {
         "DeviceFleetName": str,
         "DeviceNames": Sequence[str],
     },
 )
@@ -3980,22 +3664,14 @@
     "ModelDigestsTypeDef",
     {
         "ArtifactDigest": str,
     },
     total=False,
 )
 
-NeoVpcConfigOutputTypeDef = TypedDict(
-    "NeoVpcConfigOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "Subnets": List[str],
-    },
-)
-
 DescribeContextRequestRequestTypeDef = TypedDict(
     "DescribeContextRequestRequestTypeDef",
     {
         "ContextName": str,
     },
 )
 
@@ -4407,23 +4083,14 @@
 )
 
 
 class EndpointMetadataTypeDef(_RequiredEndpointMetadataTypeDef, _OptionalEndpointMetadataTypeDef):
     pass
 
 
-InferenceExperimentScheduleOutputTypeDef = TypedDict(
-    "InferenceExperimentScheduleOutputTypeDef",
-    {
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
-
 DescribeInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
     "DescribeInferenceRecommendationsJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 
@@ -4477,36 +4144,14 @@
 DescribeModelBiasJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelBiasJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
 
-_RequiredModelBiasAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredModelBiasAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-        "ConfigUri": str,
-    },
-)
-_OptionalModelBiasAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalModelBiasAppSpecificationOutputTypeDef",
-    {
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class ModelBiasAppSpecificationOutputTypeDef(
-    _RequiredModelBiasAppSpecificationOutputTypeDef, _OptionalModelBiasAppSpecificationOutputTypeDef
-):
-    pass
-
-
 DescribeModelCardExportJobRequestRequestTypeDef = TypedDict(
     "DescribeModelCardExportJobRequestRequestTypeDef",
     {
         "ModelCardExportJobArn": str,
     },
 )
 
@@ -4541,37 +4186,14 @@
 DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
 
-_RequiredModelExplainabilityAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredModelExplainabilityAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-        "ConfigUri": str,
-    },
-)
-_OptionalModelExplainabilityAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalModelExplainabilityAppSpecificationOutputTypeDef",
-    {
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class ModelExplainabilityAppSpecificationOutputTypeDef(
-    _RequiredModelExplainabilityAppSpecificationOutputTypeDef,
-    _OptionalModelExplainabilityAppSpecificationOutputTypeDef,
-):
-    pass
-
-
 DescribeModelInputRequestTypeDef = TypedDict(
     "DescribeModelInputRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
@@ -4592,41 +4214,14 @@
 DescribeModelQualityJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelQualityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
 
-_RequiredModelQualityAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredModelQualityAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-    },
-)
-_OptionalModelQualityAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalModelQualityAppSpecificationOutputTypeDef",
-    {
-        "ContainerEntrypoint": List[str],
-        "ContainerArguments": List[str],
-        "RecordPreprocessorSourceUri": str,
-        "PostAnalyticsProcessorSourceUri": str,
-        "ProblemType": MonitoringProblemTypeType,
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class ModelQualityAppSpecificationOutputTypeDef(
-    _RequiredModelQualityAppSpecificationOutputTypeDef,
-    _OptionalModelQualityAppSpecificationOutputTypeDef,
-):
-    pass
-
-
 DescribeMonitoringScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
     },
 )
 
@@ -4785,51 +4380,14 @@
         "MetricName": str,
         "Value": float,
         "Timestamp": datetime,
     },
     total=False,
 )
 
-ProfilerConfigOutputTypeDef = TypedDict(
-    "ProfilerConfigOutputTypeDef",
-    {
-        "S3OutputPath": str,
-        "ProfilingIntervalInMilliseconds": int,
-        "ProfilingParameters": Dict[str, str],
-        "DisableProfiler": bool,
-    },
-    total=False,
-)
-
-_RequiredProfilerRuleConfigurationOutputTypeDef = TypedDict(
-    "_RequiredProfilerRuleConfigurationOutputTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-    },
-)
-_OptionalProfilerRuleConfigurationOutputTypeDef = TypedDict(
-    "_OptionalProfilerRuleConfigurationOutputTypeDef",
-    {
-        "LocalPath": str,
-        "S3OutputPath": str,
-        "InstanceType": ProcessingInstanceTypeType,
-        "VolumeSizeInGB": int,
-        "RuleParameters": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class ProfilerRuleConfigurationOutputTypeDef(
-    _RequiredProfilerRuleConfigurationOutputTypeDef, _OptionalProfilerRuleConfigurationOutputTypeDef
-):
-    pass
-
-
 ProfilerRuleEvaluationStatusTypeDef = TypedDict(
     "ProfilerRuleEvaluationStatusTypeDef",
     {
         "RuleConfigurationName": str,
         "RuleEvaluationJobArn": str,
         "RuleEvaluationStatus": RuleEvaluationStatusType,
         "StatusDetails": str,
@@ -5219,24 +4777,37 @@
 EndpointInfoTypeDef = TypedDict(
     "EndpointInfoTypeDef",
     {
         "EndpointName": str,
     },
 )
 
-EndpointOutputConfigurationTypeDef = TypedDict(
-    "EndpointOutputConfigurationTypeDef",
+_RequiredProductionVariantServerlessConfigTypeDef = TypedDict(
+    "_RequiredProductionVariantServerlessConfigTypeDef",
     {
-        "EndpointName": str,
-        "VariantName": str,
-        "InstanceType": ProductionVariantInstanceTypeType,
-        "InitialInstanceCount": int,
+        "MemorySizeInMB": int,
+        "MaxConcurrency": int,
+    },
+)
+_OptionalProductionVariantServerlessConfigTypeDef = TypedDict(
+    "_OptionalProductionVariantServerlessConfigTypeDef",
+    {
+        "ProvisionedConcurrency": int,
     },
+    total=False,
 )
 
+
+class ProductionVariantServerlessConfigTypeDef(
+    _RequiredProductionVariantServerlessConfigTypeDef,
+    _OptionalProductionVariantServerlessConfigTypeDef,
+):
+    pass
+
+
 InferenceMetricsTypeDef = TypedDict(
     "InferenceMetricsTypeDef",
     {
         "MaxInvocations": int,
         "ModelLatency": int,
     },
 )
@@ -5363,14 +4934,32 @@
 GetModelPackageGroupPolicyInputRequestTypeDef = TypedDict(
     "GetModelPackageGroupPolicyInputRequestTypeDef",
     {
         "ModelPackageGroupName": str,
     },
 )
 
+ScalingPolicyObjectiveTypeDef = TypedDict(
+    "ScalingPolicyObjectiveTypeDef",
+    {
+        "MinInvocationsPerMinute": int,
+        "MaxInvocationsPerMinute": int,
+    },
+    total=False,
+)
+
+ScalingPolicyMetricTypeDef = TypedDict(
+    "ScalingPolicyMetricTypeDef",
+    {
+        "InvocationsPerInstance": int,
+        "ModelLatency": int,
+    },
+    total=False,
+)
+
 PropertyNameSuggestionTypeDef = TypedDict(
     "PropertyNameSuggestionTypeDef",
     {
         "PropertyName": str,
     },
     total=False,
 )
@@ -5590,14 +5179,15 @@
     },
 )
 _OptionalRecommendationMetricsTypeDef = TypedDict(
     "_OptionalRecommendationMetricsTypeDef",
     {
         "CpuUtilization": float,
         "MemoryUtilization": float,
+        "ModelSetupTime": int,
     },
     total=False,
 )
 
 
 class RecommendationMetricsTypeDef(
     _RequiredRecommendationMetricsTypeDef, _OptionalRecommendationMetricsTypeDef
@@ -5702,22 +5292,14 @@
         "HumanLabeled": int,
         "PendingHuman": int,
         "Total": int,
     },
     total=False,
 )
 
-LabelingJobDataAttributesOutputTypeDef = TypedDict(
-    "LabelingJobDataAttributesOutputTypeDef",
-    {
-        "ContentClassifiers": List[ContentClassifierType],
-    },
-    total=False,
-)
-
 LabelingJobDataAttributesTypeDef = TypedDict(
     "LabelingJobDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
     total=False,
 )
@@ -6227,14 +5809,24 @@
 )
 
 
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
 
+ResourceCatalogTypeDef = TypedDict(
+    "ResourceCatalogTypeDef",
+    {
+        "ResourceCatalogArn": str,
+        "ResourceCatalogName": str,
+        "Description": str,
+        "CreationTime": datetime,
+    },
+)
+
 ListSpacesRequestRequestTypeDef = TypedDict(
     "ListSpacesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "SortOrder": SortOrderType,
         "SortBy": SpaceSortKeyType,
@@ -6421,26 +6013,27 @@
         "NameContains": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-OidcMemberDefinitionOutputTypeDef = TypedDict(
-    "OidcMemberDefinitionOutputTypeDef",
+OidcMemberDefinitionTypeDef = TypedDict(
+    "OidcMemberDefinitionTypeDef",
     {
-        "Groups": List[str],
+        "Groups": Sequence[str],
     },
 )
 
-OidcMemberDefinitionTypeDef = TypedDict(
-    "OidcMemberDefinitionTypeDef",
+PredefinedMetricSpecificationTypeDef = TypedDict(
+    "PredefinedMetricSpecificationTypeDef",
     {
-        "Groups": Sequence[str],
+        "PredefinedMetricType": str,
     },
+    total=False,
 )
 
 MonitoringGroundTruthS3InputTypeDef = TypedDict(
     "MonitoringGroundTruthS3InputTypeDef",
     {
         "S3Uri": str,
     },
@@ -6533,39 +6126,14 @@
     "ModelStepMetadataTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-_RequiredMonitoringAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredMonitoringAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-    },
-)
-_OptionalMonitoringAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalMonitoringAppSpecificationOutputTypeDef",
-    {
-        "ContainerEntrypoint": List[str],
-        "ContainerArguments": List[str],
-        "RecordPreprocessorSourceUri": str,
-        "PostAnalyticsProcessorSourceUri": str,
-    },
-    total=False,
-)
-
-
-class MonitoringAppSpecificationOutputTypeDef(
-    _RequiredMonitoringAppSpecificationOutputTypeDef,
-    _OptionalMonitoringAppSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredMonitoringAppSpecificationTypeDef = TypedDict(
     "_RequiredMonitoringAppSpecificationTypeDef",
     {
         "ImageUri": str,
     },
 )
 _OptionalMonitoringAppSpecificationTypeDef = TypedDict(
@@ -6692,14 +6260,23 @@
     "OnlineStoreSecurityConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+TtlDurationTypeDef = TypedDict(
+    "TtlDurationTypeDef",
+    {
+        "Unit": TtlDurationUnitType,
+        "Value": int,
+    },
+    total=False,
+)
+
 _RequiredTargetPlatformTypeDef = TypedDict(
     "_RequiredTargetPlatformTypeDef",
     {
         "Os": TargetPlatformOsType,
         "Arch": TargetPlatformArchType,
     },
 )
@@ -6721,37 +6298,14 @@
     {
         "TrialName": str,
         "ExperimentName": str,
     },
     total=False,
 )
 
-_RequiredProductionVariantServerlessConfigTypeDef = TypedDict(
-    "_RequiredProductionVariantServerlessConfigTypeDef",
-    {
-        "MemorySizeInMB": int,
-        "MaxConcurrency": int,
-    },
-)
-_OptionalProductionVariantServerlessConfigTypeDef = TypedDict(
-    "_OptionalProductionVariantServerlessConfigTypeDef",
-    {
-        "ProvisionedConcurrency": int,
-    },
-    total=False,
-)
-
-
-class ProductionVariantServerlessConfigTypeDef(
-    _RequiredProductionVariantServerlessConfigTypeDef,
-    _OptionalProductionVariantServerlessConfigTypeDef,
-):
-    pass
-
-
 _RequiredProductionVariantStatusTypeDef = TypedDict(
     "_RequiredProductionVariantStatusTypeDef",
     {
         "Status": VariantStatusType,
     },
 )
 _OptionalProductionVariantStatusTypeDef = TypedDict(
@@ -6937,40 +6491,14 @@
         "ProfilingIntervalInMilliseconds": int,
         "ProfilingParameters": Mapping[str, str],
         "DisableProfiler": bool,
     },
     total=False,
 )
 
-_RequiredProfilerRuleConfigurationTypeDef = TypedDict(
-    "_RequiredProfilerRuleConfigurationTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-    },
-)
-_OptionalProfilerRuleConfigurationTypeDef = TypedDict(
-    "_OptionalProfilerRuleConfigurationTypeDef",
-    {
-        "LocalPath": str,
-        "S3OutputPath": str,
-        "InstanceType": ProcessingInstanceTypeType,
-        "VolumeSizeInGB": int,
-        "RuleParameters": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class ProfilerRuleConfigurationTypeDef(
-    _RequiredProfilerRuleConfigurationTypeDef, _OptionalProfilerRuleConfigurationTypeDef
-):
-    pass
-
-
 PropertyNameQueryTypeDef = TypedDict(
     "PropertyNameQueryTypeDef",
     {
         "PropertyNameHint": str,
     },
 )
 
@@ -7024,23 +6552,14 @@
     "RecommendationJobCompiledOutputConfigTypeDef",
     {
         "S3OutputUri": str,
     },
     total=False,
 )
 
-RecommendationJobPayloadConfigOutputTypeDef = TypedDict(
-    "RecommendationJobPayloadConfigOutputTypeDef",
-    {
-        "SamplePayloadUrl": str,
-        "SupportedContentTypes": List[str],
-    },
-    total=False,
-)
-
 RecommendationJobPayloadConfigTypeDef = TypedDict(
     "RecommendationJobPayloadConfigTypeDef",
     {
         "SamplePayloadUrl": str,
         "SupportedContentTypes": Sequence[str],
     },
     total=False,
@@ -7051,22 +6570,14 @@
     {
         "MaxNumberOfTests": int,
         "MaxParallelOfTests": int,
     },
     total=False,
 )
 
-RecommendationJobVpcConfigOutputTypeDef = TypedDict(
-    "RecommendationJobVpcConfigOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "Subnets": List[str],
-    },
-)
-
 RecommendationJobVpcConfigTypeDef = TypedDict(
     "RecommendationJobVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
@@ -7103,14 +6614,15 @@
     "_OptionalSearchRequestRequestTypeDef",
     {
         "SearchExpression": "SearchExpressionTypeDef",
         "SortBy": str,
         "SortOrder": SearchSortOrderType,
         "NextToken": str,
         "MaxResults": int,
+        "CrossAccountFilterOption": CrossAccountFilterOptionType,
     },
     total=False,
 )
 
 
 class SearchRequestRequestTypeDef(
     _RequiredSearchRequestRequestTypeDef, _OptionalSearchRequestRequestTypeDef
@@ -7181,19 +6693,22 @@
 )
 
 
 class SourceAlgorithmTypeDef(_RequiredSourceAlgorithmTypeDef, _OptionalSourceAlgorithmTypeDef):
     pass
 
 
-SourceIpConfigOutputTypeDef = TypedDict(
-    "SourceIpConfigOutputTypeDef",
+StairsTypeDef = TypedDict(
+    "StairsTypeDef",
     {
-        "Cidrs": List[str],
+        "DurationInSeconds": int,
+        "NumberOfSteps": int,
+        "UsersPerStep": int,
     },
+    total=False,
 )
 
 StartEdgeDeploymentStageRequestRequestTypeDef = TypedDict(
     "StartEdgeDeploymentStageRequestRequestTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "StageName": str,
@@ -7310,14 +6825,44 @@
 StopTransformJobRequestRequestTypeDef = TypedDict(
     "StopTransformJobRequestRequestTypeDef",
     {
         "TransformJobName": str,
     },
 )
 
+_RequiredTimeSeriesConfigTypeDef = TypedDict(
+    "_RequiredTimeSeriesConfigTypeDef",
+    {
+        "TargetAttributeName": str,
+        "TimestampAttributeName": str,
+        "ItemIdentifierAttributeName": str,
+    },
+)
+_OptionalTimeSeriesConfigTypeDef = TypedDict(
+    "_OptionalTimeSeriesConfigTypeDef",
+    {
+        "GroupingAttributeNames": Sequence[str],
+    },
+    total=False,
+)
+
+
+class TimeSeriesConfigTypeDef(_RequiredTimeSeriesConfigTypeDef, _OptionalTimeSeriesConfigTypeDef):
+    pass
+
+
+TimeSeriesTransformationsTypeDef = TypedDict(
+    "TimeSeriesTransformationsTypeDef",
+    {
+        "Filling": Mapping[str, Mapping[FillingTypeType, str]],
+        "Aggregation": Mapping[str, AggregationTransformationValueType],
+    },
+    total=False,
+)
+
 TrainingRepositoryAuthConfigTypeDef = TypedDict(
     "TrainingRepositoryAuthConfigTypeDef",
     {
         "TrainingRepositoryCredentialsProviderArn": str,
     },
 )
 
@@ -8644,54 +8189,22 @@
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AutoRollbackConfigOutputTypeDef = TypedDict(
-    "AutoRollbackConfigOutputTypeDef",
-    {
-        "Alarms": List[AlarmTypeDef],
-    },
-    total=False,
-)
-
 AutoRollbackConfigTypeDef = TypedDict(
     "AutoRollbackConfigTypeDef",
     {
         "Alarms": Sequence[AlarmTypeDef],
     },
     total=False,
 )
 
-_RequiredHyperParameterAlgorithmSpecificationOutputTypeDef = TypedDict(
-    "_RequiredHyperParameterAlgorithmSpecificationOutputTypeDef",
-    {
-        "TrainingInputMode": TrainingInputModeType,
-    },
-)
-_OptionalHyperParameterAlgorithmSpecificationOutputTypeDef = TypedDict(
-    "_OptionalHyperParameterAlgorithmSpecificationOutputTypeDef",
-    {
-        "TrainingImage": str,
-        "AlgorithmName": str,
-        "MetricDefinitions": List[MetricDefinitionTypeDef],
-    },
-    total=False,
-)
-
-
-class HyperParameterAlgorithmSpecificationOutputTypeDef(
-    _RequiredHyperParameterAlgorithmSpecificationOutputTypeDef,
-    _OptionalHyperParameterAlgorithmSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredHyperParameterAlgorithmSpecificationTypeDef = TypedDict(
     "_RequiredHyperParameterAlgorithmSpecificationTypeDef",
     {
         "TrainingInputMode": TrainingInputModeType,
     },
 )
 _OptionalHyperParameterAlgorithmSpecificationTypeDef = TypedDict(
@@ -8735,36 +8248,14 @@
     {
         "Apps": List[AppDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AppSpecificationUnionTypeDef = Union[AppSpecificationTypeDef, AppSpecificationOutputTypeDef]
-_RequiredArtifactSourceOutputTypeDef = TypedDict(
-    "_RequiredArtifactSourceOutputTypeDef",
-    {
-        "SourceUri": str,
-    },
-)
-_OptionalArtifactSourceOutputTypeDef = TypedDict(
-    "_OptionalArtifactSourceOutputTypeDef",
-    {
-        "SourceTypes": List[ArtifactSourceTypeTypeDef],
-    },
-    total=False,
-)
-
-
-class ArtifactSourceOutputTypeDef(
-    _RequiredArtifactSourceOutputTypeDef, _OptionalArtifactSourceOutputTypeDef
-):
-    pass
-
-
 _RequiredArtifactSourceTypeDef = TypedDict(
     "_RequiredArtifactSourceTypeDef",
     {
         "SourceUri": str,
     },
 )
 _OptionalArtifactSourceTypeDef = TypedDict(
@@ -8776,53 +8267,25 @@
 )
 
 
 class ArtifactSourceTypeDef(_RequiredArtifactSourceTypeDef, _OptionalArtifactSourceTypeDef):
     pass
 
 
-AsyncInferenceOutputConfigOutputTypeDef = TypedDict(
-    "AsyncInferenceOutputConfigOutputTypeDef",
-    {
-        "KmsKeyId": str,
-        "S3OutputPath": str,
-        "NotificationConfig": AsyncInferenceNotificationConfigOutputTypeDef,
-        "S3FailurePath": str,
-    },
-    total=False,
-)
-
 AsyncInferenceOutputConfigTypeDef = TypedDict(
     "AsyncInferenceOutputConfigTypeDef",
     {
         "KmsKeyId": str,
         "S3OutputPath": str,
         "NotificationConfig": AsyncInferenceNotificationConfigTypeDef,
         "S3FailurePath": str,
     },
     total=False,
 )
 
-AutoMLCandidateGenerationConfigOutputTypeDef = TypedDict(
-    "AutoMLCandidateGenerationConfigOutputTypeDef",
-    {
-        "FeatureSpecificationS3Uri": str,
-        "AlgorithmsConfig": List[AutoMLAlgorithmConfigOutputTypeDef],
-    },
-    total=False,
-)
-
-CandidateGenerationConfigOutputTypeDef = TypedDict(
-    "CandidateGenerationConfigOutputTypeDef",
-    {
-        "AlgorithmsConfig": List[AutoMLAlgorithmConfigOutputTypeDef],
-    },
-    total=False,
-)
-
 AutoMLCandidateGenerationConfigTypeDef = TypedDict(
     "AutoMLCandidateGenerationConfigTypeDef",
     {
         "FeatureSpecificationS3Uri": str,
         "AlgorithmsConfig": Sequence[AutoMLAlgorithmConfigTypeDef],
     },
     total=False,
@@ -8847,24 +8310,36 @@
     "ImageClassificationJobConfigTypeDef",
     {
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
     },
     total=False,
 )
 
-TextClassificationJobConfigTypeDef = TypedDict(
-    "TextClassificationJobConfigTypeDef",
+_RequiredTextClassificationJobConfigTypeDef = TypedDict(
+    "_RequiredTextClassificationJobConfigTypeDef",
     {
-        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
         "ContentColumn": str,
         "TargetLabelColumn": str,
     },
+)
+_OptionalTextClassificationJobConfigTypeDef = TypedDict(
+    "_OptionalTextClassificationJobConfigTypeDef",
+    {
+        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
+    },
     total=False,
 )
 
+
+class TextClassificationJobConfigTypeDef(
+    _RequiredTextClassificationJobConfigTypeDef, _OptionalTextClassificationJobConfigTypeDef
+):
+    pass
+
+
 ResolvedAttributesTypeDef = TypedDict(
     "ResolvedAttributesTypeDef",
     {
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "ProblemType": ProblemTypeType,
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
     },
@@ -8901,53 +8376,14 @@
     "AutoMLProblemTypeResolvedAttributesTypeDef",
     {
         "TabularResolvedAttributes": TabularResolvedAttributesTypeDef,
     },
     total=False,
 )
 
-AutoMLSecurityConfigOutputTypeDef = TypedDict(
-    "AutoMLSecurityConfigOutputTypeDef",
-    {
-        "VolumeKmsKeyId": str,
-        "EnableInterContainerTrafficEncryption": bool,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-LabelingJobResourceConfigOutputTypeDef = TypedDict(
-    "LabelingJobResourceConfigOutputTypeDef",
-    {
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-MonitoringNetworkConfigOutputTypeDef = TypedDict(
-    "MonitoringNetworkConfigOutputTypeDef",
-    {
-        "EnableInterContainerTrafficEncryption": bool,
-        "EnableNetworkIsolation": bool,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-NetworkConfigOutputTypeDef = TypedDict(
-    "NetworkConfigOutputTypeDef",
-    {
-        "EnableInterContainerTrafficEncryption": bool,
-        "EnableNetworkIsolation": bool,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 AutoMLSecurityConfigTypeDef = TypedDict(
     "AutoMLSecurityConfigTypeDef",
     {
         "VolumeKmsKeyId": str,
         "EnableInterContainerTrafficEncryption": bool,
         "VpcConfig": VpcConfigTypeDef,
     },
@@ -8979,15 +8415,14 @@
         "EnableInterContainerTrafficEncryption": bool,
         "EnableNetworkIsolation": bool,
         "VpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
-VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 BiasTypeDef = TypedDict(
     "BiasTypeDef",
     {
         "Report": MetricsSourceTypeDef,
         "PreTrainingReport": MetricsSourceTypeDef,
         "PostTrainingReport": MetricsSourceTypeDef,
     },
@@ -9090,60 +8525,61 @@
 )
 
 CanvasAppSettingsTypeDef = TypedDict(
     "CanvasAppSettingsTypeDef",
     {
         "TimeSeriesForecastingSettings": TimeSeriesForecastingSettingsTypeDef,
         "ModelRegisterSettings": ModelRegisterSettingsTypeDef,
+        "WorkspaceSettings": WorkspaceSettingsTypeDef,
     },
     total=False,
 )
 
-_RequiredTrafficRoutingConfigTypeDef = TypedDict(
-    "_RequiredTrafficRoutingConfigTypeDef",
+_RequiredRollingUpdatePolicyTypeDef = TypedDict(
+    "_RequiredRollingUpdatePolicyTypeDef",
     {
-        "Type": TrafficRoutingConfigTypeType,
+        "MaximumBatchSize": CapacitySizeTypeDef,
         "WaitIntervalInSeconds": int,
     },
 )
-_OptionalTrafficRoutingConfigTypeDef = TypedDict(
-    "_OptionalTrafficRoutingConfigTypeDef",
+_OptionalRollingUpdatePolicyTypeDef = TypedDict(
+    "_OptionalRollingUpdatePolicyTypeDef",
     {
-        "CanarySize": CapacitySizeTypeDef,
-        "LinearStepSize": CapacitySizeTypeDef,
+        "MaximumExecutionTimeoutInSeconds": int,
+        "RollbackMaximumBatchSize": CapacitySizeTypeDef,
     },
     total=False,
 )
 
 
-class TrafficRoutingConfigTypeDef(
-    _RequiredTrafficRoutingConfigTypeDef, _OptionalTrafficRoutingConfigTypeDef
+class RollingUpdatePolicyTypeDef(
+    _RequiredRollingUpdatePolicyTypeDef, _OptionalRollingUpdatePolicyTypeDef
 ):
     pass
 
 
-_RequiredInferenceExperimentDataStorageConfigOutputTypeDef = TypedDict(
-    "_RequiredInferenceExperimentDataStorageConfigOutputTypeDef",
+_RequiredTrafficRoutingConfigTypeDef = TypedDict(
+    "_RequiredTrafficRoutingConfigTypeDef",
     {
-        "Destination": str,
+        "Type": TrafficRoutingConfigTypeType,
+        "WaitIntervalInSeconds": int,
     },
 )
-_OptionalInferenceExperimentDataStorageConfigOutputTypeDef = TypedDict(
-    "_OptionalInferenceExperimentDataStorageConfigOutputTypeDef",
+_OptionalTrafficRoutingConfigTypeDef = TypedDict(
+    "_OptionalTrafficRoutingConfigTypeDef",
     {
-        "KmsKey": str,
-        "ContentType": CaptureContentTypeHeaderOutputTypeDef,
+        "CanarySize": CapacitySizeTypeDef,
+        "LinearStepSize": CapacitySizeTypeDef,
     },
     total=False,
 )
 
 
-class InferenceExperimentDataStorageConfigOutputTypeDef(
-    _RequiredInferenceExperimentDataStorageConfigOutputTypeDef,
-    _OptionalInferenceExperimentDataStorageConfigOutputTypeDef,
+class TrafficRoutingConfigTypeDef(
+    _RequiredTrafficRoutingConfigTypeDef, _OptionalTrafficRoutingConfigTypeDef
 ):
     pass
 
 
 _RequiredInferenceExperimentDataStorageConfigTypeDef = TypedDict(
     "_RequiredInferenceExperimentDataStorageConfigTypeDef",
     {
@@ -9163,39 +8599,14 @@
 class InferenceExperimentDataStorageConfigTypeDef(
     _RequiredInferenceExperimentDataStorageConfigTypeDef,
     _OptionalInferenceExperimentDataStorageConfigTypeDef,
 ):
     pass
 
 
-_RequiredDataCaptureConfigOutputTypeDef = TypedDict(
-    "_RequiredDataCaptureConfigOutputTypeDef",
-    {
-        "InitialSamplingPercentage": int,
-        "DestinationS3Uri": str,
-        "CaptureOptions": List[CaptureOptionTypeDef],
-    },
-)
-_OptionalDataCaptureConfigOutputTypeDef = TypedDict(
-    "_OptionalDataCaptureConfigOutputTypeDef",
-    {
-        "EnableCapture": bool,
-        "KmsKeyId": str,
-        "CaptureContentTypeHeader": CaptureContentTypeHeaderOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DataCaptureConfigOutputTypeDef(
-    _RequiredDataCaptureConfigOutputTypeDef, _OptionalDataCaptureConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredDataCaptureConfigTypeDef = TypedDict(
     "_RequiredDataCaptureConfigTypeDef",
     {
         "InitialSamplingPercentage": int,
         "DestinationS3Uri": str,
         "CaptureOptions": Sequence[CaptureOptionTypeDef],
     },
@@ -9213,22 +8624,14 @@
 
 class DataCaptureConfigTypeDef(
     _RequiredDataCaptureConfigTypeDef, _OptionalDataCaptureConfigTypeDef
 ):
     pass
 
 
-EnvironmentParameterRangesOutputTypeDef = TypedDict(
-    "EnvironmentParameterRangesOutputTypeDef",
-    {
-        "CategoricalParameterRanges": List[CategoricalParameterOutputTypeDef],
-    },
-    total=False,
-)
-
 EnvironmentParameterRangesTypeDef = TypedDict(
     "EnvironmentParameterRangesTypeDef",
     {
         "CategoricalParameterRanges": Sequence[CategoricalParameterTypeDef],
     },
     total=False,
 )
@@ -9312,37 +8715,14 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "GitConfig": GitConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDebugHookConfigOutputTypeDef = TypedDict(
-    "_RequiredDebugHookConfigOutputTypeDef",
-    {
-        "S3OutputPath": str,
-    },
-)
-_OptionalDebugHookConfigOutputTypeDef = TypedDict(
-    "_OptionalDebugHookConfigOutputTypeDef",
-    {
-        "LocalPath": str,
-        "HookParameters": Dict[str, str],
-        "CollectionConfigurations": List[CollectionConfigurationOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class DebugHookConfigOutputTypeDef(
-    _RequiredDebugHookConfigOutputTypeDef, _OptionalDebugHookConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredDebugHookConfigTypeDef = TypedDict(
     "_RequiredDebugHookConfigTypeDef",
     {
         "S3OutputPath": str,
     },
 )
 _OptionalDebugHookConfigTypeDef = TypedDict(
@@ -9509,24 +8889,14 @@
         "FailureReason": str,
         "ResourceSpec": ResourceSpecTypeDef,
         "SpaceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JupyterServerAppSettingsOutputTypeDef = TypedDict(
-    "JupyterServerAppSettingsOutputTypeDef",
-    {
-        "DefaultResourceSpec": ResourceSpecTypeDef,
-        "LifecycleConfigArns": List[str],
-        "CodeRepositories": List[CodeRepositoryTypeDef],
-    },
-    total=False,
-)
-
 JupyterServerAppSettingsTypeDef = TypedDict(
     "JupyterServerAppSettingsTypeDef",
     {
         "DefaultResourceSpec": ResourceSpecTypeDef,
         "LifecycleConfigArns": Sequence[str],
         "CodeRepositories": Sequence[CodeRepositoryTypeDef],
     },
@@ -9676,36 +9046,14 @@
 
 class UpdateDeviceFleetRequestRequestTypeDef(
     _RequiredUpdateDeviceFleetRequestRequestTypeDef, _OptionalUpdateDeviceFleetRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateFeatureGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFeatureGroupRequestRequestTypeDef",
-    {
-        "FeatureGroupName": str,
-    },
-)
-_OptionalUpdateFeatureGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFeatureGroupRequestRequestTypeDef",
-    {
-        "FeatureAdditions": Sequence[FeatureDefinitionTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateFeatureGroupRequestRequestTypeDef(
-    _RequiredUpdateFeatureGroupRequestRequestTypeDef,
-    _OptionalUpdateFeatureGroupRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredCreateHubRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHubRequestRequestTypeDef",
     {
         "HubName": str,
         "HubDescription": str,
     },
 )
@@ -10944,14 +10292,28 @@
         "NextToken": str,
         "SortBy": ProjectSortByType,
         "SortOrder": ProjectSortOrderType,
     },
     total=False,
 )
 
+ListResourceCatalogsRequestRequestTypeDef = TypedDict(
+    "ListResourceCatalogsRequestRequestTypeDef",
+    {
+        "NameContains": str,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+        "SortOrder": ResourceCatalogSortOrderType,
+        "SortBy": Literal["CreationTime"],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 ListStudioLifecycleConfigsRequestRequestTypeDef = TypedDict(
     "ListStudioLifecycleConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "NameContains": str,
         "AppTypeEquals": StudioLifecycleConfigAppTypeType,
@@ -11150,55 +10512,33 @@
 
 class UpdateWorkforceRequestRequestTypeDef(
     _RequiredUpdateWorkforceRequestRequestTypeDef, _OptionalUpdateWorkforceRequestRequestTypeDef
 ):
     pass
 
 
-KernelGatewayAppSettingsOutputTypeDef = TypedDict(
-    "KernelGatewayAppSettingsOutputTypeDef",
-    {
-        "DefaultResourceSpec": ResourceSpecTypeDef,
-        "CustomImages": List[CustomImageTypeDef],
-        "LifecycleConfigArns": List[str],
-    },
-    total=False,
-)
-
 KernelGatewayAppSettingsTypeDef = TypedDict(
     "KernelGatewayAppSettingsTypeDef",
     {
         "DefaultResourceSpec": ResourceSpecTypeDef,
         "CustomImages": Sequence[CustomImageTypeDef],
         "LifecycleConfigArns": Sequence[str],
     },
     total=False,
 )
 
-RSessionAppSettingsOutputTypeDef = TypedDict(
-    "RSessionAppSettingsOutputTypeDef",
-    {
-        "DefaultResourceSpec": ResourceSpecTypeDef,
-        "CustomImages": List[CustomImageTypeDef],
-    },
-    total=False,
-)
-
 RSessionAppSettingsTypeDef = TypedDict(
     "RSessionAppSettingsTypeDef",
     {
         "DefaultResourceSpec": ResourceSpecTypeDef,
         "CustomImages": Sequence[CustomImageTypeDef],
     },
     total=False,
 )
 
-DataQualityAppSpecificationUnionTypeDef = Union[
-    DataQualityAppSpecificationTypeDef, DataQualityAppSpecificationOutputTypeDef
-]
 ModelBiasBaselineConfigTypeDef = TypedDict(
     "ModelBiasBaselineConfigTypeDef",
     {
         "BaseliningJobName": str,
         "ConstraintsResource": MonitoringConstraintsResourceTypeDef,
     },
     total=False,
@@ -11238,23 +10578,14 @@
         "BaseliningJobName": str,
         "ConstraintsResource": MonitoringConstraintsResourceTypeDef,
         "StatisticsResource": MonitoringStatisticsResourceTypeDef,
     },
     total=False,
 )
 
-DataSourceOutputTypeDef = TypedDict(
-    "DataSourceOutputTypeDef",
-    {
-        "S3DataSource": S3DataSourceOutputTypeDef,
-        "FileSystemDataSource": FileSystemDataSourceTypeDef,
-    },
-    total=False,
-)
-
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "S3DataSource": S3DataSourceTypeDef,
         "FileSystemDataSource": FileSystemDataSourceTypeDef,
     },
     total=False,
@@ -11268,17 +10599,14 @@
         "LocalPath": str,
         "DataDistributionType": DataDistributionTypeType,
         "InputMode": InputModeType,
     },
     total=False,
 )
 
-DebugRuleConfigurationUnionTypeDef = Union[
-    DebugRuleConfigurationTypeDef, DebugRuleConfigurationOutputTypeDef
-]
 _RequiredDeleteDomainRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDomainRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalDeleteDomainRequestRequestTypeDef = TypedDict(
@@ -11313,24 +10641,14 @@
 
 class DeploymentRecommendationTypeDef(
     _RequiredDeploymentRecommendationTypeDef, _OptionalDeploymentRecommendationTypeDef
 ):
     pass
 
 
-DeploymentStageStatusSummaryTypeDef = TypedDict(
-    "DeploymentStageStatusSummaryTypeDef",
-    {
-        "StageName": str,
-        "DeviceSelectionConfig": DeviceSelectionConfigOutputTypeDef,
-        "DeploymentConfig": EdgeDeploymentConfigTypeDef,
-        "DeploymentStatus": EdgeDeploymentStatusTypeDef,
-    },
-)
-
 _RequiredDeploymentStageTypeDef = TypedDict(
     "_RequiredDeploymentStageTypeDef",
     {
         "StageName": str,
         "DeviceSelectionConfig": DeviceSelectionConfigTypeDef,
     },
 )
@@ -11343,15 +10661,24 @@
 )
 
 
 class DeploymentStageTypeDef(_RequiredDeploymentStageTypeDef, _OptionalDeploymentStageTypeDef):
     pass
 
 
-NeoVpcConfigUnionTypeDef = Union[NeoVpcConfigTypeDef, NeoVpcConfigOutputTypeDef]
+DeploymentStageStatusSummaryTypeDef = TypedDict(
+    "DeploymentStageStatusSummaryTypeDef",
+    {
+        "StageName": str,
+        "DeviceSelectionConfig": DeviceSelectionConfigTypeDef,
+        "DeploymentConfig": EdgeDeploymentConfigTypeDef,
+        "DeploymentStatus": EdgeDeploymentStatusTypeDef,
+    },
+)
+
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceArn": str,
         "DeviceName": str,
         "Description": str,
         "DeviceFleetName": str,
@@ -11801,46 +11128,14 @@
         "HumanTaskUiStatus": HumanTaskUiStatusType,
         "CreationTime": datetime,
         "UiTemplate": UiTemplateInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredInferenceExperimentSummaryTypeDef = TypedDict(
-    "_RequiredInferenceExperimentSummaryTypeDef",
-    {
-        "Name": str,
-        "Type": Literal["ShadowMode"],
-        "Status": InferenceExperimentStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalInferenceExperimentSummaryTypeDef = TypedDict(
-    "_OptionalInferenceExperimentSummaryTypeDef",
-    {
-        "Schedule": InferenceExperimentScheduleOutputTypeDef,
-        "StatusReason": str,
-        "Description": str,
-        "CompletionTime": datetime,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
-
-class InferenceExperimentSummaryTypeDef(
-    _RequiredInferenceExperimentSummaryTypeDef, _OptionalInferenceExperimentSummaryTypeDef
-):
-    pass
-
-
-ModelBiasAppSpecificationUnionTypeDef = Union[
-    ModelBiasAppSpecificationTypeDef, ModelBiasAppSpecificationOutputTypeDef
-]
 DescribeModelCardExportJobResponseTypeDef = TypedDict(
     "DescribeModelCardExportJobResponseTypeDef",
     {
         "ModelCardExportJobName": str,
         "ModelCardExportJobArn": str,
         "Status": ModelCardExportJobStatusType,
         "ModelCardName": str,
@@ -11850,20 +11145,14 @@
         "LastModifiedAt": datetime,
         "FailureReason": str,
         "ExportArtifacts": ModelCardExportArtifactsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModelExplainabilityAppSpecificationUnionTypeDef = Union[
-    ModelExplainabilityAppSpecificationTypeDef, ModelExplainabilityAppSpecificationOutputTypeDef
-]
-ModelQualityAppSpecificationUnionTypeDef = Union[
-    ModelQualityAppSpecificationTypeDef, ModelQualityAppSpecificationOutputTypeDef
-]
 ListMonitoringExecutionsResponseTypeDef = TypedDict(
     "ListMonitoringExecutionsResponseTypeDef",
     {
         "MonitoringExecutionSummaries": List[MonitoringExecutionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -11882,15 +11171,14 @@
     {
         "SubscribedWorkteams": List[SubscribedWorkteamTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProfilerConfigUnionTypeDef = Union[ProfilerConfigTypeDef, ProfilerConfigOutputTypeDef]
 _RequiredTrainingJobSummaryTypeDef = TypedDict(
     "_RequiredTrainingJobSummaryTypeDef",
     {
         "TrainingJobName": str,
         "TrainingJobArn": str,
         "CreationTime": datetime,
         "TrainingJobStatus": TrainingJobStatusType,
@@ -12089,14 +11377,38 @@
     {
         "EndpointConfigs": List[EndpointConfigSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredEndpointOutputConfigurationTypeDef = TypedDict(
+    "_RequiredEndpointOutputConfigurationTypeDef",
+    {
+        "EndpointName": str,
+        "VariantName": str,
+    },
+)
+_OptionalEndpointOutputConfigurationTypeDef = TypedDict(
+    "_OptionalEndpointOutputConfigurationTypeDef",
+    {
+        "InstanceType": ProductionVariantInstanceTypeType,
+        "InitialInstanceCount": int,
+        "ServerlessConfig": ProductionVariantServerlessConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class EndpointOutputConfigurationTypeDef(
+    _RequiredEndpointOutputConfigurationTypeDef, _OptionalEndpointOutputConfigurationTypeDef
+):
+    pass
+
+
 EndpointPerformanceTypeDef = TypedDict(
     "EndpointPerformanceTypeDef",
     {
         "Metrics": InferenceMetricsTypeDef,
         "EndpointInfo": EndpointInfoTypeDef,
     },
 )
@@ -12167,14 +11479,39 @@
     {
         "FlowDefinitionSummaries": List[FlowDefinitionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef",
+    {
+        "InferenceRecommendationsJobName": str,
+    },
+)
+_OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef",
+    {
+        "RecommendationId": str,
+        "EndpointName": str,
+        "TargetCpuUtilizationPerCore": int,
+        "ScalingPolicyObjective": ScalingPolicyObjectiveTypeDef,
+    },
+    total=False,
+)
+
+
+class GetScalingConfigurationRecommendationRequestRequestTypeDef(
+    _RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef,
+    _OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef,
+):
+    pass
+
+
 GetSearchSuggestionsResponseTypeDef = TypedDict(
     "GetSearchSuggestionsResponseTypeDef",
     {
         "PropertyNameSuggestions": List[PropertyNameSuggestionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -12240,27 +11577,14 @@
     {
         "HumanTaskUiSummaries": List[HumanTaskUiSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-HyperParameterTuningResourceConfigOutputTypeDef = TypedDict(
-    "HyperParameterTuningResourceConfigOutputTypeDef",
-    {
-        "InstanceType": TrainingInstanceTypeType,
-        "InstanceCount": int,
-        "VolumeSizeInGB": int,
-        "VolumeKmsKeyId": str,
-        "AllocationStrategy": Literal["Prioritized"],
-        "InstanceConfigs": List[HyperParameterTuningInstanceConfigTypeDef],
-    },
-    total=False,
-)
-
 HyperParameterTuningResourceConfigTypeDef = TypedDict(
     "HyperParameterTuningResourceConfigTypeDef",
     {
         "InstanceType": TrainingInstanceTypeType,
         "InstanceCount": int,
         "VolumeSizeInGB": int,
         "VolumeKmsKeyId": str,
@@ -12303,22 +11627,14 @@
     "HyperParameterTuningJobStrategyConfigTypeDef",
     {
         "HyperbandStrategyConfig": HyperbandStrategyConfigTypeDef,
     },
     total=False,
 )
 
-HyperParameterTuningJobWarmStartConfigOutputTypeDef = TypedDict(
-    "HyperParameterTuningJobWarmStartConfigOutputTypeDef",
-    {
-        "ParentHyperParameterTuningJobs": List[ParentHyperParameterTuningJobTypeDef],
-        "WarmStartType": HyperParameterTuningJobWarmStartTypeType,
-    },
-)
-
 HyperParameterTuningJobWarmStartConfigTypeDef = TypedDict(
     "HyperParameterTuningJobWarmStartConfigTypeDef",
     {
         "ParentHyperParameterTuningJobs": Sequence[ParentHyperParameterTuningJobTypeDef],
         "WarmStartType": HyperParameterTuningJobWarmStartTypeType,
     },
 )
@@ -12376,39 +11692,14 @@
     {
         "InferenceRecommendationsJobs": List[InferenceRecommendationsJobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredResourceConfigOutputTypeDef = TypedDict(
-    "_RequiredResourceConfigOutputTypeDef",
-    {
-        "VolumeSizeInGB": int,
-    },
-)
-_OptionalResourceConfigOutputTypeDef = TypedDict(
-    "_OptionalResourceConfigOutputTypeDef",
-    {
-        "InstanceType": TrainingInstanceTypeType,
-        "InstanceCount": int,
-        "VolumeKmsKeyId": str,
-        "InstanceGroups": List[InstanceGroupTypeDef],
-        "KeepAlivePeriodInSeconds": int,
-    },
-    total=False,
-)
-
-
-class ResourceConfigOutputTypeDef(
-    _RequiredResourceConfigOutputTypeDef, _OptionalResourceConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredResourceConfigTypeDef = TypedDict(
     "_RequiredResourceConfigTypeDef",
     {
         "VolumeSizeInGB": int,
     },
 )
 _OptionalResourceConfigTypeDef = TypedDict(
@@ -12424,79 +11715,35 @@
 )
 
 
 class ResourceConfigTypeDef(_RequiredResourceConfigTypeDef, _OptionalResourceConfigTypeDef):
     pass
 
 
-ParameterRangeOutputTypeDef = TypedDict(
-    "ParameterRangeOutputTypeDef",
-    {
-        "IntegerParameterRangeSpecification": IntegerParameterRangeSpecificationTypeDef,
-        "ContinuousParameterRangeSpecification": ContinuousParameterRangeSpecificationTypeDef,
-        "CategoricalParameterRangeSpecification": (
-            CategoricalParameterRangeSpecificationOutputTypeDef
-        ),
-    },
-    total=False,
-)
-
 ParameterRangeTypeDef = TypedDict(
     "ParameterRangeTypeDef",
     {
         "IntegerParameterRangeSpecification": IntegerParameterRangeSpecificationTypeDef,
         "ContinuousParameterRangeSpecification": ContinuousParameterRangeSpecificationTypeDef,
         "CategoricalParameterRangeSpecification": CategoricalParameterRangeSpecificationTypeDef,
     },
     total=False,
 )
 
-ParameterRangesOutputTypeDef = TypedDict(
-    "ParameterRangesOutputTypeDef",
-    {
-        "IntegerParameterRanges": List[IntegerParameterRangeTypeDef],
-        "ContinuousParameterRanges": List[ContinuousParameterRangeTypeDef],
-        "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
-        "AutoParameters": List[AutoParameterTypeDef],
-    },
-    total=False,
-)
-
 ParameterRangesTypeDef = TypedDict(
     "ParameterRangesTypeDef",
     {
         "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
         "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
         "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
         "AutoParameters": Sequence[AutoParameterTypeDef],
     },
     total=False,
 )
 
-_RequiredKernelGatewayImageConfigOutputTypeDef = TypedDict(
-    "_RequiredKernelGatewayImageConfigOutputTypeDef",
-    {
-        "KernelSpecs": List[KernelSpecTypeDef],
-    },
-)
-_OptionalKernelGatewayImageConfigOutputTypeDef = TypedDict(
-    "_OptionalKernelGatewayImageConfigOutputTypeDef",
-    {
-        "FileSystemConfig": FileSystemConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class KernelGatewayImageConfigOutputTypeDef(
-    _RequiredKernelGatewayImageConfigOutputTypeDef, _OptionalKernelGatewayImageConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredKernelGatewayImageConfigTypeDef = TypedDict(
     "_RequiredKernelGatewayImageConfigTypeDef",
     {
         "KernelSpecs": Sequence[KernelSpecTypeDef],
     },
 )
 _OptionalKernelGatewayImageConfigTypeDef = TypedDict(
@@ -13434,14 +12681,27 @@
         "SortBy": SortByType,
         "SortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListResourceCatalogsRequestListResourceCatalogsPaginateTypeDef = TypedDict(
+    "ListResourceCatalogsRequestListResourceCatalogsPaginateTypeDef",
+    {
+        "NameContains": str,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+        "SortOrder": ResourceCatalogSortOrderType,
+        "SortBy": Literal["CreationTime"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
     "ListSpacesRequestListSpacesPaginateTypeDef",
     {
         "SortOrder": SortOrderType,
         "SortBy": SpaceSortKeyType,
         "DomainIdEquals": str,
         "SpaceNameContains": str,
@@ -13649,14 +12909,15 @@
 )
 _OptionalSearchRequestSearchPaginateTypeDef = TypedDict(
     "_OptionalSearchRequestSearchPaginateTypeDef",
     {
         "SearchExpression": "SearchExpressionTypeDef",
         "SortBy": str,
         "SortOrder": SearchSortOrderType,
+        "CrossAccountFilterOption": CrossAccountFilterOptionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchRequestSearchPaginateTypeDef(
@@ -13841,14 +13102,23 @@
     {
         "ProjectSummaryList": List[ProjectSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListResourceCatalogsResponseTypeDef = TypedDict(
+    "ListResourceCatalogsResponseTypeDef",
+    {
+        "ResourceCatalogs": List[ResourceCatalogTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "Spaces": List[SpaceDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -13877,28 +13147,28 @@
     {
         "UserProfiles": List[UserProfileDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MemberDefinitionOutputTypeDef = TypedDict(
-    "MemberDefinitionOutputTypeDef",
+MemberDefinitionTypeDef = TypedDict(
+    "MemberDefinitionTypeDef",
     {
         "CognitoMemberDefinition": CognitoMemberDefinitionTypeDef,
-        "OidcMemberDefinition": OidcMemberDefinitionOutputTypeDef,
+        "OidcMemberDefinition": OidcMemberDefinitionTypeDef,
     },
     total=False,
 )
 
-MemberDefinitionTypeDef = TypedDict(
-    "MemberDefinitionTypeDef",
+MetricSpecificationTypeDef = TypedDict(
+    "MetricSpecificationTypeDef",
     {
-        "CognitoMemberDefinition": CognitoMemberDefinitionTypeDef,
-        "OidcMemberDefinition": OidcMemberDefinitionTypeDef,
+        "Predefined": PredefinedMetricSpecificationTypeDef,
+        "Customized": CustomizedMetricSpecificationTypeDef,
     },
     total=False,
 )
 
 MonitoringAlertActionsTypeDef = TypedDict(
     "MonitoringAlertActionsTypeDef",
     {
@@ -13918,58 +13188,28 @@
     "ModelInfrastructureConfigTypeDef",
     {
         "InfrastructureType": Literal["RealTimeInference"],
         "RealTimeInferenceConfig": RealTimeInferenceConfigTypeDef,
     },
 )
 
-_RequiredModelPackageContainerDefinitionOutputTypeDef = TypedDict(
-    "_RequiredModelPackageContainerDefinitionOutputTypeDef",
-    {
-        "Image": str,
-    },
-)
-_OptionalModelPackageContainerDefinitionOutputTypeDef = TypedDict(
-    "_OptionalModelPackageContainerDefinitionOutputTypeDef",
-    {
-        "ContainerHostname": str,
-        "ImageDigest": str,
-        "ModelDataUrl": str,
-        "ProductId": str,
-        "Environment": Dict[str, str],
-        "ModelInput": ModelInputTypeDef,
-        "Framework": str,
-        "FrameworkVersion": str,
-        "NearestModelName": str,
-    },
-    total=False,
-)
-
-
-class ModelPackageContainerDefinitionOutputTypeDef(
-    _RequiredModelPackageContainerDefinitionOutputTypeDef,
-    _OptionalModelPackageContainerDefinitionOutputTypeDef,
-):
-    pass
-
-
 _RequiredModelPackageContainerDefinitionTypeDef = TypedDict(
     "_RequiredModelPackageContainerDefinitionTypeDef",
     {
         "Image": str,
     },
 )
 _OptionalModelPackageContainerDefinitionTypeDef = TypedDict(
     "_OptionalModelPackageContainerDefinitionTypeDef",
     {
         "ContainerHostname": str,
         "ImageDigest": str,
         "ModelDataUrl": str,
         "ProductId": str,
-        "Environment": Mapping[str, str],
+        "Environment": Dict[str, str],
         "ModelInput": ModelInputTypeDef,
         "Framework": str,
         "FrameworkVersion": str,
         "NearestModelName": str,
     },
     total=False,
 )
@@ -13977,28 +13217,20 @@
 
 class ModelPackageContainerDefinitionTypeDef(
     _RequiredModelPackageContainerDefinitionTypeDef, _OptionalModelPackageContainerDefinitionTypeDef
 ):
     pass
 
 
-RecommendationJobStoppingConditionsOutputTypeDef = TypedDict(
-    "RecommendationJobStoppingConditionsOutputTypeDef",
-    {
-        "MaxInvocations": int,
-        "ModelLatencyThresholds": List[ModelLatencyThresholdTypeDef],
-    },
-    total=False,
-)
-
 RecommendationJobStoppingConditionsTypeDef = TypedDict(
     "RecommendationJobStoppingConditionsTypeDef",
     {
         "MaxInvocations": int,
         "ModelLatencyThresholds": Sequence[ModelLatencyThresholdTypeDef],
+        "FlatInvocations": FlatInvocationsType,
     },
     total=False,
 )
 
 ModelMetadataSearchExpressionTypeDef = TypedDict(
     "ModelMetadataSearchExpressionTypeDef",
     {
@@ -14031,24 +13263,14 @@
 MonitoringResourcesTypeDef = TypedDict(
     "MonitoringResourcesTypeDef",
     {
         "ClusterConfig": MonitoringClusterConfigTypeDef,
     },
 )
 
-MonitoringDatasetFormatOutputTypeDef = TypedDict(
-    "MonitoringDatasetFormatOutputTypeDef",
-    {
-        "Csv": MonitoringCsvDatasetFormatTypeDef,
-        "Json": MonitoringJsonDatasetFormatTypeDef,
-        "Parquet": Dict[str, Any],
-    },
-    total=False,
-)
-
 MonitoringDatasetFormatTypeDef = TypedDict(
     "MonitoringDatasetFormatTypeDef",
     {
         "Csv": MonitoringCsvDatasetFormatTypeDef,
         "Json": MonitoringJsonDatasetFormatTypeDef,
         "Parquet": Mapping[str, Any],
     },
@@ -14086,14 +13308,23 @@
 
 
 OnlineStoreConfigTypeDef = TypedDict(
     "OnlineStoreConfigTypeDef",
     {
         "SecurityConfig": OnlineStoreSecurityConfigTypeDef,
         "EnableOnlineStore": bool,
+        "TtlDuration": TtlDurationTypeDef,
+    },
+    total=False,
+)
+
+OnlineStoreConfigUpdateTypeDef = TypedDict(
+    "OnlineStoreConfigUpdateTypeDef",
+    {
+        "TtlDuration": TtlDurationTypeDef,
     },
     total=False,
 )
 
 _RequiredOutputConfigTypeDef = TypedDict(
     "_RequiredOutputConfigTypeDef",
     {
@@ -14170,32 +13401,14 @@
 
 class ProductionVariantSummaryTypeDef(
     _RequiredProductionVariantSummaryTypeDef, _OptionalProductionVariantSummaryTypeDef
 ):
     pass
 
 
-TrafficPatternOutputTypeDef = TypedDict(
-    "TrafficPatternOutputTypeDef",
-    {
-        "TrafficType": Literal["PHASES"],
-        "Phases": List[PhaseTypeDef],
-    },
-    total=False,
-)
-
-TrafficPatternTypeDef = TypedDict(
-    "TrafficPatternTypeDef",
-    {
-        "TrafficType": Literal["PHASES"],
-        "Phases": Sequence[PhaseTypeDef],
-    },
-    total=False,
-)
-
 ProcessingResourcesTypeDef = TypedDict(
     "ProcessingResourcesTypeDef",
     {
         "ClusterConfig": ProcessingClusterConfigTypeDef,
     },
 )
 
@@ -14247,49 +13460,22 @@
 
 class ProductionVariantTypeDef(
     _RequiredProductionVariantTypeDef, _OptionalProductionVariantTypeDef
 ):
     pass
 
 
-ProfilerRuleConfigurationUnionTypeDef = Union[
-    ProfilerRuleConfigurationTypeDef, ProfilerRuleConfigurationOutputTypeDef
-]
 SuggestionQueryTypeDef = TypedDict(
     "SuggestionQueryTypeDef",
     {
         "PropertyNameQuery": PropertyNameQueryTypeDef,
     },
     total=False,
 )
 
-_RequiredServiceCatalogProvisioningDetailsOutputTypeDef = TypedDict(
-    "_RequiredServiceCatalogProvisioningDetailsOutputTypeDef",
-    {
-        "ProductId": str,
-    },
-)
-_OptionalServiceCatalogProvisioningDetailsOutputTypeDef = TypedDict(
-    "_OptionalServiceCatalogProvisioningDetailsOutputTypeDef",
-    {
-        "ProvisioningArtifactId": str,
-        "PathId": str,
-        "ProvisioningParameters": List[ProvisioningParameterTypeDef],
-    },
-    total=False,
-)
-
-
-class ServiceCatalogProvisioningDetailsOutputTypeDef(
-    _RequiredServiceCatalogProvisioningDetailsOutputTypeDef,
-    _OptionalServiceCatalogProvisioningDetailsOutputTypeDef,
-):
-    pass
-
-
 _RequiredServiceCatalogProvisioningDetailsTypeDef = TypedDict(
     "_RequiredServiceCatalogProvisioningDetailsTypeDef",
     {
         "ProductId": str,
     },
 )
 _OptionalServiceCatalogProvisioningDetailsTypeDef = TypedDict(
@@ -14342,40 +13528,26 @@
     {
         "KmsKeyId": str,
         "CompiledOutputConfig": RecommendationJobCompiledOutputConfigTypeDef,
     },
     total=False,
 )
 
-RecommendationJobContainerConfigOutputTypeDef = TypedDict(
-    "RecommendationJobContainerConfigOutputTypeDef",
-    {
-        "Domain": str,
-        "Task": str,
-        "Framework": str,
-        "FrameworkVersion": str,
-        "PayloadConfig": RecommendationJobPayloadConfigOutputTypeDef,
-        "NearestModelName": str,
-        "SupportedInstanceTypes": List[str],
-        "DataInputConfig": str,
-    },
-    total=False,
-)
-
 RecommendationJobContainerConfigTypeDef = TypedDict(
     "RecommendationJobContainerConfigTypeDef",
     {
         "Domain": str,
         "Task": str,
         "Framework": str,
         "FrameworkVersion": str,
         "PayloadConfig": RecommendationJobPayloadConfigTypeDef,
         "NearestModelName": str,
         "SupportedInstanceTypes": Sequence[str],
         "DataInputConfig": str,
+        "SupportedEndpointType": RecommendationJobSupportedEndpointTypeType,
     },
     total=False,
 )
 
 _RequiredRenderUiTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredRenderUiTemplateRequestRequestTypeDef",
     {
@@ -14404,61 +13576,96 @@
     {
         "RenderedContent": str,
         "Errors": List[RenderingErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SelectiveExecutionConfigOutputTypeDef = TypedDict(
-    "SelectiveExecutionConfigOutputTypeDef",
+_RequiredUpdateTrainingJobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTrainingJobRequestRequestTypeDef",
     {
-        "SourcePipelineExecutionArn": str,
-        "SelectedSteps": List[SelectedStepTypeDef],
+        "TrainingJobName": str,
     },
 )
+_OptionalUpdateTrainingJobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTrainingJobRequestRequestTypeDef",
+    {
+        "ProfilerConfig": ProfilerConfigForUpdateTypeDef,
+        "ProfilerRuleConfigurations": Sequence[ProfilerRuleConfigurationTypeDef],
+        "ResourceConfig": ResourceConfigForUpdateTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateTrainingJobRequestRequestTypeDef(
+    _RequiredUpdateTrainingJobRequestRequestTypeDef, _OptionalUpdateTrainingJobRequestRequestTypeDef
+):
+    pass
+
 
 SelectiveExecutionConfigTypeDef = TypedDict(
     "SelectiveExecutionConfigTypeDef",
     {
         "SourcePipelineExecutionArn": str,
-        "SelectedSteps": Sequence[SelectedStepTypeDef],
+        "SelectedSteps": List[SelectedStepTypeDef],
     },
 )
 
-ShadowModeConfigOutputTypeDef = TypedDict(
-    "ShadowModeConfigOutputTypeDef",
+ShadowModeConfigTypeDef = TypedDict(
+    "ShadowModeConfigTypeDef",
     {
         "SourceModelVariantName": str,
-        "ShadowModelVariants": List[ShadowModelVariantConfigTypeDef],
+        "ShadowModelVariants": Sequence[ShadowModelVariantConfigTypeDef],
     },
 )
 
-ShadowModeConfigTypeDef = TypedDict(
-    "ShadowModeConfigTypeDef",
+SourceAlgorithmSpecificationTypeDef = TypedDict(
+    "SourceAlgorithmSpecificationTypeDef",
     {
-        "SourceModelVariantName": str,
-        "ShadowModelVariants": Sequence[ShadowModelVariantConfigTypeDef],
+        "SourceAlgorithms": Sequence[SourceAlgorithmTypeDef],
     },
 )
 
-SourceAlgorithmSpecificationOutputTypeDef = TypedDict(
-    "SourceAlgorithmSpecificationOutputTypeDef",
+TrafficPatternTypeDef = TypedDict(
+    "TrafficPatternTypeDef",
     {
-        "SourceAlgorithms": List[SourceAlgorithmTypeDef],
+        "TrafficType": TrafficTypeType,
+        "Phases": Sequence[PhaseTypeDef],
+        "Stairs": StairsTypeDef,
     },
+    total=False,
 )
 
-SourceAlgorithmSpecificationTypeDef = TypedDict(
-    "SourceAlgorithmSpecificationTypeDef",
+_RequiredTimeSeriesForecastingJobConfigTypeDef = TypedDict(
+    "_RequiredTimeSeriesForecastingJobConfigTypeDef",
     {
-        "SourceAlgorithms": Sequence[SourceAlgorithmTypeDef],
+        "ForecastFrequency": str,
+        "ForecastHorizon": int,
+        "TimeSeriesConfig": TimeSeriesConfigTypeDef,
     },
 )
+_OptionalTimeSeriesForecastingJobConfigTypeDef = TypedDict(
+    "_OptionalTimeSeriesForecastingJobConfigTypeDef",
+    {
+        "FeatureSpecificationS3Uri": str,
+        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
+        "ForecastQuantiles": Sequence[str],
+        "Transformations": TimeSeriesTransformationsTypeDef,
+    },
+    total=False,
+)
+
+
+class TimeSeriesForecastingJobConfigTypeDef(
+    _RequiredTimeSeriesForecastingJobConfigTypeDef, _OptionalTimeSeriesForecastingJobConfigTypeDef
+):
+    pass
+
 
-SourceIpConfigUnionTypeDef = Union[SourceIpConfigTypeDef, SourceIpConfigOutputTypeDef]
 _RequiredTrainingImageConfigTypeDef = TypedDict(
     "_RequiredTrainingImageConfigTypeDef",
     {
         "TrainingRepositoryAccessMode": TrainingRepositoryAccessModeType,
     },
 )
 _OptionalTrainingImageConfigTypeDef = TypedDict(
@@ -14490,15 +13697,15 @@
         "WorkforceArn": str,
     },
 )
 _OptionalWorkforceTypeDef = TypedDict(
     "_OptionalWorkforceTypeDef",
     {
         "LastUpdatedDate": datetime,
-        "SourceIpConfig": SourceIpConfigOutputTypeDef,
+        "SourceIpConfig": SourceIpConfigTypeDef,
         "SubDomain": str,
         "CognitoConfig": CognitoConfigTypeDef,
         "OidcConfig": OidcConfigForResponseTypeDef,
         "CreateDate": datetime,
         "WorkforceVpcConfig": WorkforceVpcConfigResponseTypeDef,
         "Status": WorkforceStatusType,
         "FailureReason": str,
@@ -14521,23 +13728,22 @@
 )
 
 ArtifactSummaryTypeDef = TypedDict(
     "ArtifactSummaryTypeDef",
     {
         "ArtifactArn": str,
         "ArtifactName": str,
-        "Source": ArtifactSourceOutputTypeDef,
+        "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-ArtifactSourceUnionTypeDef = Union[ArtifactSourceTypeDef, ArtifactSourceOutputTypeDef]
 _RequiredCreateArtifactRequestRequestTypeDef = TypedDict(
     "_RequiredCreateArtifactRequestRequestTypeDef",
     {
         "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
     },
 )
@@ -14564,35 +13770,14 @@
     {
         "ArtifactArn": str,
         "Source": ArtifactSourceTypeDef,
     },
     total=False,
 )
 
-_RequiredAsyncInferenceConfigOutputTypeDef = TypedDict(
-    "_RequiredAsyncInferenceConfigOutputTypeDef",
-    {
-        "OutputConfig": AsyncInferenceOutputConfigOutputTypeDef,
-    },
-)
-_OptionalAsyncInferenceConfigOutputTypeDef = TypedDict(
-    "_OptionalAsyncInferenceConfigOutputTypeDef",
-    {
-        "ClientConfig": AsyncInferenceClientConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class AsyncInferenceConfigOutputTypeDef(
-    _RequiredAsyncInferenceConfigOutputTypeDef, _OptionalAsyncInferenceConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredAsyncInferenceConfigTypeDef = TypedDict(
     "_RequiredAsyncInferenceConfigTypeDef",
     {
         "OutputConfig": AsyncInferenceOutputConfigTypeDef,
     },
 )
 _OptionalAsyncInferenceConfigTypeDef = TypedDict(
@@ -14606,41 +13791,14 @@
 
 class AsyncInferenceConfigTypeDef(
     _RequiredAsyncInferenceConfigTypeDef, _OptionalAsyncInferenceConfigTypeDef
 ):
     pass
 
 
-_RequiredTabularJobConfigOutputTypeDef = TypedDict(
-    "_RequiredTabularJobConfigOutputTypeDef",
-    {
-        "TargetAttributeName": str,
-    },
-)
-_OptionalTabularJobConfigOutputTypeDef = TypedDict(
-    "_OptionalTabularJobConfigOutputTypeDef",
-    {
-        "CandidateGenerationConfig": CandidateGenerationConfigOutputTypeDef,
-        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
-        "FeatureSpecificationS3Uri": str,
-        "Mode": AutoMLModeType,
-        "GenerateCandidateDefinitionsOnly": bool,
-        "ProblemType": ProblemTypeType,
-        "SampleWeightAttributeName": str,
-    },
-    total=False,
-)
-
-
-class TabularJobConfigOutputTypeDef(
-    _RequiredTabularJobConfigOutputTypeDef, _OptionalTabularJobConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredTabularJobConfigTypeDef = TypedDict(
     "_RequiredTabularJobConfigTypeDef",
     {
         "TargetAttributeName": str,
     },
 )
 _OptionalTabularJobConfigTypeDef = TypedDict(
@@ -14711,64 +13869,26 @@
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
         "AutoMLProblemTypeResolvedAttributes": AutoMLProblemTypeResolvedAttributesTypeDef,
     },
     total=False,
 )
 
-AutoMLJobConfigOutputTypeDef = TypedDict(
-    "AutoMLJobConfigOutputTypeDef",
-    {
-        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
-        "SecurityConfig": AutoMLSecurityConfigOutputTypeDef,
-        "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
-        "CandidateGenerationConfig": AutoMLCandidateGenerationConfigOutputTypeDef,
-        "Mode": AutoMLModeType,
-    },
-    total=False,
-)
-
-_RequiredLabelingJobAlgorithmsConfigOutputTypeDef = TypedDict(
-    "_RequiredLabelingJobAlgorithmsConfigOutputTypeDef",
-    {
-        "LabelingJobAlgorithmSpecificationArn": str,
-    },
-)
-_OptionalLabelingJobAlgorithmsConfigOutputTypeDef = TypedDict(
-    "_OptionalLabelingJobAlgorithmsConfigOutputTypeDef",
-    {
-        "InitialActiveLearningModelArn": str,
-        "LabelingJobResourceConfig": LabelingJobResourceConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class LabelingJobAlgorithmsConfigOutputTypeDef(
-    _RequiredLabelingJobAlgorithmsConfigOutputTypeDef,
-    _OptionalLabelingJobAlgorithmsConfigOutputTypeDef,
-):
-    pass
-
-
 AutoMLJobConfigTypeDef = TypedDict(
     "AutoMLJobConfigTypeDef",
     {
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
         "SecurityConfig": AutoMLSecurityConfigTypeDef,
         "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
         "CandidateGenerationConfig": AutoMLCandidateGenerationConfigTypeDef,
         "Mode": AutoMLModeType,
     },
     total=False,
 )
 
-AutoMLSecurityConfigUnionTypeDef = Union[
-    AutoMLSecurityConfigTypeDef, AutoMLSecurityConfigOutputTypeDef
-]
 _RequiredLabelingJobAlgorithmsConfigTypeDef = TypedDict(
     "_RequiredLabelingJobAlgorithmsConfigTypeDef",
     {
         "LabelingJobAlgorithmSpecificationArn": str,
     },
 )
 _OptionalLabelingJobAlgorithmsConfigTypeDef = TypedDict(
@@ -14783,18 +13903,14 @@
 
 class LabelingJobAlgorithmsConfigTypeDef(
     _RequiredLabelingJobAlgorithmsConfigTypeDef, _OptionalLabelingJobAlgorithmsConfigTypeDef
 ):
     pass
 
 
-MonitoringNetworkConfigUnionTypeDef = Union[
-    MonitoringNetworkConfigTypeDef, MonitoringNetworkConfigOutputTypeDef
-]
-NetworkConfigUnionTypeDef = Union[NetworkConfigTypeDef, NetworkConfigOutputTypeDef]
 ModelMetricsTypeDef = TypedDict(
     "ModelMetricsTypeDef",
     {
         "ModelQuality": ModelQualityTypeDef,
         "ModelDataQuality": ModelDataQualityTypeDef,
         "Bias": BiasTypeDef,
         "Explainability": ExplainabilityTypeDef,
@@ -14872,85 +13988,25 @@
 
 class BlueGreenUpdatePolicyTypeDef(
     _RequiredBlueGreenUpdatePolicyTypeDef, _OptionalBlueGreenUpdatePolicyTypeDef
 ):
     pass
 
 
-InferenceExperimentDataStorageConfigUnionTypeDef = Union[
-    InferenceExperimentDataStorageConfigTypeDef, InferenceExperimentDataStorageConfigOutputTypeDef
-]
-DataCaptureConfigUnionTypeDef = Union[DataCaptureConfigTypeDef, DataCaptureConfigOutputTypeDef]
-_RequiredEndpointInputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEndpointInputConfigurationOutputTypeDef",
-    {
-        "InstanceType": ProductionVariantInstanceTypeType,
-    },
-)
-_OptionalEndpointInputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEndpointInputConfigurationOutputTypeDef",
-    {
-        "InferenceSpecificationName": str,
-        "EnvironmentParameterRanges": EnvironmentParameterRangesOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class EndpointInputConfigurationOutputTypeDef(
-    _RequiredEndpointInputConfigurationOutputTypeDef,
-    _OptionalEndpointInputConfigurationOutputTypeDef,
-):
-    pass
-
-
-_RequiredEndpointInputConfigurationTypeDef = TypedDict(
-    "_RequiredEndpointInputConfigurationTypeDef",
+EndpointInputConfigurationTypeDef = TypedDict(
+    "EndpointInputConfigurationTypeDef",
     {
         "InstanceType": ProductionVariantInstanceTypeType,
-    },
-)
-_OptionalEndpointInputConfigurationTypeDef = TypedDict(
-    "_OptionalEndpointInputConfigurationTypeDef",
-    {
         "InferenceSpecificationName": str,
         "EnvironmentParameterRanges": EnvironmentParameterRangesTypeDef,
+        "ServerlessConfig": ProductionVariantServerlessConfigTypeDef,
     },
     total=False,
 )
 
-
-class EndpointInputConfigurationTypeDef(
-    _RequiredEndpointInputConfigurationTypeDef, _OptionalEndpointInputConfigurationTypeDef
-):
-    pass
-
-
-_RequiredClarifyExplainerConfigOutputTypeDef = TypedDict(
-    "_RequiredClarifyExplainerConfigOutputTypeDef",
-    {
-        "ShapConfig": ClarifyShapConfigTypeDef,
-    },
-)
-_OptionalClarifyExplainerConfigOutputTypeDef = TypedDict(
-    "_OptionalClarifyExplainerConfigOutputTypeDef",
-    {
-        "EnableExplanations": str,
-        "InferenceConfig": ClarifyInferenceConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ClarifyExplainerConfigOutputTypeDef(
-    _RequiredClarifyExplainerConfigOutputTypeDef, _OptionalClarifyExplainerConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredClarifyExplainerConfigTypeDef = TypedDict(
     "_RequiredClarifyExplainerConfigTypeDef",
     {
         "ShapConfig": ClarifyShapConfigTypeDef,
     },
 )
 _OptionalClarifyExplainerConfigTypeDef = TypedDict(
@@ -14974,15 +14030,14 @@
     {
         "CodeRepositorySummaryList": List[CodeRepositorySummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DebugHookConfigUnionTypeDef = Union[DebugHookConfigTypeDef, DebugHookConfigOutputTypeDef]
 ListContextsResponseTypeDef = TypedDict(
     "ListContextsResponseTypeDef",
     {
         "ContextSummaries": List[ContextSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -14994,71 +14049,67 @@
         "RStudioServerProDomainSettingsForUpdate": RStudioServerProDomainSettingsForUpdateTypeDef,
         "ExecutionRoleIdentityConfig": ExecutionRoleIdentityConfigType,
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-DomainSettingsOutputTypeDef = TypedDict(
-    "DomainSettingsOutputTypeDef",
+DomainSettingsTypeDef = TypedDict(
+    "DomainSettingsTypeDef",
     {
-        "SecurityGroupIds": List[str],
+        "SecurityGroupIds": Sequence[str],
         "RStudioServerProDomainSettings": RStudioServerProDomainSettingsTypeDef,
         "ExecutionRoleIdentityConfig": ExecutionRoleIdentityConfigType,
     },
     total=False,
 )
 
-DomainSettingsTypeDef = TypedDict(
-    "DomainSettingsTypeDef",
+_RequiredInferenceExperimentSummaryTypeDef = TypedDict(
+    "_RequiredInferenceExperimentSummaryTypeDef",
     {
-        "SecurityGroupIds": Sequence[str],
-        "RStudioServerProDomainSettings": RStudioServerProDomainSettingsTypeDef,
-        "ExecutionRoleIdentityConfig": ExecutionRoleIdentityConfigType,
+        "Name": str,
+        "Type": Literal["ShadowMode"],
+        "Status": InferenceExperimentStatusType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+    },
+)
+_OptionalInferenceExperimentSummaryTypeDef = TypedDict(
+    "_OptionalInferenceExperimentSummaryTypeDef",
+    {
+        "Schedule": InferenceExperimentScheduleTypeDef,
+        "StatusReason": str,
+        "Description": str,
+        "CompletionTime": datetime,
+        "RoleArn": str,
     },
     total=False,
 )
 
-InferenceExperimentScheduleUnionTypeDef = Union[
-    InferenceExperimentScheduleTypeDef, InferenceExperimentScheduleOutputTypeDef
-]
+
+class InferenceExperimentSummaryTypeDef(
+    _RequiredInferenceExperimentSummaryTypeDef, _OptionalInferenceExperimentSummaryTypeDef
+):
+    pass
+
+
 QueryLineageRequestRequestTypeDef = TypedDict(
     "QueryLineageRequestRequestTypeDef",
     {
         "StartArns": Sequence[str],
         "Direction": DirectionType,
         "IncludeEdges": bool,
         "Filters": QueryFiltersTypeDef,
         "MaxDepth": int,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DefaultSpaceSettingsOutputTypeDef = TypedDict(
-    "DefaultSpaceSettingsOutputTypeDef",
-    {
-        "ExecutionRole": str,
-        "SecurityGroups": List[str],
-        "JupyterServerAppSettings": JupyterServerAppSettingsOutputTypeDef,
-        "KernelGatewayAppSettings": KernelGatewayAppSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-SpaceSettingsOutputTypeDef = TypedDict(
-    "SpaceSettingsOutputTypeDef",
-    {
-        "JupyterServerAppSettings": JupyterServerAppSettingsOutputTypeDef,
-        "KernelGatewayAppSettings": KernelGatewayAppSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 DefaultSpaceSettingsTypeDef = TypedDict(
     "DefaultSpaceSettingsTypeDef",
     {
         "ExecutionRole": str,
         "SecurityGroups": Sequence[str],
         "JupyterServerAppSettings": JupyterServerAppSettingsTypeDef,
         "KernelGatewayAppSettings": KernelGatewayAppSettingsTypeDef,
@@ -15071,30 +14122,14 @@
     {
         "JupyterServerAppSettings": JupyterServerAppSettingsTypeDef,
         "KernelGatewayAppSettings": KernelGatewayAppSettingsTypeDef,
     },
     total=False,
 )
 
-UserSettingsOutputTypeDef = TypedDict(
-    "UserSettingsOutputTypeDef",
-    {
-        "ExecutionRole": str,
-        "SecurityGroups": List[str],
-        "SharingSettings": SharingSettingsTypeDef,
-        "JupyterServerAppSettings": JupyterServerAppSettingsOutputTypeDef,
-        "KernelGatewayAppSettings": KernelGatewayAppSettingsOutputTypeDef,
-        "TensorBoardAppSettings": TensorBoardAppSettingsTypeDef,
-        "RStudioServerProAppSettings": RStudioServerProAppSettingsTypeDef,
-        "RSessionAppSettings": RSessionAppSettingsOutputTypeDef,
-        "CanvasAppSettings": CanvasAppSettingsTypeDef,
-    },
-    total=False,
-)
-
 UserSettingsTypeDef = TypedDict(
     "UserSettingsTypeDef",
     {
         "ExecutionRole": str,
         "SecurityGroups": Sequence[str],
         "SharingSettings": SharingSettingsTypeDef,
         "JupyterServerAppSettings": JupyterServerAppSettingsTypeDef,
@@ -15103,38 +14138,14 @@
         "RStudioServerProAppSettings": RStudioServerProAppSettingsTypeDef,
         "RSessionAppSettings": RSessionAppSettingsTypeDef,
         "CanvasAppSettings": CanvasAppSettingsTypeDef,
     },
     total=False,
 )
 
-_RequiredChannelOutputTypeDef = TypedDict(
-    "_RequiredChannelOutputTypeDef",
-    {
-        "ChannelName": str,
-        "DataSource": DataSourceOutputTypeDef,
-    },
-)
-_OptionalChannelOutputTypeDef = TypedDict(
-    "_OptionalChannelOutputTypeDef",
-    {
-        "ContentType": str,
-        "CompressionType": CompressionTypeType,
-        "RecordWrapperType": RecordWrapperType,
-        "InputMode": TrainingInputModeType,
-        "ShuffleConfig": ShuffleConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
-    pass
-
-
 _RequiredChannelTypeDef = TypedDict(
     "_RequiredChannelTypeDef",
     {
         "ChannelName": str,
         "DataSource": DataSourceTypeDef,
     },
 )
@@ -15172,32 +14183,14 @@
 )
 
 
 class ProcessingInputTypeDef(_RequiredProcessingInputTypeDef, _OptionalProcessingInputTypeDef):
     pass
 
 
-DescribeEdgeDeploymentPlanResponseTypeDef = TypedDict(
-    "DescribeEdgeDeploymentPlanResponseTypeDef",
-    {
-        "EdgeDeploymentPlanArn": str,
-        "EdgeDeploymentPlanName": str,
-        "ModelConfigs": List[EdgeDeploymentModelConfigTypeDef],
-        "DeviceFleetName": str,
-        "EdgeDeploymentSuccess": int,
-        "EdgeDeploymentPending": int,
-        "EdgeDeploymentFailed": int,
-        "Stages": List[DeploymentStageStatusSummaryTypeDef],
-        "NextToken": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateEdgeDeploymentPlanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEdgeDeploymentPlanRequestRequestTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "ModelConfigs": Sequence[EdgeDeploymentModelConfigTypeDef],
         "DeviceFleetName": str,
     },
@@ -15223,36 +14216,45 @@
     "CreateEdgeDeploymentStageRequestRequestTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "Stages": Sequence[DeploymentStageTypeDef],
     },
 )
 
-ListExperimentsResponseTypeDef = TypedDict(
-    "ListExperimentsResponseTypeDef",
+DescribeEdgeDeploymentPlanResponseTypeDef = TypedDict(
+    "DescribeEdgeDeploymentPlanResponseTypeDef",
     {
-        "ExperimentSummaries": List[ExperimentSummaryTypeDef],
+        "EdgeDeploymentPlanArn": str,
+        "EdgeDeploymentPlanName": str,
+        "ModelConfigs": List[EdgeDeploymentModelConfigTypeDef],
+        "DeviceFleetName": str,
+        "EdgeDeploymentSuccess": int,
+        "EdgeDeploymentPending": int,
+        "EdgeDeploymentFailed": int,
+        "Stages": List[DeploymentStageStatusSummaryTypeDef],
         "NextToken": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListFeatureGroupsResponseTypeDef = TypedDict(
-    "ListFeatureGroupsResponseTypeDef",
+ListExperimentsResponseTypeDef = TypedDict(
+    "ListExperimentsResponseTypeDef",
     {
-        "FeatureGroupSummaries": List[FeatureGroupSummaryTypeDef],
+        "ExperimentSummaries": List[ExperimentSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListInferenceExperimentsResponseTypeDef = TypedDict(
-    "ListInferenceExperimentsResponseTypeDef",
+ListFeatureGroupsResponseTypeDef = TypedDict(
+    "ListFeatureGroupsResponseTypeDef",
     {
-        "InferenceExperiments": List[InferenceExperimentSummaryTypeDef],
+        "FeatureGroupSummaries": List[FeatureGroupSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrainingJobsResponseTypeDef = TypedDict(
     "ListTrainingJobsResponseTypeDef",
@@ -15377,18 +14379,14 @@
     {
         "HyperParameterTuningJobSummaries": List[HyperParameterTuningJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-HyperParameterTuningJobWarmStartConfigUnionTypeDef = Union[
-    HyperParameterTuningJobWarmStartConfigTypeDef,
-    HyperParameterTuningJobWarmStartConfigOutputTypeDef,
-]
 AssociationSummaryTypeDef = TypedDict(
     "AssociationSummaryTypeDef",
     {
         "SourceArn": str,
         "DestinationArn": str,
         "SourceType": str,
         "DestinationType": str,
@@ -15422,15 +14420,15 @@
 )
 
 DescribeArtifactResponseTypeDef = TypedDict(
     "DescribeArtifactResponseTypeDef",
     {
         "ArtifactName": str,
         "ArtifactArn": str,
-        "Source": ArtifactSourceOutputTypeDef,
+        "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
         "Properties": Dict[str, str],
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
@@ -15610,14 +14608,15 @@
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "Tags": List[TagTypeDef],
         "ModelId": str,
         "RiskRating": str,
+        "ModelPackageGroupName": str,
     },
     total=False,
 )
 
 ModelDashboardModelCardTypeDef = TypedDict(
     "ModelDashboardModelCardTypeDef",
     {
@@ -15697,42 +14696,14 @@
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
     },
     total=False,
 )
 
-ResourceConfigUnionTypeDef = Union[ResourceConfigTypeDef, ResourceConfigOutputTypeDef]
-_RequiredHyperParameterSpecificationOutputTypeDef = TypedDict(
-    "_RequiredHyperParameterSpecificationOutputTypeDef",
-    {
-        "Name": str,
-        "Type": ParameterTypeType,
-    },
-)
-_OptionalHyperParameterSpecificationOutputTypeDef = TypedDict(
-    "_OptionalHyperParameterSpecificationOutputTypeDef",
-    {
-        "Description": str,
-        "Range": ParameterRangeOutputTypeDef,
-        "IsTunable": bool,
-        "IsRequired": bool,
-        "DefaultValue": str,
-    },
-    total=False,
-)
-
-
-class HyperParameterSpecificationOutputTypeDef(
-    _RequiredHyperParameterSpecificationOutputTypeDef,
-    _OptionalHyperParameterSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredHyperParameterSpecificationTypeDef = TypedDict(
     "_RequiredHyperParameterSpecificationTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
     },
 )
@@ -15751,42 +14722,14 @@
 
 class HyperParameterSpecificationTypeDef(
     _RequiredHyperParameterSpecificationTypeDef, _OptionalHyperParameterSpecificationTypeDef
 ):
     pass
 
 
-_RequiredHyperParameterTuningJobConfigOutputTypeDef = TypedDict(
-    "_RequiredHyperParameterTuningJobConfigOutputTypeDef",
-    {
-        "Strategy": HyperParameterTuningJobStrategyTypeType,
-        "ResourceLimits": ResourceLimitsTypeDef,
-    },
-)
-_OptionalHyperParameterTuningJobConfigOutputTypeDef = TypedDict(
-    "_OptionalHyperParameterTuningJobConfigOutputTypeDef",
-    {
-        "StrategyConfig": HyperParameterTuningJobStrategyConfigTypeDef,
-        "HyperParameterTuningJobObjective": HyperParameterTuningJobObjectiveTypeDef,
-        "ParameterRanges": ParameterRangesOutputTypeDef,
-        "TrainingJobEarlyStoppingType": TrainingJobEarlyStoppingTypeType,
-        "TuningJobCompletionCriteria": TuningJobCompletionCriteriaTypeDef,
-        "RandomSeed": int,
-    },
-    total=False,
-)
-
-
-class HyperParameterTuningJobConfigOutputTypeDef(
-    _RequiredHyperParameterTuningJobConfigOutputTypeDef,
-    _OptionalHyperParameterTuningJobConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredHyperParameterTuningJobConfigTypeDef = TypedDict(
     "_RequiredHyperParameterTuningJobConfigTypeDef",
     {
         "Strategy": HyperParameterTuningJobStrategyTypeType,
         "ResourceLimits": ResourceLimitsTypeDef,
     },
 )
@@ -15813,31 +14756,19 @@
 AppImageConfigDetailsTypeDef = TypedDict(
     "AppImageConfigDetailsTypeDef",
     {
         "AppImageConfigArn": str,
         "AppImageConfigName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "KernelGatewayImageConfig": KernelGatewayImageConfigOutputTypeDef,
+        "KernelGatewayImageConfig": KernelGatewayImageConfigTypeDef,
     },
     total=False,
 )
 
-DescribeAppImageConfigResponseTypeDef = TypedDict(
-    "DescribeAppImageConfigResponseTypeDef",
-    {
-        "AppImageConfigArn": str,
-        "AppImageConfigName": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "KernelGatewayImageConfig": KernelGatewayImageConfigOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateAppImageConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppImageConfigRequestRequestTypeDef",
     {
         "AppImageConfigName": str,
     },
 )
 _OptionalCreateAppImageConfigRequestRequestTypeDef = TypedDict(
@@ -15853,17 +14784,26 @@
 class CreateAppImageConfigRequestRequestTypeDef(
     _RequiredCreateAppImageConfigRequestRequestTypeDef,
     _OptionalCreateAppImageConfigRequestRequestTypeDef,
 ):
     pass
 
 
-KernelGatewayImageConfigUnionTypeDef = Union[
-    KernelGatewayImageConfigTypeDef, KernelGatewayImageConfigOutputTypeDef
-]
+DescribeAppImageConfigResponseTypeDef = TypedDict(
+    "DescribeAppImageConfigResponseTypeDef",
+    {
+        "AppImageConfigArn": str,
+        "AppImageConfigName": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "KernelGatewayImageConfig": KernelGatewayImageConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateAppImageConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppImageConfigRequestRequestTypeDef",
     {
         "AppImageConfigName": str,
     },
 )
 _OptionalUpdateAppImageConfigRequestRequestTypeDef = TypedDict(
@@ -15887,61 +14827,88 @@
     {
         "LabelingJobSummaryList": List[LabelingJobForWorkteamSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLabelingJobInputConfigOutputTypeDef = TypedDict(
-    "_RequiredLabelingJobInputConfigOutputTypeDef",
+_RequiredLabelingJobInputConfigTypeDef = TypedDict(
+    "_RequiredLabelingJobInputConfigTypeDef",
     {
         "DataSource": LabelingJobDataSourceTypeDef,
     },
 )
-_OptionalLabelingJobInputConfigOutputTypeDef = TypedDict(
-    "_OptionalLabelingJobInputConfigOutputTypeDef",
+_OptionalLabelingJobInputConfigTypeDef = TypedDict(
+    "_OptionalLabelingJobInputConfigTypeDef",
     {
-        "DataAttributes": LabelingJobDataAttributesOutputTypeDef,
+        "DataAttributes": LabelingJobDataAttributesTypeDef,
     },
     total=False,
 )
 
 
-class LabelingJobInputConfigOutputTypeDef(
-    _RequiredLabelingJobInputConfigOutputTypeDef, _OptionalLabelingJobInputConfigOutputTypeDef
+class LabelingJobInputConfigTypeDef(
+    _RequiredLabelingJobInputConfigTypeDef, _OptionalLabelingJobInputConfigTypeDef
 ):
     pass
 
 
-_RequiredLabelingJobInputConfigTypeDef = TypedDict(
-    "_RequiredLabelingJobInputConfigTypeDef",
+_RequiredCreateWorkteamRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkteamRequestRequestTypeDef",
     {
-        "DataSource": LabelingJobDataSourceTypeDef,
+        "WorkteamName": str,
+        "MemberDefinitions": Sequence[MemberDefinitionTypeDef],
+        "Description": str,
     },
 )
-_OptionalLabelingJobInputConfigTypeDef = TypedDict(
-    "_OptionalLabelingJobInputConfigTypeDef",
+_OptionalCreateWorkteamRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkteamRequestRequestTypeDef",
     {
-        "DataAttributes": LabelingJobDataAttributesTypeDef,
+        "WorkforceName": str,
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class LabelingJobInputConfigTypeDef(
-    _RequiredLabelingJobInputConfigTypeDef, _OptionalLabelingJobInputConfigTypeDef
+class CreateWorkteamRequestRequestTypeDef(
+    _RequiredCreateWorkteamRequestRequestTypeDef, _OptionalCreateWorkteamRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateWorkteamRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkteamRequestRequestTypeDef",
+    {
+        "WorkteamName": str,
+    },
+)
+_OptionalUpdateWorkteamRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkteamRequestRequestTypeDef",
+    {
+        "MemberDefinitions": Sequence[MemberDefinitionTypeDef],
+        "Description": str,
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateWorkteamRequestRequestTypeDef(
+    _RequiredUpdateWorkteamRequestRequestTypeDef, _OptionalUpdateWorkteamRequestRequestTypeDef
 ):
     pass
 
 
 _RequiredWorkteamTypeDef = TypedDict(
     "_RequiredWorkteamTypeDef",
     {
         "WorkteamName": str,
-        "MemberDefinitions": List[MemberDefinitionOutputTypeDef],
+        "MemberDefinitions": List[MemberDefinitionTypeDef],
         "WorkteamArn": str,
         "Description": str,
     },
 )
 _OptionalWorkteamTypeDef = TypedDict(
     "_OptionalWorkteamTypeDef",
     {
@@ -15956,45 +14923,36 @@
 )
 
 
 class WorkteamTypeDef(_RequiredWorkteamTypeDef, _OptionalWorkteamTypeDef):
     pass
 
 
-MemberDefinitionUnionTypeDef = Union[MemberDefinitionTypeDef, MemberDefinitionOutputTypeDef]
+TargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
+    "TargetTrackingScalingPolicyConfigurationTypeDef",
+    {
+        "MetricSpecification": MetricSpecificationTypeDef,
+        "TargetValue": float,
+    },
+    total=False,
+)
+
 MonitoringAlertSummaryTypeDef = TypedDict(
     "MonitoringAlertSummaryTypeDef",
     {
         "MonitoringAlertName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "AlertStatus": MonitoringAlertStatusType,
         "DatapointsToAlert": int,
         "EvaluationPeriod": int,
         "Actions": MonitoringAlertActionsTypeDef,
     },
 )
 
-ContainerDefinitionOutputTypeDef = TypedDict(
-    "ContainerDefinitionOutputTypeDef",
-    {
-        "ContainerHostname": str,
-        "Image": str,
-        "ImageConfig": ImageConfigTypeDef,
-        "Mode": ContainerModeType,
-        "ModelDataUrl": str,
-        "Environment": Dict[str, str],
-        "ModelPackageName": str,
-        "InferenceSpecificationName": str,
-        "MultiModelConfig": MultiModelConfigTypeDef,
-        "ModelDataSource": ModelDataSourceTypeDef,
-    },
-    total=False,
-)
-
 ContainerDefinitionTypeDef = TypedDict(
     "ContainerDefinitionTypeDef",
     {
         "ContainerHostname": str,
         "Image": str,
         "ImageConfig": ImageConfigTypeDef,
         "Mode": ContainerModeType,
@@ -16023,65 +14981,14 @@
     {
         "ModelName": str,
         "VariantName": str,
         "InfrastructureConfig": ModelInfrastructureConfigTypeDef,
     },
 )
 
-_RequiredAdditionalInferenceSpecificationDefinitionOutputTypeDef = TypedDict(
-    "_RequiredAdditionalInferenceSpecificationDefinitionOutputTypeDef",
-    {
-        "Name": str,
-        "Containers": List[ModelPackageContainerDefinitionOutputTypeDef],
-    },
-)
-_OptionalAdditionalInferenceSpecificationDefinitionOutputTypeDef = TypedDict(
-    "_OptionalAdditionalInferenceSpecificationDefinitionOutputTypeDef",
-    {
-        "Description": str,
-        "SupportedTransformInstanceTypes": List[TransformInstanceTypeType],
-        "SupportedRealtimeInferenceInstanceTypes": List[ProductionVariantInstanceTypeType],
-        "SupportedContentTypes": List[str],
-        "SupportedResponseMIMETypes": List[str],
-    },
-    total=False,
-)
-
-
-class AdditionalInferenceSpecificationDefinitionOutputTypeDef(
-    _RequiredAdditionalInferenceSpecificationDefinitionOutputTypeDef,
-    _OptionalAdditionalInferenceSpecificationDefinitionOutputTypeDef,
-):
-    pass
-
-
-_RequiredInferenceSpecificationOutputTypeDef = TypedDict(
-    "_RequiredInferenceSpecificationOutputTypeDef",
-    {
-        "Containers": List[ModelPackageContainerDefinitionOutputTypeDef],
-        "SupportedContentTypes": List[str],
-        "SupportedResponseMIMETypes": List[str],
-    },
-)
-_OptionalInferenceSpecificationOutputTypeDef = TypedDict(
-    "_OptionalInferenceSpecificationOutputTypeDef",
-    {
-        "SupportedTransformInstanceTypes": List[TransformInstanceTypeType],
-        "SupportedRealtimeInferenceInstanceTypes": List[ProductionVariantInstanceTypeType],
-    },
-    total=False,
-)
-
-
-class InferenceSpecificationOutputTypeDef(
-    _RequiredInferenceSpecificationOutputTypeDef, _OptionalInferenceSpecificationOutputTypeDef
-):
-    pass
-
-
 _RequiredAdditionalInferenceSpecificationDefinitionTypeDef = TypedDict(
     "_RequiredAdditionalInferenceSpecificationDefinitionTypeDef",
     {
         "Name": str,
         "Containers": Sequence[ModelPackageContainerDefinitionTypeDef],
     },
 )
@@ -16104,38 +15011,35 @@
 ):
     pass
 
 
 _RequiredInferenceSpecificationTypeDef = TypedDict(
     "_RequiredInferenceSpecificationTypeDef",
     {
-        "Containers": Sequence[ModelPackageContainerDefinitionTypeDef],
-        "SupportedContentTypes": Sequence[str],
-        "SupportedResponseMIMETypes": Sequence[str],
+        "Containers": List[ModelPackageContainerDefinitionTypeDef],
+        "SupportedContentTypes": List[str],
+        "SupportedResponseMIMETypes": List[str],
     },
 )
 _OptionalInferenceSpecificationTypeDef = TypedDict(
     "_OptionalInferenceSpecificationTypeDef",
     {
-        "SupportedTransformInstanceTypes": Sequence[TransformInstanceTypeType],
-        "SupportedRealtimeInferenceInstanceTypes": Sequence[ProductionVariantInstanceTypeType],
+        "SupportedTransformInstanceTypes": List[TransformInstanceTypeType],
+        "SupportedRealtimeInferenceInstanceTypes": List[ProductionVariantInstanceTypeType],
     },
     total=False,
 )
 
 
 class InferenceSpecificationTypeDef(
     _RequiredInferenceSpecificationTypeDef, _OptionalInferenceSpecificationTypeDef
 ):
     pass
 
 
-RecommendationJobStoppingConditionsUnionTypeDef = Union[
-    RecommendationJobStoppingConditionsTypeDef, RecommendationJobStoppingConditionsOutputTypeDef
-]
 ListModelMetadataRequestListModelMetadataPaginateTypeDef = TypedDict(
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
     {
         "SearchExpression": ModelMetadataSearchExpressionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -16147,44 +15051,14 @@
         "SearchExpression": ModelMetadataSearchExpressionTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredBatchTransformInputOutputTypeDef = TypedDict(
-    "_RequiredBatchTransformInputOutputTypeDef",
-    {
-        "DataCapturedDestinationS3Uri": str,
-        "DatasetFormat": MonitoringDatasetFormatOutputTypeDef,
-        "LocalPath": str,
-    },
-)
-_OptionalBatchTransformInputOutputTypeDef = TypedDict(
-    "_OptionalBatchTransformInputOutputTypeDef",
-    {
-        "S3InputMode": ProcessingS3InputModeType,
-        "S3DataDistributionType": ProcessingS3DataDistributionTypeType,
-        "FeaturesAttribute": str,
-        "InferenceAttribute": str,
-        "ProbabilityAttribute": str,
-        "ProbabilityThresholdAttribute": float,
-        "StartTimeOffset": str,
-        "EndTimeOffset": str,
-    },
-    total=False,
-)
-
-
-class BatchTransformInputOutputTypeDef(
-    _RequiredBatchTransformInputOutputTypeDef, _OptionalBatchTransformInputOutputTypeDef
-):
-    pass
-
-
 _RequiredBatchTransformInputTypeDef = TypedDict(
     "_RequiredBatchTransformInputTypeDef",
     {
         "DataCapturedDestinationS3Uri": str,
         "DatasetFormat": MonitoringDatasetFormatTypeDef,
         "LocalPath": str,
     },
@@ -16207,35 +15081,14 @@
 
 class BatchTransformInputTypeDef(
     _RequiredBatchTransformInputTypeDef, _OptionalBatchTransformInputTypeDef
 ):
     pass
 
 
-_RequiredMonitoringOutputConfigOutputTypeDef = TypedDict(
-    "_RequiredMonitoringOutputConfigOutputTypeDef",
-    {
-        "MonitoringOutputs": List[MonitoringOutputTypeDef],
-    },
-)
-_OptionalMonitoringOutputConfigOutputTypeDef = TypedDict(
-    "_OptionalMonitoringOutputConfigOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class MonitoringOutputConfigOutputTypeDef(
-    _RequiredMonitoringOutputConfigOutputTypeDef, _OptionalMonitoringOutputConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredMonitoringOutputConfigTypeDef = TypedDict(
     "_RequiredMonitoringOutputConfigTypeDef",
     {
         "MonitoringOutputs": Sequence[MonitoringOutputTypeDef],
     },
 )
 _OptionalMonitoringOutputConfigTypeDef = TypedDict(
@@ -16325,14 +15178,37 @@
         "FailureReason": str,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateFeatureGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFeatureGroupRequestRequestTypeDef",
+    {
+        "FeatureGroupName": str,
+    },
+)
+_OptionalUpdateFeatureGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFeatureGroupRequestRequestTypeDef",
+    {
+        "FeatureAdditions": Sequence[FeatureDefinitionTypeDef],
+        "OnlineStoreConfig": OnlineStoreConfigUpdateTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateFeatureGroupRequestRequestTypeDef(
+    _RequiredUpdateFeatureGroupRequestRequestTypeDef,
+    _OptionalUpdateFeatureGroupRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredCreateCompilationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCompilationJobRequestRequestTypeDef",
     {
         "CompilationJobName": str,
         "RoleArn": str,
         "OutputConfig": OutputConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
@@ -16372,15 +15248,15 @@
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "ModelArtifacts": ModelArtifactsTypeDef,
         "ModelDigests": ModelDigestsTypeDef,
         "RoleArn": str,
         "InputConfig": InputConfigTypeDef,
         "OutputConfig": OutputConfigTypeDef,
-        "VpcConfig": NeoVpcConfigOutputTypeDef,
+        "VpcConfig": NeoVpcConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPendingDeploymentSummaryTypeDef = TypedDict(
     "_RequiredPendingDeploymentSummaryTypeDef",
     {
@@ -16400,35 +15276,14 @@
 
 class PendingDeploymentSummaryTypeDef(
     _RequiredPendingDeploymentSummaryTypeDef, _OptionalPendingDeploymentSummaryTypeDef
 ):
     pass
 
 
-_RequiredProcessingOutputConfigOutputTypeDef = TypedDict(
-    "_RequiredProcessingOutputConfigOutputTypeDef",
-    {
-        "Outputs": List[ProcessingOutputTypeDef],
-    },
-)
-_OptionalProcessingOutputConfigOutputTypeDef = TypedDict(
-    "_OptionalProcessingOutputConfigOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class ProcessingOutputConfigOutputTypeDef(
-    _RequiredProcessingOutputConfigOutputTypeDef, _OptionalProcessingOutputConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredProcessingOutputConfigTypeDef = TypedDict(
     "_RequiredProcessingOutputConfigTypeDef",
     {
         "Outputs": Sequence[ProcessingOutputTypeDef],
     },
 )
 _OptionalProcessingOutputConfigTypeDef = TypedDict(
@@ -16442,67 +15297,67 @@
 
 class ProcessingOutputConfigTypeDef(
     _RequiredProcessingOutputConfigTypeDef, _OptionalProcessingOutputConfigTypeDef
 ):
     pass
 
 
-_RequiredUpdateTrainingJobRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTrainingJobRequestRequestTypeDef",
+_RequiredGetSearchSuggestionsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetSearchSuggestionsRequestRequestTypeDef",
     {
-        "TrainingJobName": str,
+        "Resource": ResourceTypeType,
     },
 )
-_OptionalUpdateTrainingJobRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTrainingJobRequestRequestTypeDef",
+_OptionalGetSearchSuggestionsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetSearchSuggestionsRequestRequestTypeDef",
     {
-        "ProfilerConfig": ProfilerConfigForUpdateTypeDef,
-        "ProfilerRuleConfigurations": Sequence[ProfilerRuleConfigurationUnionTypeDef],
-        "ResourceConfig": ResourceConfigForUpdateTypeDef,
+        "SuggestionQuery": SuggestionQueryTypeDef,
     },
     total=False,
 )
 
 
-class UpdateTrainingJobRequestRequestTypeDef(
-    _RequiredUpdateTrainingJobRequestRequestTypeDef, _OptionalUpdateTrainingJobRequestRequestTypeDef
+class GetSearchSuggestionsRequestRequestTypeDef(
+    _RequiredGetSearchSuggestionsRequestRequestTypeDef,
+    _OptionalGetSearchSuggestionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetSearchSuggestionsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetSearchSuggestionsRequestRequestTypeDef",
+_RequiredCreateProjectInputRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectInputRequestTypeDef",
     {
-        "Resource": ResourceTypeType,
+        "ProjectName": str,
+        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
     },
 )
-_OptionalGetSearchSuggestionsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetSearchSuggestionsRequestRequestTypeDef",
+_OptionalCreateProjectInputRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectInputRequestTypeDef",
     {
-        "SuggestionQuery": SuggestionQueryTypeDef,
+        "ProjectDescription": str,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class GetSearchSuggestionsRequestRequestTypeDef(
-    _RequiredGetSearchSuggestionsRequestRequestTypeDef,
-    _OptionalGetSearchSuggestionsRequestRequestTypeDef,
+class CreateProjectInputRequestTypeDef(
+    _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
 ):
     pass
 
 
 DescribeProjectOutputTypeDef = TypedDict(
     "DescribeProjectOutputTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "ProjectId": str,
         "ProjectDescription": str,
-        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsOutputTypeDef,
+        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
         "ServiceCatalogProvisionedProductDetails": ServiceCatalogProvisionedProductDetailsTypeDef,
         "ProjectStatus": ProjectStatusType,
         "CreatedBy": UserContextTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -16512,52 +15367,26 @@
 ProjectTypeDef = TypedDict(
     "ProjectTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "ProjectId": str,
         "ProjectDescription": str,
-        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsOutputTypeDef,
+        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
         "ServiceCatalogProvisionedProductDetails": ServiceCatalogProvisionedProductDetailsTypeDef,
         "ProjectStatus": ProjectStatusType,
         "CreatedBy": UserContextTypeDef,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateProjectInputRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectInputRequestTypeDef",
-    {
-        "ProjectName": str,
-        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
-    },
-)
-_OptionalCreateProjectInputRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectInputRequestTypeDef",
-    {
-        "ProjectDescription": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateProjectInputRequestTypeDef(
-    _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
-):
-    pass
-
-
-ServiceCatalogProvisioningDetailsUnionTypeDef = Union[
-    ServiceCatalogProvisioningDetailsTypeDef, ServiceCatalogProvisioningDetailsOutputTypeDef
-]
 _RequiredUpdateProjectInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectInputRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalUpdateProjectInputRequestTypeDef = TypedDict(
@@ -16573,42 +15402,14 @@
 
 class UpdateProjectInputRequestTypeDef(
     _RequiredUpdateProjectInputRequestTypeDef, _OptionalUpdateProjectInputRequestTypeDef
 ):
     pass
 
 
-_RequiredHumanLoopConfigOutputTypeDef = TypedDict(
-    "_RequiredHumanLoopConfigOutputTypeDef",
-    {
-        "WorkteamArn": str,
-        "HumanTaskUiArn": str,
-        "TaskTitle": str,
-        "TaskDescription": str,
-        "TaskCount": int,
-    },
-)
-_OptionalHumanLoopConfigOutputTypeDef = TypedDict(
-    "_OptionalHumanLoopConfigOutputTypeDef",
-    {
-        "TaskAvailabilityLifetimeInSeconds": int,
-        "TaskTimeLimitInSeconds": int,
-        "TaskKeywords": List[str],
-        "PublicWorkforceTaskPrice": PublicWorkforceTaskPriceTypeDef,
-    },
-    total=False,
-)
-
-
-class HumanLoopConfigOutputTypeDef(
-    _RequiredHumanLoopConfigOutputTypeDef, _OptionalHumanLoopConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredHumanLoopConfigTypeDef = TypedDict(
     "_RequiredHumanLoopConfigTypeDef",
     {
         "WorkteamArn": str,
         "HumanTaskUiArn": str,
         "TaskTitle": str,
         "TaskDescription": str,
@@ -16627,45 +15428,14 @@
 )
 
 
 class HumanLoopConfigTypeDef(_RequiredHumanLoopConfigTypeDef, _OptionalHumanLoopConfigTypeDef):
     pass
 
 
-_RequiredHumanTaskConfigOutputTypeDef = TypedDict(
-    "_RequiredHumanTaskConfigOutputTypeDef",
-    {
-        "WorkteamArn": str,
-        "UiConfig": UiConfigTypeDef,
-        "PreHumanTaskLambdaArn": str,
-        "TaskTitle": str,
-        "TaskDescription": str,
-        "NumberOfHumanWorkersPerDataObject": int,
-        "TaskTimeLimitInSeconds": int,
-        "AnnotationConsolidationConfig": AnnotationConsolidationConfigTypeDef,
-    },
-)
-_OptionalHumanTaskConfigOutputTypeDef = TypedDict(
-    "_OptionalHumanTaskConfigOutputTypeDef",
-    {
-        "TaskKeywords": List[str],
-        "TaskAvailabilityLifetimeInSeconds": int,
-        "MaxConcurrentTaskCount": int,
-        "PublicWorkforceTaskPrice": PublicWorkforceTaskPriceTypeDef,
-    },
-    total=False,
-)
-
-
-class HumanTaskConfigOutputTypeDef(
-    _RequiredHumanTaskConfigOutputTypeDef, _OptionalHumanTaskConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredHumanTaskConfigTypeDef = TypedDict(
     "_RequiredHumanTaskConfigTypeDef",
     {
         "WorkteamArn": str,
         "UiConfig": UiConfigTypeDef,
         "PreHumanTaskLambdaArn": str,
         "TaskTitle": str,
@@ -16702,15 +15472,15 @@
         "PipelineExperimentConfig": PipelineExperimentConfigTypeDef,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedBy": UserContextTypeDef,
         "ParallelismConfiguration": ParallelismConfigurationTypeDef,
-        "SelectiveExecutionConfig": SelectiveExecutionConfigOutputTypeDef,
+        "SelectiveExecutionConfig": SelectiveExecutionConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PipelineExecutionTypeDef = TypedDict(
     "PipelineExecutionTypeDef",
     {
@@ -16723,22 +15493,19 @@
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedBy": UserContextTypeDef,
         "ParallelismConfiguration": ParallelismConfigurationTypeDef,
         "PipelineParameters": List[ParameterTypeDef],
-        "SelectiveExecutionConfig": SelectiveExecutionConfigOutputTypeDef,
+        "SelectiveExecutionConfig": SelectiveExecutionConfigTypeDef,
     },
     total=False,
 )
 
-SelectiveExecutionConfigUnionTypeDef = Union[
-    SelectiveExecutionConfigTypeDef, SelectiveExecutionConfigOutputTypeDef
-]
 _RequiredStartPipelineExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartPipelineExecutionRequestRequestTypeDef",
     {
         "PipelineName": str,
         "ClientRequestToken": str,
     },
 )
@@ -16758,45 +15525,14 @@
 class StartPipelineExecutionRequestRequestTypeDef(
     _RequiredStartPipelineExecutionRequestRequestTypeDef,
     _OptionalStartPipelineExecutionRequestRequestTypeDef,
 ):
     pass
 
 
-ShadowModeConfigUnionTypeDef = Union[ShadowModeConfigTypeDef, ShadowModeConfigOutputTypeDef]
-SourceAlgorithmSpecificationUnionTypeDef = Union[
-    SourceAlgorithmSpecificationTypeDef, SourceAlgorithmSpecificationOutputTypeDef
-]
-_RequiredAlgorithmSpecificationOutputTypeDef = TypedDict(
-    "_RequiredAlgorithmSpecificationOutputTypeDef",
-    {
-        "TrainingInputMode": TrainingInputModeType,
-    },
-)
-_OptionalAlgorithmSpecificationOutputTypeDef = TypedDict(
-    "_OptionalAlgorithmSpecificationOutputTypeDef",
-    {
-        "TrainingImage": str,
-        "AlgorithmName": str,
-        "MetricDefinitions": List[MetricDefinitionTypeDef],
-        "EnableSageMakerMetricsTimeSeries": bool,
-        "ContainerEntrypoint": List[str],
-        "ContainerArguments": List[str],
-        "TrainingImageConfig": TrainingImageConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class AlgorithmSpecificationOutputTypeDef(
-    _RequiredAlgorithmSpecificationOutputTypeDef, _OptionalAlgorithmSpecificationOutputTypeDef
-):
-    pass
-
-
 _RequiredAlgorithmSpecificationTypeDef = TypedDict(
     "_RequiredAlgorithmSpecificationTypeDef",
     {
         "TrainingInputMode": TrainingInputModeType,
     },
 )
 _OptionalAlgorithmSpecificationTypeDef = TypedDict(
@@ -16871,38 +15607,25 @@
     {
         "ArtifactSummaries": List[ArtifactSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AsyncInferenceConfigUnionTypeDef = Union[
-    AsyncInferenceConfigTypeDef, AsyncInferenceConfigOutputTypeDef
-]
-AutoMLProblemTypeConfigOutputTypeDef = TypedDict(
-    "AutoMLProblemTypeConfigOutputTypeDef",
-    {
-        "ImageClassificationJobConfig": ImageClassificationJobConfigTypeDef,
-        "TextClassificationJobConfig": TextClassificationJobConfigTypeDef,
-        "TabularJobConfig": TabularJobConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 AutoMLProblemTypeConfigTypeDef = TypedDict(
     "AutoMLProblemTypeConfigTypeDef",
     {
         "ImageClassificationJobConfig": ImageClassificationJobConfigTypeDef,
         "TextClassificationJobConfig": TextClassificationJobConfigTypeDef,
         "TabularJobConfig": TabularJobConfigTypeDef,
+        "TimeSeriesForecastingJobConfig": TimeSeriesForecastingJobConfigTypeDef,
     },
     total=False,
 )
 
-AutoMLJobConfigUnionTypeDef = Union[AutoMLJobConfigTypeDef, AutoMLJobConfigOutputTypeDef]
 _RequiredCreateAutoMLJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoMLJobRequestRequestTypeDef",
     {
         "AutoMLJobName": str,
         "InputDataConfig": Sequence[AutoMLChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
@@ -16924,17 +15647,14 @@
 
 class CreateAutoMLJobRequestRequestTypeDef(
     _RequiredCreateAutoMLJobRequestRequestTypeDef, _OptionalCreateAutoMLJobRequestRequestTypeDef
 ):
     pass
 
 
-LabelingJobAlgorithmsConfigUnionTypeDef = Union[
-    LabelingJobAlgorithmsConfigTypeDef, LabelingJobAlgorithmsConfigOutputTypeDef
-]
 PipelineExecutionStepTypeDef = TypedDict(
     "PipelineExecutionStepTypeDef",
     {
         "StepName": str,
         "StepDisplayName": str,
         "StepDescription": str,
         "StartTime": datetime,
@@ -16955,15 +15675,15 @@
         "AutoMLJobName": str,
         "AutoMLJobArn": str,
         "InputDataConfig": List[AutoMLChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "ProblemType": ProblemTypeType,
-        "AutoMLJobConfig": AutoMLJobConfigOutputTypeDef,
+        "AutoMLJobConfig": AutoMLJobConfigTypeDef,
         "CreationTime": datetime,
         "EndTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
         "BestCandidate": AutoMLCandidateTypeDef,
         "AutoMLJobStatus": AutoMLJobStatusType,
@@ -16982,67 +15702,20 @@
     {
         "Candidates": List[AutoMLCandidateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDeploymentConfigOutputTypeDef = TypedDict(
-    "_RequiredDeploymentConfigOutputTypeDef",
-    {
-        "BlueGreenUpdatePolicy": BlueGreenUpdatePolicyTypeDef,
-    },
-)
-_OptionalDeploymentConfigOutputTypeDef = TypedDict(
-    "_OptionalDeploymentConfigOutputTypeDef",
-    {
-        "AutoRollbackConfiguration": AutoRollbackConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DeploymentConfigOutputTypeDef(
-    _RequiredDeploymentConfigOutputTypeDef, _OptionalDeploymentConfigOutputTypeDef
-):
-    pass
-
-
-_RequiredDeploymentConfigTypeDef = TypedDict(
-    "_RequiredDeploymentConfigTypeDef",
+DeploymentConfigTypeDef = TypedDict(
+    "DeploymentConfigTypeDef",
     {
         "BlueGreenUpdatePolicy": BlueGreenUpdatePolicyTypeDef,
-    },
-)
-_OptionalDeploymentConfigTypeDef = TypedDict(
-    "_OptionalDeploymentConfigTypeDef",
-    {
         "AutoRollbackConfiguration": AutoRollbackConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class DeploymentConfigTypeDef(_RequiredDeploymentConfigTypeDef, _OptionalDeploymentConfigTypeDef):
-    pass
-
-
-RecommendationJobInputConfigOutputTypeDef = TypedDict(
-    "RecommendationJobInputConfigOutputTypeDef",
-    {
-        "ModelPackageVersionArn": str,
-        "JobDurationInSeconds": int,
-        "TrafficPattern": TrafficPatternOutputTypeDef,
-        "ResourceLimit": RecommendationJobResourceLimitTypeDef,
-        "EndpointConfigurations": List[EndpointInputConfigurationOutputTypeDef],
-        "VolumeKmsKeyId": str,
-        "ContainerConfig": RecommendationJobContainerConfigOutputTypeDef,
-        "Endpoints": List[EndpointInfoTypeDef],
-        "VpcConfig": RecommendationJobVpcConfigOutputTypeDef,
-        "ModelName": str,
+        "RollingUpdatePolicy": RollingUpdatePolicyTypeDef,
     },
     total=False,
 )
 
 RecommendationJobInputConfigTypeDef = TypedDict(
     "RecommendationJobInputConfigTypeDef",
     {
@@ -17056,50 +15729,31 @@
         "Endpoints": Sequence[EndpointInfoTypeDef],
         "VpcConfig": RecommendationJobVpcConfigTypeDef,
         "ModelName": str,
     },
     total=False,
 )
 
-ExplainerConfigOutputTypeDef = TypedDict(
-    "ExplainerConfigOutputTypeDef",
-    {
-        "ClarifyExplainerConfig": ClarifyExplainerConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ExplainerConfigTypeDef = TypedDict(
     "ExplainerConfigTypeDef",
     {
         "ClarifyExplainerConfig": ClarifyExplainerConfigTypeDef,
     },
     total=False,
 )
 
-DomainSettingsUnionTypeDef = Union[DomainSettingsTypeDef, DomainSettingsOutputTypeDef]
-DescribeSpaceResponseTypeDef = TypedDict(
-    "DescribeSpaceResponseTypeDef",
+ListInferenceExperimentsResponseTypeDef = TypedDict(
+    "ListInferenceExperimentsResponseTypeDef",
     {
-        "DomainId": str,
-        "SpaceArn": str,
-        "SpaceName": str,
-        "HomeEfsFileSystemUid": str,
-        "Status": SpaceStatusType,
-        "LastModifiedTime": datetime,
-        "CreationTime": datetime,
-        "FailureReason": str,
-        "SpaceSettings": SpaceSettingsOutputTypeDef,
+        "InferenceExperiments": List[InferenceExperimentSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DefaultSpaceSettingsUnionTypeDef = Union[
-    DefaultSpaceSettingsTypeDef, DefaultSpaceSettingsOutputTypeDef
-]
 _RequiredCreateSpaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSpaceRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpaceName": str,
     },
 )
@@ -17115,15 +15769,30 @@
 
 class CreateSpaceRequestRequestTypeDef(
     _RequiredCreateSpaceRequestRequestTypeDef, _OptionalCreateSpaceRequestRequestTypeDef
 ):
     pass
 
 
-SpaceSettingsUnionTypeDef = Union[SpaceSettingsTypeDef, SpaceSettingsOutputTypeDef]
+DescribeSpaceResponseTypeDef = TypedDict(
+    "DescribeSpaceResponseTypeDef",
+    {
+        "DomainId": str,
+        "SpaceArn": str,
+        "SpaceName": str,
+        "HomeEfsFileSystemUid": str,
+        "Status": SpaceStatusType,
+        "LastModifiedTime": datetime,
+        "CreationTime": datetime,
+        "FailureReason": str,
+        "SpaceSettings": SpaceSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateSpaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSpaceRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpaceName": str,
     },
 )
@@ -17138,60 +15807,14 @@
 
 class UpdateSpaceRequestRequestTypeDef(
     _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
 ):
     pass
 
 
-DescribeDomainResponseTypeDef = TypedDict(
-    "DescribeDomainResponseTypeDef",
-    {
-        "DomainArn": str,
-        "DomainId": str,
-        "DomainName": str,
-        "HomeEfsFileSystemId": str,
-        "SingleSignOnManagedApplicationInstanceId": str,
-        "Status": DomainStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "AuthMode": AuthModeType,
-        "DefaultUserSettings": UserSettingsOutputTypeDef,
-        "AppNetworkAccessType": AppNetworkAccessTypeType,
-        "HomeEfsFileSystemKmsKeyId": str,
-        "SubnetIds": List[str],
-        "Url": str,
-        "VpcId": str,
-        "KmsKeyId": str,
-        "DomainSettings": DomainSettingsOutputTypeDef,
-        "AppSecurityGroupManagement": AppSecurityGroupManagementType,
-        "SecurityGroupIdForDomainBoundary": str,
-        "DefaultSpaceSettings": DefaultSpaceSettingsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeUserProfileResponseTypeDef = TypedDict(
-    "DescribeUserProfileResponseTypeDef",
-    {
-        "DomainId": str,
-        "UserProfileArn": str,
-        "UserProfileName": str,
-        "HomeEfsFileSystemUid": str,
-        "Status": UserProfileStatusType,
-        "LastModifiedTime": datetime,
-        "CreationTime": datetime,
-        "FailureReason": str,
-        "SingleSignOnUserIdentifier": str,
-        "SingleSignOnUserValue": str,
-        "UserSettings": UserSettingsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "AuthMode": AuthModeType,
         "DefaultUserSettings": UserSettingsTypeDef,
         "SubnetIds": Sequence[str],
@@ -17240,14 +15863,60 @@
 
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
 
+DescribeDomainResponseTypeDef = TypedDict(
+    "DescribeDomainResponseTypeDef",
+    {
+        "DomainArn": str,
+        "DomainId": str,
+        "DomainName": str,
+        "HomeEfsFileSystemId": str,
+        "SingleSignOnManagedApplicationInstanceId": str,
+        "Status": DomainStatusType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "AuthMode": AuthModeType,
+        "DefaultUserSettings": UserSettingsTypeDef,
+        "AppNetworkAccessType": AppNetworkAccessTypeType,
+        "HomeEfsFileSystemKmsKeyId": str,
+        "SubnetIds": List[str],
+        "Url": str,
+        "VpcId": str,
+        "KmsKeyId": str,
+        "DomainSettings": DomainSettingsTypeDef,
+        "AppSecurityGroupManagement": AppSecurityGroupManagementType,
+        "SecurityGroupIdForDomainBoundary": str,
+        "DefaultSpaceSettings": DefaultSpaceSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUserProfileResponseTypeDef = TypedDict(
+    "DescribeUserProfileResponseTypeDef",
+    {
+        "DomainId": str,
+        "UserProfileArn": str,
+        "UserProfileName": str,
+        "HomeEfsFileSystemUid": str,
+        "Status": UserProfileStatusType,
+        "LastModifiedTime": datetime,
+        "CreationTime": datetime,
+        "FailureReason": str,
+        "SingleSignOnUserIdentifier": str,
+        "SingleSignOnUserValue": str,
+        "UserSettings": UserSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalUpdateDomainRequestRequestTypeDef = TypedDict(
@@ -17286,79 +15955,14 @@
 
 class UpdateUserProfileRequestRequestTypeDef(
     _RequiredUpdateUserProfileRequestRequestTypeDef, _OptionalUpdateUserProfileRequestRequestTypeDef
 ):
     pass
 
 
-UserSettingsUnionTypeDef = Union[UserSettingsTypeDef, UserSettingsOutputTypeDef]
-_RequiredHyperParameterTrainingJobDefinitionOutputTypeDef = TypedDict(
-    "_RequiredHyperParameterTrainingJobDefinitionOutputTypeDef",
-    {
-        "AlgorithmSpecification": HyperParameterAlgorithmSpecificationOutputTypeDef,
-        "RoleArn": str,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "StoppingCondition": StoppingConditionTypeDef,
-    },
-)
-_OptionalHyperParameterTrainingJobDefinitionOutputTypeDef = TypedDict(
-    "_OptionalHyperParameterTrainingJobDefinitionOutputTypeDef",
-    {
-        "DefinitionName": str,
-        "TuningObjective": HyperParameterTuningJobObjectiveTypeDef,
-        "HyperParameterRanges": ParameterRangesOutputTypeDef,
-        "StaticHyperParameters": Dict[str, str],
-        "InputDataConfig": List[ChannelOutputTypeDef],
-        "VpcConfig": VpcConfigOutputTypeDef,
-        "ResourceConfig": ResourceConfigOutputTypeDef,
-        "EnableNetworkIsolation": bool,
-        "EnableInterContainerTrafficEncryption": bool,
-        "EnableManagedSpotTraining": bool,
-        "CheckpointConfig": CheckpointConfigTypeDef,
-        "RetryStrategy": RetryStrategyTypeDef,
-        "HyperParameterTuningResourceConfig": HyperParameterTuningResourceConfigOutputTypeDef,
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class HyperParameterTrainingJobDefinitionOutputTypeDef(
-    _RequiredHyperParameterTrainingJobDefinitionOutputTypeDef,
-    _OptionalHyperParameterTrainingJobDefinitionOutputTypeDef,
-):
-    pass
-
-
-_RequiredTrainingJobDefinitionOutputTypeDef = TypedDict(
-    "_RequiredTrainingJobDefinitionOutputTypeDef",
-    {
-        "TrainingInputMode": TrainingInputModeType,
-        "InputDataConfig": List[ChannelOutputTypeDef],
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigOutputTypeDef,
-        "StoppingCondition": StoppingConditionTypeDef,
-    },
-)
-_OptionalTrainingJobDefinitionOutputTypeDef = TypedDict(
-    "_OptionalTrainingJobDefinitionOutputTypeDef",
-    {
-        "HyperParameters": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class TrainingJobDefinitionOutputTypeDef(
-    _RequiredTrainingJobDefinitionOutputTypeDef, _OptionalTrainingJobDefinitionOutputTypeDef
-):
-    pass
-
-
-ChannelUnionTypeDef = Union[ChannelTypeDef, ChannelOutputTypeDef]
 _RequiredHyperParameterTrainingJobDefinitionTypeDef = TypedDict(
     "_RequiredHyperParameterTrainingJobDefinitionTypeDef",
     {
         "AlgorithmSpecification": HyperParameterAlgorithmSpecificationTypeDef,
         "RoleArn": str,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
@@ -17474,41 +16078,14 @@
     {
         "TrialComponentSummaries": List[TrialComponentSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTrainingSpecificationOutputTypeDef = TypedDict(
-    "_RequiredTrainingSpecificationOutputTypeDef",
-    {
-        "TrainingImage": str,
-        "SupportedTrainingInstanceTypes": List[TrainingInstanceTypeType],
-        "TrainingChannels": List[ChannelSpecificationOutputTypeDef],
-    },
-)
-_OptionalTrainingSpecificationOutputTypeDef = TypedDict(
-    "_OptionalTrainingSpecificationOutputTypeDef",
-    {
-        "TrainingImageDigest": str,
-        "SupportedHyperParameters": List[HyperParameterSpecificationOutputTypeDef],
-        "SupportsDistributedTraining": bool,
-        "MetricDefinitions": List[MetricDefinitionTypeDef],
-        "SupportedTuningJobObjectiveMetrics": List[HyperParameterTuningJobObjectiveTypeDef],
-    },
-    total=False,
-)
-
-
-class TrainingSpecificationOutputTypeDef(
-    _RequiredTrainingSpecificationOutputTypeDef, _OptionalTrainingSpecificationOutputTypeDef
-):
-    pass
-
-
 _RequiredTrainingSpecificationTypeDef = TypedDict(
     "_RequiredTrainingSpecificationTypeDef",
     {
         "TrainingImage": str,
         "SupportedTrainingInstanceTypes": Sequence[TrainingInstanceTypeType],
         "TrainingChannels": Sequence[ChannelSpecificationTypeDef],
     },
@@ -17528,17 +16105,14 @@
 
 class TrainingSpecificationTypeDef(
     _RequiredTrainingSpecificationTypeDef, _OptionalTrainingSpecificationTypeDef
 ):
     pass
 
 
-HyperParameterTuningJobConfigUnionTypeDef = Union[
-    HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
-]
 ListAppImageConfigsResponseTypeDef = TypedDict(
     "ListAppImageConfigsResponseTypeDef",
     {
         "NextToken": str,
         "AppImageConfigs": List[AppImageConfigDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -17559,29 +16133,26 @@
 )
 _OptionalLabelingJobSummaryTypeDef = TypedDict(
     "_OptionalLabelingJobSummaryTypeDef",
     {
         "AnnotationConsolidationLambdaArn": str,
         "FailureReason": str,
         "LabelingJobOutput": LabelingJobOutputTypeDef,
-        "InputConfig": LabelingJobInputConfigOutputTypeDef,
+        "InputConfig": LabelingJobInputConfigTypeDef,
     },
     total=False,
 )
 
 
 class LabelingJobSummaryTypeDef(
     _RequiredLabelingJobSummaryTypeDef, _OptionalLabelingJobSummaryTypeDef
 ):
     pass
 
 
-LabelingJobInputConfigUnionTypeDef = Union[
-    LabelingJobInputConfigTypeDef, LabelingJobInputConfigOutputTypeDef
-]
 DescribeWorkteamResponseTypeDef = TypedDict(
     "DescribeWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -17599,127 +16170,111 @@
     "UpdateWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateWorkteamRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkteamRequestRequestTypeDef",
+ScalingPolicyTypeDef = TypedDict(
+    "ScalingPolicyTypeDef",
     {
-        "WorkteamName": str,
-        "MemberDefinitions": Sequence[MemberDefinitionUnionTypeDef],
-        "Description": str,
+        "TargetTracking": TargetTrackingScalingPolicyConfigurationTypeDef,
     },
+    total=False,
 )
-_OptionalCreateWorkteamRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkteamRequestRequestTypeDef",
+
+ListMonitoringAlertsResponseTypeDef = TypedDict(
+    "ListMonitoringAlertsResponseTypeDef",
     {
-        "WorkforceName": str,
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
+        "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateWorkteamRequestRequestTypeDef(
-    _RequiredCreateWorkteamRequestRequestTypeDef, _OptionalCreateWorkteamRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateWorkteamRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateWorkteamRequestRequestTypeDef",
+_RequiredCreateModelInputRequestTypeDef = TypedDict(
+    "_RequiredCreateModelInputRequestTypeDef",
     {
-        "WorkteamName": str,
+        "ModelName": str,
+        "ExecutionRoleArn": str,
     },
 )
-_OptionalUpdateWorkteamRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateWorkteamRequestRequestTypeDef",
+_OptionalCreateModelInputRequestTypeDef = TypedDict(
+    "_OptionalCreateModelInputRequestTypeDef",
     {
-        "MemberDefinitions": Sequence[MemberDefinitionUnionTypeDef],
-        "Description": str,
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "PrimaryContainer": ContainerDefinitionTypeDef,
+        "Containers": Sequence[ContainerDefinitionTypeDef],
+        "InferenceExecutionConfig": InferenceExecutionConfigTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "VpcConfig": VpcConfigTypeDef,
+        "EnableNetworkIsolation": bool,
     },
     total=False,
 )
 
 
-class UpdateWorkteamRequestRequestTypeDef(
-    _RequiredUpdateWorkteamRequestRequestTypeDef, _OptionalUpdateWorkteamRequestRequestTypeDef
+class CreateModelInputRequestTypeDef(
+    _RequiredCreateModelInputRequestTypeDef, _OptionalCreateModelInputRequestTypeDef
 ):
     pass
 
 
-ListMonitoringAlertsResponseTypeDef = TypedDict(
-    "ListMonitoringAlertsResponseTypeDef",
-    {
-        "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeModelOutputTypeDef = TypedDict(
     "DescribeModelOutputTypeDef",
     {
         "ModelName": str,
-        "PrimaryContainer": ContainerDefinitionOutputTypeDef,
-        "Containers": List[ContainerDefinitionOutputTypeDef],
+        "PrimaryContainer": ContainerDefinitionTypeDef,
+        "Containers": List[ContainerDefinitionTypeDef],
         "InferenceExecutionConfig": InferenceExecutionConfigTypeDef,
         "ExecutionRoleArn": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "CreationTime": datetime,
         "ModelArn": str,
         "EnableNetworkIsolation": bool,
         "DeploymentRecommendation": DeploymentRecommendationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelTypeDef = TypedDict(
     "ModelTypeDef",
     {
         "ModelName": str,
-        "PrimaryContainer": ContainerDefinitionOutputTypeDef,
-        "Containers": List[ContainerDefinitionOutputTypeDef],
+        "PrimaryContainer": ContainerDefinitionTypeDef,
+        "Containers": List[ContainerDefinitionTypeDef],
         "InferenceExecutionConfig": InferenceExecutionConfigTypeDef,
         "ExecutionRoleArn": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "CreationTime": datetime,
         "ModelArn": str,
         "EnableNetworkIsolation": bool,
         "Tags": List[TagTypeDef],
         "DeploymentRecommendation": DeploymentRecommendationTypeDef,
     },
     total=False,
 )
 
-ContainerDefinitionUnionTypeDef = Union[
-    ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef
-]
 DescribeInferenceExperimentResponseTypeDef = TypedDict(
     "DescribeInferenceExperimentResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": Literal["ShadowMode"],
-        "Schedule": InferenceExperimentScheduleOutputTypeDef,
+        "Schedule": InferenceExperimentScheduleTypeDef,
         "Status": InferenceExperimentStatusType,
         "StatusReason": str,
         "Description": str,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "LastModifiedTime": datetime,
         "RoleArn": str,
         "EndpointMetadata": EndpointMetadataTypeDef,
         "ModelVariants": List[ModelVariantConfigSummaryTypeDef],
-        "DataStorageConfig": InferenceExperimentDataStorageConfigOutputTypeDef,
-        "ShadowModeConfig": ShadowModeConfigOutputTypeDef,
+        "DataStorageConfig": InferenceExperimentDataStorageConfigTypeDef,
+        "ShadowModeConfig": ShadowModeConfigTypeDef,
         "KmsKey": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateInferenceExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInferenceExperimentRequestRequestTypeDef",
@@ -17799,120 +16354,69 @@
 class UpdateInferenceExperimentRequestRequestTypeDef(
     _RequiredUpdateInferenceExperimentRequestRequestTypeDef,
     _OptionalUpdateInferenceExperimentRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredBatchDescribeModelPackageSummaryTypeDef = TypedDict(
-    "_RequiredBatchDescribeModelPackageSummaryTypeDef",
+_RequiredUpdateModelPackageInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateModelPackageInputRequestTypeDef",
     {
-        "ModelPackageGroupName": str,
         "ModelPackageArn": str,
-        "CreationTime": datetime,
-        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
-        "ModelPackageStatus": ModelPackageStatusType,
     },
 )
-_OptionalBatchDescribeModelPackageSummaryTypeDef = TypedDict(
-    "_OptionalBatchDescribeModelPackageSummaryTypeDef",
+_OptionalUpdateModelPackageInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateModelPackageInputRequestTypeDef",
     {
-        "ModelPackageVersion": int,
-        "ModelPackageDescription": str,
         "ModelApprovalStatus": ModelApprovalStatusType,
+        "ApprovalDescription": str,
+        "CustomerMetadataProperties": Mapping[str, str],
+        "CustomerMetadataPropertiesToRemove": Sequence[str],
+        "AdditionalInferenceSpecificationsToAdd": Sequence[
+            AdditionalInferenceSpecificationDefinitionTypeDef
+        ],
     },
     total=False,
 )
 
 
-class BatchDescribeModelPackageSummaryTypeDef(
-    _RequiredBatchDescribeModelPackageSummaryTypeDef,
-    _OptionalBatchDescribeModelPackageSummaryTypeDef,
-):
-    pass
-
-
-AdditionalInferenceSpecificationDefinitionUnionTypeDef = Union[
-    AdditionalInferenceSpecificationDefinitionTypeDef,
-    AdditionalInferenceSpecificationDefinitionOutputTypeDef,
-]
-InferenceSpecificationUnionTypeDef = Union[
-    InferenceSpecificationTypeDef, InferenceSpecificationOutputTypeDef
-]
-DataQualityJobInputOutputTypeDef = TypedDict(
-    "DataQualityJobInputOutputTypeDef",
-    {
-        "EndpointInput": EndpointInputTypeDef,
-        "BatchTransformInput": BatchTransformInputOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredModelBiasJobInputOutputTypeDef = TypedDict(
-    "_RequiredModelBiasJobInputOutputTypeDef",
-    {
-        "GroundTruthS3Input": MonitoringGroundTruthS3InputTypeDef,
-    },
-)
-_OptionalModelBiasJobInputOutputTypeDef = TypedDict(
-    "_OptionalModelBiasJobInputOutputTypeDef",
-    {
-        "EndpointInput": EndpointInputTypeDef,
-        "BatchTransformInput": BatchTransformInputOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ModelBiasJobInputOutputTypeDef(
-    _RequiredModelBiasJobInputOutputTypeDef, _OptionalModelBiasJobInputOutputTypeDef
+class UpdateModelPackageInputRequestTypeDef(
+    _RequiredUpdateModelPackageInputRequestTypeDef, _OptionalUpdateModelPackageInputRequestTypeDef
 ):
     pass
 
 
-ModelExplainabilityJobInputOutputTypeDef = TypedDict(
-    "ModelExplainabilityJobInputOutputTypeDef",
-    {
-        "EndpointInput": EndpointInputTypeDef,
-        "BatchTransformInput": BatchTransformInputOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredModelQualityJobInputOutputTypeDef = TypedDict(
-    "_RequiredModelQualityJobInputOutputTypeDef",
+_RequiredBatchDescribeModelPackageSummaryTypeDef = TypedDict(
+    "_RequiredBatchDescribeModelPackageSummaryTypeDef",
     {
-        "GroundTruthS3Input": MonitoringGroundTruthS3InputTypeDef,
+        "ModelPackageGroupName": str,
+        "ModelPackageArn": str,
+        "CreationTime": datetime,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "ModelPackageStatus": ModelPackageStatusType,
     },
 )
-_OptionalModelQualityJobInputOutputTypeDef = TypedDict(
-    "_OptionalModelQualityJobInputOutputTypeDef",
+_OptionalBatchDescribeModelPackageSummaryTypeDef = TypedDict(
+    "_OptionalBatchDescribeModelPackageSummaryTypeDef",
     {
-        "EndpointInput": EndpointInputTypeDef,
-        "BatchTransformInput": BatchTransformInputOutputTypeDef,
+        "ModelPackageVersion": int,
+        "ModelPackageDescription": str,
+        "ModelApprovalStatus": ModelApprovalStatusType,
     },
     total=False,
 )
 
 
-class ModelQualityJobInputOutputTypeDef(
-    _RequiredModelQualityJobInputOutputTypeDef, _OptionalModelQualityJobInputOutputTypeDef
+class BatchDescribeModelPackageSummaryTypeDef(
+    _RequiredBatchDescribeModelPackageSummaryTypeDef,
+    _OptionalBatchDescribeModelPackageSummaryTypeDef,
 ):
     pass
 
 
-MonitoringInputOutputTypeDef = TypedDict(
-    "MonitoringInputOutputTypeDef",
-    {
-        "EndpointInput": EndpointInputTypeDef,
-        "BatchTransformInput": BatchTransformInputOutputTypeDef,
-    },
-    total=False,
-)
-
 DataQualityJobInputTypeDef = TypedDict(
     "DataQualityJobInputTypeDef",
     {
         "EndpointInput": EndpointInputTypeDef,
         "BatchTransformInput": BatchTransformInputTypeDef,
     },
     total=False,
@@ -17976,28 +16480,56 @@
     {
         "EndpointInput": EndpointInputTypeDef,
         "BatchTransformInput": BatchTransformInputTypeDef,
     },
     total=False,
 )
 
-MonitoringOutputConfigUnionTypeDef = Union[
-    MonitoringOutputConfigTypeDef, MonitoringOutputConfigOutputTypeDef
-]
+_RequiredCreateProcessingJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProcessingJobRequestRequestTypeDef",
+    {
+        "ProcessingJobName": str,
+        "ProcessingResources": ProcessingResourcesTypeDef,
+        "AppSpecification": AppSpecificationTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateProcessingJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProcessingJobRequestRequestTypeDef",
+    {
+        "ProcessingInputs": Sequence[ProcessingInputTypeDef],
+        "ProcessingOutputConfig": ProcessingOutputConfigTypeDef,
+        "StoppingCondition": ProcessingStoppingConditionTypeDef,
+        "Environment": Mapping[str, str],
+        "NetworkConfig": NetworkConfigTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "ExperimentConfig": ExperimentConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateProcessingJobRequestRequestTypeDef(
+    _RequiredCreateProcessingJobRequestRequestTypeDef,
+    _OptionalCreateProcessingJobRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeProcessingJobResponseTypeDef = TypedDict(
     "DescribeProcessingJobResponseTypeDef",
     {
         "ProcessingInputs": List[ProcessingInputTypeDef],
-        "ProcessingOutputConfig": ProcessingOutputConfigOutputTypeDef,
+        "ProcessingOutputConfig": ProcessingOutputConfigTypeDef,
         "ProcessingJobName": str,
         "ProcessingResources": ProcessingResourcesTypeDef,
         "StoppingCondition": ProcessingStoppingConditionTypeDef,
-        "AppSpecification": AppSpecificationOutputTypeDef,
+        "AppSpecification": AppSpecificationTypeDef,
         "Environment": Dict[str, str],
-        "NetworkConfig": NetworkConfigOutputTypeDef,
+        "NetworkConfig": NetworkConfigTypeDef,
         "RoleArn": str,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "ProcessingJobArn": str,
         "ProcessingJobStatus": ProcessingJobStatusType,
         "ExitMessage": str,
         "FailureReason": str,
         "ProcessingEndTime": datetime,
@@ -18011,21 +16543,21 @@
     },
 )
 
 ProcessingJobTypeDef = TypedDict(
     "ProcessingJobTypeDef",
     {
         "ProcessingInputs": List[ProcessingInputTypeDef],
-        "ProcessingOutputConfig": ProcessingOutputConfigOutputTypeDef,
+        "ProcessingOutputConfig": ProcessingOutputConfigTypeDef,
         "ProcessingJobName": str,
         "ProcessingResources": ProcessingResourcesTypeDef,
         "StoppingCondition": ProcessingStoppingConditionTypeDef,
-        "AppSpecification": AppSpecificationOutputTypeDef,
+        "AppSpecification": AppSpecificationTypeDef,
         "Environment": Dict[str, str],
-        "NetworkConfig": NetworkConfigOutputTypeDef,
+        "NetworkConfig": NetworkConfigTypeDef,
         "RoleArn": str,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "ProcessingJobArn": str,
         "ProcessingJobStatus": ProcessingJobStatusType,
         "ExitMessage": str,
         "FailureReason": str,
         "ProcessingEndTime": datetime,
@@ -18036,187 +16568,192 @@
         "AutoMLJobArn": str,
         "TrainingJobArn": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateProcessingJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProcessingJobRequestRequestTypeDef",
+_RequiredCreateFlowDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFlowDefinitionRequestRequestTypeDef",
     {
-        "ProcessingJobName": str,
-        "ProcessingResources": ProcessingResourcesTypeDef,
-        "AppSpecification": AppSpecificationTypeDef,
+        "FlowDefinitionName": str,
+        "HumanLoopConfig": HumanLoopConfigTypeDef,
+        "OutputConfig": FlowDefinitionOutputConfigTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalCreateProcessingJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProcessingJobRequestRequestTypeDef",
+_OptionalCreateFlowDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFlowDefinitionRequestRequestTypeDef",
     {
-        "ProcessingInputs": Sequence[ProcessingInputTypeDef],
-        "ProcessingOutputConfig": ProcessingOutputConfigTypeDef,
-        "StoppingCondition": ProcessingStoppingConditionTypeDef,
-        "Environment": Mapping[str, str],
-        "NetworkConfig": NetworkConfigTypeDef,
+        "HumanLoopRequestSource": HumanLoopRequestSourceTypeDef,
+        "HumanLoopActivationConfig": HumanLoopActivationConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
-        "ExperimentConfig": ExperimentConfigTypeDef,
     },
     total=False,
 )
 
 
-class CreateProcessingJobRequestRequestTypeDef(
-    _RequiredCreateProcessingJobRequestRequestTypeDef,
-    _OptionalCreateProcessingJobRequestRequestTypeDef,
+class CreateFlowDefinitionRequestRequestTypeDef(
+    _RequiredCreateFlowDefinitionRequestRequestTypeDef,
+    _OptionalCreateFlowDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
-ProcessingOutputConfigUnionTypeDef = Union[
-    ProcessingOutputConfigTypeDef, ProcessingOutputConfigOutputTypeDef
-]
 DescribeFlowDefinitionResponseTypeDef = TypedDict(
     "DescribeFlowDefinitionResponseTypeDef",
     {
         "FlowDefinitionArn": str,
         "FlowDefinitionName": str,
         "FlowDefinitionStatus": FlowDefinitionStatusType,
         "CreationTime": datetime,
         "HumanLoopRequestSource": HumanLoopRequestSourceTypeDef,
         "HumanLoopActivationConfig": HumanLoopActivationConfigTypeDef,
-        "HumanLoopConfig": HumanLoopConfigOutputTypeDef,
+        "HumanLoopConfig": HumanLoopConfigTypeDef,
         "OutputConfig": FlowDefinitionOutputConfigTypeDef,
         "RoleArn": str,
         "FailureReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateFlowDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFlowDefinitionRequestRequestTypeDef",
+_RequiredCreateLabelingJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLabelingJobRequestRequestTypeDef",
     {
-        "FlowDefinitionName": str,
-        "HumanLoopConfig": HumanLoopConfigTypeDef,
-        "OutputConfig": FlowDefinitionOutputConfigTypeDef,
+        "LabelingJobName": str,
+        "LabelAttributeName": str,
+        "InputConfig": LabelingJobInputConfigTypeDef,
+        "OutputConfig": LabelingJobOutputConfigTypeDef,
         "RoleArn": str,
+        "HumanTaskConfig": HumanTaskConfigTypeDef,
     },
 )
-_OptionalCreateFlowDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFlowDefinitionRequestRequestTypeDef",
+_OptionalCreateLabelingJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLabelingJobRequestRequestTypeDef",
     {
-        "HumanLoopRequestSource": HumanLoopRequestSourceTypeDef,
-        "HumanLoopActivationConfig": HumanLoopActivationConfigTypeDef,
+        "LabelCategoryConfigS3Uri": str,
+        "StoppingConditions": LabelingJobStoppingConditionsTypeDef,
+        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class CreateFlowDefinitionRequestRequestTypeDef(
-    _RequiredCreateFlowDefinitionRequestRequestTypeDef,
-    _OptionalCreateFlowDefinitionRequestRequestTypeDef,
+class CreateLabelingJobRequestRequestTypeDef(
+    _RequiredCreateLabelingJobRequestRequestTypeDef, _OptionalCreateLabelingJobRequestRequestTypeDef
 ):
     pass
 
 
-HumanLoopConfigUnionTypeDef = Union[HumanLoopConfigTypeDef, HumanLoopConfigOutputTypeDef]
 DescribeLabelingJobResponseTypeDef = TypedDict(
     "DescribeLabelingJobResponseTypeDef",
     {
         "LabelingJobStatus": LabelingJobStatusType,
         "LabelCounters": LabelCountersTypeDef,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "JobReferenceCode": str,
         "LabelingJobName": str,
         "LabelingJobArn": str,
         "LabelAttributeName": str,
-        "InputConfig": LabelingJobInputConfigOutputTypeDef,
+        "InputConfig": LabelingJobInputConfigTypeDef,
         "OutputConfig": LabelingJobOutputConfigTypeDef,
         "RoleArn": str,
         "LabelCategoryConfigS3Uri": str,
         "StoppingConditions": LabelingJobStoppingConditionsTypeDef,
-        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigOutputTypeDef,
-        "HumanTaskConfig": HumanTaskConfigOutputTypeDef,
+        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigTypeDef,
+        "HumanTaskConfig": HumanTaskConfigTypeDef,
         "Tags": List[TagTypeDef],
         "LabelingJobOutput": LabelingJobOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateLabelingJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLabelingJobRequestRequestTypeDef",
+_RequiredCreateTrainingJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTrainingJobRequestRequestTypeDef",
     {
-        "LabelingJobName": str,
-        "LabelAttributeName": str,
-        "InputConfig": LabelingJobInputConfigTypeDef,
-        "OutputConfig": LabelingJobOutputConfigTypeDef,
+        "TrainingJobName": str,
+        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
         "RoleArn": str,
-        "HumanTaskConfig": HumanTaskConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "ResourceConfig": ResourceConfigTypeDef,
+        "StoppingCondition": StoppingConditionTypeDef,
     },
 )
-_OptionalCreateLabelingJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLabelingJobRequestRequestTypeDef",
+_OptionalCreateTrainingJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTrainingJobRequestRequestTypeDef",
     {
-        "LabelCategoryConfigS3Uri": str,
-        "StoppingConditions": LabelingJobStoppingConditionsTypeDef,
-        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigTypeDef,
+        "HyperParameters": Mapping[str, str],
+        "InputDataConfig": Sequence[ChannelTypeDef],
+        "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
+        "EnableNetworkIsolation": bool,
+        "EnableInterContainerTrafficEncryption": bool,
+        "EnableManagedSpotTraining": bool,
+        "CheckpointConfig": CheckpointConfigTypeDef,
+        "DebugHookConfig": DebugHookConfigTypeDef,
+        "DebugRuleConfigurations": Sequence[DebugRuleConfigurationTypeDef],
+        "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
+        "ExperimentConfig": ExperimentConfigTypeDef,
+        "ProfilerConfig": ProfilerConfigTypeDef,
+        "ProfilerRuleConfigurations": Sequence[ProfilerRuleConfigurationTypeDef],
+        "Environment": Mapping[str, str],
+        "RetryStrategy": RetryStrategyTypeDef,
     },
     total=False,
 )
 
 
-class CreateLabelingJobRequestRequestTypeDef(
-    _RequiredCreateLabelingJobRequestRequestTypeDef, _OptionalCreateLabelingJobRequestRequestTypeDef
+class CreateTrainingJobRequestRequestTypeDef(
+    _RequiredCreateTrainingJobRequestRequestTypeDef, _OptionalCreateTrainingJobRequestRequestTypeDef
 ):
     pass
 
 
-HumanTaskConfigUnionTypeDef = Union[HumanTaskConfigTypeDef, HumanTaskConfigOutputTypeDef]
 DescribeTrainingJobResponseTypeDef = TypedDict(
     "DescribeTrainingJobResponseTypeDef",
     {
         "TrainingJobName": str,
         "TrainingJobArn": str,
         "TuningJobArn": str,
         "LabelingJobArn": str,
         "AutoMLJobArn": str,
         "ModelArtifacts": ModelArtifactsTypeDef,
         "TrainingJobStatus": TrainingJobStatusType,
         "SecondaryStatus": SecondaryStatusType,
         "FailureReason": str,
         "HyperParameters": Dict[str, str],
-        "AlgorithmSpecification": AlgorithmSpecificationOutputTypeDef,
+        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
         "RoleArn": str,
-        "InputDataConfig": List[ChannelOutputTypeDef],
+        "InputDataConfig": List[ChannelTypeDef],
         "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigOutputTypeDef,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "ResourceConfig": ResourceConfigTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
         "CreationTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
         "LastModifiedTime": datetime,
         "SecondaryStatusTransitions": List[SecondaryStatusTransitionTypeDef],
         "FinalMetricDataList": List[MetricDataTypeDef],
         "EnableNetworkIsolation": bool,
         "EnableInterContainerTrafficEncryption": bool,
         "EnableManagedSpotTraining": bool,
         "CheckpointConfig": CheckpointConfigTypeDef,
         "TrainingTimeInSeconds": int,
         "BillableTimeInSeconds": int,
-        "DebugHookConfig": DebugHookConfigOutputTypeDef,
+        "DebugHookConfig": DebugHookConfigTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
-        "DebugRuleConfigurations": List[DebugRuleConfigurationOutputTypeDef],
+        "DebugRuleConfigurations": List[DebugRuleConfigurationTypeDef],
         "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
         "DebugRuleEvaluationStatuses": List[DebugRuleEvaluationStatusTypeDef],
-        "ProfilerConfig": ProfilerConfigOutputTypeDef,
-        "ProfilerRuleConfigurations": List[ProfilerRuleConfigurationOutputTypeDef],
+        "ProfilerConfig": ProfilerConfigTypeDef,
+        "ProfilerRuleConfigurations": List[ProfilerRuleConfigurationTypeDef],
         "ProfilerRuleEvaluationStatuses": List[ProfilerRuleEvaluationStatusTypeDef],
         "ProfilingStatus": ProfilingStatusType,
         "RetryStrategy": RetryStrategyTypeDef,
         "Environment": Dict[str, str],
         "WarmPoolStatus": WarmPoolStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -18231,48 +16768,46 @@
         "LabelingJobArn": str,
         "AutoMLJobArn": str,
         "ModelArtifacts": ModelArtifactsTypeDef,
         "TrainingJobStatus": TrainingJobStatusType,
         "SecondaryStatus": SecondaryStatusType,
         "FailureReason": str,
         "HyperParameters": Dict[str, str],
-        "AlgorithmSpecification": AlgorithmSpecificationOutputTypeDef,
+        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
         "RoleArn": str,
-        "InputDataConfig": List[ChannelOutputTypeDef],
+        "InputDataConfig": List[ChannelTypeDef],
         "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigOutputTypeDef,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "ResourceConfig": ResourceConfigTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
         "CreationTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
         "LastModifiedTime": datetime,
         "SecondaryStatusTransitions": List[SecondaryStatusTransitionTypeDef],
         "FinalMetricDataList": List[MetricDataTypeDef],
         "EnableNetworkIsolation": bool,
         "EnableInterContainerTrafficEncryption": bool,
         "EnableManagedSpotTraining": bool,
         "CheckpointConfig": CheckpointConfigTypeDef,
         "TrainingTimeInSeconds": int,
         "BillableTimeInSeconds": int,
-        "DebugHookConfig": DebugHookConfigOutputTypeDef,
+        "DebugHookConfig": DebugHookConfigTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
-        "DebugRuleConfigurations": List[DebugRuleConfigurationOutputTypeDef],
+        "DebugRuleConfigurations": List[DebugRuleConfigurationTypeDef],
         "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
         "DebugRuleEvaluationStatuses": List[DebugRuleEvaluationStatusTypeDef],
+        "ProfilerConfig": ProfilerConfigTypeDef,
         "Environment": Dict[str, str],
         "RetryStrategy": RetryStrategyTypeDef,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-AlgorithmSpecificationUnionTypeDef = Union[
-    AlgorithmSpecificationTypeDef, AlgorithmSpecificationOutputTypeDef
-]
 _RequiredCreateTransformJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTransformJobRequestRequestTypeDef",
     {
         "TransformJobName": str,
         "ModelName": str,
         "TransformInput": TransformInputTypeDef,
         "TransformOutput": TransformOutputTypeDef,
@@ -18327,40 +16862,14 @@
         "AutoMLJobArn": str,
         "DataProcessing": DataProcessingTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTransformJobDefinitionOutputTypeDef = TypedDict(
-    "_RequiredTransformJobDefinitionOutputTypeDef",
-    {
-        "TransformInput": TransformInputTypeDef,
-        "TransformOutput": TransformOutputTypeDef,
-        "TransformResources": TransformResourcesTypeDef,
-    },
-)
-_OptionalTransformJobDefinitionOutputTypeDef = TypedDict(
-    "_OptionalTransformJobDefinitionOutputTypeDef",
-    {
-        "MaxConcurrentTransforms": int,
-        "MaxPayloadInMB": int,
-        "BatchStrategy": BatchStrategyType,
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class TransformJobDefinitionOutputTypeDef(
-    _RequiredTransformJobDefinitionOutputTypeDef, _OptionalTransformJobDefinitionOutputTypeDef
-):
-    pass
-
-
 _RequiredTransformJobDefinitionTypeDef = TypedDict(
     "_RequiredTransformJobDefinitionTypeDef",
     {
         "TransformInput": TransformInputTypeDef,
         "TransformOutput": TransformOutputTypeDef,
         "TransformResources": TransformResourcesTypeDef,
     },
@@ -18407,46 +16916,14 @@
         "DataProcessing": DataProcessingTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-DescribeAutoMLJobV2ResponseTypeDef = TypedDict(
-    "DescribeAutoMLJobV2ResponseTypeDef",
-    {
-        "AutoMLJobName": str,
-        "AutoMLJobArn": str,
-        "AutoMLJobInputDataConfig": List[AutoMLJobChannelTypeDef],
-        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
-        "RoleArn": str,
-        "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
-        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigOutputTypeDef,
-        "CreationTime": datetime,
-        "EndTime": datetime,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
-        "BestCandidate": AutoMLCandidateTypeDef,
-        "AutoMLJobStatus": AutoMLJobStatusType,
-        "AutoMLJobSecondaryStatus": AutoMLJobSecondaryStatusType,
-        "ModelDeployConfig": ModelDeployConfigTypeDef,
-        "ModelDeployResult": ModelDeployResultTypeDef,
-        "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
-        "SecurityConfig": AutoMLSecurityConfigOutputTypeDef,
-        "AutoMLJobArtifacts": AutoMLJobArtifactsTypeDef,
-        "ResolvedAttributes": AutoMLResolvedAttributesTypeDef,
-        "AutoMLProblemTypeConfigName": AutoMLProblemTypeConfigNameType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AutoMLProblemTypeConfigUnionTypeDef = Union[
-    AutoMLProblemTypeConfigTypeDef, AutoMLProblemTypeConfigOutputTypeDef
-]
 _RequiredCreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoMLJobV2RequestRequestTypeDef",
     {
         "AutoMLJobName": str,
         "AutoMLJobInputDataConfig": Sequence[AutoMLJobChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
@@ -18468,14 +16945,43 @@
 
 class CreateAutoMLJobV2RequestRequestTypeDef(
     _RequiredCreateAutoMLJobV2RequestRequestTypeDef, _OptionalCreateAutoMLJobV2RequestRequestTypeDef
 ):
     pass
 
 
+DescribeAutoMLJobV2ResponseTypeDef = TypedDict(
+    "DescribeAutoMLJobV2ResponseTypeDef",
+    {
+        "AutoMLJobName": str,
+        "AutoMLJobArn": str,
+        "AutoMLJobInputDataConfig": List[AutoMLJobChannelTypeDef],
+        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
+        "RoleArn": str,
+        "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
+        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
+        "CreationTime": datetime,
+        "EndTime": datetime,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
+        "BestCandidate": AutoMLCandidateTypeDef,
+        "AutoMLJobStatus": AutoMLJobStatusType,
+        "AutoMLJobSecondaryStatus": AutoMLJobSecondaryStatusType,
+        "ModelDeployConfig": ModelDeployConfigTypeDef,
+        "ModelDeployResult": ModelDeployResultTypeDef,
+        "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
+        "SecurityConfig": AutoMLSecurityConfigTypeDef,
+        "AutoMLJobArtifacts": AutoMLJobArtifactsTypeDef,
+        "ResolvedAttributes": AutoMLResolvedAttributesTypeDef,
+        "AutoMLProblemTypeConfigName": AutoMLProblemTypeConfigNameType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPipelineExecutionStepsResponseTypeDef = TypedDict(
     "ListPipelineExecutionStepsResponseTypeDef",
     {
         "PipelineExecutionSteps": List[PipelineExecutionStepTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -18500,15 +17006,14 @@
 
 class CreateEndpointInputRequestTypeDef(
     _RequiredCreateEndpointInputRequestTypeDef, _OptionalCreateEndpointInputRequestTypeDef
 ):
     pass
 
 
-DeploymentConfigUnionTypeDef = Union[DeploymentConfigTypeDef, DeploymentConfigOutputTypeDef]
 _RequiredUpdateEndpointInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
         "EndpointConfigName": str,
     },
 )
@@ -18526,77 +17031,102 @@
 
 class UpdateEndpointInputRequestTypeDef(
     _RequiredUpdateEndpointInputRequestTypeDef, _OptionalUpdateEndpointInputRequestTypeDef
 ):
     pass
 
 
+_RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef",
+    {
+        "JobName": str,
+        "JobType": RecommendationJobTypeType,
+        "RoleArn": str,
+        "InputConfig": RecommendationJobInputConfigTypeDef,
+    },
+)
+_OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef",
+    {
+        "JobDescription": str,
+        "StoppingConditions": RecommendationJobStoppingConditionsTypeDef,
+        "OutputConfig": RecommendationJobOutputConfigTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateInferenceRecommendationsJobRequestRequestTypeDef(
+    _RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef,
+    _OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeInferenceRecommendationsJobResponseTypeDef = TypedDict(
     "DescribeInferenceRecommendationsJobResponseTypeDef",
     {
         "JobName": str,
         "JobDescription": str,
         "JobType": RecommendationJobTypeType,
         "JobArn": str,
         "RoleArn": str,
         "Status": RecommendationJobStatusType,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
-        "InputConfig": RecommendationJobInputConfigOutputTypeDef,
-        "StoppingConditions": RecommendationJobStoppingConditionsOutputTypeDef,
+        "InputConfig": RecommendationJobInputConfigTypeDef,
+        "StoppingConditions": RecommendationJobStoppingConditionsTypeDef,
         "InferenceRecommendations": List[InferenceRecommendationTypeDef],
         "EndpointPerformances": List[EndpointPerformanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef",
+_RequiredCreateEndpointConfigInputRequestTypeDef = TypedDict(
+    "_RequiredCreateEndpointConfigInputRequestTypeDef",
     {
-        "JobName": str,
-        "JobType": RecommendationJobTypeType,
-        "RoleArn": str,
-        "InputConfig": RecommendationJobInputConfigTypeDef,
+        "EndpointConfigName": str,
+        "ProductionVariants": Sequence[ProductionVariantTypeDef],
     },
 )
-_OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef",
+_OptionalCreateEndpointConfigInputRequestTypeDef = TypedDict(
+    "_OptionalCreateEndpointConfigInputRequestTypeDef",
     {
-        "JobDescription": str,
-        "StoppingConditions": RecommendationJobStoppingConditionsTypeDef,
-        "OutputConfig": RecommendationJobOutputConfigTypeDef,
+        "DataCaptureConfig": DataCaptureConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
+        "ExplainerConfig": ExplainerConfigTypeDef,
+        "ShadowProductionVariants": Sequence[ProductionVariantTypeDef],
     },
     total=False,
 )
 
 
-class CreateInferenceRecommendationsJobRequestRequestTypeDef(
-    _RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef,
-    _OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef,
+class CreateEndpointConfigInputRequestTypeDef(
+    _RequiredCreateEndpointConfigInputRequestTypeDef,
+    _OptionalCreateEndpointConfigInputRequestTypeDef,
 ):
     pass
 
 
-RecommendationJobInputConfigUnionTypeDef = Union[
-    RecommendationJobInputConfigTypeDef, RecommendationJobInputConfigOutputTypeDef
-]
 DescribeEndpointConfigOutputTypeDef = TypedDict(
     "DescribeEndpointConfigOutputTypeDef",
     {
         "EndpointConfigName": str,
         "EndpointConfigArn": str,
         "ProductionVariants": List[ProductionVariantTypeDef],
-        "DataCaptureConfig": DataCaptureConfigOutputTypeDef,
+        "DataCaptureConfig": DataCaptureConfigTypeDef,
         "KmsKeyId": str,
         "CreationTime": datetime,
-        "AsyncInferenceConfig": AsyncInferenceConfigOutputTypeDef,
-        "ExplainerConfig": ExplainerConfigOutputTypeDef,
+        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
+        "ExplainerConfig": ExplainerConfigTypeDef,
         "ShadowProductionVariants": List[ProductionVariantTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointOutputTypeDef = TypedDict(
     "DescribeEndpointOutputTypeDef",
@@ -18606,330 +17136,139 @@
         "EndpointConfigName": str,
         "ProductionVariants": List[ProductionVariantSummaryTypeDef],
         "DataCaptureConfig": DataCaptureConfigSummaryTypeDef,
         "EndpointStatus": EndpointStatusType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "LastDeploymentConfig": DeploymentConfigOutputTypeDef,
-        "AsyncInferenceConfig": AsyncInferenceConfigOutputTypeDef,
+        "LastDeploymentConfig": DeploymentConfigTypeDef,
+        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
         "PendingDeploymentSummary": PendingDeploymentSummaryTypeDef,
-        "ExplainerConfig": ExplainerConfigOutputTypeDef,
+        "ExplainerConfig": ExplainerConfigTypeDef,
         "ShadowProductionVariants": List[ProductionVariantSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateEndpointConfigInputRequestTypeDef = TypedDict(
-    "_RequiredCreateEndpointConfigInputRequestTypeDef",
+_RequiredCreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHyperParameterTuningJobRequestRequestTypeDef",
     {
-        "EndpointConfigName": str,
-        "ProductionVariants": Sequence[ProductionVariantTypeDef],
+        "HyperParameterTuningJobName": str,
+        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
     },
 )
-_OptionalCreateEndpointConfigInputRequestTypeDef = TypedDict(
-    "_OptionalCreateEndpointConfigInputRequestTypeDef",
+_OptionalCreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHyperParameterTuningJobRequestRequestTypeDef",
     {
-        "DataCaptureConfig": DataCaptureConfigTypeDef,
+        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionTypeDef,
+        "TrainingJobDefinitions": Sequence[HyperParameterTrainingJobDefinitionTypeDef],
+        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
-        "ExplainerConfig": ExplainerConfigTypeDef,
-        "ShadowProductionVariants": Sequence[ProductionVariantTypeDef],
+        "Autotune": AutotuneTypeDef,
     },
     total=False,
 )
 
 
-class CreateEndpointConfigInputRequestTypeDef(
-    _RequiredCreateEndpointConfigInputRequestTypeDef,
-    _OptionalCreateEndpointConfigInputRequestTypeDef,
+class CreateHyperParameterTuningJobRequestRequestTypeDef(
+    _RequiredCreateHyperParameterTuningJobRequestRequestTypeDef,
+    _OptionalCreateHyperParameterTuningJobRequestRequestTypeDef,
 ):
     pass
 
 
-ExplainerConfigUnionTypeDef = Union[ExplainerConfigTypeDef, ExplainerConfigOutputTypeDef]
 DescribeHyperParameterTuningJobResponseTypeDef = TypedDict(
     "DescribeHyperParameterTuningJobResponseTypeDef",
     {
         "HyperParameterTuningJobName": str,
         "HyperParameterTuningJobArn": str,
-        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigOutputTypeDef,
-        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionOutputTypeDef,
-        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionOutputTypeDef],
+        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
+        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionTypeDef,
+        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionTypeDef],
         "HyperParameterTuningJobStatus": HyperParameterTuningJobStatusType,
         "CreationTime": datetime,
         "HyperParameterTuningEndTime": datetime,
         "LastModifiedTime": datetime,
         "TrainingJobStatusCounters": TrainingJobStatusCountersTypeDef,
         "ObjectiveStatusCounters": ObjectiveStatusCountersTypeDef,
         "BestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
         "OverallBestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
-        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigOutputTypeDef,
+        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
         "FailureReason": str,
         "TuningJobCompletionDetails": HyperParameterTuningJobCompletionDetailsTypeDef,
         "ConsumedResources": HyperParameterTuningJobConsumedResourcesTypeDef,
         "Autotune": AutotuneTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HyperParameterTuningJobSearchEntityTypeDef = TypedDict(
     "HyperParameterTuningJobSearchEntityTypeDef",
     {
         "HyperParameterTuningJobName": str,
         "HyperParameterTuningJobArn": str,
-        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigOutputTypeDef,
-        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionOutputTypeDef,
-        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionOutputTypeDef],
+        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
+        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionTypeDef,
+        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionTypeDef],
         "HyperParameterTuningJobStatus": HyperParameterTuningJobStatusType,
         "CreationTime": datetime,
         "HyperParameterTuningEndTime": datetime,
         "LastModifiedTime": datetime,
         "TrainingJobStatusCounters": TrainingJobStatusCountersTypeDef,
         "ObjectiveStatusCounters": ObjectiveStatusCountersTypeDef,
         "BestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
         "OverallBestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
-        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigOutputTypeDef,
+        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
         "FailureReason": str,
         "Tags": List[TagTypeDef],
         "TuningJobCompletionDetails": HyperParameterTuningJobCompletionDetailsTypeDef,
         "ConsumedResources": HyperParameterTuningJobConsumedResourcesTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateTrainingJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTrainingJobRequestRequestTypeDef",
-    {
-        "TrainingJobName": str,
-        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
-        "RoleArn": str,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigTypeDef,
-        "StoppingCondition": StoppingConditionTypeDef,
-    },
-)
-_OptionalCreateTrainingJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTrainingJobRequestRequestTypeDef",
-    {
-        "HyperParameters": Mapping[str, str],
-        "InputDataConfig": Sequence[ChannelUnionTypeDef],
-        "VpcConfig": VpcConfigTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "EnableNetworkIsolation": bool,
-        "EnableInterContainerTrafficEncryption": bool,
-        "EnableManagedSpotTraining": bool,
-        "CheckpointConfig": CheckpointConfigTypeDef,
-        "DebugHookConfig": DebugHookConfigTypeDef,
-        "DebugRuleConfigurations": Sequence[DebugRuleConfigurationUnionTypeDef],
-        "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
-        "ExperimentConfig": ExperimentConfigTypeDef,
-        "ProfilerConfig": ProfilerConfigTypeDef,
-        "ProfilerRuleConfigurations": Sequence[ProfilerRuleConfigurationUnionTypeDef],
-        "Environment": Mapping[str, str],
-        "RetryStrategy": RetryStrategyTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateTrainingJobRequestRequestTypeDef(
-    _RequiredCreateTrainingJobRequestRequestTypeDef, _OptionalCreateTrainingJobRequestRequestTypeDef
-):
-    pass
-
-
-HyperParameterTrainingJobDefinitionUnionTypeDef = Union[
-    HyperParameterTrainingJobDefinitionTypeDef, HyperParameterTrainingJobDefinitionOutputTypeDef
-]
 ListInferenceRecommendationsJobStepsResponseTypeDef = TypedDict(
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
     {
         "Steps": List[InferenceRecommendationsJobStepTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TrainingSpecificationUnionTypeDef = Union[
-    TrainingSpecificationTypeDef, TrainingSpecificationOutputTypeDef
-]
 ListLabelingJobsResponseTypeDef = TypedDict(
     "ListLabelingJobsResponseTypeDef",
     {
         "LabelingJobSummaryList": List[LabelingJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateModelInputRequestTypeDef = TypedDict(
-    "_RequiredCreateModelInputRequestTypeDef",
+DynamicScalingConfigurationTypeDef = TypedDict(
+    "DynamicScalingConfigurationTypeDef",
     {
-        "ModelName": str,
-        "ExecutionRoleArn": str,
-    },
-)
-_OptionalCreateModelInputRequestTypeDef = TypedDict(
-    "_OptionalCreateModelInputRequestTypeDef",
-    {
-        "PrimaryContainer": ContainerDefinitionTypeDef,
-        "Containers": Sequence[ContainerDefinitionUnionTypeDef],
-        "InferenceExecutionConfig": InferenceExecutionConfigTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "VpcConfig": VpcConfigTypeDef,
-        "EnableNetworkIsolation": bool,
+        "MinCapacity": int,
+        "MaxCapacity": int,
+        "ScaleInCooldown": int,
+        "ScaleOutCooldown": int,
+        "ScalingPolicies": List[ScalingPolicyTypeDef],
     },
     total=False,
 )
 
-
-class CreateModelInputRequestTypeDef(
-    _RequiredCreateModelInputRequestTypeDef, _OptionalCreateModelInputRequestTypeDef
-):
-    pass
-
-
 BatchDescribeModelPackageOutputTypeDef = TypedDict(
     "BatchDescribeModelPackageOutputTypeDef",
     {
         "ModelPackageSummaries": Dict[str, BatchDescribeModelPackageSummaryTypeDef],
         "BatchDescribeModelPackageErrorMap": Dict[str, BatchDescribeModelPackageErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateModelPackageInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateModelPackageInputRequestTypeDef",
-    {
-        "ModelPackageArn": str,
-    },
-)
-_OptionalUpdateModelPackageInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateModelPackageInputRequestTypeDef",
-    {
-        "ModelApprovalStatus": ModelApprovalStatusType,
-        "ApprovalDescription": str,
-        "CustomerMetadataProperties": Mapping[str, str],
-        "CustomerMetadataPropertiesToRemove": Sequence[str],
-        "AdditionalInferenceSpecificationsToAdd": Sequence[
-            AdditionalInferenceSpecificationDefinitionUnionTypeDef
-        ],
-    },
-    total=False,
-)
-
-
-class UpdateModelPackageInputRequestTypeDef(
-    _RequiredUpdateModelPackageInputRequestTypeDef, _OptionalUpdateModelPackageInputRequestTypeDef
-):
-    pass
-
-
-DescribeDataQualityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeDataQualityJobDefinitionResponseTypeDef",
-    {
-        "JobDefinitionArn": str,
-        "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "DataQualityBaselineConfig": DataQualityBaselineConfigTypeDef,
-        "DataQualityAppSpecification": DataQualityAppSpecificationOutputTypeDef,
-        "DataQualityJobInput": DataQualityJobInputOutputTypeDef,
-        "DataQualityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
-        "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
-        "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeModelBiasJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelBiasJobDefinitionResponseTypeDef",
-    {
-        "JobDefinitionArn": str,
-        "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "ModelBiasBaselineConfig": ModelBiasBaselineConfigTypeDef,
-        "ModelBiasAppSpecification": ModelBiasAppSpecificationOutputTypeDef,
-        "ModelBiasJobInput": ModelBiasJobInputOutputTypeDef,
-        "ModelBiasJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
-        "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
-        "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeModelExplainabilityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
-    {
-        "JobDefinitionArn": str,
-        "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "ModelExplainabilityBaselineConfig": ModelExplainabilityBaselineConfigTypeDef,
-        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationOutputTypeDef,
-        "ModelExplainabilityJobInput": ModelExplainabilityJobInputOutputTypeDef,
-        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
-        "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
-        "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeModelQualityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelQualityJobDefinitionResponseTypeDef",
-    {
-        "JobDefinitionArn": str,
-        "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "ModelQualityBaselineConfig": ModelQualityBaselineConfigTypeDef,
-        "ModelQualityAppSpecification": ModelQualityAppSpecificationOutputTypeDef,
-        "ModelQualityJobInput": ModelQualityJobInputOutputTypeDef,
-        "ModelQualityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
-        "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
-        "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredMonitoringJobDefinitionOutputTypeDef = TypedDict(
-    "_RequiredMonitoringJobDefinitionOutputTypeDef",
-    {
-        "MonitoringInputs": List[MonitoringInputOutputTypeDef],
-        "MonitoringOutputConfig": MonitoringOutputConfigOutputTypeDef,
-        "MonitoringResources": MonitoringResourcesTypeDef,
-        "MonitoringAppSpecification": MonitoringAppSpecificationOutputTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalMonitoringJobDefinitionOutputTypeDef = TypedDict(
-    "_OptionalMonitoringJobDefinitionOutputTypeDef",
-    {
-        "BaselineConfig": MonitoringBaselineConfigTypeDef,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "Environment": Dict[str, str],
-        "NetworkConfig": NetworkConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class MonitoringJobDefinitionOutputTypeDef(
-    _RequiredMonitoringJobDefinitionOutputTypeDef, _OptionalMonitoringJobDefinitionOutputTypeDef
-):
-    pass
-
-
 _RequiredCreateDataQualityJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataQualityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
         "DataQualityAppSpecification": DataQualityAppSpecificationTypeDef,
         "DataQualityJobInput": DataQualityJobInputTypeDef,
         "DataQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
@@ -18952,17 +17291,32 @@
 class CreateDataQualityJobDefinitionRequestRequestTypeDef(
     _RequiredCreateDataQualityJobDefinitionRequestRequestTypeDef,
     _OptionalCreateDataQualityJobDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
-DataQualityJobInputUnionTypeDef = Union[
-    DataQualityJobInputTypeDef, DataQualityJobInputOutputTypeDef
-]
+DescribeDataQualityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeDataQualityJobDefinitionResponseTypeDef",
+    {
+        "JobDefinitionArn": str,
+        "JobDefinitionName": str,
+        "CreationTime": datetime,
+        "DataQualityBaselineConfig": DataQualityBaselineConfigTypeDef,
+        "DataQualityAppSpecification": DataQualityAppSpecificationTypeDef,
+        "DataQualityJobInput": DataQualityJobInputTypeDef,
+        "DataQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "RoleArn": str,
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateModelBiasJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelBiasJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
         "ModelBiasAppSpecification": ModelBiasAppSpecificationTypeDef,
         "ModelBiasJobInput": ModelBiasJobInputTypeDef,
         "ModelBiasJobOutputConfig": MonitoringOutputConfigTypeDef,
@@ -18985,15 +17339,32 @@
 class CreateModelBiasJobDefinitionRequestRequestTypeDef(
     _RequiredCreateModelBiasJobDefinitionRequestRequestTypeDef,
     _OptionalCreateModelBiasJobDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
-ModelBiasJobInputUnionTypeDef = Union[ModelBiasJobInputTypeDef, ModelBiasJobInputOutputTypeDef]
+DescribeModelBiasJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelBiasJobDefinitionResponseTypeDef",
+    {
+        "JobDefinitionArn": str,
+        "JobDefinitionName": str,
+        "CreationTime": datetime,
+        "ModelBiasBaselineConfig": ModelBiasBaselineConfigTypeDef,
+        "ModelBiasAppSpecification": ModelBiasAppSpecificationTypeDef,
+        "ModelBiasJobInput": ModelBiasJobInputTypeDef,
+        "ModelBiasJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "RoleArn": str,
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateModelExplainabilityJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
         "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationTypeDef,
         "ModelExplainabilityJobInput": ModelExplainabilityJobInputTypeDef,
         "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigTypeDef,
@@ -19016,17 +17387,32 @@
 class CreateModelExplainabilityJobDefinitionRequestRequestTypeDef(
     _RequiredCreateModelExplainabilityJobDefinitionRequestRequestTypeDef,
     _OptionalCreateModelExplainabilityJobDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
-ModelExplainabilityJobInputUnionTypeDef = Union[
-    ModelExplainabilityJobInputTypeDef, ModelExplainabilityJobInputOutputTypeDef
-]
+DescribeModelExplainabilityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
+    {
+        "JobDefinitionArn": str,
+        "JobDefinitionName": str,
+        "CreationTime": datetime,
+        "ModelExplainabilityBaselineConfig": ModelExplainabilityBaselineConfigTypeDef,
+        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationTypeDef,
+        "ModelExplainabilityJobInput": ModelExplainabilityJobInputTypeDef,
+        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "RoleArn": str,
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateModelQualityJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelQualityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
         "ModelQualityAppSpecification": ModelQualityAppSpecificationTypeDef,
         "ModelQualityJobInput": ModelQualityJobInputTypeDef,
         "ModelQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
@@ -19049,17 +17435,32 @@
 class CreateModelQualityJobDefinitionRequestRequestTypeDef(
     _RequiredCreateModelQualityJobDefinitionRequestRequestTypeDef,
     _OptionalCreateModelQualityJobDefinitionRequestRequestTypeDef,
 ):
     pass
 
 
-ModelQualityJobInputUnionTypeDef = Union[
-    ModelQualityJobInputTypeDef, ModelQualityJobInputOutputTypeDef
-]
+DescribeModelQualityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelQualityJobDefinitionResponseTypeDef",
+    {
+        "JobDefinitionArn": str,
+        "JobDefinitionName": str,
+        "CreationTime": datetime,
+        "ModelQualityBaselineConfig": ModelQualityBaselineConfigTypeDef,
+        "ModelQualityAppSpecification": ModelQualityAppSpecificationTypeDef,
+        "ModelQualityJobInput": ModelQualityJobInputTypeDef,
+        "ModelQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "RoleArn": str,
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredMonitoringJobDefinitionTypeDef = TypedDict(
     "_RequiredMonitoringJobDefinitionTypeDef",
     {
         "MonitoringInputs": Sequence[MonitoringInputTypeDef],
         "MonitoringOutputConfig": MonitoringOutputConfigTypeDef,
         "MonitoringResources": MonitoringResourcesTypeDef,
         "MonitoringAppSpecification": MonitoringAppSpecificationTypeDef,
@@ -19080,45 +17481,14 @@
 
 class MonitoringJobDefinitionTypeDef(
     _RequiredMonitoringJobDefinitionTypeDef, _OptionalMonitoringJobDefinitionTypeDef
 ):
     pass
 
 
-_RequiredAlgorithmValidationProfileOutputTypeDef = TypedDict(
-    "_RequiredAlgorithmValidationProfileOutputTypeDef",
-    {
-        "ProfileName": str,
-        "TrainingJobDefinition": TrainingJobDefinitionOutputTypeDef,
-    },
-)
-_OptionalAlgorithmValidationProfileOutputTypeDef = TypedDict(
-    "_OptionalAlgorithmValidationProfileOutputTypeDef",
-    {
-        "TransformJobDefinition": TransformJobDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class AlgorithmValidationProfileOutputTypeDef(
-    _RequiredAlgorithmValidationProfileOutputTypeDef,
-    _OptionalAlgorithmValidationProfileOutputTypeDef,
-):
-    pass
-
-
-ModelPackageValidationProfileOutputTypeDef = TypedDict(
-    "ModelPackageValidationProfileOutputTypeDef",
-    {
-        "ProfileName": str,
-        "TransformJobDefinition": TransformJobDefinitionOutputTypeDef,
-    },
-)
-
 _RequiredAlgorithmValidationProfileTypeDef = TypedDict(
     "_RequiredAlgorithmValidationProfileTypeDef",
     {
         "ProfileName": str,
         "TrainingJobDefinition": TrainingJobDefinitionTypeDef,
     },
 )
@@ -19152,79 +17522,39 @@
         "TrainingJob": TrainingJobTypeDef,
         "ProcessingJob": ProcessingJobTypeDef,
         "TransformJob": TransformJobTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHyperParameterTuningJobRequestRequestTypeDef",
-    {
-        "HyperParameterTuningJobName": str,
-        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
-    },
-)
-_OptionalCreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHyperParameterTuningJobRequestRequestTypeDef",
-    {
-        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionTypeDef,
-        "TrainingJobDefinitions": Sequence[HyperParameterTrainingJobDefinitionUnionTypeDef],
-        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "Autotune": AutotuneTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateHyperParameterTuningJobRequestRequestTypeDef(
-    _RequiredCreateHyperParameterTuningJobRequestRequestTypeDef,
-    _OptionalCreateHyperParameterTuningJobRequestRequestTypeDef,
-):
-    pass
-
-
-MonitoringScheduleConfigOutputTypeDef = TypedDict(
-    "MonitoringScheduleConfigOutputTypeDef",
+GetScalingConfigurationRecommendationResponseTypeDef = TypedDict(
+    "GetScalingConfigurationRecommendationResponseTypeDef",
     {
-        "ScheduleConfig": ScheduleConfigTypeDef,
-        "MonitoringJobDefinition": MonitoringJobDefinitionOutputTypeDef,
-        "MonitoringJobDefinitionName": str,
-        "MonitoringType": MonitoringTypeType,
+        "InferenceRecommendationsJobName": str,
+        "RecommendationId": str,
+        "EndpointName": str,
+        "TargetCpuUtilizationPerCore": int,
+        "ScalingPolicyObjective": ScalingPolicyObjectiveTypeDef,
+        "Metric": ScalingPolicyMetricTypeDef,
+        "DynamicScalingConfiguration": DynamicScalingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 MonitoringScheduleConfigTypeDef = TypedDict(
     "MonitoringScheduleConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
         "MonitoringJobDefinition": MonitoringJobDefinitionTypeDef,
         "MonitoringJobDefinitionName": str,
         "MonitoringType": MonitoringTypeType,
     },
     total=False,
 )
 
-AlgorithmValidationSpecificationOutputTypeDef = TypedDict(
-    "AlgorithmValidationSpecificationOutputTypeDef",
-    {
-        "ValidationRole": str,
-        "ValidationProfiles": List[AlgorithmValidationProfileOutputTypeDef],
-    },
-)
-
-ModelPackageValidationSpecificationOutputTypeDef = TypedDict(
-    "ModelPackageValidationSpecificationOutputTypeDef",
-    {
-        "ValidationRole": str,
-        "ValidationProfiles": List[ModelPackageValidationProfileOutputTypeDef],
-    },
-)
-
 AlgorithmValidationSpecificationTypeDef = TypedDict(
     "AlgorithmValidationSpecificationTypeDef",
     {
         "ValidationRole": str,
         "ValidationProfiles": Sequence[AlgorithmValidationProfileTypeDef],
     },
 )
@@ -19261,25 +17591,48 @@
         "Tags": List[TagTypeDef],
         "Parents": List[ParentTypeDef],
         "RunName": str,
     },
     total=False,
 )
 
+_RequiredCreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMonitoringScheduleRequestRequestTypeDef",
+    {
+        "MonitoringScheduleName": str,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
+    },
+)
+_OptionalCreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMonitoringScheduleRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateMonitoringScheduleRequestRequestTypeDef(
+    _RequiredCreateMonitoringScheduleRequestRequestTypeDef,
+    _OptionalCreateMonitoringScheduleRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeMonitoringScheduleResponseTypeDef = TypedDict(
     "DescribeMonitoringScheduleResponseTypeDef",
     {
         "MonitoringScheduleArn": str,
         "MonitoringScheduleName": str,
         "MonitoringScheduleStatus": ScheduleStatusType,
         "MonitoringType": MonitoringTypeType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigOutputTypeDef,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
         "EndpointName": str,
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelDashboardMonitoringScheduleTypeDef = TypedDict(
@@ -19288,15 +17641,15 @@
         "MonitoringScheduleArn": str,
         "MonitoringScheduleName": str,
         "MonitoringScheduleStatus": ScheduleStatusType,
         "MonitoringType": MonitoringTypeType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigOutputTypeDef,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
         "EndpointName": str,
         "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
     },
     total=False,
 )
 
@@ -19306,86 +17659,113 @@
         "MonitoringScheduleArn": str,
         "MonitoringScheduleName": str,
         "MonitoringScheduleStatus": ScheduleStatusType,
         "MonitoringType": MonitoringTypeType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigOutputTypeDef,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
         "EndpointName": str,
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMonitoringScheduleRequestRequestTypeDef",
+UpdateMonitoringScheduleRequestRequestTypeDef = TypedDict(
+    "UpdateMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
     },
 )
-_OptionalCreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMonitoringScheduleRequestRequestTypeDef",
+
+_RequiredCreateAlgorithmInputRequestTypeDef = TypedDict(
+    "_RequiredCreateAlgorithmInputRequestTypeDef",
+    {
+        "AlgorithmName": str,
+        "TrainingSpecification": TrainingSpecificationTypeDef,
+    },
+)
+_OptionalCreateAlgorithmInputRequestTypeDef = TypedDict(
+    "_OptionalCreateAlgorithmInputRequestTypeDef",
     {
+        "AlgorithmDescription": str,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "ValidationSpecification": AlgorithmValidationSpecificationTypeDef,
+        "CertifyForMarketplace": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class CreateMonitoringScheduleRequestRequestTypeDef(
-    _RequiredCreateMonitoringScheduleRequestRequestTypeDef,
-    _OptionalCreateMonitoringScheduleRequestRequestTypeDef,
+class CreateAlgorithmInputRequestTypeDef(
+    _RequiredCreateAlgorithmInputRequestTypeDef, _OptionalCreateAlgorithmInputRequestTypeDef
 ):
     pass
 
 
-MonitoringScheduleConfigUnionTypeDef = Union[
-    MonitoringScheduleConfigTypeDef, MonitoringScheduleConfigOutputTypeDef
-]
-UpdateMonitoringScheduleRequestRequestTypeDef = TypedDict(
-    "UpdateMonitoringScheduleRequestRequestTypeDef",
-    {
-        "MonitoringScheduleName": str,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
-    },
-)
-
 DescribeAlgorithmOutputTypeDef = TypedDict(
     "DescribeAlgorithmOutputTypeDef",
     {
         "AlgorithmName": str,
         "AlgorithmArn": str,
         "AlgorithmDescription": str,
         "CreationTime": datetime,
-        "TrainingSpecification": TrainingSpecificationOutputTypeDef,
-        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
-        "ValidationSpecification": AlgorithmValidationSpecificationOutputTypeDef,
+        "TrainingSpecification": TrainingSpecificationTypeDef,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "ValidationSpecification": AlgorithmValidationSpecificationTypeDef,
         "AlgorithmStatus": AlgorithmStatusType,
         "AlgorithmStatusDetails": AlgorithmStatusDetailsTypeDef,
         "ProductId": str,
         "CertifyForMarketplace": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateModelPackageInputRequestTypeDef = TypedDict(
+    "CreateModelPackageInputRequestTypeDef",
+    {
+        "ModelPackageName": str,
+        "ModelPackageGroupName": str,
+        "ModelPackageDescription": str,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "ValidationSpecification": ModelPackageValidationSpecificationTypeDef,
+        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationTypeDef,
+        "CertifyForMarketplace": bool,
+        "Tags": Sequence[TagTypeDef],
+        "ModelApprovalStatus": ModelApprovalStatusType,
+        "MetadataProperties": MetadataPropertiesTypeDef,
+        "ModelMetrics": ModelMetricsTypeDef,
+        "ClientToken": str,
+        "CustomerMetadataProperties": Mapping[str, str],
+        "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
+        "Domain": str,
+        "Task": str,
+        "SamplePayloadUrl": str,
+        "AdditionalInferenceSpecifications": Sequence[
+            AdditionalInferenceSpecificationDefinitionTypeDef
+        ],
+    },
+    total=False,
+)
+
 DescribeModelPackageOutputTypeDef = TypedDict(
     "DescribeModelPackageOutputTypeDef",
     {
         "ModelPackageName": str,
         "ModelPackageGroupName": str,
         "ModelPackageVersion": int,
         "ModelPackageArn": str,
         "ModelPackageDescription": str,
         "CreationTime": datetime,
-        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
-        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationOutputTypeDef,
-        "ValidationSpecification": ModelPackageValidationSpecificationOutputTypeDef,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationTypeDef,
+        "ValidationSpecification": ModelPackageValidationSpecificationTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
         "ModelPackageStatusDetails": ModelPackageStatusDetailsTypeDef,
         "CertifyForMarketplace": bool,
         "ModelApprovalStatus": ModelApprovalStatusType,
         "CreatedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
         "ModelMetrics": ModelMetricsTypeDef,
@@ -19394,114 +17774,55 @@
         "ApprovalDescription": str,
         "CustomerMetadataProperties": Dict[str, str],
         "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
         "Domain": str,
         "Task": str,
         "SamplePayloadUrl": str,
         "AdditionalInferenceSpecifications": List[
-            AdditionalInferenceSpecificationDefinitionOutputTypeDef
+            AdditionalInferenceSpecificationDefinitionTypeDef
         ],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelPackageTypeDef = TypedDict(
     "ModelPackageTypeDef",
     {
         "ModelPackageName": str,
         "ModelPackageGroupName": str,
         "ModelPackageVersion": int,
         "ModelPackageArn": str,
         "ModelPackageDescription": str,
         "CreationTime": datetime,
-        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
-        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationOutputTypeDef,
-        "ValidationSpecification": ModelPackageValidationSpecificationOutputTypeDef,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationTypeDef,
+        "ValidationSpecification": ModelPackageValidationSpecificationTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
         "ModelPackageStatusDetails": ModelPackageStatusDetailsTypeDef,
         "CertifyForMarketplace": bool,
         "ModelApprovalStatus": ModelApprovalStatusType,
         "CreatedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
         "ModelMetrics": ModelMetricsTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "ApprovalDescription": str,
         "Domain": str,
         "Task": str,
         "SamplePayloadUrl": str,
         "AdditionalInferenceSpecifications": List[
-            AdditionalInferenceSpecificationDefinitionOutputTypeDef
+            AdditionalInferenceSpecificationDefinitionTypeDef
         ],
         "Tags": List[TagTypeDef],
         "CustomerMetadataProperties": Dict[str, str],
         "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
     },
     total=False,
 )
 
-AlgorithmValidationSpecificationUnionTypeDef = Union[
-    AlgorithmValidationSpecificationTypeDef, AlgorithmValidationSpecificationOutputTypeDef
-]
-_RequiredCreateAlgorithmInputRequestTypeDef = TypedDict(
-    "_RequiredCreateAlgorithmInputRequestTypeDef",
-    {
-        "AlgorithmName": str,
-        "TrainingSpecification": TrainingSpecificationTypeDef,
-    },
-)
-_OptionalCreateAlgorithmInputRequestTypeDef = TypedDict(
-    "_OptionalCreateAlgorithmInputRequestTypeDef",
-    {
-        "AlgorithmDescription": str,
-        "InferenceSpecification": InferenceSpecificationTypeDef,
-        "ValidationSpecification": AlgorithmValidationSpecificationTypeDef,
-        "CertifyForMarketplace": bool,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateAlgorithmInputRequestTypeDef(
-    _RequiredCreateAlgorithmInputRequestTypeDef, _OptionalCreateAlgorithmInputRequestTypeDef
-):
-    pass
-
-
-CreateModelPackageInputRequestTypeDef = TypedDict(
-    "CreateModelPackageInputRequestTypeDef",
-    {
-        "ModelPackageName": str,
-        "ModelPackageGroupName": str,
-        "ModelPackageDescription": str,
-        "InferenceSpecification": InferenceSpecificationTypeDef,
-        "ValidationSpecification": ModelPackageValidationSpecificationTypeDef,
-        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationTypeDef,
-        "CertifyForMarketplace": bool,
-        "Tags": Sequence[TagTypeDef],
-        "ModelApprovalStatus": ModelApprovalStatusType,
-        "MetadataProperties": MetadataPropertiesTypeDef,
-        "ModelMetrics": ModelMetricsTypeDef,
-        "ClientToken": str,
-        "CustomerMetadataProperties": Mapping[str, str],
-        "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
-        "Domain": str,
-        "Task": str,
-        "SamplePayloadUrl": str,
-        "AdditionalInferenceSpecifications": Sequence[
-            AdditionalInferenceSpecificationDefinitionUnionTypeDef
-        ],
-    },
-    total=False,
-)
-
-ModelPackageValidationSpecificationUnionTypeDef = Union[
-    ModelPackageValidationSpecificationTypeDef, ModelPackageValidationSpecificationOutputTypeDef
-]
 ModelDashboardModelTypeDef = TypedDict(
     "ModelDashboardModelTypeDef",
     {
         "Model": ModelTypeDef,
         "Endpoints": List[ModelDashboardEndpointTypeDef],
         "LastBatchTransformJob": TransformJobTypeDef,
         "MonitoringSchedules": List[ModelDashboardMonitoringScheduleTypeDef],
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/type_defs.pyi` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ActionStatusType,
+    AggregationTransformationValueType,
     AlgorithmSortByType,
     AlgorithmStatusType,
     AppImageConfigSortKeyType,
     AppInstanceTypeType,
     AppNetworkAccessTypeType,
     AppSecurityGroupManagementType,
     AppStatusType,
@@ -61,14 +62,15 @@
     CodeRepositorySortOrderType,
     CompilationJobStatusType,
     CompleteOnConvergenceType,
     CompressionTypeType,
     ConditionOutcomeType,
     ContainerModeType,
     ContentClassifierType,
+    CrossAccountFilterOptionType,
     DataDistributionTypeType,
     DetailedAlgorithmStatusType,
     DetailedModelPackageStatusType,
     DeviceDeploymentStatusType,
     DeviceSubsetTypeType,
     DirectInternetAccessType,
     DirectionType,
@@ -84,14 +86,16 @@
     FeatureGroupSortByType,
     FeatureGroupSortOrderType,
     FeatureGroupStatusType,
     FeatureStatusType,
     FeatureTypeType,
     FileSystemAccessModeType,
     FileSystemTypeType,
+    FillingTypeType,
+    FlatInvocationsType,
     FlowDefinitionStatusType,
     FrameworkType,
     HubContentSortByType,
     HubContentStatusType,
     HubContentTypeType,
     HubSortByType,
     HubStatusType,
@@ -178,20 +182,22 @@
     ProductionVariantAcceleratorTypeType,
     ProductionVariantInstanceTypeType,
     ProfilingStatusType,
     ProjectSortByType,
     ProjectSortOrderType,
     ProjectStatusType,
     RecommendationJobStatusType,
+    RecommendationJobSupportedEndpointTypeType,
     RecommendationJobTypeType,
     RecommendationStatusType,
     RecordWrapperType,
     RedshiftResultCompressionTypeType,
     RedshiftResultFormatType,
     RepositoryAccessModeType,
+    ResourceCatalogSortOrderType,
     ResourceTypeType,
     RetentionTypeType,
     RootAccessType,
     RStudioServerProAccessStatusType,
     RStudioServerProUserGroupType,
     RuleEvaluationStatusType,
     S3DataDistributionType,
@@ -213,32 +219,35 @@
     SortPipelinesByType,
     SortTrialComponentsByType,
     SortTrialsByType,
     SpaceSortKeyType,
     SpaceStatusType,
     SplitTypeType,
     StageStatusType,
+    StatisticType,
     StepStatusType,
     StudioLifecycleConfigAppTypeType,
     StudioLifecycleConfigSortKeyType,
     TableFormatType,
     TargetDeviceType,
     TargetPlatformAcceleratorType,
     TargetPlatformArchType,
     TargetPlatformOsType,
     TrafficRoutingConfigTypeType,
+    TrafficTypeType,
     TrainingInputModeType,
     TrainingInstanceTypeType,
     TrainingJobEarlyStoppingTypeType,
     TrainingJobSortByOptionsType,
     TrainingJobStatusType,
     TrainingRepositoryAccessModeType,
     TransformInstanceTypeType,
     TransformJobStatusType,
     TrialComponentPrimaryStatusType,
+    TtlDurationUnitType,
     UserProfileSortKeyType,
     UserProfileStatusType,
     VariantPropertyTypeType,
     VariantStatusType,
     VendorGuidanceType,
     WarmPoolResourceStatusType,
     WorkforceStatusType,
@@ -261,75 +270,65 @@
     "AgentVersionTypeDef",
     "AlarmTypeDef",
     "MetricDefinitionTypeDef",
     "AlgorithmStatusItemTypeDef",
     "AlgorithmSummaryTypeDef",
     "AnnotationConsolidationConfigTypeDef",
     "AppDetailsTypeDef",
-    "AppSpecificationOutputTypeDef",
     "AppSpecificationTypeDef",
     "ArtifactSourceTypeTypeDef",
     "AssociateTrialComponentRequestRequestTypeDef",
     "AsyncInferenceClientConfigTypeDef",
-    "AsyncInferenceNotificationConfigOutputTypeDef",
     "AsyncInferenceNotificationConfigTypeDef",
     "AthenaDatasetDefinitionTypeDef",
-    "AutoMLAlgorithmConfigOutputTypeDef",
     "AutoMLAlgorithmConfigTypeDef",
     "AutoMLCandidateStepTypeDef",
     "AutoMLContainerDefinitionTypeDef",
     "FinalAutoMLJobObjectiveMetricTypeDef",
     "AutoMLS3DataSourceTypeDef",
     "AutoMLDataSplitConfigTypeDef",
     "AutoMLJobArtifactsTypeDef",
     "AutoMLJobCompletionCriteriaTypeDef",
     "AutoMLJobObjectiveTypeDef",
     "AutoMLJobStepMetadataTypeDef",
     "AutoMLPartialFailureReasonTypeDef",
     "AutoMLOutputDataConfigTypeDef",
     "TabularResolvedAttributesTypeDef",
-    "VpcConfigOutputTypeDef",
     "VpcConfigTypeDef",
     "AutoParameterTypeDef",
     "AutotuneTypeDef",
     "BatchDataCaptureConfigTypeDef",
     "BatchDescribeModelPackageErrorTypeDef",
     "BatchDescribeModelPackageInputRequestTypeDef",
     "BestObjectiveNotImprovingTypeDef",
     "MetricsSourceTypeDef",
     "CacheHitResultTypeDef",
     "OutputParameterTypeDef",
     "CandidateArtifactLocationsTypeDef",
     "MetricDatumTypeDef",
     "ModelRegisterSettingsTypeDef",
     "TimeSeriesForecastingSettingsTypeDef",
+    "WorkspaceSettingsTypeDef",
     "CapacitySizeTypeDef",
-    "CaptureContentTypeHeaderOutputTypeDef",
     "CaptureContentTypeHeaderTypeDef",
     "CaptureOptionTypeDef",
-    "CategoricalParameterOutputTypeDef",
-    "CategoricalParameterRangeOutputTypeDef",
-    "CategoricalParameterRangeSpecificationOutputTypeDef",
     "CategoricalParameterRangeSpecificationTypeDef",
     "CategoricalParameterRangeTypeDef",
     "CategoricalParameterTypeDef",
-    "ShuffleConfigTypeDef",
-    "ChannelSpecificationOutputTypeDef",
     "ChannelSpecificationTypeDef",
+    "ShuffleConfigTypeDef",
     "CheckpointConfigTypeDef",
     "ClarifyCheckStepMetadataTypeDef",
-    "ClarifyInferenceConfigOutputTypeDef",
     "ClarifyInferenceConfigTypeDef",
     "ClarifyShapBaselineConfigTypeDef",
     "ClarifyTextConfigTypeDef",
     "GitConfigTypeDef",
     "CodeRepositoryTypeDef",
     "CognitoConfigTypeDef",
     "CognitoMemberDefinitionTypeDef",
-    "CollectionConfigurationOutputTypeDef",
     "CollectionConfigurationTypeDef",
     "CompilationJobSummaryTypeDef",
     "ConditionStepMetadataTypeDef",
     "MultiModelConfigTypeDef",
     "ContextSourceTypeDef",
     "ContinuousParameterRangeSpecificationTypeDef",
     "ContinuousParameterRangeTypeDef",
@@ -362,16 +361,18 @@
     "NotebookInstanceLifecycleHookTypeDef",
     "ParallelismConfigurationTypeDef",
     "PipelineDefinitionS3LocationTypeDef",
     "CreatePresignedDomainUrlRequestRequestTypeDef",
     "CreatePresignedNotebookInstanceUrlInputRequestTypeDef",
     "ExperimentConfigTypeDef",
     "ProcessingStoppingConditionTypeDef",
+    "DebugRuleConfigurationTypeDef",
     "OutputDataConfigTypeDef",
     "ProfilerConfigTypeDef",
+    "ProfilerRuleConfigurationTypeDef",
     "RetryStrategyTypeDef",
     "TensorBoardOutputConfigTypeDef",
     "DataProcessingTypeDef",
     "ModelClientConfigTypeDef",
     "TransformOutputTypeDef",
     "TransformResourcesTypeDef",
     "TimestampTypeDef",
@@ -379,26 +380,23 @@
     "TrialComponentParameterValueTypeDef",
     "TrialComponentStatusTypeDef",
     "OidcConfigTypeDef",
     "SourceIpConfigTypeDef",
     "WorkforceVpcConfigRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "CustomImageTypeDef",
+    "CustomizedMetricSpecificationTypeDef",
     "DataCaptureConfigSummaryTypeDef",
     "DataCatalogConfigTypeDef",
-    "DataQualityAppSpecificationOutputTypeDef",
     "MonitoringConstraintsResourceTypeDef",
     "MonitoringStatisticsResourceTypeDef",
     "EndpointInputTypeDef",
     "FileSystemDataSourceTypeDef",
-    "S3DataSourceOutputTypeDef",
     "S3DataSourceTypeDef",
     "RedshiftDatasetDefinitionTypeDef",
-    "DebugRuleConfigurationOutputTypeDef",
-    "DebugRuleConfigurationTypeDef",
     "DebugRuleEvaluationStatusTypeDef",
     "DeleteActionRequestRequestTypeDef",
     "DeleteAlgorithmInputRequestTypeDef",
     "DeleteAppImageConfigRequestRequestTypeDef",
     "DeleteAppRequestRequestTypeDef",
     "DeleteAssociationRequestRequestTypeDef",
     "DeleteCodeRepositoryInputRequestTypeDef",
@@ -438,32 +436,30 @@
     "DeleteTrialComponentRequestRequestTypeDef",
     "DeleteTrialRequestRequestTypeDef",
     "DeleteUserProfileRequestRequestTypeDef",
     "DeleteWorkforceRequestRequestTypeDef",
     "DeleteWorkteamRequestRequestTypeDef",
     "DeployedImageTypeDef",
     "RealTimeInferenceRecommendationTypeDef",
-    "DeviceSelectionConfigOutputTypeDef",
+    "DeviceSelectionConfigTypeDef",
     "EdgeDeploymentConfigTypeDef",
     "EdgeDeploymentStatusTypeDef",
-    "DeviceSelectionConfigTypeDef",
     "DeregisterDevicesRequestRequestTypeDef",
     "DescribeActionRequestRequestTypeDef",
     "DescribeAlgorithmInputRequestTypeDef",
     "DescribeAppImageConfigRequestRequestTypeDef",
     "DescribeAppRequestRequestTypeDef",
     "DescribeArtifactRequestRequestTypeDef",
     "DescribeAutoMLJobRequestRequestTypeDef",
     "ModelDeployResultTypeDef",
     "DescribeAutoMLJobV2RequestRequestTypeDef",
     "DescribeCodeRepositoryInputRequestTypeDef",
     "DescribeCompilationJobRequestRequestTypeDef",
     "ModelArtifactsTypeDef",
     "ModelDigestsTypeDef",
-    "NeoVpcConfigOutputTypeDef",
     "DescribeContextRequestRequestTypeDef",
     "DescribeDataQualityJobDefinitionRequestRequestTypeDef",
     "DescribeDeviceFleetRequestRequestTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "EdgeModelTypeDef",
     "DescribeDomainRequestRequestTypeDef",
     "DescribeEdgeDeploymentPlanRequestRequestTypeDef",
@@ -490,32 +486,28 @@
     "HyperParameterTuningJobConsumedResourcesTypeDef",
     "ObjectiveStatusCountersTypeDef",
     "TrainingJobStatusCountersTypeDef",
     "DescribeImageRequestRequestTypeDef",
     "DescribeImageVersionRequestRequestTypeDef",
     "DescribeInferenceExperimentRequestRequestTypeDef",
     "EndpointMetadataTypeDef",
-    "InferenceExperimentScheduleOutputTypeDef",
     "DescribeInferenceRecommendationsJobRequestRequestTypeDef",
     "DescribeLabelingJobRequestRequestTypeDef",
     "LabelCountersTypeDef",
     "LabelingJobOutputTypeDef",
     "DescribeLineageGroupRequestRequestTypeDef",
     "DescribeModelBiasJobDefinitionRequestRequestTypeDef",
-    "ModelBiasAppSpecificationOutputTypeDef",
     "DescribeModelCardExportJobRequestRequestTypeDef",
     "ModelCardExportArtifactsTypeDef",
     "DescribeModelCardRequestRequestTypeDef",
     "DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef",
-    "ModelExplainabilityAppSpecificationOutputTypeDef",
     "DescribeModelInputRequestTypeDef",
     "DescribeModelPackageGroupInputRequestTypeDef",
     "DescribeModelPackageInputRequestTypeDef",
     "DescribeModelQualityJobDefinitionRequestRequestTypeDef",
-    "ModelQualityAppSpecificationOutputTypeDef",
     "DescribeMonitoringScheduleRequestRequestTypeDef",
     "MonitoringExecutionSummaryTypeDef",
     "DescribeNotebookInstanceInputRequestTypeDef",
     "DescribeNotebookInstanceLifecycleConfigInputRequestTypeDef",
     "DescribePipelineDefinitionForExecutionRequestRequestTypeDef",
     "DescribePipelineExecutionRequestRequestTypeDef",
     "PipelineExperimentConfigTypeDef",
@@ -525,16 +517,14 @@
     "ServiceCatalogProvisionedProductDetailsTypeDef",
     "DescribeSpaceRequestRequestTypeDef",
     "DescribeStudioLifecycleConfigRequestRequestTypeDef",
     "DescribeSubscribedWorkteamRequestRequestTypeDef",
     "SubscribedWorkteamTypeDef",
     "DescribeTrainingJobRequestRequestTypeDef",
     "MetricDataTypeDef",
-    "ProfilerConfigOutputTypeDef",
-    "ProfilerRuleConfigurationOutputTypeDef",
     "ProfilerRuleEvaluationStatusTypeDef",
     "SecondaryStatusTransitionTypeDef",
     "WarmPoolStatusTypeDef",
     "DescribeTransformJobRequestRequestTypeDef",
     "DescribeTrialComponentRequestRequestTypeDef",
     "TrialComponentMetricSummaryTypeDef",
     "TrialComponentSourceTypeDef",
@@ -555,26 +545,28 @@
     "EMRStepMetadataTypeDef",
     "EdgeDeploymentPlanSummaryTypeDef",
     "EdgeModelStatTypeDef",
     "EdgePackagingJobSummaryTypeDef",
     "EdgeTypeDef",
     "EndpointConfigSummaryTypeDef",
     "EndpointInfoTypeDef",
-    "EndpointOutputConfigurationTypeDef",
+    "ProductionVariantServerlessConfigTypeDef",
     "InferenceMetricsTypeDef",
     "EndpointSummaryTypeDef",
     "EnvironmentParameterTypeDef",
     "FailStepMetadataTypeDef",
     "FileSystemConfigTypeDef",
     "FilterTypeDef",
     "FinalHyperParameterTuningJobObjectiveMetricTypeDef",
     "FlowDefinitionSummaryTypeDef",
     "GetDeviceFleetReportRequestRequestTypeDef",
     "GetLineageGroupPolicyRequestRequestTypeDef",
     "GetModelPackageGroupPolicyInputRequestTypeDef",
+    "ScalingPolicyObjectiveTypeDef",
+    "ScalingPolicyMetricTypeDef",
     "PropertyNameSuggestionTypeDef",
     "GitConfigForUpdateTypeDef",
     "HubContentInfoTypeDef",
     "HubInfoTypeDef",
     "HumanLoopActivationConditionsConfigTypeDef",
     "UiConfigTypeDef",
     "HumanTaskUiSummaryTypeDef",
@@ -590,15 +582,14 @@
     "RecommendationMetricsTypeDef",
     "InferenceRecommendationsJobTypeDef",
     "InstanceGroupTypeDef",
     "IntegerParameterRangeSpecificationTypeDef",
     "IntegerParameterRangeTypeDef",
     "KernelSpecTypeDef",
     "LabelCountersForWorkteamTypeDef",
-    "LabelingJobDataAttributesOutputTypeDef",
     "LabelingJobDataAttributesTypeDef",
     "LabelingJobS3DataSourceTypeDef",
     "LabelingJobSnsDataSourceTypeDef",
     "LineageGroupSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListAppsRequestRequestTypeDef",
@@ -621,51 +612,51 @@
     "ListPipelineExecutionStepsRequestRequestTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "ListPipelineParametersForExecutionRequestRequestTypeDef",
     "ParameterTypeDef",
     "PipelineSummaryTypeDef",
     "ProcessingJobSummaryTypeDef",
     "ProjectSummaryTypeDef",
+    "ResourceCatalogTypeDef",
     "ListSpacesRequestRequestTypeDef",
     "SpaceDetailsTypeDef",
     "ListStageDevicesRequestRequestTypeDef",
     "StudioLifecycleConfigDetailsTypeDef",
     "ListSubscribedWorkteamsRequestRequestTypeDef",
     "ListTagsInputRequestTypeDef",
     "ListTrainingJobsForHyperParameterTuningJobRequestRequestTypeDef",
     "TransformJobSummaryTypeDef",
     "ListUserProfilesRequestRequestTypeDef",
     "UserProfileDetailsTypeDef",
     "ListWorkforcesRequestRequestTypeDef",
     "ListWorkteamsRequestRequestTypeDef",
-    "OidcMemberDefinitionOutputTypeDef",
     "OidcMemberDefinitionTypeDef",
+    "PredefinedMetricSpecificationTypeDef",
     "MonitoringGroundTruthS3InputTypeDef",
     "ModelDashboardEndpointTypeDef",
     "ModelDashboardIndicatorActionTypeDef",
     "S3ModelDataSourceTypeDef",
     "RealTimeInferenceConfigTypeDef",
     "ModelInputTypeDef",
     "ModelLatencyThresholdTypeDef",
     "ModelMetadataFilterTypeDef",
     "ModelPackageStatusItemTypeDef",
     "ModelStepMetadataTypeDef",
-    "MonitoringAppSpecificationOutputTypeDef",
     "MonitoringAppSpecificationTypeDef",
     "MonitoringClusterConfigTypeDef",
     "MonitoringCsvDatasetFormatTypeDef",
     "MonitoringJsonDatasetFormatTypeDef",
     "MonitoringS3OutputTypeDef",
     "ScheduleConfigTypeDef",
     "S3StorageConfigTypeDef",
     "OidcConfigForResponseTypeDef",
     "OnlineStoreSecurityConfigTypeDef",
+    "TtlDurationTypeDef",
     "TargetPlatformTypeDef",
     "ParentTypeDef",
-    "ProductionVariantServerlessConfigTypeDef",
     "ProductionVariantStatusTypeDef",
     "PhaseTypeDef",
     "ProcessingJobStepMetadataTypeDef",
     "QualityCheckStepMetadataTypeDef",
     "RegisterModelStepMetadataTypeDef",
     "TrainingJobStepMetadataTypeDef",
     "TransformJobStepMetadataTypeDef",
@@ -673,37 +664,34 @@
     "SelectiveExecutionResultTypeDef",
     "ProcessingClusterConfigTypeDef",
     "ProcessingFeatureStoreOutputTypeDef",
     "ProcessingS3InputTypeDef",
     "ProcessingS3OutputTypeDef",
     "ProductionVariantCoreDumpConfigTypeDef",
     "ProfilerConfigForUpdateTypeDef",
-    "ProfilerRuleConfigurationTypeDef",
     "PropertyNameQueryTypeDef",
     "ProvisioningParameterTypeDef",
     "USDTypeDef",
     "PutModelPackageGroupPolicyInputRequestTypeDef",
     "VertexTypeDef",
     "RStudioServerProAppSettingsTypeDef",
     "RecommendationJobCompiledOutputConfigTypeDef",
-    "RecommendationJobPayloadConfigOutputTypeDef",
     "RecommendationJobPayloadConfigTypeDef",
     "RecommendationJobResourceLimitTypeDef",
-    "RecommendationJobVpcConfigOutputTypeDef",
     "RecommendationJobVpcConfigTypeDef",
     "RenderableTaskTypeDef",
     "RenderingErrorTypeDef",
     "ResourceConfigForUpdateTypeDef",
     "SearchRequestRequestTypeDef",
     "SelectedStepTypeDef",
     "SendPipelineExecutionStepFailureRequestRequestTypeDef",
     "ShadowModelVariantConfigTypeDef",
     "SharingSettingsTypeDef",
     "SourceAlgorithmTypeDef",
-    "SourceIpConfigOutputTypeDef",
+    "StairsTypeDef",
     "StartEdgeDeploymentStageRequestRequestTypeDef",
     "StartInferenceExperimentRequestRequestTypeDef",
     "StartMonitoringScheduleRequestRequestTypeDef",
     "StartNotebookInstanceInputRequestTypeDef",
     "StopAutoMLJobRequestRequestTypeDef",
     "StopCompilationJobRequestRequestTypeDef",
     "StopEdgeDeploymentStageRequestRequestTypeDef",
@@ -713,14 +701,16 @@
     "StopLabelingJobRequestRequestTypeDef",
     "StopMonitoringScheduleRequestRequestTypeDef",
     "StopNotebookInstanceInputRequestTypeDef",
     "StopPipelineExecutionRequestRequestTypeDef",
     "StopProcessingJobRequestRequestTypeDef",
     "StopTrainingJobRequestRequestTypeDef",
     "StopTransformJobRequestRequestTypeDef",
+    "TimeSeriesConfigTypeDef",
+    "TimeSeriesTransformationsTypeDef",
     "TrainingRepositoryAuthConfigTypeDef",
     "TransformS3DataSourceTypeDef",
     "UpdateActionRequestRequestTypeDef",
     "UpdateArtifactRequestRequestTypeDef",
     "UpdateContextRequestRequestTypeDef",
     "VariantPropertyTypeDef",
     "UpdateExperimentRequestRequestTypeDef",
@@ -844,87 +834,70 @@
     "AddTagsOutputTypeDef",
     "CreateExperimentRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
     "CreateModelPackageGroupInputRequestTypeDef",
     "CreateStudioLifecycleConfigRequestRequestTypeDef",
     "ImportHubContentRequestRequestTypeDef",
     "ListTagsOutputTypeDef",
-    "AutoRollbackConfigOutputTypeDef",
     "AutoRollbackConfigTypeDef",
-    "HyperParameterAlgorithmSpecificationOutputTypeDef",
     "HyperParameterAlgorithmSpecificationTypeDef",
     "AlgorithmStatusDetailsTypeDef",
     "ListAlgorithmsOutputTypeDef",
     "ListAppsResponseTypeDef",
-    "AppSpecificationUnionTypeDef",
-    "ArtifactSourceOutputTypeDef",
     "ArtifactSourceTypeDef",
-    "AsyncInferenceOutputConfigOutputTypeDef",
     "AsyncInferenceOutputConfigTypeDef",
-    "AutoMLCandidateGenerationConfigOutputTypeDef",
-    "CandidateGenerationConfigOutputTypeDef",
     "AutoMLCandidateGenerationConfigTypeDef",
     "CandidateGenerationConfigTypeDef",
     "AutoMLDataSourceTypeDef",
     "ImageClassificationJobConfigTypeDef",
     "TextClassificationJobConfigTypeDef",
     "ResolvedAttributesTypeDef",
     "AutoMLJobSummaryTypeDef",
     "AutoMLProblemTypeResolvedAttributesTypeDef",
-    "AutoMLSecurityConfigOutputTypeDef",
-    "LabelingJobResourceConfigOutputTypeDef",
-    "MonitoringNetworkConfigOutputTypeDef",
-    "NetworkConfigOutputTypeDef",
     "AutoMLSecurityConfigTypeDef",
     "LabelingJobResourceConfigTypeDef",
     "MonitoringNetworkConfigTypeDef",
     "NetworkConfigTypeDef",
-    "VpcConfigUnionTypeDef",
     "BiasTypeDef",
     "DriftCheckModelDataQualityTypeDef",
     "DriftCheckModelQualityTypeDef",
     "ExplainabilityTypeDef",
     "ModelDataQualityTypeDef",
     "ModelQualityTypeDef",
     "CallbackStepMetadataTypeDef",
     "LambdaStepMetadataTypeDef",
     "SendPipelineExecutionStepSuccessRequestRequestTypeDef",
     "CandidatePropertiesTypeDef",
     "CanvasAppSettingsTypeDef",
+    "RollingUpdatePolicyTypeDef",
     "TrafficRoutingConfigTypeDef",
-    "InferenceExperimentDataStorageConfigOutputTypeDef",
     "InferenceExperimentDataStorageConfigTypeDef",
-    "DataCaptureConfigOutputTypeDef",
     "DataCaptureConfigTypeDef",
-    "EnvironmentParameterRangesOutputTypeDef",
     "EnvironmentParameterRangesTypeDef",
     "ClarifyShapConfigTypeDef",
     "CodeRepositorySummaryTypeDef",
     "CreateCodeRepositoryInputRequestTypeDef",
     "DescribeCodeRepositoryOutputTypeDef",
-    "DebugHookConfigOutputTypeDef",
     "DebugHookConfigTypeDef",
     "ListCompilationJobsResponseTypeDef",
     "ContextSummaryTypeDef",
     "CreateContextRequestRequestTypeDef",
     "TuningJobCompletionCriteriaTypeDef",
     "CreateActionRequestRequestTypeDef",
     "CreateTrialRequestRequestTypeDef",
     "CreateAppRequestRequestTypeDef",
     "DescribeAppResponseTypeDef",
-    "JupyterServerAppSettingsOutputTypeDef",
     "JupyterServerAppSettingsTypeDef",
     "RStudioServerProDomainSettingsForUpdateTypeDef",
     "RStudioServerProDomainSettingsTypeDef",
     "TensorBoardAppSettingsTypeDef",
     "CreateDeviceFleetRequestRequestTypeDef",
     "CreateEdgePackagingJobRequestRequestTypeDef",
     "DescribeDeviceFleetResponseTypeDef",
     "UpdateDeviceFleetRequestRequestTypeDef",
-    "UpdateFeatureGroupRequestRequestTypeDef",
     "CreateHubRequestRequestTypeDef",
     "DescribeHubResponseTypeDef",
     "CreateHumanTaskUiRequestRequestTypeDef",
     "CreateModelCardExportJobRequestRequestTypeDef",
     "CreateModelCardRequestRequestTypeDef",
     "CreateNotebookInstanceInputRequestTypeDef",
     "DescribeNotebookInstanceOutputTypeDef",
@@ -982,43 +955,38 @@
     "ListMonitoringSchedulesRequestRequestTypeDef",
     "ListNotebookInstanceLifecycleConfigsInputRequestTypeDef",
     "ListNotebookInstancesInputRequestTypeDef",
     "ListPipelineExecutionsRequestRequestTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListProcessingJobsRequestRequestTypeDef",
     "ListProjectsInputRequestTypeDef",
+    "ListResourceCatalogsRequestRequestTypeDef",
     "ListStudioLifecycleConfigsRequestRequestTypeDef",
     "ListTrainingJobsRequestRequestTypeDef",
     "ListTransformJobsRequestRequestTypeDef",
     "ListTrialComponentsRequestRequestTypeDef",
     "ListTrialsRequestRequestTypeDef",
     "QueryFiltersTypeDef",
     "CreateTrialComponentRequestRequestTypeDef",
     "UpdateTrialComponentRequestRequestTypeDef",
     "CreateWorkforceRequestRequestTypeDef",
     "UpdateWorkforceRequestRequestTypeDef",
-    "KernelGatewayAppSettingsOutputTypeDef",
     "KernelGatewayAppSettingsTypeDef",
-    "RSessionAppSettingsOutputTypeDef",
     "RSessionAppSettingsTypeDef",
-    "DataQualityAppSpecificationUnionTypeDef",
     "ModelBiasBaselineConfigTypeDef",
     "ModelExplainabilityBaselineConfigTypeDef",
     "ModelQualityBaselineConfigTypeDef",
     "DataQualityBaselineConfigTypeDef",
     "MonitoringBaselineConfigTypeDef",
-    "DataSourceOutputTypeDef",
     "DataSourceTypeDef",
     "DatasetDefinitionTypeDef",
-    "DebugRuleConfigurationUnionTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DeploymentRecommendationTypeDef",
-    "DeploymentStageStatusSummaryTypeDef",
     "DeploymentStageTypeDef",
-    "NeoVpcConfigUnionTypeDef",
+    "DeploymentStageStatusSummaryTypeDef",
     "DescribeDeviceResponseTypeDef",
     "DescribeEdgePackagingJobResponseTypeDef",
     "DescribeEndpointInputEndpointDeletedWaitTypeDef",
     "DescribeEndpointInputEndpointInServiceWaitTypeDef",
     "DescribeImageRequestImageCreatedWaitTypeDef",
     "DescribeImageRequestImageDeletedWaitTypeDef",
     "DescribeImageRequestImageUpdatedWaitTypeDef",
@@ -1033,23 +1001,18 @@
     "ExperimentSummaryTypeDef",
     "FeatureGroupSummaryTypeDef",
     "DescribeFeatureMetadataResponseTypeDef",
     "FeatureMetadataTypeDef",
     "UpdateFeatureMetadataRequestRequestTypeDef",
     "DescribeHubContentResponseTypeDef",
     "DescribeHumanTaskUiResponseTypeDef",
-    "InferenceExperimentSummaryTypeDef",
-    "ModelBiasAppSpecificationUnionTypeDef",
     "DescribeModelCardExportJobResponseTypeDef",
-    "ModelExplainabilityAppSpecificationUnionTypeDef",
-    "ModelQualityAppSpecificationUnionTypeDef",
     "ListMonitoringExecutionsResponseTypeDef",
     "DescribeSubscribedWorkteamResponseTypeDef",
     "ListSubscribedWorkteamsResponseTypeDef",
-    "ProfilerConfigUnionTypeDef",
     "TrainingJobSummaryTypeDef",
     "TrialSummaryTypeDef",
     "DesiredWeightAndCapacityTypeDef",
     "ListStageDevicesResponseTypeDef",
     "ListDeviceFleetsResponseTypeDef",
     "DeviceSummaryTypeDef",
     "RegisterDevicesRequestRequestTypeDef",
@@ -1057,45 +1020,41 @@
     "ListDomainsResponseTypeDef",
     "DriftCheckBiasTypeDef",
     "DriftCheckExplainabilityTypeDef",
     "ListEdgeDeploymentPlansResponseTypeDef",
     "GetDeviceFleetReportResponseTypeDef",
     "ListEdgePackagingJobsResponseTypeDef",
     "ListEndpointConfigsOutputTypeDef",
+    "EndpointOutputConfigurationTypeDef",
     "EndpointPerformanceTypeDef",
     "ListEndpointsOutputTypeDef",
     "ModelConfigurationTypeDef",
     "NestedFiltersTypeDef",
     "HyperParameterTrainingJobSummaryTypeDef",
     "ListFlowDefinitionsResponseTypeDef",
+    "GetScalingConfigurationRecommendationRequestRequestTypeDef",
     "GetSearchSuggestionsResponseTypeDef",
     "UpdateCodeRepositoryInputRequestTypeDef",
     "ListHubContentVersionsResponseTypeDef",
     "ListHubContentsResponseTypeDef",
     "ListHubsResponseTypeDef",
     "HumanLoopActivationConfigTypeDef",
     "ListHumanTaskUisResponseTypeDef",
-    "HyperParameterTuningResourceConfigOutputTypeDef",
     "HyperParameterTuningResourceConfigTypeDef",
     "HyperParameterTuningJobSummaryTypeDef",
     "HyperParameterTuningJobStrategyConfigTypeDef",
-    "HyperParameterTuningJobWarmStartConfigOutputTypeDef",
     "HyperParameterTuningJobWarmStartConfigTypeDef",
     "UserContextTypeDef",
     "ImageConfigTypeDef",
     "ListImagesResponseTypeDef",
     "ListImageVersionsResponseTypeDef",
     "ListInferenceRecommendationsJobsResponseTypeDef",
-    "ResourceConfigOutputTypeDef",
     "ResourceConfigTypeDef",
-    "ParameterRangeOutputTypeDef",
     "ParameterRangeTypeDef",
-    "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
-    "KernelGatewayImageConfigOutputTypeDef",
     "KernelGatewayImageConfigTypeDef",
     "LabelingJobForWorkteamSummaryTypeDef",
     "LabelingJobDataSourceTypeDef",
     "ListLineageGroupsResponseTypeDef",
     "ListActionsRequestListActionsPaginateTypeDef",
     "ListAlgorithmsInputListAlgorithmsPaginateTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
@@ -1145,14 +1104,15 @@
     "ListNotebookInstanceLifecycleConfigsInputListNotebookInstanceLifecycleConfigsPaginateTypeDef",
     "ListNotebookInstancesInputListNotebookInstancesPaginateTypeDef",
     "ListPipelineExecutionStepsRequestListPipelineExecutionStepsPaginateTypeDef",
     "ListPipelineExecutionsRequestListPipelineExecutionsPaginateTypeDef",
     "ListPipelineParametersForExecutionRequestListPipelineParametersForExecutionPaginateTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListProcessingJobsRequestListProcessingJobsPaginateTypeDef",
+    "ListResourceCatalogsRequestListResourceCatalogsPaginateTypeDef",
     "ListSpacesRequestListSpacesPaginateTypeDef",
     "ListStageDevicesRequestListStageDevicesPaginateTypeDef",
     "ListStudioLifecycleConfigsRequestListStudioLifecycleConfigsPaginateTypeDef",
     "ListSubscribedWorkteamsRequestListSubscribedWorkteamsPaginateTypeDef",
     "ListTagsInputListTagsPaginateTypeDef",
     "ListTrainingJobsForHyperParameterTuningJobRequestListTrainingJobsForHyperParameterTuningJobPaginateTypeDef",
     "ListTrainingJobsRequestListTrainingJobsPaginateTypeDef",
@@ -1179,129 +1139,102 @@
     "ListNotebookInstanceLifecycleConfigsOutputTypeDef",
     "ListNotebookInstancesOutputTypeDef",
     "ListPipelineExecutionsResponseTypeDef",
     "ListPipelineParametersForExecutionResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ListProcessingJobsResponseTypeDef",
     "ListProjectsOutputTypeDef",
+    "ListResourceCatalogsResponseTypeDef",
     "ListSpacesResponseTypeDef",
     "ListStudioLifecycleConfigsResponseTypeDef",
     "ListTransformJobsResponseTypeDef",
     "ListUserProfilesResponseTypeDef",
-    "MemberDefinitionOutputTypeDef",
     "MemberDefinitionTypeDef",
+    "MetricSpecificationTypeDef",
     "MonitoringAlertActionsTypeDef",
     "ModelDataSourceTypeDef",
     "ModelInfrastructureConfigTypeDef",
-    "ModelPackageContainerDefinitionOutputTypeDef",
     "ModelPackageContainerDefinitionTypeDef",
-    "RecommendationJobStoppingConditionsOutputTypeDef",
     "RecommendationJobStoppingConditionsTypeDef",
     "ModelMetadataSearchExpressionTypeDef",
     "ModelPackageStatusDetailsTypeDef",
     "MonitoringResourcesTypeDef",
-    "MonitoringDatasetFormatOutputTypeDef",
     "MonitoringDatasetFormatTypeDef",
     "MonitoringOutputTypeDef",
     "OfflineStoreConfigTypeDef",
     "OnlineStoreConfigTypeDef",
+    "OnlineStoreConfigUpdateTypeDef",
     "OutputConfigTypeDef",
     "PendingProductionVariantSummaryTypeDef",
     "ProductionVariantSummaryTypeDef",
-    "TrafficPatternOutputTypeDef",
-    "TrafficPatternTypeDef",
     "ProcessingResourcesTypeDef",
     "ProcessingOutputTypeDef",
     "ProductionVariantTypeDef",
-    "ProfilerRuleConfigurationUnionTypeDef",
     "SuggestionQueryTypeDef",
-    "ServiceCatalogProvisioningDetailsOutputTypeDef",
     "ServiceCatalogProvisioningDetailsTypeDef",
     "ServiceCatalogProvisioningUpdateDetailsTypeDef",
     "PublicWorkforceTaskPriceTypeDef",
     "QueryLineageResponseTypeDef",
     "RecommendationJobOutputConfigTypeDef",
-    "RecommendationJobContainerConfigOutputTypeDef",
     "RecommendationJobContainerConfigTypeDef",
     "RenderUiTemplateRequestRequestTypeDef",
     "RenderUiTemplateResponseTypeDef",
-    "SelectiveExecutionConfigOutputTypeDef",
+    "UpdateTrainingJobRequestRequestTypeDef",
     "SelectiveExecutionConfigTypeDef",
-    "ShadowModeConfigOutputTypeDef",
     "ShadowModeConfigTypeDef",
-    "SourceAlgorithmSpecificationOutputTypeDef",
     "SourceAlgorithmSpecificationTypeDef",
-    "SourceIpConfigUnionTypeDef",
+    "TrafficPatternTypeDef",
+    "TimeSeriesForecastingJobConfigTypeDef",
     "TrainingImageConfigTypeDef",
     "TransformDataSourceTypeDef",
     "WorkforceTypeDef",
     "ListActionsResponseTypeDef",
     "ArtifactSummaryTypeDef",
-    "ArtifactSourceUnionTypeDef",
     "CreateArtifactRequestRequestTypeDef",
     "DeleteArtifactRequestRequestTypeDef",
-    "AsyncInferenceConfigOutputTypeDef",
     "AsyncInferenceConfigTypeDef",
-    "TabularJobConfigOutputTypeDef",
     "TabularJobConfigTypeDef",
     "AutoMLChannelTypeDef",
     "AutoMLJobChannelTypeDef",
     "ListAutoMLJobsResponseTypeDef",
     "AutoMLResolvedAttributesTypeDef",
-    "AutoMLJobConfigOutputTypeDef",
-    "LabelingJobAlgorithmsConfigOutputTypeDef",
     "AutoMLJobConfigTypeDef",
-    "AutoMLSecurityConfigUnionTypeDef",
     "LabelingJobAlgorithmsConfigTypeDef",
-    "MonitoringNetworkConfigUnionTypeDef",
-    "NetworkConfigUnionTypeDef",
     "ModelMetricsTypeDef",
     "PipelineExecutionStepMetadataTypeDef",
     "AutoMLCandidateTypeDef",
     "BlueGreenUpdatePolicyTypeDef",
-    "InferenceExperimentDataStorageConfigUnionTypeDef",
-    "DataCaptureConfigUnionTypeDef",
-    "EndpointInputConfigurationOutputTypeDef",
     "EndpointInputConfigurationTypeDef",
-    "ClarifyExplainerConfigOutputTypeDef",
     "ClarifyExplainerConfigTypeDef",
     "ListCodeRepositoriesOutputTypeDef",
-    "DebugHookConfigUnionTypeDef",
     "ListContextsResponseTypeDef",
     "DomainSettingsForUpdateTypeDef",
-    "DomainSettingsOutputTypeDef",
     "DomainSettingsTypeDef",
-    "InferenceExperimentScheduleUnionTypeDef",
+    "InferenceExperimentSummaryTypeDef",
     "QueryLineageRequestRequestTypeDef",
-    "DefaultSpaceSettingsOutputTypeDef",
-    "SpaceSettingsOutputTypeDef",
     "DefaultSpaceSettingsTypeDef",
     "SpaceSettingsTypeDef",
-    "UserSettingsOutputTypeDef",
     "UserSettingsTypeDef",
-    "ChannelOutputTypeDef",
     "ChannelTypeDef",
     "ProcessingInputTypeDef",
-    "DescribeEdgeDeploymentPlanResponseTypeDef",
     "CreateEdgeDeploymentPlanRequestRequestTypeDef",
     "CreateEdgeDeploymentStageRequestRequestTypeDef",
+    "DescribeEdgeDeploymentPlanResponseTypeDef",
     "ListExperimentsResponseTypeDef",
     "ListFeatureGroupsResponseTypeDef",
-    "ListInferenceExperimentsResponseTypeDef",
     "ListTrainingJobsResponseTypeDef",
     "ListTrialsResponseTypeDef",
     "UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef",
     "ListDevicesResponseTypeDef",
     "DriftCheckBaselinesTypeDef",
     "InferenceRecommendationTypeDef",
     "RecommendationJobInferenceBenchmarkTypeDef",
     "SearchExpressionTypeDef",
     "ListTrainingJobsForHyperParameterTuningJobResponseTypeDef",
     "ListHyperParameterTuningJobsResponseTypeDef",
-    "HyperParameterTuningJobWarmStartConfigUnionTypeDef",
     "AssociationSummaryTypeDef",
     "DescribeActionResponseTypeDef",
     "DescribeArtifactResponseTypeDef",
     "DescribeContextResponseTypeDef",
     "DescribeExperimentResponseTypeDef",
     "DescribeLineageGroupResponseTypeDef",
     "DescribeModelCardResponseTypeDef",
@@ -1312,229 +1245,164 @@
     "ExperimentTypeDef",
     "ModelCardTypeDef",
     "ModelDashboardModelCardTypeDef",
     "ModelPackageGroupTypeDef",
     "PipelineTypeDef",
     "TrialComponentSimpleSummaryTypeDef",
     "TrialComponentSummaryTypeDef",
-    "ResourceConfigUnionTypeDef",
-    "HyperParameterSpecificationOutputTypeDef",
     "HyperParameterSpecificationTypeDef",
-    "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "AppImageConfigDetailsTypeDef",
-    "DescribeAppImageConfigResponseTypeDef",
     "CreateAppImageConfigRequestRequestTypeDef",
-    "KernelGatewayImageConfigUnionTypeDef",
+    "DescribeAppImageConfigResponseTypeDef",
     "UpdateAppImageConfigRequestRequestTypeDef",
     "ListLabelingJobsForWorkteamResponseTypeDef",
-    "LabelingJobInputConfigOutputTypeDef",
     "LabelingJobInputConfigTypeDef",
+    "CreateWorkteamRequestRequestTypeDef",
+    "UpdateWorkteamRequestRequestTypeDef",
     "WorkteamTypeDef",
-    "MemberDefinitionUnionTypeDef",
+    "TargetTrackingScalingPolicyConfigurationTypeDef",
     "MonitoringAlertSummaryTypeDef",
-    "ContainerDefinitionOutputTypeDef",
     "ContainerDefinitionTypeDef",
     "ModelVariantConfigSummaryTypeDef",
     "ModelVariantConfigTypeDef",
-    "AdditionalInferenceSpecificationDefinitionOutputTypeDef",
-    "InferenceSpecificationOutputTypeDef",
     "AdditionalInferenceSpecificationDefinitionTypeDef",
     "InferenceSpecificationTypeDef",
-    "RecommendationJobStoppingConditionsUnionTypeDef",
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
     "ListModelMetadataRequestRequestTypeDef",
-    "BatchTransformInputOutputTypeDef",
     "BatchTransformInputTypeDef",
-    "MonitoringOutputConfigOutputTypeDef",
     "MonitoringOutputConfigTypeDef",
     "CreateFeatureGroupRequestRequestTypeDef",
     "DescribeFeatureGroupResponseTypeDef",
     "FeatureGroupTypeDef",
+    "UpdateFeatureGroupRequestRequestTypeDef",
     "CreateCompilationJobRequestRequestTypeDef",
     "DescribeCompilationJobResponseTypeDef",
     "PendingDeploymentSummaryTypeDef",
-    "ProcessingOutputConfigOutputTypeDef",
     "ProcessingOutputConfigTypeDef",
-    "UpdateTrainingJobRequestRequestTypeDef",
     "GetSearchSuggestionsRequestRequestTypeDef",
+    "CreateProjectInputRequestTypeDef",
     "DescribeProjectOutputTypeDef",
     "ProjectTypeDef",
-    "CreateProjectInputRequestTypeDef",
-    "ServiceCatalogProvisioningDetailsUnionTypeDef",
     "UpdateProjectInputRequestTypeDef",
-    "HumanLoopConfigOutputTypeDef",
     "HumanLoopConfigTypeDef",
-    "HumanTaskConfigOutputTypeDef",
     "HumanTaskConfigTypeDef",
     "DescribePipelineExecutionResponseTypeDef",
     "PipelineExecutionTypeDef",
-    "SelectiveExecutionConfigUnionTypeDef",
     "StartPipelineExecutionRequestRequestTypeDef",
-    "ShadowModeConfigUnionTypeDef",
-    "SourceAlgorithmSpecificationUnionTypeDef",
-    "AlgorithmSpecificationOutputTypeDef",
     "AlgorithmSpecificationTypeDef",
     "TransformInputTypeDef",
     "DescribeWorkforceResponseTypeDef",
     "ListWorkforcesResponseTypeDef",
     "UpdateWorkforceResponseTypeDef",
     "ListArtifactsResponseTypeDef",
-    "AsyncInferenceConfigUnionTypeDef",
-    "AutoMLProblemTypeConfigOutputTypeDef",
     "AutoMLProblemTypeConfigTypeDef",
-    "AutoMLJobConfigUnionTypeDef",
     "CreateAutoMLJobRequestRequestTypeDef",
-    "LabelingJobAlgorithmsConfigUnionTypeDef",
     "PipelineExecutionStepTypeDef",
     "DescribeAutoMLJobResponseTypeDef",
     "ListCandidatesForAutoMLJobResponseTypeDef",
-    "DeploymentConfigOutputTypeDef",
     "DeploymentConfigTypeDef",
-    "RecommendationJobInputConfigOutputTypeDef",
     "RecommendationJobInputConfigTypeDef",
-    "ExplainerConfigOutputTypeDef",
     "ExplainerConfigTypeDef",
-    "DomainSettingsUnionTypeDef",
-    "DescribeSpaceResponseTypeDef",
-    "DefaultSpaceSettingsUnionTypeDef",
+    "ListInferenceExperimentsResponseTypeDef",
     "CreateSpaceRequestRequestTypeDef",
-    "SpaceSettingsUnionTypeDef",
+    "DescribeSpaceResponseTypeDef",
     "UpdateSpaceRequestRequestTypeDef",
-    "DescribeDomainResponseTypeDef",
-    "DescribeUserProfileResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "CreateUserProfileRequestRequestTypeDef",
+    "DescribeDomainResponseTypeDef",
+    "DescribeUserProfileResponseTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "UpdateUserProfileRequestRequestTypeDef",
-    "UserSettingsUnionTypeDef",
-    "HyperParameterTrainingJobDefinitionOutputTypeDef",
-    "TrainingJobDefinitionOutputTypeDef",
-    "ChannelUnionTypeDef",
     "HyperParameterTrainingJobDefinitionTypeDef",
     "TrainingJobDefinitionTypeDef",
     "InferenceRecommendationsJobStepTypeDef",
     "ListAssociationsResponseTypeDef",
     "TrialTypeDef",
     "ListTrialComponentsResponseTypeDef",
-    "TrainingSpecificationOutputTypeDef",
     "TrainingSpecificationTypeDef",
-    "HyperParameterTuningJobConfigUnionTypeDef",
     "ListAppImageConfigsResponseTypeDef",
     "LabelingJobSummaryTypeDef",
-    "LabelingJobInputConfigUnionTypeDef",
     "DescribeWorkteamResponseTypeDef",
     "ListWorkteamsResponseTypeDef",
     "UpdateWorkteamResponseTypeDef",
-    "CreateWorkteamRequestRequestTypeDef",
-    "UpdateWorkteamRequestRequestTypeDef",
+    "ScalingPolicyTypeDef",
     "ListMonitoringAlertsResponseTypeDef",
+    "CreateModelInputRequestTypeDef",
     "DescribeModelOutputTypeDef",
     "ModelTypeDef",
-    "ContainerDefinitionUnionTypeDef",
     "DescribeInferenceExperimentResponseTypeDef",
     "CreateInferenceExperimentRequestRequestTypeDef",
     "StopInferenceExperimentRequestRequestTypeDef",
     "UpdateInferenceExperimentRequestRequestTypeDef",
+    "UpdateModelPackageInputRequestTypeDef",
     "BatchDescribeModelPackageSummaryTypeDef",
-    "AdditionalInferenceSpecificationDefinitionUnionTypeDef",
-    "InferenceSpecificationUnionTypeDef",
-    "DataQualityJobInputOutputTypeDef",
-    "ModelBiasJobInputOutputTypeDef",
-    "ModelExplainabilityJobInputOutputTypeDef",
-    "ModelQualityJobInputOutputTypeDef",
-    "MonitoringInputOutputTypeDef",
     "DataQualityJobInputTypeDef",
     "ModelBiasJobInputTypeDef",
     "ModelExplainabilityJobInputTypeDef",
     "ModelQualityJobInputTypeDef",
     "MonitoringInputTypeDef",
-    "MonitoringOutputConfigUnionTypeDef",
+    "CreateProcessingJobRequestRequestTypeDef",
     "DescribeProcessingJobResponseTypeDef",
     "ProcessingJobTypeDef",
-    "CreateProcessingJobRequestRequestTypeDef",
-    "ProcessingOutputConfigUnionTypeDef",
-    "DescribeFlowDefinitionResponseTypeDef",
     "CreateFlowDefinitionRequestRequestTypeDef",
-    "HumanLoopConfigUnionTypeDef",
-    "DescribeLabelingJobResponseTypeDef",
+    "DescribeFlowDefinitionResponseTypeDef",
     "CreateLabelingJobRequestRequestTypeDef",
-    "HumanTaskConfigUnionTypeDef",
+    "DescribeLabelingJobResponseTypeDef",
+    "CreateTrainingJobRequestRequestTypeDef",
     "DescribeTrainingJobResponseTypeDef",
     "TrainingJobTypeDef",
-    "AlgorithmSpecificationUnionTypeDef",
     "CreateTransformJobRequestRequestTypeDef",
     "DescribeTransformJobResponseTypeDef",
-    "TransformJobDefinitionOutputTypeDef",
     "TransformJobDefinitionTypeDef",
     "TransformJobTypeDef",
-    "DescribeAutoMLJobV2ResponseTypeDef",
-    "AutoMLProblemTypeConfigUnionTypeDef",
     "CreateAutoMLJobV2RequestRequestTypeDef",
+    "DescribeAutoMLJobV2ResponseTypeDef",
     "ListPipelineExecutionStepsResponseTypeDef",
     "CreateEndpointInputRequestTypeDef",
-    "DeploymentConfigUnionTypeDef",
     "UpdateEndpointInputRequestTypeDef",
-    "DescribeInferenceRecommendationsJobResponseTypeDef",
     "CreateInferenceRecommendationsJobRequestRequestTypeDef",
-    "RecommendationJobInputConfigUnionTypeDef",
+    "DescribeInferenceRecommendationsJobResponseTypeDef",
+    "CreateEndpointConfigInputRequestTypeDef",
     "DescribeEndpointConfigOutputTypeDef",
     "DescribeEndpointOutputTypeDef",
-    "CreateEndpointConfigInputRequestTypeDef",
-    "ExplainerConfigUnionTypeDef",
+    "CreateHyperParameterTuningJobRequestRequestTypeDef",
     "DescribeHyperParameterTuningJobResponseTypeDef",
     "HyperParameterTuningJobSearchEntityTypeDef",
-    "CreateTrainingJobRequestRequestTypeDef",
-    "HyperParameterTrainingJobDefinitionUnionTypeDef",
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
-    "TrainingSpecificationUnionTypeDef",
     "ListLabelingJobsResponseTypeDef",
-    "CreateModelInputRequestTypeDef",
+    "DynamicScalingConfigurationTypeDef",
     "BatchDescribeModelPackageOutputTypeDef",
-    "UpdateModelPackageInputRequestTypeDef",
-    "DescribeDataQualityJobDefinitionResponseTypeDef",
-    "DescribeModelBiasJobDefinitionResponseTypeDef",
-    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
-    "DescribeModelQualityJobDefinitionResponseTypeDef",
-    "MonitoringJobDefinitionOutputTypeDef",
     "CreateDataQualityJobDefinitionRequestRequestTypeDef",
-    "DataQualityJobInputUnionTypeDef",
+    "DescribeDataQualityJobDefinitionResponseTypeDef",
     "CreateModelBiasJobDefinitionRequestRequestTypeDef",
-    "ModelBiasJobInputUnionTypeDef",
+    "DescribeModelBiasJobDefinitionResponseTypeDef",
     "CreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
-    "ModelExplainabilityJobInputUnionTypeDef",
+    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
     "CreateModelQualityJobDefinitionRequestRequestTypeDef",
-    "ModelQualityJobInputUnionTypeDef",
+    "DescribeModelQualityJobDefinitionResponseTypeDef",
     "MonitoringJobDefinitionTypeDef",
-    "AlgorithmValidationProfileOutputTypeDef",
-    "ModelPackageValidationProfileOutputTypeDef",
     "AlgorithmValidationProfileTypeDef",
     "ModelPackageValidationProfileTypeDef",
     "TrialComponentSourceDetailTypeDef",
-    "CreateHyperParameterTuningJobRequestRequestTypeDef",
-    "MonitoringScheduleConfigOutputTypeDef",
+    "GetScalingConfigurationRecommendationResponseTypeDef",
     "MonitoringScheduleConfigTypeDef",
-    "AlgorithmValidationSpecificationOutputTypeDef",
-    "ModelPackageValidationSpecificationOutputTypeDef",
     "AlgorithmValidationSpecificationTypeDef",
     "ModelPackageValidationSpecificationTypeDef",
     "TrialComponentTypeDef",
+    "CreateMonitoringScheduleRequestRequestTypeDef",
     "DescribeMonitoringScheduleResponseTypeDef",
     "ModelDashboardMonitoringScheduleTypeDef",
     "MonitoringScheduleTypeDef",
-    "CreateMonitoringScheduleRequestRequestTypeDef",
-    "MonitoringScheduleConfigUnionTypeDef",
     "UpdateMonitoringScheduleRequestRequestTypeDef",
+    "CreateAlgorithmInputRequestTypeDef",
     "DescribeAlgorithmOutputTypeDef",
+    "CreateModelPackageInputRequestTypeDef",
     "DescribeModelPackageOutputTypeDef",
     "ModelPackageTypeDef",
-    "AlgorithmValidationSpecificationUnionTypeDef",
-    "CreateAlgorithmInputRequestTypeDef",
-    "CreateModelPackageInputRequestTypeDef",
-    "ModelPackageValidationSpecificationUnionTypeDef",
     "ModelDashboardModelTypeDef",
     "EndpointTypeDef",
     "SearchRecordTypeDef",
     "SearchResponseTypeDef",
 )
 
 _RequiredActionSourceTypeDef = TypedDict(
@@ -1675,34 +1543,14 @@
         "Status": AppStatusType,
         "CreationTime": datetime,
         "SpaceName": str,
     },
     total=False,
 )
 
-_RequiredAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-    },
-)
-_OptionalAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalAppSpecificationOutputTypeDef",
-    {
-        "ContainerEntrypoint": List[str],
-        "ContainerArguments": List[str],
-    },
-    total=False,
-)
-
-class AppSpecificationOutputTypeDef(
-    _RequiredAppSpecificationOutputTypeDef, _OptionalAppSpecificationOutputTypeDef
-):
-    pass
-
 _RequiredAppSpecificationTypeDef = TypedDict(
     "_RequiredAppSpecificationTypeDef",
     {
         "ImageUri": str,
     },
 )
 _OptionalAppSpecificationTypeDef = TypedDict(
@@ -1737,24 +1585,14 @@
     "AsyncInferenceClientConfigTypeDef",
     {
         "MaxConcurrentInvocationsPerInstance": int,
     },
     total=False,
 )
 
-AsyncInferenceNotificationConfigOutputTypeDef = TypedDict(
-    "AsyncInferenceNotificationConfigOutputTypeDef",
-    {
-        "SuccessTopic": str,
-        "ErrorTopic": str,
-        "IncludeInferenceResponseIn": List[AsyncNotificationTopicTypesType],
-    },
-    total=False,
-)
-
 AsyncInferenceNotificationConfigTypeDef = TypedDict(
     "AsyncInferenceNotificationConfigTypeDef",
     {
         "SuccessTopic": str,
         "ErrorTopic": str,
         "IncludeInferenceResponseIn": Sequence[AsyncNotificationTopicTypesType],
     },
@@ -1782,21 +1620,14 @@
 )
 
 class AthenaDatasetDefinitionTypeDef(
     _RequiredAthenaDatasetDefinitionTypeDef, _OptionalAthenaDatasetDefinitionTypeDef
 ):
     pass
 
-AutoMLAlgorithmConfigOutputTypeDef = TypedDict(
-    "AutoMLAlgorithmConfigOutputTypeDef",
-    {
-        "AutoMLAlgorithms": List[AutoMLAlgorithmType],
-    },
-)
-
 AutoMLAlgorithmConfigTypeDef = TypedDict(
     "AutoMLAlgorithmConfigTypeDef",
     {
         "AutoMLAlgorithms": Sequence[AutoMLAlgorithmType],
     },
 )
 
@@ -1931,22 +1762,14 @@
     "TabularResolvedAttributesTypeDef",
     {
         "ProblemType": ProblemTypeType,
     },
     total=False,
 )
 
-VpcConfigOutputTypeDef = TypedDict(
-    "VpcConfigOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "Subnets": List[str],
-    },
-)
-
 VpcConfigTypeDef = TypedDict(
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
@@ -2049,14 +1872,15 @@
         "Explainability": str,
     },
 )
 _OptionalCandidateArtifactLocationsTypeDef = TypedDict(
     "_OptionalCandidateArtifactLocationsTypeDef",
     {
         "ModelInsights": str,
+        "BacktestResults": str,
     },
     total=False,
 )
 
 class CandidateArtifactLocationsTypeDef(
     _RequiredCandidateArtifactLocationsTypeDef, _OptionalCandidateArtifactLocationsTypeDef
 ):
@@ -2087,29 +1911,29 @@
     {
         "Status": FeatureStatusType,
         "AmazonForecastRoleArn": str,
     },
     total=False,
 )
 
-CapacitySizeTypeDef = TypedDict(
-    "CapacitySizeTypeDef",
+WorkspaceSettingsTypeDef = TypedDict(
+    "WorkspaceSettingsTypeDef",
     {
-        "Type": CapacitySizeTypeType,
-        "Value": int,
+        "S3ArtifactPath": str,
+        "S3KmsKeyId": str,
     },
+    total=False,
 )
 
-CaptureContentTypeHeaderOutputTypeDef = TypedDict(
-    "CaptureContentTypeHeaderOutputTypeDef",
+CapacitySizeTypeDef = TypedDict(
+    "CapacitySizeTypeDef",
     {
-        "CsvContentTypes": List[str],
-        "JsonContentTypes": List[str],
+        "Type": CapacitySizeTypeType,
+        "Value": int,
     },
-    total=False,
 )
 
 CaptureContentTypeHeaderTypeDef = TypedDict(
     "CaptureContentTypeHeaderTypeDef",
     {
         "CsvContentTypes": Sequence[str],
         "JsonContentTypes": Sequence[str],
@@ -2120,37 +1944,14 @@
 CaptureOptionTypeDef = TypedDict(
     "CaptureOptionTypeDef",
     {
         "CaptureMode": CaptureModeType,
     },
 )
 
-CategoricalParameterOutputTypeDef = TypedDict(
-    "CategoricalParameterOutputTypeDef",
-    {
-        "Name": str,
-        "Value": List[str],
-    },
-)
-
-CategoricalParameterRangeOutputTypeDef = TypedDict(
-    "CategoricalParameterRangeOutputTypeDef",
-    {
-        "Name": str,
-        "Values": List[str],
-    },
-)
-
-CategoricalParameterRangeSpecificationOutputTypeDef = TypedDict(
-    "CategoricalParameterRangeSpecificationOutputTypeDef",
-    {
-        "Values": List[str],
-    },
-)
-
 CategoricalParameterRangeSpecificationTypeDef = TypedDict(
     "CategoricalParameterRangeSpecificationTypeDef",
     {
         "Values": Sequence[str],
     },
 )
 
@@ -2166,44 +1967,14 @@
     "CategoricalParameterTypeDef",
     {
         "Name": str,
         "Value": Sequence[str],
     },
 )
 
-ShuffleConfigTypeDef = TypedDict(
-    "ShuffleConfigTypeDef",
-    {
-        "Seed": int,
-    },
-)
-
-_RequiredChannelSpecificationOutputTypeDef = TypedDict(
-    "_RequiredChannelSpecificationOutputTypeDef",
-    {
-        "Name": str,
-        "SupportedContentTypes": List[str],
-        "SupportedInputModes": List[TrainingInputModeType],
-    },
-)
-_OptionalChannelSpecificationOutputTypeDef = TypedDict(
-    "_OptionalChannelSpecificationOutputTypeDef",
-    {
-        "Description": str,
-        "IsRequired": bool,
-        "SupportedCompressionTypes": List[CompressionTypeType],
-    },
-    total=False,
-)
-
-class ChannelSpecificationOutputTypeDef(
-    _RequiredChannelSpecificationOutputTypeDef, _OptionalChannelSpecificationOutputTypeDef
-):
-    pass
-
 _RequiredChannelSpecificationTypeDef = TypedDict(
     "_RequiredChannelSpecificationTypeDef",
     {
         "Name": str,
         "SupportedContentTypes": Sequence[str],
         "SupportedInputModes": Sequence[TrainingInputModeType],
     },
@@ -2219,14 +1990,21 @@
 )
 
 class ChannelSpecificationTypeDef(
     _RequiredChannelSpecificationTypeDef, _OptionalChannelSpecificationTypeDef
 ):
     pass
 
+ShuffleConfigTypeDef = TypedDict(
+    "ShuffleConfigTypeDef",
+    {
+        "Seed": int,
+    },
+)
+
 _RequiredCheckpointConfigTypeDef = TypedDict(
     "_RequiredCheckpointConfigTypeDef",
     {
         "S3Uri": str,
     },
 )
 _OptionalCheckpointConfigTypeDef = TypedDict(
@@ -2251,32 +2029,14 @@
         "CheckJobArn": str,
         "SkipCheck": bool,
         "RegisterNewBaseline": bool,
     },
     total=False,
 )
 
-ClarifyInferenceConfigOutputTypeDef = TypedDict(
-    "ClarifyInferenceConfigOutputTypeDef",
-    {
-        "FeaturesAttribute": str,
-        "ContentTemplate": str,
-        "MaxRecordCount": int,
-        "MaxPayloadInMB": int,
-        "ProbabilityIndex": int,
-        "LabelIndex": int,
-        "ProbabilityAttribute": str,
-        "LabelAttribute": str,
-        "LabelHeaders": List[str],
-        "FeatureHeaders": List[str],
-        "FeatureTypes": List[ClarifyFeatureTypeType],
-    },
-    total=False,
-)
-
 ClarifyInferenceConfigTypeDef = TypedDict(
     "ClarifyInferenceConfigTypeDef",
     {
         "FeaturesAttribute": str,
         "ContentTemplate": str,
         "MaxRecordCount": int,
         "MaxPayloadInMB": int,
@@ -2347,23 +2107,14 @@
     {
         "UserPool": str,
         "UserGroup": str,
         "ClientId": str,
     },
 )
 
-CollectionConfigurationOutputTypeDef = TypedDict(
-    "CollectionConfigurationOutputTypeDef",
-    {
-        "CollectionName": str,
-        "CollectionParameters": Dict[str, str],
-    },
-    total=False,
-)
-
 CollectionConfigurationTypeDef = TypedDict(
     "CollectionConfigurationTypeDef",
     {
         "CollectionName": str,
         "CollectionParameters": Mapping[str, str],
     },
     total=False,
@@ -2886,14 +2637,38 @@
 ProcessingStoppingConditionTypeDef = TypedDict(
     "ProcessingStoppingConditionTypeDef",
     {
         "MaxRuntimeInSeconds": int,
     },
 )
 
+_RequiredDebugRuleConfigurationTypeDef = TypedDict(
+    "_RequiredDebugRuleConfigurationTypeDef",
+    {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+    },
+)
+_OptionalDebugRuleConfigurationTypeDef = TypedDict(
+    "_OptionalDebugRuleConfigurationTypeDef",
+    {
+        "LocalPath": str,
+        "S3OutputPath": str,
+        "InstanceType": ProcessingInstanceTypeType,
+        "VolumeSizeInGB": int,
+        "RuleParameters": Mapping[str, str],
+    },
+    total=False,
+)
+
+class DebugRuleConfigurationTypeDef(
+    _RequiredDebugRuleConfigurationTypeDef, _OptionalDebugRuleConfigurationTypeDef
+):
+    pass
+
 _RequiredOutputDataConfigTypeDef = TypedDict(
     "_RequiredOutputDataConfigTypeDef",
     {
         "S3OutputPath": str,
     },
 )
 _OptionalOutputDataConfigTypeDef = TypedDict(
@@ -2915,14 +2690,38 @@
         "ProfilingIntervalInMilliseconds": int,
         "ProfilingParameters": Mapping[str, str],
         "DisableProfiler": bool,
     },
     total=False,
 )
 
+_RequiredProfilerRuleConfigurationTypeDef = TypedDict(
+    "_RequiredProfilerRuleConfigurationTypeDef",
+    {
+        "RuleConfigurationName": str,
+        "RuleEvaluatorImage": str,
+    },
+)
+_OptionalProfilerRuleConfigurationTypeDef = TypedDict(
+    "_OptionalProfilerRuleConfigurationTypeDef",
+    {
+        "LocalPath": str,
+        "S3OutputPath": str,
+        "InstanceType": ProcessingInstanceTypeType,
+        "VolumeSizeInGB": int,
+        "RuleParameters": Mapping[str, str],
+    },
+    total=False,
+)
+
+class ProfilerRuleConfigurationTypeDef(
+    _RequiredProfilerRuleConfigurationTypeDef, _OptionalProfilerRuleConfigurationTypeDef
+):
+    pass
+
 RetryStrategyTypeDef = TypedDict(
     "RetryStrategyTypeDef",
     {
         "MaximumRetryAttempts": int,
     },
 )
 
@@ -3094,14 +2893,24 @@
     },
     total=False,
 )
 
 class CustomImageTypeDef(_RequiredCustomImageTypeDef, _OptionalCustomImageTypeDef):
     pass
 
+CustomizedMetricSpecificationTypeDef = TypedDict(
+    "CustomizedMetricSpecificationTypeDef",
+    {
+        "MetricName": str,
+        "Namespace": str,
+        "Statistic": StatisticType,
+    },
+    total=False,
+)
+
 DataCaptureConfigSummaryTypeDef = TypedDict(
     "DataCaptureConfigSummaryTypeDef",
     {
         "EnableCapture": bool,
         "CaptureStatus": CaptureStatusType,
         "CurrentSamplingPercentage": int,
         "DestinationS3Uri": str,
@@ -3114,38 +2923,14 @@
     {
         "TableName": str,
         "Catalog": str,
         "Database": str,
     },
 )
 
-_RequiredDataQualityAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredDataQualityAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-    },
-)
-_OptionalDataQualityAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalDataQualityAppSpecificationOutputTypeDef",
-    {
-        "ContainerEntrypoint": List[str],
-        "ContainerArguments": List[str],
-        "RecordPreprocessorSourceUri": str,
-        "PostAnalyticsProcessorSourceUri": str,
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-class DataQualityAppSpecificationOutputTypeDef(
-    _RequiredDataQualityAppSpecificationOutputTypeDef,
-    _OptionalDataQualityAppSpecificationOutputTypeDef,
-):
-    pass
-
 MonitoringConstraintsResourceTypeDef = TypedDict(
     "MonitoringConstraintsResourceTypeDef",
     {
         "S3Uri": str,
     },
     total=False,
 )
@@ -3189,36 +2974,14 @@
         "FileSystemId": str,
         "FileSystemAccessMode": FileSystemAccessModeType,
         "FileSystemType": FileSystemTypeType,
         "DirectoryPath": str,
     },
 )
 
-_RequiredS3DataSourceOutputTypeDef = TypedDict(
-    "_RequiredS3DataSourceOutputTypeDef",
-    {
-        "S3DataType": S3DataTypeType,
-        "S3Uri": str,
-    },
-)
-_OptionalS3DataSourceOutputTypeDef = TypedDict(
-    "_OptionalS3DataSourceOutputTypeDef",
-    {
-        "S3DataDistributionType": S3DataDistributionType,
-        "AttributeNames": List[str],
-        "InstanceGroupNames": List[str],
-    },
-    total=False,
-)
-
-class S3DataSourceOutputTypeDef(
-    _RequiredS3DataSourceOutputTypeDef, _OptionalS3DataSourceOutputTypeDef
-):
-    pass
-
 _RequiredS3DataSourceTypeDef = TypedDict(
     "_RequiredS3DataSourceTypeDef",
     {
         "S3DataType": S3DataTypeType,
         "S3Uri": str,
     },
 )
@@ -3257,62 +3020,14 @@
 )
 
 class RedshiftDatasetDefinitionTypeDef(
     _RequiredRedshiftDatasetDefinitionTypeDef, _OptionalRedshiftDatasetDefinitionTypeDef
 ):
     pass
 
-_RequiredDebugRuleConfigurationOutputTypeDef = TypedDict(
-    "_RequiredDebugRuleConfigurationOutputTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-    },
-)
-_OptionalDebugRuleConfigurationOutputTypeDef = TypedDict(
-    "_OptionalDebugRuleConfigurationOutputTypeDef",
-    {
-        "LocalPath": str,
-        "S3OutputPath": str,
-        "InstanceType": ProcessingInstanceTypeType,
-        "VolumeSizeInGB": int,
-        "RuleParameters": Dict[str, str],
-    },
-    total=False,
-)
-
-class DebugRuleConfigurationOutputTypeDef(
-    _RequiredDebugRuleConfigurationOutputTypeDef, _OptionalDebugRuleConfigurationOutputTypeDef
-):
-    pass
-
-_RequiredDebugRuleConfigurationTypeDef = TypedDict(
-    "_RequiredDebugRuleConfigurationTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-    },
-)
-_OptionalDebugRuleConfigurationTypeDef = TypedDict(
-    "_OptionalDebugRuleConfigurationTypeDef",
-    {
-        "LocalPath": str,
-        "S3OutputPath": str,
-        "InstanceType": ProcessingInstanceTypeType,
-        "VolumeSizeInGB": int,
-        "RuleParameters": Mapping[str, str],
-    },
-    total=False,
-)
-
-class DebugRuleConfigurationTypeDef(
-    _RequiredDebugRuleConfigurationTypeDef, _OptionalDebugRuleConfigurationTypeDef
-):
-    pass
-
 DebugRuleEvaluationStatusTypeDef = TypedDict(
     "DebugRuleEvaluationStatusTypeDef",
     {
         "RuleConfigurationName": str,
         "RuleEvaluationJobArn": str,
         "RuleEvaluationStatus": RuleEvaluationStatusType,
         "StatusDetails": str,
@@ -3694,32 +3409,32 @@
 )
 
 class RealTimeInferenceRecommendationTypeDef(
     _RequiredRealTimeInferenceRecommendationTypeDef, _OptionalRealTimeInferenceRecommendationTypeDef
 ):
     pass
 
-_RequiredDeviceSelectionConfigOutputTypeDef = TypedDict(
-    "_RequiredDeviceSelectionConfigOutputTypeDef",
+_RequiredDeviceSelectionConfigTypeDef = TypedDict(
+    "_RequiredDeviceSelectionConfigTypeDef",
     {
         "DeviceSubsetType": DeviceSubsetTypeType,
     },
 )
-_OptionalDeviceSelectionConfigOutputTypeDef = TypedDict(
-    "_OptionalDeviceSelectionConfigOutputTypeDef",
+_OptionalDeviceSelectionConfigTypeDef = TypedDict(
+    "_OptionalDeviceSelectionConfigTypeDef",
     {
         "Percentage": int,
-        "DeviceNames": List[str],
+        "DeviceNames": Sequence[str],
         "DeviceNameContains": str,
     },
     total=False,
 )
 
-class DeviceSelectionConfigOutputTypeDef(
-    _RequiredDeviceSelectionConfigOutputTypeDef, _OptionalDeviceSelectionConfigOutputTypeDef
+class DeviceSelectionConfigTypeDef(
+    _RequiredDeviceSelectionConfigTypeDef, _OptionalDeviceSelectionConfigTypeDef
 ):
     pass
 
 EdgeDeploymentConfigTypeDef = TypedDict(
     "EdgeDeploymentConfigTypeDef",
     {
         "FailureHandlingPolicy": FailureHandlingPolicyType,
@@ -3745,35 +3460,14 @@
 )
 
 class EdgeDeploymentStatusTypeDef(
     _RequiredEdgeDeploymentStatusTypeDef, _OptionalEdgeDeploymentStatusTypeDef
 ):
     pass
 
-_RequiredDeviceSelectionConfigTypeDef = TypedDict(
-    "_RequiredDeviceSelectionConfigTypeDef",
-    {
-        "DeviceSubsetType": DeviceSubsetTypeType,
-    },
-)
-_OptionalDeviceSelectionConfigTypeDef = TypedDict(
-    "_OptionalDeviceSelectionConfigTypeDef",
-    {
-        "Percentage": int,
-        "DeviceNames": Sequence[str],
-        "DeviceNameContains": str,
-    },
-    total=False,
-)
-
-class DeviceSelectionConfigTypeDef(
-    _RequiredDeviceSelectionConfigTypeDef, _OptionalDeviceSelectionConfigTypeDef
-):
-    pass
-
 DeregisterDevicesRequestRequestTypeDef = TypedDict(
     "DeregisterDevicesRequestRequestTypeDef",
     {
         "DeviceFleetName": str,
         "DeviceNames": Sequence[str],
     },
 )
@@ -3875,22 +3569,14 @@
     "ModelDigestsTypeDef",
     {
         "ArtifactDigest": str,
     },
     total=False,
 )
 
-NeoVpcConfigOutputTypeDef = TypedDict(
-    "NeoVpcConfigOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "Subnets": List[str],
-    },
-)
-
 DescribeContextRequestRequestTypeDef = TypedDict(
     "DescribeContextRequestRequestTypeDef",
     {
         "ContextName": str,
     },
 )
 
@@ -4280,23 +3966,14 @@
     },
     total=False,
 )
 
 class EndpointMetadataTypeDef(_RequiredEndpointMetadataTypeDef, _OptionalEndpointMetadataTypeDef):
     pass
 
-InferenceExperimentScheduleOutputTypeDef = TypedDict(
-    "InferenceExperimentScheduleOutputTypeDef",
-    {
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
-
 DescribeInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
     "DescribeInferenceRecommendationsJobRequestRequestTypeDef",
     {
         "JobName": str,
     },
 )
 
@@ -4348,34 +4025,14 @@
 DescribeModelBiasJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelBiasJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
 
-_RequiredModelBiasAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredModelBiasAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-        "ConfigUri": str,
-    },
-)
-_OptionalModelBiasAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalModelBiasAppSpecificationOutputTypeDef",
-    {
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-class ModelBiasAppSpecificationOutputTypeDef(
-    _RequiredModelBiasAppSpecificationOutputTypeDef, _OptionalModelBiasAppSpecificationOutputTypeDef
-):
-    pass
-
 DescribeModelCardExportJobRequestRequestTypeDef = TypedDict(
     "DescribeModelCardExportJobRequestRequestTypeDef",
     {
         "ModelCardExportJobArn": str,
     },
 )
 
@@ -4408,35 +4065,14 @@
 DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
 
-_RequiredModelExplainabilityAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredModelExplainabilityAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-        "ConfigUri": str,
-    },
-)
-_OptionalModelExplainabilityAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalModelExplainabilityAppSpecificationOutputTypeDef",
-    {
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-class ModelExplainabilityAppSpecificationOutputTypeDef(
-    _RequiredModelExplainabilityAppSpecificationOutputTypeDef,
-    _OptionalModelExplainabilityAppSpecificationOutputTypeDef,
-):
-    pass
-
 DescribeModelInputRequestTypeDef = TypedDict(
     "DescribeModelInputRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
@@ -4457,39 +4093,14 @@
 DescribeModelQualityJobDefinitionRequestRequestTypeDef = TypedDict(
     "DescribeModelQualityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
     },
 )
 
-_RequiredModelQualityAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredModelQualityAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-    },
-)
-_OptionalModelQualityAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalModelQualityAppSpecificationOutputTypeDef",
-    {
-        "ContainerEntrypoint": List[str],
-        "ContainerArguments": List[str],
-        "RecordPreprocessorSourceUri": str,
-        "PostAnalyticsProcessorSourceUri": str,
-        "ProblemType": MonitoringProblemTypeType,
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-class ModelQualityAppSpecificationOutputTypeDef(
-    _RequiredModelQualityAppSpecificationOutputTypeDef,
-    _OptionalModelQualityAppSpecificationOutputTypeDef,
-):
-    pass
-
 DescribeMonitoringScheduleRequestRequestTypeDef = TypedDict(
     "DescribeMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
     },
 )
 
@@ -4644,49 +4255,14 @@
         "MetricName": str,
         "Value": float,
         "Timestamp": datetime,
     },
     total=False,
 )
 
-ProfilerConfigOutputTypeDef = TypedDict(
-    "ProfilerConfigOutputTypeDef",
-    {
-        "S3OutputPath": str,
-        "ProfilingIntervalInMilliseconds": int,
-        "ProfilingParameters": Dict[str, str],
-        "DisableProfiler": bool,
-    },
-    total=False,
-)
-
-_RequiredProfilerRuleConfigurationOutputTypeDef = TypedDict(
-    "_RequiredProfilerRuleConfigurationOutputTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-    },
-)
-_OptionalProfilerRuleConfigurationOutputTypeDef = TypedDict(
-    "_OptionalProfilerRuleConfigurationOutputTypeDef",
-    {
-        "LocalPath": str,
-        "S3OutputPath": str,
-        "InstanceType": ProcessingInstanceTypeType,
-        "VolumeSizeInGB": int,
-        "RuleParameters": Dict[str, str],
-    },
-    total=False,
-)
-
-class ProfilerRuleConfigurationOutputTypeDef(
-    _RequiredProfilerRuleConfigurationOutputTypeDef, _OptionalProfilerRuleConfigurationOutputTypeDef
-):
-    pass
-
 ProfilerRuleEvaluationStatusTypeDef = TypedDict(
     "ProfilerRuleEvaluationStatusTypeDef",
     {
         "RuleConfigurationName": str,
         "RuleEvaluationJobArn": str,
         "RuleEvaluationStatus": RuleEvaluationStatusType,
         "StatusDetails": str,
@@ -5056,23 +4632,34 @@
 EndpointInfoTypeDef = TypedDict(
     "EndpointInfoTypeDef",
     {
         "EndpointName": str,
     },
 )
 
-EndpointOutputConfigurationTypeDef = TypedDict(
-    "EndpointOutputConfigurationTypeDef",
+_RequiredProductionVariantServerlessConfigTypeDef = TypedDict(
+    "_RequiredProductionVariantServerlessConfigTypeDef",
     {
-        "EndpointName": str,
-        "VariantName": str,
-        "InstanceType": ProductionVariantInstanceTypeType,
-        "InitialInstanceCount": int,
+        "MemorySizeInMB": int,
+        "MaxConcurrency": int,
     },
 )
+_OptionalProductionVariantServerlessConfigTypeDef = TypedDict(
+    "_OptionalProductionVariantServerlessConfigTypeDef",
+    {
+        "ProvisionedConcurrency": int,
+    },
+    total=False,
+)
+
+class ProductionVariantServerlessConfigTypeDef(
+    _RequiredProductionVariantServerlessConfigTypeDef,
+    _OptionalProductionVariantServerlessConfigTypeDef,
+):
+    pass
 
 InferenceMetricsTypeDef = TypedDict(
     "InferenceMetricsTypeDef",
     {
         "MaxInvocations": int,
         "ModelLatency": int,
     },
@@ -5194,14 +4781,32 @@
 GetModelPackageGroupPolicyInputRequestTypeDef = TypedDict(
     "GetModelPackageGroupPolicyInputRequestTypeDef",
     {
         "ModelPackageGroupName": str,
     },
 )
 
+ScalingPolicyObjectiveTypeDef = TypedDict(
+    "ScalingPolicyObjectiveTypeDef",
+    {
+        "MinInvocationsPerMinute": int,
+        "MaxInvocationsPerMinute": int,
+    },
+    total=False,
+)
+
+ScalingPolicyMetricTypeDef = TypedDict(
+    "ScalingPolicyMetricTypeDef",
+    {
+        "InvocationsPerInstance": int,
+        "ModelLatency": int,
+    },
+    total=False,
+)
+
 PropertyNameSuggestionTypeDef = TypedDict(
     "PropertyNameSuggestionTypeDef",
     {
         "PropertyName": str,
     },
     total=False,
 )
@@ -5411,14 +5016,15 @@
     },
 )
 _OptionalRecommendationMetricsTypeDef = TypedDict(
     "_OptionalRecommendationMetricsTypeDef",
     {
         "CpuUtilization": float,
         "MemoryUtilization": float,
+        "ModelSetupTime": int,
     },
     total=False,
 )
 
 class RecommendationMetricsTypeDef(
     _RequiredRecommendationMetricsTypeDef, _OptionalRecommendationMetricsTypeDef
 ):
@@ -5515,22 +5121,14 @@
         "HumanLabeled": int,
         "PendingHuman": int,
         "Total": int,
     },
     total=False,
 )
 
-LabelingJobDataAttributesOutputTypeDef = TypedDict(
-    "LabelingJobDataAttributesOutputTypeDef",
-    {
-        "ContentClassifiers": List[ContentClassifierType],
-    },
-    total=False,
-)
-
 LabelingJobDataAttributesTypeDef = TypedDict(
     "LabelingJobDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
     total=False,
 )
@@ -6012,14 +5610,24 @@
     },
     total=False,
 )
 
 class ProjectSummaryTypeDef(_RequiredProjectSummaryTypeDef, _OptionalProjectSummaryTypeDef):
     pass
 
+ResourceCatalogTypeDef = TypedDict(
+    "ResourceCatalogTypeDef",
+    {
+        "ResourceCatalogArn": str,
+        "ResourceCatalogName": str,
+        "Description": str,
+        "CreationTime": datetime,
+    },
+)
+
 ListSpacesRequestRequestTypeDef = TypedDict(
     "ListSpacesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "SortOrder": SortOrderType,
         "SortBy": SpaceSortKeyType,
@@ -6198,26 +5806,27 @@
         "NameContains": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-OidcMemberDefinitionOutputTypeDef = TypedDict(
-    "OidcMemberDefinitionOutputTypeDef",
+OidcMemberDefinitionTypeDef = TypedDict(
+    "OidcMemberDefinitionTypeDef",
     {
-        "Groups": List[str],
+        "Groups": Sequence[str],
     },
 )
 
-OidcMemberDefinitionTypeDef = TypedDict(
-    "OidcMemberDefinitionTypeDef",
+PredefinedMetricSpecificationTypeDef = TypedDict(
+    "PredefinedMetricSpecificationTypeDef",
     {
-        "Groups": Sequence[str],
+        "PredefinedMetricType": str,
     },
+    total=False,
 )
 
 MonitoringGroundTruthS3InputTypeDef = TypedDict(
     "MonitoringGroundTruthS3InputTypeDef",
     {
         "S3Uri": str,
     },
@@ -6308,37 +5917,14 @@
     "ModelStepMetadataTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-_RequiredMonitoringAppSpecificationOutputTypeDef = TypedDict(
-    "_RequiredMonitoringAppSpecificationOutputTypeDef",
-    {
-        "ImageUri": str,
-    },
-)
-_OptionalMonitoringAppSpecificationOutputTypeDef = TypedDict(
-    "_OptionalMonitoringAppSpecificationOutputTypeDef",
-    {
-        "ContainerEntrypoint": List[str],
-        "ContainerArguments": List[str],
-        "RecordPreprocessorSourceUri": str,
-        "PostAnalyticsProcessorSourceUri": str,
-    },
-    total=False,
-)
-
-class MonitoringAppSpecificationOutputTypeDef(
-    _RequiredMonitoringAppSpecificationOutputTypeDef,
-    _OptionalMonitoringAppSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredMonitoringAppSpecificationTypeDef = TypedDict(
     "_RequiredMonitoringAppSpecificationTypeDef",
     {
         "ImageUri": str,
     },
 )
 _OptionalMonitoringAppSpecificationTypeDef = TypedDict(
@@ -6457,14 +6043,23 @@
     "OnlineStoreSecurityConfigTypeDef",
     {
         "KmsKeyId": str,
     },
     total=False,
 )
 
+TtlDurationTypeDef = TypedDict(
+    "TtlDurationTypeDef",
+    {
+        "Unit": TtlDurationUnitType,
+        "Value": int,
+    },
+    total=False,
+)
+
 _RequiredTargetPlatformTypeDef = TypedDict(
     "_RequiredTargetPlatformTypeDef",
     {
         "Os": TargetPlatformOsType,
         "Arch": TargetPlatformArchType,
     },
 )
@@ -6484,35 +6079,14 @@
     {
         "TrialName": str,
         "ExperimentName": str,
     },
     total=False,
 )
 
-_RequiredProductionVariantServerlessConfigTypeDef = TypedDict(
-    "_RequiredProductionVariantServerlessConfigTypeDef",
-    {
-        "MemorySizeInMB": int,
-        "MaxConcurrency": int,
-    },
-)
-_OptionalProductionVariantServerlessConfigTypeDef = TypedDict(
-    "_OptionalProductionVariantServerlessConfigTypeDef",
-    {
-        "ProvisionedConcurrency": int,
-    },
-    total=False,
-)
-
-class ProductionVariantServerlessConfigTypeDef(
-    _RequiredProductionVariantServerlessConfigTypeDef,
-    _OptionalProductionVariantServerlessConfigTypeDef,
-):
-    pass
-
 _RequiredProductionVariantStatusTypeDef = TypedDict(
     "_RequiredProductionVariantStatusTypeDef",
     {
         "Status": VariantStatusType,
     },
 )
 _OptionalProductionVariantStatusTypeDef = TypedDict(
@@ -6690,38 +6264,14 @@
         "ProfilingIntervalInMilliseconds": int,
         "ProfilingParameters": Mapping[str, str],
         "DisableProfiler": bool,
     },
     total=False,
 )
 
-_RequiredProfilerRuleConfigurationTypeDef = TypedDict(
-    "_RequiredProfilerRuleConfigurationTypeDef",
-    {
-        "RuleConfigurationName": str,
-        "RuleEvaluatorImage": str,
-    },
-)
-_OptionalProfilerRuleConfigurationTypeDef = TypedDict(
-    "_OptionalProfilerRuleConfigurationTypeDef",
-    {
-        "LocalPath": str,
-        "S3OutputPath": str,
-        "InstanceType": ProcessingInstanceTypeType,
-        "VolumeSizeInGB": int,
-        "RuleParameters": Mapping[str, str],
-    },
-    total=False,
-)
-
-class ProfilerRuleConfigurationTypeDef(
-    _RequiredProfilerRuleConfigurationTypeDef, _OptionalProfilerRuleConfigurationTypeDef
-):
-    pass
-
 PropertyNameQueryTypeDef = TypedDict(
     "PropertyNameQueryTypeDef",
     {
         "PropertyNameHint": str,
     },
 )
 
@@ -6775,23 +6325,14 @@
     "RecommendationJobCompiledOutputConfigTypeDef",
     {
         "S3OutputUri": str,
     },
     total=False,
 )
 
-RecommendationJobPayloadConfigOutputTypeDef = TypedDict(
-    "RecommendationJobPayloadConfigOutputTypeDef",
-    {
-        "SamplePayloadUrl": str,
-        "SupportedContentTypes": List[str],
-    },
-    total=False,
-)
-
 RecommendationJobPayloadConfigTypeDef = TypedDict(
     "RecommendationJobPayloadConfigTypeDef",
     {
         "SamplePayloadUrl": str,
         "SupportedContentTypes": Sequence[str],
     },
     total=False,
@@ -6802,22 +6343,14 @@
     {
         "MaxNumberOfTests": int,
         "MaxParallelOfTests": int,
     },
     total=False,
 )
 
-RecommendationJobVpcConfigOutputTypeDef = TypedDict(
-    "RecommendationJobVpcConfigOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "Subnets": List[str],
-    },
-)
-
 RecommendationJobVpcConfigTypeDef = TypedDict(
     "RecommendationJobVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
@@ -6854,14 +6387,15 @@
     "_OptionalSearchRequestRequestTypeDef",
     {
         "SearchExpression": "SearchExpressionTypeDef",
         "SortBy": str,
         "SortOrder": SearchSortOrderType,
         "NextToken": str,
         "MaxResults": int,
+        "CrossAccountFilterOption": CrossAccountFilterOptionType,
     },
     total=False,
 )
 
 class SearchRequestRequestTypeDef(
     _RequiredSearchRequestRequestTypeDef, _OptionalSearchRequestRequestTypeDef
 ):
@@ -6926,19 +6460,22 @@
     },
     total=False,
 )
 
 class SourceAlgorithmTypeDef(_RequiredSourceAlgorithmTypeDef, _OptionalSourceAlgorithmTypeDef):
     pass
 
-SourceIpConfigOutputTypeDef = TypedDict(
-    "SourceIpConfigOutputTypeDef",
+StairsTypeDef = TypedDict(
+    "StairsTypeDef",
     {
-        "Cidrs": List[str],
+        "DurationInSeconds": int,
+        "NumberOfSteps": int,
+        "UsersPerStep": int,
     },
+    total=False,
 )
 
 StartEdgeDeploymentStageRequestRequestTypeDef = TypedDict(
     "StartEdgeDeploymentStageRequestRequestTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "StageName": str,
@@ -7055,14 +6592,42 @@
 StopTransformJobRequestRequestTypeDef = TypedDict(
     "StopTransformJobRequestRequestTypeDef",
     {
         "TransformJobName": str,
     },
 )
 
+_RequiredTimeSeriesConfigTypeDef = TypedDict(
+    "_RequiredTimeSeriesConfigTypeDef",
+    {
+        "TargetAttributeName": str,
+        "TimestampAttributeName": str,
+        "ItemIdentifierAttributeName": str,
+    },
+)
+_OptionalTimeSeriesConfigTypeDef = TypedDict(
+    "_OptionalTimeSeriesConfigTypeDef",
+    {
+        "GroupingAttributeNames": Sequence[str],
+    },
+    total=False,
+)
+
+class TimeSeriesConfigTypeDef(_RequiredTimeSeriesConfigTypeDef, _OptionalTimeSeriesConfigTypeDef):
+    pass
+
+TimeSeriesTransformationsTypeDef = TypedDict(
+    "TimeSeriesTransformationsTypeDef",
+    {
+        "Filling": Mapping[str, Mapping[FillingTypeType, str]],
+        "Aggregation": Mapping[str, AggregationTransformationValueType],
+    },
+    total=False,
+)
+
 TrainingRepositoryAuthConfigTypeDef = TypedDict(
     "TrainingRepositoryAuthConfigTypeDef",
     {
         "TrainingRepositoryCredentialsProviderArn": str,
     },
 )
 
@@ -8359,52 +7924,22 @@
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AutoRollbackConfigOutputTypeDef = TypedDict(
-    "AutoRollbackConfigOutputTypeDef",
-    {
-        "Alarms": List[AlarmTypeDef],
-    },
-    total=False,
-)
-
 AutoRollbackConfigTypeDef = TypedDict(
     "AutoRollbackConfigTypeDef",
     {
         "Alarms": Sequence[AlarmTypeDef],
     },
     total=False,
 )
 
-_RequiredHyperParameterAlgorithmSpecificationOutputTypeDef = TypedDict(
-    "_RequiredHyperParameterAlgorithmSpecificationOutputTypeDef",
-    {
-        "TrainingInputMode": TrainingInputModeType,
-    },
-)
-_OptionalHyperParameterAlgorithmSpecificationOutputTypeDef = TypedDict(
-    "_OptionalHyperParameterAlgorithmSpecificationOutputTypeDef",
-    {
-        "TrainingImage": str,
-        "AlgorithmName": str,
-        "MetricDefinitions": List[MetricDefinitionTypeDef],
-    },
-    total=False,
-)
-
-class HyperParameterAlgorithmSpecificationOutputTypeDef(
-    _RequiredHyperParameterAlgorithmSpecificationOutputTypeDef,
-    _OptionalHyperParameterAlgorithmSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredHyperParameterAlgorithmSpecificationTypeDef = TypedDict(
     "_RequiredHyperParameterAlgorithmSpecificationTypeDef",
     {
         "TrainingInputMode": TrainingInputModeType,
     },
 )
 _OptionalHyperParameterAlgorithmSpecificationTypeDef = TypedDict(
@@ -8446,34 +7981,14 @@
     {
         "Apps": List[AppDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AppSpecificationUnionTypeDef = Union[AppSpecificationTypeDef, AppSpecificationOutputTypeDef]
-_RequiredArtifactSourceOutputTypeDef = TypedDict(
-    "_RequiredArtifactSourceOutputTypeDef",
-    {
-        "SourceUri": str,
-    },
-)
-_OptionalArtifactSourceOutputTypeDef = TypedDict(
-    "_OptionalArtifactSourceOutputTypeDef",
-    {
-        "SourceTypes": List[ArtifactSourceTypeTypeDef],
-    },
-    total=False,
-)
-
-class ArtifactSourceOutputTypeDef(
-    _RequiredArtifactSourceOutputTypeDef, _OptionalArtifactSourceOutputTypeDef
-):
-    pass
-
 _RequiredArtifactSourceTypeDef = TypedDict(
     "_RequiredArtifactSourceTypeDef",
     {
         "SourceUri": str,
     },
 )
 _OptionalArtifactSourceTypeDef = TypedDict(
@@ -8483,53 +7998,25 @@
     },
     total=False,
 )
 
 class ArtifactSourceTypeDef(_RequiredArtifactSourceTypeDef, _OptionalArtifactSourceTypeDef):
     pass
 
-AsyncInferenceOutputConfigOutputTypeDef = TypedDict(
-    "AsyncInferenceOutputConfigOutputTypeDef",
-    {
-        "KmsKeyId": str,
-        "S3OutputPath": str,
-        "NotificationConfig": AsyncInferenceNotificationConfigOutputTypeDef,
-        "S3FailurePath": str,
-    },
-    total=False,
-)
-
 AsyncInferenceOutputConfigTypeDef = TypedDict(
     "AsyncInferenceOutputConfigTypeDef",
     {
         "KmsKeyId": str,
         "S3OutputPath": str,
         "NotificationConfig": AsyncInferenceNotificationConfigTypeDef,
         "S3FailurePath": str,
     },
     total=False,
 )
 
-AutoMLCandidateGenerationConfigOutputTypeDef = TypedDict(
-    "AutoMLCandidateGenerationConfigOutputTypeDef",
-    {
-        "FeatureSpecificationS3Uri": str,
-        "AlgorithmsConfig": List[AutoMLAlgorithmConfigOutputTypeDef],
-    },
-    total=False,
-)
-
-CandidateGenerationConfigOutputTypeDef = TypedDict(
-    "CandidateGenerationConfigOutputTypeDef",
-    {
-        "AlgorithmsConfig": List[AutoMLAlgorithmConfigOutputTypeDef],
-    },
-    total=False,
-)
-
 AutoMLCandidateGenerationConfigTypeDef = TypedDict(
     "AutoMLCandidateGenerationConfigTypeDef",
     {
         "FeatureSpecificationS3Uri": str,
         "AlgorithmsConfig": Sequence[AutoMLAlgorithmConfigTypeDef],
     },
     total=False,
@@ -8554,24 +8041,34 @@
     "ImageClassificationJobConfigTypeDef",
     {
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
     },
     total=False,
 )
 
-TextClassificationJobConfigTypeDef = TypedDict(
-    "TextClassificationJobConfigTypeDef",
+_RequiredTextClassificationJobConfigTypeDef = TypedDict(
+    "_RequiredTextClassificationJobConfigTypeDef",
     {
-        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
         "ContentColumn": str,
         "TargetLabelColumn": str,
     },
+)
+_OptionalTextClassificationJobConfigTypeDef = TypedDict(
+    "_OptionalTextClassificationJobConfigTypeDef",
+    {
+        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
+    },
     total=False,
 )
 
+class TextClassificationJobConfigTypeDef(
+    _RequiredTextClassificationJobConfigTypeDef, _OptionalTextClassificationJobConfigTypeDef
+):
+    pass
+
 ResolvedAttributesTypeDef = TypedDict(
     "ResolvedAttributesTypeDef",
     {
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "ProblemType": ProblemTypeType,
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
     },
@@ -8606,53 +8103,14 @@
     "AutoMLProblemTypeResolvedAttributesTypeDef",
     {
         "TabularResolvedAttributes": TabularResolvedAttributesTypeDef,
     },
     total=False,
 )
 
-AutoMLSecurityConfigOutputTypeDef = TypedDict(
-    "AutoMLSecurityConfigOutputTypeDef",
-    {
-        "VolumeKmsKeyId": str,
-        "EnableInterContainerTrafficEncryption": bool,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-LabelingJobResourceConfigOutputTypeDef = TypedDict(
-    "LabelingJobResourceConfigOutputTypeDef",
-    {
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-MonitoringNetworkConfigOutputTypeDef = TypedDict(
-    "MonitoringNetworkConfigOutputTypeDef",
-    {
-        "EnableInterContainerTrafficEncryption": bool,
-        "EnableNetworkIsolation": bool,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-NetworkConfigOutputTypeDef = TypedDict(
-    "NetworkConfigOutputTypeDef",
-    {
-        "EnableInterContainerTrafficEncryption": bool,
-        "EnableNetworkIsolation": bool,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 AutoMLSecurityConfigTypeDef = TypedDict(
     "AutoMLSecurityConfigTypeDef",
     {
         "VolumeKmsKeyId": str,
         "EnableInterContainerTrafficEncryption": bool,
         "VpcConfig": VpcConfigTypeDef,
     },
@@ -8684,15 +8142,14 @@
         "EnableInterContainerTrafficEncryption": bool,
         "EnableNetworkIsolation": bool,
         "VpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
-VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 BiasTypeDef = TypedDict(
     "BiasTypeDef",
     {
         "Report": MetricsSourceTypeDef,
         "PreTrainingReport": MetricsSourceTypeDef,
         "PostTrainingReport": MetricsSourceTypeDef,
     },
@@ -8793,57 +8250,58 @@
 )
 
 CanvasAppSettingsTypeDef = TypedDict(
     "CanvasAppSettingsTypeDef",
     {
         "TimeSeriesForecastingSettings": TimeSeriesForecastingSettingsTypeDef,
         "ModelRegisterSettings": ModelRegisterSettingsTypeDef,
+        "WorkspaceSettings": WorkspaceSettingsTypeDef,
     },
     total=False,
 )
 
-_RequiredTrafficRoutingConfigTypeDef = TypedDict(
-    "_RequiredTrafficRoutingConfigTypeDef",
+_RequiredRollingUpdatePolicyTypeDef = TypedDict(
+    "_RequiredRollingUpdatePolicyTypeDef",
     {
-        "Type": TrafficRoutingConfigTypeType,
+        "MaximumBatchSize": CapacitySizeTypeDef,
         "WaitIntervalInSeconds": int,
     },
 )
-_OptionalTrafficRoutingConfigTypeDef = TypedDict(
-    "_OptionalTrafficRoutingConfigTypeDef",
+_OptionalRollingUpdatePolicyTypeDef = TypedDict(
+    "_OptionalRollingUpdatePolicyTypeDef",
     {
-        "CanarySize": CapacitySizeTypeDef,
-        "LinearStepSize": CapacitySizeTypeDef,
+        "MaximumExecutionTimeoutInSeconds": int,
+        "RollbackMaximumBatchSize": CapacitySizeTypeDef,
     },
     total=False,
 )
 
-class TrafficRoutingConfigTypeDef(
-    _RequiredTrafficRoutingConfigTypeDef, _OptionalTrafficRoutingConfigTypeDef
+class RollingUpdatePolicyTypeDef(
+    _RequiredRollingUpdatePolicyTypeDef, _OptionalRollingUpdatePolicyTypeDef
 ):
     pass
 
-_RequiredInferenceExperimentDataStorageConfigOutputTypeDef = TypedDict(
-    "_RequiredInferenceExperimentDataStorageConfigOutputTypeDef",
+_RequiredTrafficRoutingConfigTypeDef = TypedDict(
+    "_RequiredTrafficRoutingConfigTypeDef",
     {
-        "Destination": str,
+        "Type": TrafficRoutingConfigTypeType,
+        "WaitIntervalInSeconds": int,
     },
 )
-_OptionalInferenceExperimentDataStorageConfigOutputTypeDef = TypedDict(
-    "_OptionalInferenceExperimentDataStorageConfigOutputTypeDef",
+_OptionalTrafficRoutingConfigTypeDef = TypedDict(
+    "_OptionalTrafficRoutingConfigTypeDef",
     {
-        "KmsKey": str,
-        "ContentType": CaptureContentTypeHeaderOutputTypeDef,
+        "CanarySize": CapacitySizeTypeDef,
+        "LinearStepSize": CapacitySizeTypeDef,
     },
     total=False,
 )
 
-class InferenceExperimentDataStorageConfigOutputTypeDef(
-    _RequiredInferenceExperimentDataStorageConfigOutputTypeDef,
-    _OptionalInferenceExperimentDataStorageConfigOutputTypeDef,
+class TrafficRoutingConfigTypeDef(
+    _RequiredTrafficRoutingConfigTypeDef, _OptionalTrafficRoutingConfigTypeDef
 ):
     pass
 
 _RequiredInferenceExperimentDataStorageConfigTypeDef = TypedDict(
     "_RequiredInferenceExperimentDataStorageConfigTypeDef",
     {
         "Destination": str,
@@ -8860,37 +8318,14 @@
 
 class InferenceExperimentDataStorageConfigTypeDef(
     _RequiredInferenceExperimentDataStorageConfigTypeDef,
     _OptionalInferenceExperimentDataStorageConfigTypeDef,
 ):
     pass
 
-_RequiredDataCaptureConfigOutputTypeDef = TypedDict(
-    "_RequiredDataCaptureConfigOutputTypeDef",
-    {
-        "InitialSamplingPercentage": int,
-        "DestinationS3Uri": str,
-        "CaptureOptions": List[CaptureOptionTypeDef],
-    },
-)
-_OptionalDataCaptureConfigOutputTypeDef = TypedDict(
-    "_OptionalDataCaptureConfigOutputTypeDef",
-    {
-        "EnableCapture": bool,
-        "KmsKeyId": str,
-        "CaptureContentTypeHeader": CaptureContentTypeHeaderOutputTypeDef,
-    },
-    total=False,
-)
-
-class DataCaptureConfigOutputTypeDef(
-    _RequiredDataCaptureConfigOutputTypeDef, _OptionalDataCaptureConfigOutputTypeDef
-):
-    pass
-
 _RequiredDataCaptureConfigTypeDef = TypedDict(
     "_RequiredDataCaptureConfigTypeDef",
     {
         "InitialSamplingPercentage": int,
         "DestinationS3Uri": str,
         "CaptureOptions": Sequence[CaptureOptionTypeDef],
     },
@@ -8906,22 +8341,14 @@
 )
 
 class DataCaptureConfigTypeDef(
     _RequiredDataCaptureConfigTypeDef, _OptionalDataCaptureConfigTypeDef
 ):
     pass
 
-EnvironmentParameterRangesOutputTypeDef = TypedDict(
-    "EnvironmentParameterRangesOutputTypeDef",
-    {
-        "CategoricalParameterRanges": List[CategoricalParameterOutputTypeDef],
-    },
-    total=False,
-)
-
 EnvironmentParameterRangesTypeDef = TypedDict(
     "EnvironmentParameterRangesTypeDef",
     {
         "CategoricalParameterRanges": Sequence[CategoricalParameterTypeDef],
     },
     total=False,
 )
@@ -8999,35 +8426,14 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "GitConfig": GitConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDebugHookConfigOutputTypeDef = TypedDict(
-    "_RequiredDebugHookConfigOutputTypeDef",
-    {
-        "S3OutputPath": str,
-    },
-)
-_OptionalDebugHookConfigOutputTypeDef = TypedDict(
-    "_OptionalDebugHookConfigOutputTypeDef",
-    {
-        "LocalPath": str,
-        "HookParameters": Dict[str, str],
-        "CollectionConfigurations": List[CollectionConfigurationOutputTypeDef],
-    },
-    total=False,
-)
-
-class DebugHookConfigOutputTypeDef(
-    _RequiredDebugHookConfigOutputTypeDef, _OptionalDebugHookConfigOutputTypeDef
-):
-    pass
-
 _RequiredDebugHookConfigTypeDef = TypedDict(
     "_RequiredDebugHookConfigTypeDef",
     {
         "S3OutputPath": str,
     },
 )
 _OptionalDebugHookConfigTypeDef = TypedDict(
@@ -9184,24 +8590,14 @@
         "FailureReason": str,
         "ResourceSpec": ResourceSpecTypeDef,
         "SpaceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JupyterServerAppSettingsOutputTypeDef = TypedDict(
-    "JupyterServerAppSettingsOutputTypeDef",
-    {
-        "DefaultResourceSpec": ResourceSpecTypeDef,
-        "LifecycleConfigArns": List[str],
-        "CodeRepositories": List[CodeRepositoryTypeDef],
-    },
-    total=False,
-)
-
 JupyterServerAppSettingsTypeDef = TypedDict(
     "JupyterServerAppSettingsTypeDef",
     {
         "DefaultResourceSpec": ResourceSpecTypeDef,
         "LifecycleConfigArns": Sequence[str],
         "CodeRepositories": Sequence[CodeRepositoryTypeDef],
     },
@@ -9341,34 +8737,14 @@
 )
 
 class UpdateDeviceFleetRequestRequestTypeDef(
     _RequiredUpdateDeviceFleetRequestRequestTypeDef, _OptionalUpdateDeviceFleetRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateFeatureGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFeatureGroupRequestRequestTypeDef",
-    {
-        "FeatureGroupName": str,
-    },
-)
-_OptionalUpdateFeatureGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFeatureGroupRequestRequestTypeDef",
-    {
-        "FeatureAdditions": Sequence[FeatureDefinitionTypeDef],
-    },
-    total=False,
-)
-
-class UpdateFeatureGroupRequestRequestTypeDef(
-    _RequiredUpdateFeatureGroupRequestRequestTypeDef,
-    _OptionalUpdateFeatureGroupRequestRequestTypeDef,
-):
-    pass
-
 _RequiredCreateHubRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHubRequestRequestTypeDef",
     {
         "HubName": str,
         "HubDescription": str,
     },
 )
@@ -10569,14 +9945,28 @@
         "NextToken": str,
         "SortBy": ProjectSortByType,
         "SortOrder": ProjectSortOrderType,
     },
     total=False,
 )
 
+ListResourceCatalogsRequestRequestTypeDef = TypedDict(
+    "ListResourceCatalogsRequestRequestTypeDef",
+    {
+        "NameContains": str,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+        "SortOrder": ResourceCatalogSortOrderType,
+        "SortBy": Literal["CreationTime"],
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 ListStudioLifecycleConfigsRequestRequestTypeDef = TypedDict(
     "ListStudioLifecycleConfigsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "NameContains": str,
         "AppTypeEquals": StudioLifecycleConfigAppTypeType,
@@ -10767,55 +10157,33 @@
 )
 
 class UpdateWorkforceRequestRequestTypeDef(
     _RequiredUpdateWorkforceRequestRequestTypeDef, _OptionalUpdateWorkforceRequestRequestTypeDef
 ):
     pass
 
-KernelGatewayAppSettingsOutputTypeDef = TypedDict(
-    "KernelGatewayAppSettingsOutputTypeDef",
-    {
-        "DefaultResourceSpec": ResourceSpecTypeDef,
-        "CustomImages": List[CustomImageTypeDef],
-        "LifecycleConfigArns": List[str],
-    },
-    total=False,
-)
-
 KernelGatewayAppSettingsTypeDef = TypedDict(
     "KernelGatewayAppSettingsTypeDef",
     {
         "DefaultResourceSpec": ResourceSpecTypeDef,
         "CustomImages": Sequence[CustomImageTypeDef],
         "LifecycleConfigArns": Sequence[str],
     },
     total=False,
 )
 
-RSessionAppSettingsOutputTypeDef = TypedDict(
-    "RSessionAppSettingsOutputTypeDef",
-    {
-        "DefaultResourceSpec": ResourceSpecTypeDef,
-        "CustomImages": List[CustomImageTypeDef],
-    },
-    total=False,
-)
-
 RSessionAppSettingsTypeDef = TypedDict(
     "RSessionAppSettingsTypeDef",
     {
         "DefaultResourceSpec": ResourceSpecTypeDef,
         "CustomImages": Sequence[CustomImageTypeDef],
     },
     total=False,
 )
 
-DataQualityAppSpecificationUnionTypeDef = Union[
-    DataQualityAppSpecificationTypeDef, DataQualityAppSpecificationOutputTypeDef
-]
 ModelBiasBaselineConfigTypeDef = TypedDict(
     "ModelBiasBaselineConfigTypeDef",
     {
         "BaseliningJobName": str,
         "ConstraintsResource": MonitoringConstraintsResourceTypeDef,
     },
     total=False,
@@ -10855,23 +10223,14 @@
         "BaseliningJobName": str,
         "ConstraintsResource": MonitoringConstraintsResourceTypeDef,
         "StatisticsResource": MonitoringStatisticsResourceTypeDef,
     },
     total=False,
 )
 
-DataSourceOutputTypeDef = TypedDict(
-    "DataSourceOutputTypeDef",
-    {
-        "S3DataSource": S3DataSourceOutputTypeDef,
-        "FileSystemDataSource": FileSystemDataSourceTypeDef,
-    },
-    total=False,
-)
-
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "S3DataSource": S3DataSourceTypeDef,
         "FileSystemDataSource": FileSystemDataSourceTypeDef,
     },
     total=False,
@@ -10885,17 +10244,14 @@
         "LocalPath": str,
         "DataDistributionType": DataDistributionTypeType,
         "InputMode": InputModeType,
     },
     total=False,
 )
 
-DebugRuleConfigurationUnionTypeDef = Union[
-    DebugRuleConfigurationTypeDef, DebugRuleConfigurationOutputTypeDef
-]
 _RequiredDeleteDomainRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDomainRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalDeleteDomainRequestRequestTypeDef = TypedDict(
@@ -10926,24 +10282,14 @@
 )
 
 class DeploymentRecommendationTypeDef(
     _RequiredDeploymentRecommendationTypeDef, _OptionalDeploymentRecommendationTypeDef
 ):
     pass
 
-DeploymentStageStatusSummaryTypeDef = TypedDict(
-    "DeploymentStageStatusSummaryTypeDef",
-    {
-        "StageName": str,
-        "DeviceSelectionConfig": DeviceSelectionConfigOutputTypeDef,
-        "DeploymentConfig": EdgeDeploymentConfigTypeDef,
-        "DeploymentStatus": EdgeDeploymentStatusTypeDef,
-    },
-)
-
 _RequiredDeploymentStageTypeDef = TypedDict(
     "_RequiredDeploymentStageTypeDef",
     {
         "StageName": str,
         "DeviceSelectionConfig": DeviceSelectionConfigTypeDef,
     },
 )
@@ -10954,15 +10300,24 @@
     },
     total=False,
 )
 
 class DeploymentStageTypeDef(_RequiredDeploymentStageTypeDef, _OptionalDeploymentStageTypeDef):
     pass
 
-NeoVpcConfigUnionTypeDef = Union[NeoVpcConfigTypeDef, NeoVpcConfigOutputTypeDef]
+DeploymentStageStatusSummaryTypeDef = TypedDict(
+    "DeploymentStageStatusSummaryTypeDef",
+    {
+        "StageName": str,
+        "DeviceSelectionConfig": DeviceSelectionConfigTypeDef,
+        "DeploymentConfig": EdgeDeploymentConfigTypeDef,
+        "DeploymentStatus": EdgeDeploymentStatusTypeDef,
+    },
+)
+
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceArn": str,
         "DeviceName": str,
         "Description": str,
         "DeviceFleetName": str,
@@ -11382,44 +10737,14 @@
         "HumanTaskUiStatus": HumanTaskUiStatusType,
         "CreationTime": datetime,
         "UiTemplate": UiTemplateInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredInferenceExperimentSummaryTypeDef = TypedDict(
-    "_RequiredInferenceExperimentSummaryTypeDef",
-    {
-        "Name": str,
-        "Type": Literal["ShadowMode"],
-        "Status": InferenceExperimentStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-    },
-)
-_OptionalInferenceExperimentSummaryTypeDef = TypedDict(
-    "_OptionalInferenceExperimentSummaryTypeDef",
-    {
-        "Schedule": InferenceExperimentScheduleOutputTypeDef,
-        "StatusReason": str,
-        "Description": str,
-        "CompletionTime": datetime,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
-class InferenceExperimentSummaryTypeDef(
-    _RequiredInferenceExperimentSummaryTypeDef, _OptionalInferenceExperimentSummaryTypeDef
-):
-    pass
-
-ModelBiasAppSpecificationUnionTypeDef = Union[
-    ModelBiasAppSpecificationTypeDef, ModelBiasAppSpecificationOutputTypeDef
-]
 DescribeModelCardExportJobResponseTypeDef = TypedDict(
     "DescribeModelCardExportJobResponseTypeDef",
     {
         "ModelCardExportJobName": str,
         "ModelCardExportJobArn": str,
         "Status": ModelCardExportJobStatusType,
         "ModelCardName": str,
@@ -11429,20 +10754,14 @@
         "LastModifiedAt": datetime,
         "FailureReason": str,
         "ExportArtifacts": ModelCardExportArtifactsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModelExplainabilityAppSpecificationUnionTypeDef = Union[
-    ModelExplainabilityAppSpecificationTypeDef, ModelExplainabilityAppSpecificationOutputTypeDef
-]
-ModelQualityAppSpecificationUnionTypeDef = Union[
-    ModelQualityAppSpecificationTypeDef, ModelQualityAppSpecificationOutputTypeDef
-]
 ListMonitoringExecutionsResponseTypeDef = TypedDict(
     "ListMonitoringExecutionsResponseTypeDef",
     {
         "MonitoringExecutionSummaries": List[MonitoringExecutionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -11461,15 +10780,14 @@
     {
         "SubscribedWorkteams": List[SubscribedWorkteamTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProfilerConfigUnionTypeDef = Union[ProfilerConfigTypeDef, ProfilerConfigOutputTypeDef]
 _RequiredTrainingJobSummaryTypeDef = TypedDict(
     "_RequiredTrainingJobSummaryTypeDef",
     {
         "TrainingJobName": str,
         "TrainingJobArn": str,
         "CreationTime": datetime,
         "TrainingJobStatus": TrainingJobStatusType,
@@ -11660,14 +10978,36 @@
     {
         "EndpointConfigs": List[EndpointConfigSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredEndpointOutputConfigurationTypeDef = TypedDict(
+    "_RequiredEndpointOutputConfigurationTypeDef",
+    {
+        "EndpointName": str,
+        "VariantName": str,
+    },
+)
+_OptionalEndpointOutputConfigurationTypeDef = TypedDict(
+    "_OptionalEndpointOutputConfigurationTypeDef",
+    {
+        "InstanceType": ProductionVariantInstanceTypeType,
+        "InitialInstanceCount": int,
+        "ServerlessConfig": ProductionVariantServerlessConfigTypeDef,
+    },
+    total=False,
+)
+
+class EndpointOutputConfigurationTypeDef(
+    _RequiredEndpointOutputConfigurationTypeDef, _OptionalEndpointOutputConfigurationTypeDef
+):
+    pass
+
 EndpointPerformanceTypeDef = TypedDict(
     "EndpointPerformanceTypeDef",
     {
         "Metrics": InferenceMetricsTypeDef,
         "EndpointInfo": EndpointInfoTypeDef,
     },
 )
@@ -11736,14 +11076,37 @@
     {
         "FlowDefinitionSummaries": List[FlowDefinitionSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef",
+    {
+        "InferenceRecommendationsJobName": str,
+    },
+)
+_OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef = TypedDict(
+    "_OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef",
+    {
+        "RecommendationId": str,
+        "EndpointName": str,
+        "TargetCpuUtilizationPerCore": int,
+        "ScalingPolicyObjective": ScalingPolicyObjectiveTypeDef,
+    },
+    total=False,
+)
+
+class GetScalingConfigurationRecommendationRequestRequestTypeDef(
+    _RequiredGetScalingConfigurationRecommendationRequestRequestTypeDef,
+    _OptionalGetScalingConfigurationRecommendationRequestRequestTypeDef,
+):
+    pass
+
 GetSearchSuggestionsResponseTypeDef = TypedDict(
     "GetSearchSuggestionsResponseTypeDef",
     {
         "PropertyNameSuggestions": List[PropertyNameSuggestionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -11807,27 +11170,14 @@
     {
         "HumanTaskUiSummaries": List[HumanTaskUiSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-HyperParameterTuningResourceConfigOutputTypeDef = TypedDict(
-    "HyperParameterTuningResourceConfigOutputTypeDef",
-    {
-        "InstanceType": TrainingInstanceTypeType,
-        "InstanceCount": int,
-        "VolumeSizeInGB": int,
-        "VolumeKmsKeyId": str,
-        "AllocationStrategy": Literal["Prioritized"],
-        "InstanceConfigs": List[HyperParameterTuningInstanceConfigTypeDef],
-    },
-    total=False,
-)
-
 HyperParameterTuningResourceConfigTypeDef = TypedDict(
     "HyperParameterTuningResourceConfigTypeDef",
     {
         "InstanceType": TrainingInstanceTypeType,
         "InstanceCount": int,
         "VolumeSizeInGB": int,
         "VolumeKmsKeyId": str,
@@ -11868,22 +11218,14 @@
     "HyperParameterTuningJobStrategyConfigTypeDef",
     {
         "HyperbandStrategyConfig": HyperbandStrategyConfigTypeDef,
     },
     total=False,
 )
 
-HyperParameterTuningJobWarmStartConfigOutputTypeDef = TypedDict(
-    "HyperParameterTuningJobWarmStartConfigOutputTypeDef",
-    {
-        "ParentHyperParameterTuningJobs": List[ParentHyperParameterTuningJobTypeDef],
-        "WarmStartType": HyperParameterTuningJobWarmStartTypeType,
-    },
-)
-
 HyperParameterTuningJobWarmStartConfigTypeDef = TypedDict(
     "HyperParameterTuningJobWarmStartConfigTypeDef",
     {
         "ParentHyperParameterTuningJobs": Sequence[ParentHyperParameterTuningJobTypeDef],
         "WarmStartType": HyperParameterTuningJobWarmStartTypeType,
     },
 )
@@ -11939,37 +11281,14 @@
     {
         "InferenceRecommendationsJobs": List[InferenceRecommendationsJobTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredResourceConfigOutputTypeDef = TypedDict(
-    "_RequiredResourceConfigOutputTypeDef",
-    {
-        "VolumeSizeInGB": int,
-    },
-)
-_OptionalResourceConfigOutputTypeDef = TypedDict(
-    "_OptionalResourceConfigOutputTypeDef",
-    {
-        "InstanceType": TrainingInstanceTypeType,
-        "InstanceCount": int,
-        "VolumeKmsKeyId": str,
-        "InstanceGroups": List[InstanceGroupTypeDef],
-        "KeepAlivePeriodInSeconds": int,
-    },
-    total=False,
-)
-
-class ResourceConfigOutputTypeDef(
-    _RequiredResourceConfigOutputTypeDef, _OptionalResourceConfigOutputTypeDef
-):
-    pass
-
 _RequiredResourceConfigTypeDef = TypedDict(
     "_RequiredResourceConfigTypeDef",
     {
         "VolumeSizeInGB": int,
     },
 )
 _OptionalResourceConfigTypeDef = TypedDict(
@@ -11983,77 +11302,35 @@
     },
     total=False,
 )
 
 class ResourceConfigTypeDef(_RequiredResourceConfigTypeDef, _OptionalResourceConfigTypeDef):
     pass
 
-ParameterRangeOutputTypeDef = TypedDict(
-    "ParameterRangeOutputTypeDef",
-    {
-        "IntegerParameterRangeSpecification": IntegerParameterRangeSpecificationTypeDef,
-        "ContinuousParameterRangeSpecification": ContinuousParameterRangeSpecificationTypeDef,
-        "CategoricalParameterRangeSpecification": (
-            CategoricalParameterRangeSpecificationOutputTypeDef
-        ),
-    },
-    total=False,
-)
-
 ParameterRangeTypeDef = TypedDict(
     "ParameterRangeTypeDef",
     {
         "IntegerParameterRangeSpecification": IntegerParameterRangeSpecificationTypeDef,
         "ContinuousParameterRangeSpecification": ContinuousParameterRangeSpecificationTypeDef,
         "CategoricalParameterRangeSpecification": CategoricalParameterRangeSpecificationTypeDef,
     },
     total=False,
 )
 
-ParameterRangesOutputTypeDef = TypedDict(
-    "ParameterRangesOutputTypeDef",
-    {
-        "IntegerParameterRanges": List[IntegerParameterRangeTypeDef],
-        "ContinuousParameterRanges": List[ContinuousParameterRangeTypeDef],
-        "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
-        "AutoParameters": List[AutoParameterTypeDef],
-    },
-    total=False,
-)
-
 ParameterRangesTypeDef = TypedDict(
     "ParameterRangesTypeDef",
     {
         "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
         "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
         "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
         "AutoParameters": Sequence[AutoParameterTypeDef],
     },
     total=False,
 )
 
-_RequiredKernelGatewayImageConfigOutputTypeDef = TypedDict(
-    "_RequiredKernelGatewayImageConfigOutputTypeDef",
-    {
-        "KernelSpecs": List[KernelSpecTypeDef],
-    },
-)
-_OptionalKernelGatewayImageConfigOutputTypeDef = TypedDict(
-    "_OptionalKernelGatewayImageConfigOutputTypeDef",
-    {
-        "FileSystemConfig": FileSystemConfigTypeDef,
-    },
-    total=False,
-)
-
-class KernelGatewayImageConfigOutputTypeDef(
-    _RequiredKernelGatewayImageConfigOutputTypeDef, _OptionalKernelGatewayImageConfigOutputTypeDef
-):
-    pass
-
 _RequiredKernelGatewayImageConfigTypeDef = TypedDict(
     "_RequiredKernelGatewayImageConfigTypeDef",
     {
         "KernelSpecs": Sequence[KernelSpecTypeDef],
     },
 )
 _OptionalKernelGatewayImageConfigTypeDef = TypedDict(
@@ -12967,14 +12244,27 @@
         "SortBy": SortByType,
         "SortOrder": SortOrderType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+ListResourceCatalogsRequestListResourceCatalogsPaginateTypeDef = TypedDict(
+    "ListResourceCatalogsRequestListResourceCatalogsPaginateTypeDef",
+    {
+        "NameContains": str,
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+        "SortOrder": ResourceCatalogSortOrderType,
+        "SortBy": Literal["CreationTime"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListSpacesRequestListSpacesPaginateTypeDef = TypedDict(
     "ListSpacesRequestListSpacesPaginateTypeDef",
     {
         "SortOrder": SortOrderType,
         "SortBy": SpaceSortKeyType,
         "DomainIdEquals": str,
         "SpaceNameContains": str,
@@ -13176,14 +12466,15 @@
 )
 _OptionalSearchRequestSearchPaginateTypeDef = TypedDict(
     "_OptionalSearchRequestSearchPaginateTypeDef",
     {
         "SearchExpression": "SearchExpressionTypeDef",
         "SortBy": str,
         "SortOrder": SearchSortOrderType,
+        "CrossAccountFilterOption": CrossAccountFilterOptionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchRequestSearchPaginateTypeDef(
     _RequiredSearchRequestSearchPaginateTypeDef, _OptionalSearchRequestSearchPaginateTypeDef
@@ -13366,14 +12657,23 @@
     {
         "ProjectSummaryList": List[ProjectSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListResourceCatalogsResponseTypeDef = TypedDict(
+    "ListResourceCatalogsResponseTypeDef",
+    {
+        "ResourceCatalogs": List[ResourceCatalogTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListSpacesResponseTypeDef = TypedDict(
     "ListSpacesResponseTypeDef",
     {
         "Spaces": List[SpaceDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -13402,28 +12702,28 @@
     {
         "UserProfiles": List[UserProfileDetailsTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MemberDefinitionOutputTypeDef = TypedDict(
-    "MemberDefinitionOutputTypeDef",
+MemberDefinitionTypeDef = TypedDict(
+    "MemberDefinitionTypeDef",
     {
         "CognitoMemberDefinition": CognitoMemberDefinitionTypeDef,
-        "OidcMemberDefinition": OidcMemberDefinitionOutputTypeDef,
+        "OidcMemberDefinition": OidcMemberDefinitionTypeDef,
     },
     total=False,
 )
 
-MemberDefinitionTypeDef = TypedDict(
-    "MemberDefinitionTypeDef",
+MetricSpecificationTypeDef = TypedDict(
+    "MetricSpecificationTypeDef",
     {
-        "CognitoMemberDefinition": CognitoMemberDefinitionTypeDef,
-        "OidcMemberDefinition": OidcMemberDefinitionTypeDef,
+        "Predefined": PredefinedMetricSpecificationTypeDef,
+        "Customized": CustomizedMetricSpecificationTypeDef,
     },
     total=False,
 )
 
 MonitoringAlertActionsTypeDef = TypedDict(
     "MonitoringAlertActionsTypeDef",
     {
@@ -13443,83 +12743,47 @@
     "ModelInfrastructureConfigTypeDef",
     {
         "InfrastructureType": Literal["RealTimeInference"],
         "RealTimeInferenceConfig": RealTimeInferenceConfigTypeDef,
     },
 )
 
-_RequiredModelPackageContainerDefinitionOutputTypeDef = TypedDict(
-    "_RequiredModelPackageContainerDefinitionOutputTypeDef",
-    {
-        "Image": str,
-    },
-)
-_OptionalModelPackageContainerDefinitionOutputTypeDef = TypedDict(
-    "_OptionalModelPackageContainerDefinitionOutputTypeDef",
-    {
-        "ContainerHostname": str,
-        "ImageDigest": str,
-        "ModelDataUrl": str,
-        "ProductId": str,
-        "Environment": Dict[str, str],
-        "ModelInput": ModelInputTypeDef,
-        "Framework": str,
-        "FrameworkVersion": str,
-        "NearestModelName": str,
-    },
-    total=False,
-)
-
-class ModelPackageContainerDefinitionOutputTypeDef(
-    _RequiredModelPackageContainerDefinitionOutputTypeDef,
-    _OptionalModelPackageContainerDefinitionOutputTypeDef,
-):
-    pass
-
 _RequiredModelPackageContainerDefinitionTypeDef = TypedDict(
     "_RequiredModelPackageContainerDefinitionTypeDef",
     {
         "Image": str,
     },
 )
 _OptionalModelPackageContainerDefinitionTypeDef = TypedDict(
     "_OptionalModelPackageContainerDefinitionTypeDef",
     {
         "ContainerHostname": str,
         "ImageDigest": str,
         "ModelDataUrl": str,
         "ProductId": str,
-        "Environment": Mapping[str, str],
+        "Environment": Dict[str, str],
         "ModelInput": ModelInputTypeDef,
         "Framework": str,
         "FrameworkVersion": str,
         "NearestModelName": str,
     },
     total=False,
 )
 
 class ModelPackageContainerDefinitionTypeDef(
     _RequiredModelPackageContainerDefinitionTypeDef, _OptionalModelPackageContainerDefinitionTypeDef
 ):
     pass
 
-RecommendationJobStoppingConditionsOutputTypeDef = TypedDict(
-    "RecommendationJobStoppingConditionsOutputTypeDef",
-    {
-        "MaxInvocations": int,
-        "ModelLatencyThresholds": List[ModelLatencyThresholdTypeDef],
-    },
-    total=False,
-)
-
 RecommendationJobStoppingConditionsTypeDef = TypedDict(
     "RecommendationJobStoppingConditionsTypeDef",
     {
         "MaxInvocations": int,
         "ModelLatencyThresholds": Sequence[ModelLatencyThresholdTypeDef],
+        "FlatInvocations": FlatInvocationsType,
     },
     total=False,
 )
 
 ModelMetadataSearchExpressionTypeDef = TypedDict(
     "ModelMetadataSearchExpressionTypeDef",
     {
@@ -13550,24 +12814,14 @@
 MonitoringResourcesTypeDef = TypedDict(
     "MonitoringResourcesTypeDef",
     {
         "ClusterConfig": MonitoringClusterConfigTypeDef,
     },
 )
 
-MonitoringDatasetFormatOutputTypeDef = TypedDict(
-    "MonitoringDatasetFormatOutputTypeDef",
-    {
-        "Csv": MonitoringCsvDatasetFormatTypeDef,
-        "Json": MonitoringJsonDatasetFormatTypeDef,
-        "Parquet": Dict[str, Any],
-    },
-    total=False,
-)
-
 MonitoringDatasetFormatTypeDef = TypedDict(
     "MonitoringDatasetFormatTypeDef",
     {
         "Csv": MonitoringCsvDatasetFormatTypeDef,
         "Json": MonitoringJsonDatasetFormatTypeDef,
         "Parquet": Mapping[str, Any],
     },
@@ -13603,14 +12857,23 @@
     pass
 
 OnlineStoreConfigTypeDef = TypedDict(
     "OnlineStoreConfigTypeDef",
     {
         "SecurityConfig": OnlineStoreSecurityConfigTypeDef,
         "EnableOnlineStore": bool,
+        "TtlDuration": TtlDurationTypeDef,
+    },
+    total=False,
+)
+
+OnlineStoreConfigUpdateTypeDef = TypedDict(
+    "OnlineStoreConfigUpdateTypeDef",
+    {
+        "TtlDuration": TtlDurationTypeDef,
     },
     total=False,
 )
 
 _RequiredOutputConfigTypeDef = TypedDict(
     "_RequiredOutputConfigTypeDef",
     {
@@ -13681,32 +12944,14 @@
 )
 
 class ProductionVariantSummaryTypeDef(
     _RequiredProductionVariantSummaryTypeDef, _OptionalProductionVariantSummaryTypeDef
 ):
     pass
 
-TrafficPatternOutputTypeDef = TypedDict(
-    "TrafficPatternOutputTypeDef",
-    {
-        "TrafficType": Literal["PHASES"],
-        "Phases": List[PhaseTypeDef],
-    },
-    total=False,
-)
-
-TrafficPatternTypeDef = TypedDict(
-    "TrafficPatternTypeDef",
-    {
-        "TrafficType": Literal["PHASES"],
-        "Phases": Sequence[PhaseTypeDef],
-    },
-    total=False,
-)
-
 ProcessingResourcesTypeDef = TypedDict(
     "ProcessingResourcesTypeDef",
     {
         "ClusterConfig": ProcessingClusterConfigTypeDef,
     },
 )
 
@@ -13754,47 +12999,22 @@
 )
 
 class ProductionVariantTypeDef(
     _RequiredProductionVariantTypeDef, _OptionalProductionVariantTypeDef
 ):
     pass
 
-ProfilerRuleConfigurationUnionTypeDef = Union[
-    ProfilerRuleConfigurationTypeDef, ProfilerRuleConfigurationOutputTypeDef
-]
 SuggestionQueryTypeDef = TypedDict(
     "SuggestionQueryTypeDef",
     {
         "PropertyNameQuery": PropertyNameQueryTypeDef,
     },
     total=False,
 )
 
-_RequiredServiceCatalogProvisioningDetailsOutputTypeDef = TypedDict(
-    "_RequiredServiceCatalogProvisioningDetailsOutputTypeDef",
-    {
-        "ProductId": str,
-    },
-)
-_OptionalServiceCatalogProvisioningDetailsOutputTypeDef = TypedDict(
-    "_OptionalServiceCatalogProvisioningDetailsOutputTypeDef",
-    {
-        "ProvisioningArtifactId": str,
-        "PathId": str,
-        "ProvisioningParameters": List[ProvisioningParameterTypeDef],
-    },
-    total=False,
-)
-
-class ServiceCatalogProvisioningDetailsOutputTypeDef(
-    _RequiredServiceCatalogProvisioningDetailsOutputTypeDef,
-    _OptionalServiceCatalogProvisioningDetailsOutputTypeDef,
-):
-    pass
-
 _RequiredServiceCatalogProvisioningDetailsTypeDef = TypedDict(
     "_RequiredServiceCatalogProvisioningDetailsTypeDef",
     {
         "ProductId": str,
     },
 )
 _OptionalServiceCatalogProvisioningDetailsTypeDef = TypedDict(
@@ -13845,40 +13065,26 @@
     {
         "KmsKeyId": str,
         "CompiledOutputConfig": RecommendationJobCompiledOutputConfigTypeDef,
     },
     total=False,
 )
 
-RecommendationJobContainerConfigOutputTypeDef = TypedDict(
-    "RecommendationJobContainerConfigOutputTypeDef",
-    {
-        "Domain": str,
-        "Task": str,
-        "Framework": str,
-        "FrameworkVersion": str,
-        "PayloadConfig": RecommendationJobPayloadConfigOutputTypeDef,
-        "NearestModelName": str,
-        "SupportedInstanceTypes": List[str],
-        "DataInputConfig": str,
-    },
-    total=False,
-)
-
 RecommendationJobContainerConfigTypeDef = TypedDict(
     "RecommendationJobContainerConfigTypeDef",
     {
         "Domain": str,
         "Task": str,
         "Framework": str,
         "FrameworkVersion": str,
         "PayloadConfig": RecommendationJobPayloadConfigTypeDef,
         "NearestModelName": str,
         "SupportedInstanceTypes": Sequence[str],
         "DataInputConfig": str,
+        "SupportedEndpointType": RecommendationJobSupportedEndpointTypeType,
     },
     total=False,
 )
 
 _RequiredRenderUiTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredRenderUiTemplateRequestRequestTypeDef",
     {
@@ -13905,61 +13111,92 @@
     {
         "RenderedContent": str,
         "Errors": List[RenderingErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SelectiveExecutionConfigOutputTypeDef = TypedDict(
-    "SelectiveExecutionConfigOutputTypeDef",
+_RequiredUpdateTrainingJobRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateTrainingJobRequestRequestTypeDef",
     {
-        "SourcePipelineExecutionArn": str,
-        "SelectedSteps": List[SelectedStepTypeDef],
+        "TrainingJobName": str,
+    },
+)
+_OptionalUpdateTrainingJobRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateTrainingJobRequestRequestTypeDef",
+    {
+        "ProfilerConfig": ProfilerConfigForUpdateTypeDef,
+        "ProfilerRuleConfigurations": Sequence[ProfilerRuleConfigurationTypeDef],
+        "ResourceConfig": ResourceConfigForUpdateTypeDef,
     },
+    total=False,
 )
 
+class UpdateTrainingJobRequestRequestTypeDef(
+    _RequiredUpdateTrainingJobRequestRequestTypeDef, _OptionalUpdateTrainingJobRequestRequestTypeDef
+):
+    pass
+
 SelectiveExecutionConfigTypeDef = TypedDict(
     "SelectiveExecutionConfigTypeDef",
     {
         "SourcePipelineExecutionArn": str,
-        "SelectedSteps": Sequence[SelectedStepTypeDef],
+        "SelectedSteps": List[SelectedStepTypeDef],
     },
 )
 
-ShadowModeConfigOutputTypeDef = TypedDict(
-    "ShadowModeConfigOutputTypeDef",
+ShadowModeConfigTypeDef = TypedDict(
+    "ShadowModeConfigTypeDef",
     {
         "SourceModelVariantName": str,
-        "ShadowModelVariants": List[ShadowModelVariantConfigTypeDef],
+        "ShadowModelVariants": Sequence[ShadowModelVariantConfigTypeDef],
     },
 )
 
-ShadowModeConfigTypeDef = TypedDict(
-    "ShadowModeConfigTypeDef",
+SourceAlgorithmSpecificationTypeDef = TypedDict(
+    "SourceAlgorithmSpecificationTypeDef",
     {
-        "SourceModelVariantName": str,
-        "ShadowModelVariants": Sequence[ShadowModelVariantConfigTypeDef],
+        "SourceAlgorithms": Sequence[SourceAlgorithmTypeDef],
     },
 )
 
-SourceAlgorithmSpecificationOutputTypeDef = TypedDict(
-    "SourceAlgorithmSpecificationOutputTypeDef",
+TrafficPatternTypeDef = TypedDict(
+    "TrafficPatternTypeDef",
     {
-        "SourceAlgorithms": List[SourceAlgorithmTypeDef],
+        "TrafficType": TrafficTypeType,
+        "Phases": Sequence[PhaseTypeDef],
+        "Stairs": StairsTypeDef,
     },
+    total=False,
 )
 
-SourceAlgorithmSpecificationTypeDef = TypedDict(
-    "SourceAlgorithmSpecificationTypeDef",
+_RequiredTimeSeriesForecastingJobConfigTypeDef = TypedDict(
+    "_RequiredTimeSeriesForecastingJobConfigTypeDef",
     {
-        "SourceAlgorithms": Sequence[SourceAlgorithmTypeDef],
+        "ForecastFrequency": str,
+        "ForecastHorizon": int,
+        "TimeSeriesConfig": TimeSeriesConfigTypeDef,
     },
 )
+_OptionalTimeSeriesForecastingJobConfigTypeDef = TypedDict(
+    "_OptionalTimeSeriesForecastingJobConfigTypeDef",
+    {
+        "FeatureSpecificationS3Uri": str,
+        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
+        "ForecastQuantiles": Sequence[str],
+        "Transformations": TimeSeriesTransformationsTypeDef,
+    },
+    total=False,
+)
+
+class TimeSeriesForecastingJobConfigTypeDef(
+    _RequiredTimeSeriesForecastingJobConfigTypeDef, _OptionalTimeSeriesForecastingJobConfigTypeDef
+):
+    pass
 
-SourceIpConfigUnionTypeDef = Union[SourceIpConfigTypeDef, SourceIpConfigOutputTypeDef]
 _RequiredTrainingImageConfigTypeDef = TypedDict(
     "_RequiredTrainingImageConfigTypeDef",
     {
         "TrainingRepositoryAccessMode": TrainingRepositoryAccessModeType,
     },
 )
 _OptionalTrainingImageConfigTypeDef = TypedDict(
@@ -13989,15 +13226,15 @@
         "WorkforceArn": str,
     },
 )
 _OptionalWorkforceTypeDef = TypedDict(
     "_OptionalWorkforceTypeDef",
     {
         "LastUpdatedDate": datetime,
-        "SourceIpConfig": SourceIpConfigOutputTypeDef,
+        "SourceIpConfig": SourceIpConfigTypeDef,
         "SubDomain": str,
         "CognitoConfig": CognitoConfigTypeDef,
         "OidcConfig": OidcConfigForResponseTypeDef,
         "CreateDate": datetime,
         "WorkforceVpcConfig": WorkforceVpcConfigResponseTypeDef,
         "Status": WorkforceStatusType,
         "FailureReason": str,
@@ -14018,23 +13255,22 @@
 )
 
 ArtifactSummaryTypeDef = TypedDict(
     "ArtifactSummaryTypeDef",
     {
         "ArtifactArn": str,
         "ArtifactName": str,
-        "Source": ArtifactSourceOutputTypeDef,
+        "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-ArtifactSourceUnionTypeDef = Union[ArtifactSourceTypeDef, ArtifactSourceOutputTypeDef]
 _RequiredCreateArtifactRequestRequestTypeDef = TypedDict(
     "_RequiredCreateArtifactRequestRequestTypeDef",
     {
         "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
     },
 )
@@ -14059,33 +13295,14 @@
     {
         "ArtifactArn": str,
         "Source": ArtifactSourceTypeDef,
     },
     total=False,
 )
 
-_RequiredAsyncInferenceConfigOutputTypeDef = TypedDict(
-    "_RequiredAsyncInferenceConfigOutputTypeDef",
-    {
-        "OutputConfig": AsyncInferenceOutputConfigOutputTypeDef,
-    },
-)
-_OptionalAsyncInferenceConfigOutputTypeDef = TypedDict(
-    "_OptionalAsyncInferenceConfigOutputTypeDef",
-    {
-        "ClientConfig": AsyncInferenceClientConfigTypeDef,
-    },
-    total=False,
-)
-
-class AsyncInferenceConfigOutputTypeDef(
-    _RequiredAsyncInferenceConfigOutputTypeDef, _OptionalAsyncInferenceConfigOutputTypeDef
-):
-    pass
-
 _RequiredAsyncInferenceConfigTypeDef = TypedDict(
     "_RequiredAsyncInferenceConfigTypeDef",
     {
         "OutputConfig": AsyncInferenceOutputConfigTypeDef,
     },
 )
 _OptionalAsyncInferenceConfigTypeDef = TypedDict(
@@ -14097,39 +13314,14 @@
 )
 
 class AsyncInferenceConfigTypeDef(
     _RequiredAsyncInferenceConfigTypeDef, _OptionalAsyncInferenceConfigTypeDef
 ):
     pass
 
-_RequiredTabularJobConfigOutputTypeDef = TypedDict(
-    "_RequiredTabularJobConfigOutputTypeDef",
-    {
-        "TargetAttributeName": str,
-    },
-)
-_OptionalTabularJobConfigOutputTypeDef = TypedDict(
-    "_OptionalTabularJobConfigOutputTypeDef",
-    {
-        "CandidateGenerationConfig": CandidateGenerationConfigOutputTypeDef,
-        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
-        "FeatureSpecificationS3Uri": str,
-        "Mode": AutoMLModeType,
-        "GenerateCandidateDefinitionsOnly": bool,
-        "ProblemType": ProblemTypeType,
-        "SampleWeightAttributeName": str,
-    },
-    total=False,
-)
-
-class TabularJobConfigOutputTypeDef(
-    _RequiredTabularJobConfigOutputTypeDef, _OptionalTabularJobConfigOutputTypeDef
-):
-    pass
-
 _RequiredTabularJobConfigTypeDef = TypedDict(
     "_RequiredTabularJobConfigTypeDef",
     {
         "TargetAttributeName": str,
     },
 )
 _OptionalTabularJobConfigTypeDef = TypedDict(
@@ -14196,62 +13388,26 @@
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
         "AutoMLProblemTypeResolvedAttributes": AutoMLProblemTypeResolvedAttributesTypeDef,
     },
     total=False,
 )
 
-AutoMLJobConfigOutputTypeDef = TypedDict(
-    "AutoMLJobConfigOutputTypeDef",
-    {
-        "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
-        "SecurityConfig": AutoMLSecurityConfigOutputTypeDef,
-        "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
-        "CandidateGenerationConfig": AutoMLCandidateGenerationConfigOutputTypeDef,
-        "Mode": AutoMLModeType,
-    },
-    total=False,
-)
-
-_RequiredLabelingJobAlgorithmsConfigOutputTypeDef = TypedDict(
-    "_RequiredLabelingJobAlgorithmsConfigOutputTypeDef",
-    {
-        "LabelingJobAlgorithmSpecificationArn": str,
-    },
-)
-_OptionalLabelingJobAlgorithmsConfigOutputTypeDef = TypedDict(
-    "_OptionalLabelingJobAlgorithmsConfigOutputTypeDef",
-    {
-        "InitialActiveLearningModelArn": str,
-        "LabelingJobResourceConfig": LabelingJobResourceConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class LabelingJobAlgorithmsConfigOutputTypeDef(
-    _RequiredLabelingJobAlgorithmsConfigOutputTypeDef,
-    _OptionalLabelingJobAlgorithmsConfigOutputTypeDef,
-):
-    pass
-
 AutoMLJobConfigTypeDef = TypedDict(
     "AutoMLJobConfigTypeDef",
     {
         "CompletionCriteria": AutoMLJobCompletionCriteriaTypeDef,
         "SecurityConfig": AutoMLSecurityConfigTypeDef,
         "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
         "CandidateGenerationConfig": AutoMLCandidateGenerationConfigTypeDef,
         "Mode": AutoMLModeType,
     },
     total=False,
 )
 
-AutoMLSecurityConfigUnionTypeDef = Union[
-    AutoMLSecurityConfigTypeDef, AutoMLSecurityConfigOutputTypeDef
-]
 _RequiredLabelingJobAlgorithmsConfigTypeDef = TypedDict(
     "_RequiredLabelingJobAlgorithmsConfigTypeDef",
     {
         "LabelingJobAlgorithmSpecificationArn": str,
     },
 )
 _OptionalLabelingJobAlgorithmsConfigTypeDef = TypedDict(
@@ -14264,18 +13420,14 @@
 )
 
 class LabelingJobAlgorithmsConfigTypeDef(
     _RequiredLabelingJobAlgorithmsConfigTypeDef, _OptionalLabelingJobAlgorithmsConfigTypeDef
 ):
     pass
 
-MonitoringNetworkConfigUnionTypeDef = Union[
-    MonitoringNetworkConfigTypeDef, MonitoringNetworkConfigOutputTypeDef
-]
-NetworkConfigUnionTypeDef = Union[NetworkConfigTypeDef, NetworkConfigOutputTypeDef]
 ModelMetricsTypeDef = TypedDict(
     "ModelMetricsTypeDef",
     {
         "ModelQuality": ModelQualityTypeDef,
         "ModelDataQuality": ModelDataQualityTypeDef,
         "Bias": BiasTypeDef,
         "Explainability": ExplainabilityTypeDef,
@@ -14349,79 +13501,25 @@
 )
 
 class BlueGreenUpdatePolicyTypeDef(
     _RequiredBlueGreenUpdatePolicyTypeDef, _OptionalBlueGreenUpdatePolicyTypeDef
 ):
     pass
 
-InferenceExperimentDataStorageConfigUnionTypeDef = Union[
-    InferenceExperimentDataStorageConfigTypeDef, InferenceExperimentDataStorageConfigOutputTypeDef
-]
-DataCaptureConfigUnionTypeDef = Union[DataCaptureConfigTypeDef, DataCaptureConfigOutputTypeDef]
-_RequiredEndpointInputConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEndpointInputConfigurationOutputTypeDef",
-    {
-        "InstanceType": ProductionVariantInstanceTypeType,
-    },
-)
-_OptionalEndpointInputConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEndpointInputConfigurationOutputTypeDef",
-    {
-        "InferenceSpecificationName": str,
-        "EnvironmentParameterRanges": EnvironmentParameterRangesOutputTypeDef,
-    },
-    total=False,
-)
-
-class EndpointInputConfigurationOutputTypeDef(
-    _RequiredEndpointInputConfigurationOutputTypeDef,
-    _OptionalEndpointInputConfigurationOutputTypeDef,
-):
-    pass
-
-_RequiredEndpointInputConfigurationTypeDef = TypedDict(
-    "_RequiredEndpointInputConfigurationTypeDef",
+EndpointInputConfigurationTypeDef = TypedDict(
+    "EndpointInputConfigurationTypeDef",
     {
         "InstanceType": ProductionVariantInstanceTypeType,
-    },
-)
-_OptionalEndpointInputConfigurationTypeDef = TypedDict(
-    "_OptionalEndpointInputConfigurationTypeDef",
-    {
         "InferenceSpecificationName": str,
         "EnvironmentParameterRanges": EnvironmentParameterRangesTypeDef,
+        "ServerlessConfig": ProductionVariantServerlessConfigTypeDef,
     },
     total=False,
 )
 
-class EndpointInputConfigurationTypeDef(
-    _RequiredEndpointInputConfigurationTypeDef, _OptionalEndpointInputConfigurationTypeDef
-):
-    pass
-
-_RequiredClarifyExplainerConfigOutputTypeDef = TypedDict(
-    "_RequiredClarifyExplainerConfigOutputTypeDef",
-    {
-        "ShapConfig": ClarifyShapConfigTypeDef,
-    },
-)
-_OptionalClarifyExplainerConfigOutputTypeDef = TypedDict(
-    "_OptionalClarifyExplainerConfigOutputTypeDef",
-    {
-        "EnableExplanations": str,
-        "InferenceConfig": ClarifyInferenceConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class ClarifyExplainerConfigOutputTypeDef(
-    _RequiredClarifyExplainerConfigOutputTypeDef, _OptionalClarifyExplainerConfigOutputTypeDef
-):
-    pass
-
 _RequiredClarifyExplainerConfigTypeDef = TypedDict(
     "_RequiredClarifyExplainerConfigTypeDef",
     {
         "ShapConfig": ClarifyShapConfigTypeDef,
     },
 )
 _OptionalClarifyExplainerConfigTypeDef = TypedDict(
@@ -14443,15 +13541,14 @@
     {
         "CodeRepositorySummaryList": List[CodeRepositorySummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DebugHookConfigUnionTypeDef = Union[DebugHookConfigTypeDef, DebugHookConfigOutputTypeDef]
 ListContextsResponseTypeDef = TypedDict(
     "ListContextsResponseTypeDef",
     {
         "ContextSummaries": List[ContextSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -14463,71 +13560,65 @@
         "RStudioServerProDomainSettingsForUpdate": RStudioServerProDomainSettingsForUpdateTypeDef,
         "ExecutionRoleIdentityConfig": ExecutionRoleIdentityConfigType,
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-DomainSettingsOutputTypeDef = TypedDict(
-    "DomainSettingsOutputTypeDef",
+DomainSettingsTypeDef = TypedDict(
+    "DomainSettingsTypeDef",
     {
-        "SecurityGroupIds": List[str],
+        "SecurityGroupIds": Sequence[str],
         "RStudioServerProDomainSettings": RStudioServerProDomainSettingsTypeDef,
         "ExecutionRoleIdentityConfig": ExecutionRoleIdentityConfigType,
     },
     total=False,
 )
 
-DomainSettingsTypeDef = TypedDict(
-    "DomainSettingsTypeDef",
+_RequiredInferenceExperimentSummaryTypeDef = TypedDict(
+    "_RequiredInferenceExperimentSummaryTypeDef",
     {
-        "SecurityGroupIds": Sequence[str],
-        "RStudioServerProDomainSettings": RStudioServerProDomainSettingsTypeDef,
-        "ExecutionRoleIdentityConfig": ExecutionRoleIdentityConfigType,
+        "Name": str,
+        "Type": Literal["ShadowMode"],
+        "Status": InferenceExperimentStatusType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+    },
+)
+_OptionalInferenceExperimentSummaryTypeDef = TypedDict(
+    "_OptionalInferenceExperimentSummaryTypeDef",
+    {
+        "Schedule": InferenceExperimentScheduleTypeDef,
+        "StatusReason": str,
+        "Description": str,
+        "CompletionTime": datetime,
+        "RoleArn": str,
     },
     total=False,
 )
 
-InferenceExperimentScheduleUnionTypeDef = Union[
-    InferenceExperimentScheduleTypeDef, InferenceExperimentScheduleOutputTypeDef
-]
+class InferenceExperimentSummaryTypeDef(
+    _RequiredInferenceExperimentSummaryTypeDef, _OptionalInferenceExperimentSummaryTypeDef
+):
+    pass
+
 QueryLineageRequestRequestTypeDef = TypedDict(
     "QueryLineageRequestRequestTypeDef",
     {
         "StartArns": Sequence[str],
         "Direction": DirectionType,
         "IncludeEdges": bool,
         "Filters": QueryFiltersTypeDef,
         "MaxDepth": int,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DefaultSpaceSettingsOutputTypeDef = TypedDict(
-    "DefaultSpaceSettingsOutputTypeDef",
-    {
-        "ExecutionRole": str,
-        "SecurityGroups": List[str],
-        "JupyterServerAppSettings": JupyterServerAppSettingsOutputTypeDef,
-        "KernelGatewayAppSettings": KernelGatewayAppSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-SpaceSettingsOutputTypeDef = TypedDict(
-    "SpaceSettingsOutputTypeDef",
-    {
-        "JupyterServerAppSettings": JupyterServerAppSettingsOutputTypeDef,
-        "KernelGatewayAppSettings": KernelGatewayAppSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 DefaultSpaceSettingsTypeDef = TypedDict(
     "DefaultSpaceSettingsTypeDef",
     {
         "ExecutionRole": str,
         "SecurityGroups": Sequence[str],
         "JupyterServerAppSettings": JupyterServerAppSettingsTypeDef,
         "KernelGatewayAppSettings": KernelGatewayAppSettingsTypeDef,
@@ -14540,30 +13631,14 @@
     {
         "JupyterServerAppSettings": JupyterServerAppSettingsTypeDef,
         "KernelGatewayAppSettings": KernelGatewayAppSettingsTypeDef,
     },
     total=False,
 )
 
-UserSettingsOutputTypeDef = TypedDict(
-    "UserSettingsOutputTypeDef",
-    {
-        "ExecutionRole": str,
-        "SecurityGroups": List[str],
-        "SharingSettings": SharingSettingsTypeDef,
-        "JupyterServerAppSettings": JupyterServerAppSettingsOutputTypeDef,
-        "KernelGatewayAppSettings": KernelGatewayAppSettingsOutputTypeDef,
-        "TensorBoardAppSettings": TensorBoardAppSettingsTypeDef,
-        "RStudioServerProAppSettings": RStudioServerProAppSettingsTypeDef,
-        "RSessionAppSettings": RSessionAppSettingsOutputTypeDef,
-        "CanvasAppSettings": CanvasAppSettingsTypeDef,
-    },
-    total=False,
-)
-
 UserSettingsTypeDef = TypedDict(
     "UserSettingsTypeDef",
     {
         "ExecutionRole": str,
         "SecurityGroups": Sequence[str],
         "SharingSettings": SharingSettingsTypeDef,
         "JupyterServerAppSettings": JupyterServerAppSettingsTypeDef,
@@ -14572,36 +13647,14 @@
         "RStudioServerProAppSettings": RStudioServerProAppSettingsTypeDef,
         "RSessionAppSettings": RSessionAppSettingsTypeDef,
         "CanvasAppSettings": CanvasAppSettingsTypeDef,
     },
     total=False,
 )
 
-_RequiredChannelOutputTypeDef = TypedDict(
-    "_RequiredChannelOutputTypeDef",
-    {
-        "ChannelName": str,
-        "DataSource": DataSourceOutputTypeDef,
-    },
-)
-_OptionalChannelOutputTypeDef = TypedDict(
-    "_OptionalChannelOutputTypeDef",
-    {
-        "ContentType": str,
-        "CompressionType": CompressionTypeType,
-        "RecordWrapperType": RecordWrapperType,
-        "InputMode": TrainingInputModeType,
-        "ShuffleConfig": ShuffleConfigTypeDef,
-    },
-    total=False,
-)
-
-class ChannelOutputTypeDef(_RequiredChannelOutputTypeDef, _OptionalChannelOutputTypeDef):
-    pass
-
 _RequiredChannelTypeDef = TypedDict(
     "_RequiredChannelTypeDef",
     {
         "ChannelName": str,
         "DataSource": DataSourceTypeDef,
     },
 )
@@ -14635,32 +13688,14 @@
     },
     total=False,
 )
 
 class ProcessingInputTypeDef(_RequiredProcessingInputTypeDef, _OptionalProcessingInputTypeDef):
     pass
 
-DescribeEdgeDeploymentPlanResponseTypeDef = TypedDict(
-    "DescribeEdgeDeploymentPlanResponseTypeDef",
-    {
-        "EdgeDeploymentPlanArn": str,
-        "EdgeDeploymentPlanName": str,
-        "ModelConfigs": List[EdgeDeploymentModelConfigTypeDef],
-        "DeviceFleetName": str,
-        "EdgeDeploymentSuccess": int,
-        "EdgeDeploymentPending": int,
-        "EdgeDeploymentFailed": int,
-        "Stages": List[DeploymentStageStatusSummaryTypeDef],
-        "NextToken": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateEdgeDeploymentPlanRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEdgeDeploymentPlanRequestRequestTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "ModelConfigs": Sequence[EdgeDeploymentModelConfigTypeDef],
         "DeviceFleetName": str,
     },
@@ -14684,36 +13719,45 @@
     "CreateEdgeDeploymentStageRequestRequestTypeDef",
     {
         "EdgeDeploymentPlanName": str,
         "Stages": Sequence[DeploymentStageTypeDef],
     },
 )
 
-ListExperimentsResponseTypeDef = TypedDict(
-    "ListExperimentsResponseTypeDef",
+DescribeEdgeDeploymentPlanResponseTypeDef = TypedDict(
+    "DescribeEdgeDeploymentPlanResponseTypeDef",
     {
-        "ExperimentSummaries": List[ExperimentSummaryTypeDef],
+        "EdgeDeploymentPlanArn": str,
+        "EdgeDeploymentPlanName": str,
+        "ModelConfigs": List[EdgeDeploymentModelConfigTypeDef],
+        "DeviceFleetName": str,
+        "EdgeDeploymentSuccess": int,
+        "EdgeDeploymentPending": int,
+        "EdgeDeploymentFailed": int,
+        "Stages": List[DeploymentStageStatusSummaryTypeDef],
         "NextToken": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListFeatureGroupsResponseTypeDef = TypedDict(
-    "ListFeatureGroupsResponseTypeDef",
+ListExperimentsResponseTypeDef = TypedDict(
+    "ListExperimentsResponseTypeDef",
     {
-        "FeatureGroupSummaries": List[FeatureGroupSummaryTypeDef],
+        "ExperimentSummaries": List[ExperimentSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListInferenceExperimentsResponseTypeDef = TypedDict(
-    "ListInferenceExperimentsResponseTypeDef",
+ListFeatureGroupsResponseTypeDef = TypedDict(
+    "ListFeatureGroupsResponseTypeDef",
     {
-        "InferenceExperiments": List[InferenceExperimentSummaryTypeDef],
+        "FeatureGroupSummaries": List[FeatureGroupSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrainingJobsResponseTypeDef = TypedDict(
     "ListTrainingJobsResponseTypeDef",
@@ -14834,18 +13878,14 @@
     {
         "HyperParameterTuningJobSummaries": List[HyperParameterTuningJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-HyperParameterTuningJobWarmStartConfigUnionTypeDef = Union[
-    HyperParameterTuningJobWarmStartConfigTypeDef,
-    HyperParameterTuningJobWarmStartConfigOutputTypeDef,
-]
 AssociationSummaryTypeDef = TypedDict(
     "AssociationSummaryTypeDef",
     {
         "SourceArn": str,
         "DestinationArn": str,
         "SourceType": str,
         "DestinationType": str,
@@ -14879,15 +13919,15 @@
 )
 
 DescribeArtifactResponseTypeDef = TypedDict(
     "DescribeArtifactResponseTypeDef",
     {
         "ArtifactName": str,
         "ArtifactArn": str,
-        "Source": ArtifactSourceOutputTypeDef,
+        "Source": ArtifactSourceTypeDef,
         "ArtifactType": str,
         "Properties": Dict[str, str],
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
@@ -15067,14 +14107,15 @@
         "CreationTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "Tags": List[TagTypeDef],
         "ModelId": str,
         "RiskRating": str,
+        "ModelPackageGroupName": str,
     },
     total=False,
 )
 
 ModelDashboardModelCardTypeDef = TypedDict(
     "ModelDashboardModelCardTypeDef",
     {
@@ -15154,40 +14195,14 @@
         "CreatedBy": UserContextTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
     },
     total=False,
 )
 
-ResourceConfigUnionTypeDef = Union[ResourceConfigTypeDef, ResourceConfigOutputTypeDef]
-_RequiredHyperParameterSpecificationOutputTypeDef = TypedDict(
-    "_RequiredHyperParameterSpecificationOutputTypeDef",
-    {
-        "Name": str,
-        "Type": ParameterTypeType,
-    },
-)
-_OptionalHyperParameterSpecificationOutputTypeDef = TypedDict(
-    "_OptionalHyperParameterSpecificationOutputTypeDef",
-    {
-        "Description": str,
-        "Range": ParameterRangeOutputTypeDef,
-        "IsTunable": bool,
-        "IsRequired": bool,
-        "DefaultValue": str,
-    },
-    total=False,
-)
-
-class HyperParameterSpecificationOutputTypeDef(
-    _RequiredHyperParameterSpecificationOutputTypeDef,
-    _OptionalHyperParameterSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredHyperParameterSpecificationTypeDef = TypedDict(
     "_RequiredHyperParameterSpecificationTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
     },
 )
@@ -15204,40 +14219,14 @@
 )
 
 class HyperParameterSpecificationTypeDef(
     _RequiredHyperParameterSpecificationTypeDef, _OptionalHyperParameterSpecificationTypeDef
 ):
     pass
 
-_RequiredHyperParameterTuningJobConfigOutputTypeDef = TypedDict(
-    "_RequiredHyperParameterTuningJobConfigOutputTypeDef",
-    {
-        "Strategy": HyperParameterTuningJobStrategyTypeType,
-        "ResourceLimits": ResourceLimitsTypeDef,
-    },
-)
-_OptionalHyperParameterTuningJobConfigOutputTypeDef = TypedDict(
-    "_OptionalHyperParameterTuningJobConfigOutputTypeDef",
-    {
-        "StrategyConfig": HyperParameterTuningJobStrategyConfigTypeDef,
-        "HyperParameterTuningJobObjective": HyperParameterTuningJobObjectiveTypeDef,
-        "ParameterRanges": ParameterRangesOutputTypeDef,
-        "TrainingJobEarlyStoppingType": TrainingJobEarlyStoppingTypeType,
-        "TuningJobCompletionCriteria": TuningJobCompletionCriteriaTypeDef,
-        "RandomSeed": int,
-    },
-    total=False,
-)
-
-class HyperParameterTuningJobConfigOutputTypeDef(
-    _RequiredHyperParameterTuningJobConfigOutputTypeDef,
-    _OptionalHyperParameterTuningJobConfigOutputTypeDef,
-):
-    pass
-
 _RequiredHyperParameterTuningJobConfigTypeDef = TypedDict(
     "_RequiredHyperParameterTuningJobConfigTypeDef",
     {
         "Strategy": HyperParameterTuningJobStrategyTypeType,
         "ResourceLimits": ResourceLimitsTypeDef,
     },
 )
@@ -15262,31 +14251,19 @@
 AppImageConfigDetailsTypeDef = TypedDict(
     "AppImageConfigDetailsTypeDef",
     {
         "AppImageConfigArn": str,
         "AppImageConfigName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "KernelGatewayImageConfig": KernelGatewayImageConfigOutputTypeDef,
+        "KernelGatewayImageConfig": KernelGatewayImageConfigTypeDef,
     },
     total=False,
 )
 
-DescribeAppImageConfigResponseTypeDef = TypedDict(
-    "DescribeAppImageConfigResponseTypeDef",
-    {
-        "AppImageConfigArn": str,
-        "AppImageConfigName": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "KernelGatewayImageConfig": KernelGatewayImageConfigOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateAppImageConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppImageConfigRequestRequestTypeDef",
     {
         "AppImageConfigName": str,
     },
 )
 _OptionalCreateAppImageConfigRequestRequestTypeDef = TypedDict(
@@ -15300,17 +14277,26 @@
 
 class CreateAppImageConfigRequestRequestTypeDef(
     _RequiredCreateAppImageConfigRequestRequestTypeDef,
     _OptionalCreateAppImageConfigRequestRequestTypeDef,
 ):
     pass
 
-KernelGatewayImageConfigUnionTypeDef = Union[
-    KernelGatewayImageConfigTypeDef, KernelGatewayImageConfigOutputTypeDef
-]
+DescribeAppImageConfigResponseTypeDef = TypedDict(
+    "DescribeAppImageConfigResponseTypeDef",
+    {
+        "AppImageConfigArn": str,
+        "AppImageConfigName": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "KernelGatewayImageConfig": KernelGatewayImageConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateAppImageConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAppImageConfigRequestRequestTypeDef",
     {
         "AppImageConfigName": str,
     },
 )
 _OptionalUpdateAppImageConfigRequestRequestTypeDef = TypedDict(
@@ -15332,57 +14318,82 @@
     {
         "LabelingJobSummaryList": List[LabelingJobForWorkteamSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLabelingJobInputConfigOutputTypeDef = TypedDict(
-    "_RequiredLabelingJobInputConfigOutputTypeDef",
+_RequiredLabelingJobInputConfigTypeDef = TypedDict(
+    "_RequiredLabelingJobInputConfigTypeDef",
     {
         "DataSource": LabelingJobDataSourceTypeDef,
     },
 )
-_OptionalLabelingJobInputConfigOutputTypeDef = TypedDict(
-    "_OptionalLabelingJobInputConfigOutputTypeDef",
+_OptionalLabelingJobInputConfigTypeDef = TypedDict(
+    "_OptionalLabelingJobInputConfigTypeDef",
     {
-        "DataAttributes": LabelingJobDataAttributesOutputTypeDef,
+        "DataAttributes": LabelingJobDataAttributesTypeDef,
     },
     total=False,
 )
 
-class LabelingJobInputConfigOutputTypeDef(
-    _RequiredLabelingJobInputConfigOutputTypeDef, _OptionalLabelingJobInputConfigOutputTypeDef
+class LabelingJobInputConfigTypeDef(
+    _RequiredLabelingJobInputConfigTypeDef, _OptionalLabelingJobInputConfigTypeDef
 ):
     pass
 
-_RequiredLabelingJobInputConfigTypeDef = TypedDict(
-    "_RequiredLabelingJobInputConfigTypeDef",
+_RequiredCreateWorkteamRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkteamRequestRequestTypeDef",
     {
-        "DataSource": LabelingJobDataSourceTypeDef,
+        "WorkteamName": str,
+        "MemberDefinitions": Sequence[MemberDefinitionTypeDef],
+        "Description": str,
     },
 )
-_OptionalLabelingJobInputConfigTypeDef = TypedDict(
-    "_OptionalLabelingJobInputConfigTypeDef",
+_OptionalCreateWorkteamRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkteamRequestRequestTypeDef",
     {
-        "DataAttributes": LabelingJobDataAttributesTypeDef,
+        "WorkforceName": str,
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class LabelingJobInputConfigTypeDef(
-    _RequiredLabelingJobInputConfigTypeDef, _OptionalLabelingJobInputConfigTypeDef
+class CreateWorkteamRequestRequestTypeDef(
+    _RequiredCreateWorkteamRequestRequestTypeDef, _OptionalCreateWorkteamRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateWorkteamRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateWorkteamRequestRequestTypeDef",
+    {
+        "WorkteamName": str,
+    },
+)
+_OptionalUpdateWorkteamRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateWorkteamRequestRequestTypeDef",
+    {
+        "MemberDefinitions": Sequence[MemberDefinitionTypeDef],
+        "Description": str,
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateWorkteamRequestRequestTypeDef(
+    _RequiredUpdateWorkteamRequestRequestTypeDef, _OptionalUpdateWorkteamRequestRequestTypeDef
 ):
     pass
 
 _RequiredWorkteamTypeDef = TypedDict(
     "_RequiredWorkteamTypeDef",
     {
         "WorkteamName": str,
-        "MemberDefinitions": List[MemberDefinitionOutputTypeDef],
+        "MemberDefinitions": List[MemberDefinitionTypeDef],
         "WorkteamArn": str,
         "Description": str,
     },
 )
 _OptionalWorkteamTypeDef = TypedDict(
     "_OptionalWorkteamTypeDef",
     {
@@ -15395,45 +14406,36 @@
     },
     total=False,
 )
 
 class WorkteamTypeDef(_RequiredWorkteamTypeDef, _OptionalWorkteamTypeDef):
     pass
 
-MemberDefinitionUnionTypeDef = Union[MemberDefinitionTypeDef, MemberDefinitionOutputTypeDef]
+TargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
+    "TargetTrackingScalingPolicyConfigurationTypeDef",
+    {
+        "MetricSpecification": MetricSpecificationTypeDef,
+        "TargetValue": float,
+    },
+    total=False,
+)
+
 MonitoringAlertSummaryTypeDef = TypedDict(
     "MonitoringAlertSummaryTypeDef",
     {
         "MonitoringAlertName": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "AlertStatus": MonitoringAlertStatusType,
         "DatapointsToAlert": int,
         "EvaluationPeriod": int,
         "Actions": MonitoringAlertActionsTypeDef,
     },
 )
 
-ContainerDefinitionOutputTypeDef = TypedDict(
-    "ContainerDefinitionOutputTypeDef",
-    {
-        "ContainerHostname": str,
-        "Image": str,
-        "ImageConfig": ImageConfigTypeDef,
-        "Mode": ContainerModeType,
-        "ModelDataUrl": str,
-        "Environment": Dict[str, str],
-        "ModelPackageName": str,
-        "InferenceSpecificationName": str,
-        "MultiModelConfig": MultiModelConfigTypeDef,
-        "ModelDataSource": ModelDataSourceTypeDef,
-    },
-    total=False,
-)
-
 ContainerDefinitionTypeDef = TypedDict(
     "ContainerDefinitionTypeDef",
     {
         "ContainerHostname": str,
         "Image": str,
         "ImageConfig": ImageConfigTypeDef,
         "Mode": ContainerModeType,
@@ -15462,61 +14464,14 @@
     {
         "ModelName": str,
         "VariantName": str,
         "InfrastructureConfig": ModelInfrastructureConfigTypeDef,
     },
 )
 
-_RequiredAdditionalInferenceSpecificationDefinitionOutputTypeDef = TypedDict(
-    "_RequiredAdditionalInferenceSpecificationDefinitionOutputTypeDef",
-    {
-        "Name": str,
-        "Containers": List[ModelPackageContainerDefinitionOutputTypeDef],
-    },
-)
-_OptionalAdditionalInferenceSpecificationDefinitionOutputTypeDef = TypedDict(
-    "_OptionalAdditionalInferenceSpecificationDefinitionOutputTypeDef",
-    {
-        "Description": str,
-        "SupportedTransformInstanceTypes": List[TransformInstanceTypeType],
-        "SupportedRealtimeInferenceInstanceTypes": List[ProductionVariantInstanceTypeType],
-        "SupportedContentTypes": List[str],
-        "SupportedResponseMIMETypes": List[str],
-    },
-    total=False,
-)
-
-class AdditionalInferenceSpecificationDefinitionOutputTypeDef(
-    _RequiredAdditionalInferenceSpecificationDefinitionOutputTypeDef,
-    _OptionalAdditionalInferenceSpecificationDefinitionOutputTypeDef,
-):
-    pass
-
-_RequiredInferenceSpecificationOutputTypeDef = TypedDict(
-    "_RequiredInferenceSpecificationOutputTypeDef",
-    {
-        "Containers": List[ModelPackageContainerDefinitionOutputTypeDef],
-        "SupportedContentTypes": List[str],
-        "SupportedResponseMIMETypes": List[str],
-    },
-)
-_OptionalInferenceSpecificationOutputTypeDef = TypedDict(
-    "_OptionalInferenceSpecificationOutputTypeDef",
-    {
-        "SupportedTransformInstanceTypes": List[TransformInstanceTypeType],
-        "SupportedRealtimeInferenceInstanceTypes": List[ProductionVariantInstanceTypeType],
-    },
-    total=False,
-)
-
-class InferenceSpecificationOutputTypeDef(
-    _RequiredInferenceSpecificationOutputTypeDef, _OptionalInferenceSpecificationOutputTypeDef
-):
-    pass
-
 _RequiredAdditionalInferenceSpecificationDefinitionTypeDef = TypedDict(
     "_RequiredAdditionalInferenceSpecificationDefinitionTypeDef",
     {
         "Name": str,
         "Containers": Sequence[ModelPackageContainerDefinitionTypeDef],
     },
 )
@@ -15537,36 +14492,33 @@
     _OptionalAdditionalInferenceSpecificationDefinitionTypeDef,
 ):
     pass
 
 _RequiredInferenceSpecificationTypeDef = TypedDict(
     "_RequiredInferenceSpecificationTypeDef",
     {
-        "Containers": Sequence[ModelPackageContainerDefinitionTypeDef],
-        "SupportedContentTypes": Sequence[str],
-        "SupportedResponseMIMETypes": Sequence[str],
+        "Containers": List[ModelPackageContainerDefinitionTypeDef],
+        "SupportedContentTypes": List[str],
+        "SupportedResponseMIMETypes": List[str],
     },
 )
 _OptionalInferenceSpecificationTypeDef = TypedDict(
     "_OptionalInferenceSpecificationTypeDef",
     {
-        "SupportedTransformInstanceTypes": Sequence[TransformInstanceTypeType],
-        "SupportedRealtimeInferenceInstanceTypes": Sequence[ProductionVariantInstanceTypeType],
+        "SupportedTransformInstanceTypes": List[TransformInstanceTypeType],
+        "SupportedRealtimeInferenceInstanceTypes": List[ProductionVariantInstanceTypeType],
     },
     total=False,
 )
 
 class InferenceSpecificationTypeDef(
     _RequiredInferenceSpecificationTypeDef, _OptionalInferenceSpecificationTypeDef
 ):
     pass
 
-RecommendationJobStoppingConditionsUnionTypeDef = Union[
-    RecommendationJobStoppingConditionsTypeDef, RecommendationJobStoppingConditionsOutputTypeDef
-]
 ListModelMetadataRequestListModelMetadataPaginateTypeDef = TypedDict(
     "ListModelMetadataRequestListModelMetadataPaginateTypeDef",
     {
         "SearchExpression": ModelMetadataSearchExpressionTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -15578,42 +14530,14 @@
         "SearchExpression": ModelMetadataSearchExpressionTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredBatchTransformInputOutputTypeDef = TypedDict(
-    "_RequiredBatchTransformInputOutputTypeDef",
-    {
-        "DataCapturedDestinationS3Uri": str,
-        "DatasetFormat": MonitoringDatasetFormatOutputTypeDef,
-        "LocalPath": str,
-    },
-)
-_OptionalBatchTransformInputOutputTypeDef = TypedDict(
-    "_OptionalBatchTransformInputOutputTypeDef",
-    {
-        "S3InputMode": ProcessingS3InputModeType,
-        "S3DataDistributionType": ProcessingS3DataDistributionTypeType,
-        "FeaturesAttribute": str,
-        "InferenceAttribute": str,
-        "ProbabilityAttribute": str,
-        "ProbabilityThresholdAttribute": float,
-        "StartTimeOffset": str,
-        "EndTimeOffset": str,
-    },
-    total=False,
-)
-
-class BatchTransformInputOutputTypeDef(
-    _RequiredBatchTransformInputOutputTypeDef, _OptionalBatchTransformInputOutputTypeDef
-):
-    pass
-
 _RequiredBatchTransformInputTypeDef = TypedDict(
     "_RequiredBatchTransformInputTypeDef",
     {
         "DataCapturedDestinationS3Uri": str,
         "DatasetFormat": MonitoringDatasetFormatTypeDef,
         "LocalPath": str,
     },
@@ -15634,33 +14558,14 @@
 )
 
 class BatchTransformInputTypeDef(
     _RequiredBatchTransformInputTypeDef, _OptionalBatchTransformInputTypeDef
 ):
     pass
 
-_RequiredMonitoringOutputConfigOutputTypeDef = TypedDict(
-    "_RequiredMonitoringOutputConfigOutputTypeDef",
-    {
-        "MonitoringOutputs": List[MonitoringOutputTypeDef],
-    },
-)
-_OptionalMonitoringOutputConfigOutputTypeDef = TypedDict(
-    "_OptionalMonitoringOutputConfigOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class MonitoringOutputConfigOutputTypeDef(
-    _RequiredMonitoringOutputConfigOutputTypeDef, _OptionalMonitoringOutputConfigOutputTypeDef
-):
-    pass
-
 _RequiredMonitoringOutputConfigTypeDef = TypedDict(
     "_RequiredMonitoringOutputConfigTypeDef",
     {
         "MonitoringOutputs": Sequence[MonitoringOutputTypeDef],
     },
 )
 _OptionalMonitoringOutputConfigTypeDef = TypedDict(
@@ -15746,14 +14651,35 @@
         "FailureReason": str,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateFeatureGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFeatureGroupRequestRequestTypeDef",
+    {
+        "FeatureGroupName": str,
+    },
+)
+_OptionalUpdateFeatureGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFeatureGroupRequestRequestTypeDef",
+    {
+        "FeatureAdditions": Sequence[FeatureDefinitionTypeDef],
+        "OnlineStoreConfig": OnlineStoreConfigUpdateTypeDef,
+    },
+    total=False,
+)
+
+class UpdateFeatureGroupRequestRequestTypeDef(
+    _RequiredUpdateFeatureGroupRequestRequestTypeDef,
+    _OptionalUpdateFeatureGroupRequestRequestTypeDef,
+):
+    pass
+
 _RequiredCreateCompilationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCompilationJobRequestRequestTypeDef",
     {
         "CompilationJobName": str,
         "RoleArn": str,
         "OutputConfig": OutputConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
@@ -15791,15 +14717,15 @@
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "ModelArtifacts": ModelArtifactsTypeDef,
         "ModelDigests": ModelDigestsTypeDef,
         "RoleArn": str,
         "InputConfig": InputConfigTypeDef,
         "OutputConfig": OutputConfigTypeDef,
-        "VpcConfig": NeoVpcConfigOutputTypeDef,
+        "VpcConfig": NeoVpcConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPendingDeploymentSummaryTypeDef = TypedDict(
     "_RequiredPendingDeploymentSummaryTypeDef",
     {
@@ -15817,33 +14743,14 @@
 )
 
 class PendingDeploymentSummaryTypeDef(
     _RequiredPendingDeploymentSummaryTypeDef, _OptionalPendingDeploymentSummaryTypeDef
 ):
     pass
 
-_RequiredProcessingOutputConfigOutputTypeDef = TypedDict(
-    "_RequiredProcessingOutputConfigOutputTypeDef",
-    {
-        "Outputs": List[ProcessingOutputTypeDef],
-    },
-)
-_OptionalProcessingOutputConfigOutputTypeDef = TypedDict(
-    "_OptionalProcessingOutputConfigOutputTypeDef",
-    {
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class ProcessingOutputConfigOutputTypeDef(
-    _RequiredProcessingOutputConfigOutputTypeDef, _OptionalProcessingOutputConfigOutputTypeDef
-):
-    pass
-
 _RequiredProcessingOutputConfigTypeDef = TypedDict(
     "_RequiredProcessingOutputConfigTypeDef",
     {
         "Outputs": Sequence[ProcessingOutputTypeDef],
     },
 )
 _OptionalProcessingOutputConfigTypeDef = TypedDict(
@@ -15855,63 +14762,63 @@
 )
 
 class ProcessingOutputConfigTypeDef(
     _RequiredProcessingOutputConfigTypeDef, _OptionalProcessingOutputConfigTypeDef
 ):
     pass
 
-_RequiredUpdateTrainingJobRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateTrainingJobRequestRequestTypeDef",
+_RequiredGetSearchSuggestionsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetSearchSuggestionsRequestRequestTypeDef",
     {
-        "TrainingJobName": str,
+        "Resource": ResourceTypeType,
     },
 )
-_OptionalUpdateTrainingJobRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateTrainingJobRequestRequestTypeDef",
+_OptionalGetSearchSuggestionsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetSearchSuggestionsRequestRequestTypeDef",
     {
-        "ProfilerConfig": ProfilerConfigForUpdateTypeDef,
-        "ProfilerRuleConfigurations": Sequence[ProfilerRuleConfigurationUnionTypeDef],
-        "ResourceConfig": ResourceConfigForUpdateTypeDef,
+        "SuggestionQuery": SuggestionQueryTypeDef,
     },
     total=False,
 )
 
-class UpdateTrainingJobRequestRequestTypeDef(
-    _RequiredUpdateTrainingJobRequestRequestTypeDef, _OptionalUpdateTrainingJobRequestRequestTypeDef
+class GetSearchSuggestionsRequestRequestTypeDef(
+    _RequiredGetSearchSuggestionsRequestRequestTypeDef,
+    _OptionalGetSearchSuggestionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetSearchSuggestionsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetSearchSuggestionsRequestRequestTypeDef",
+_RequiredCreateProjectInputRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectInputRequestTypeDef",
     {
-        "Resource": ResourceTypeType,
+        "ProjectName": str,
+        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
     },
 )
-_OptionalGetSearchSuggestionsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetSearchSuggestionsRequestRequestTypeDef",
+_OptionalCreateProjectInputRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectInputRequestTypeDef",
     {
-        "SuggestionQuery": SuggestionQueryTypeDef,
+        "ProjectDescription": str,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class GetSearchSuggestionsRequestRequestTypeDef(
-    _RequiredGetSearchSuggestionsRequestRequestTypeDef,
-    _OptionalGetSearchSuggestionsRequestRequestTypeDef,
+class CreateProjectInputRequestTypeDef(
+    _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
 ):
     pass
 
 DescribeProjectOutputTypeDef = TypedDict(
     "DescribeProjectOutputTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "ProjectId": str,
         "ProjectDescription": str,
-        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsOutputTypeDef,
+        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
         "ServiceCatalogProvisionedProductDetails": ServiceCatalogProvisionedProductDetailsTypeDef,
         "ProjectStatus": ProjectStatusType,
         "CreatedBy": UserContextTypeDef,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -15921,50 +14828,26 @@
 ProjectTypeDef = TypedDict(
     "ProjectTypeDef",
     {
         "ProjectArn": str,
         "ProjectName": str,
         "ProjectId": str,
         "ProjectDescription": str,
-        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsOutputTypeDef,
+        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
         "ServiceCatalogProvisionedProductDetails": ServiceCatalogProvisionedProductDetailsTypeDef,
         "ProjectStatus": ProjectStatusType,
         "CreatedBy": UserContextTypeDef,
         "CreationTime": datetime,
         "Tags": List[TagTypeDef],
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateProjectInputRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectInputRequestTypeDef",
-    {
-        "ProjectName": str,
-        "ServiceCatalogProvisioningDetails": ServiceCatalogProvisioningDetailsTypeDef,
-    },
-)
-_OptionalCreateProjectInputRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectInputRequestTypeDef",
-    {
-        "ProjectDescription": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateProjectInputRequestTypeDef(
-    _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
-):
-    pass
-
-ServiceCatalogProvisioningDetailsUnionTypeDef = Union[
-    ServiceCatalogProvisioningDetailsTypeDef, ServiceCatalogProvisioningDetailsOutputTypeDef
-]
 _RequiredUpdateProjectInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectInputRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 _OptionalUpdateProjectInputRequestTypeDef = TypedDict(
@@ -15978,40 +14861,14 @@
 )
 
 class UpdateProjectInputRequestTypeDef(
     _RequiredUpdateProjectInputRequestTypeDef, _OptionalUpdateProjectInputRequestTypeDef
 ):
     pass
 
-_RequiredHumanLoopConfigOutputTypeDef = TypedDict(
-    "_RequiredHumanLoopConfigOutputTypeDef",
-    {
-        "WorkteamArn": str,
-        "HumanTaskUiArn": str,
-        "TaskTitle": str,
-        "TaskDescription": str,
-        "TaskCount": int,
-    },
-)
-_OptionalHumanLoopConfigOutputTypeDef = TypedDict(
-    "_OptionalHumanLoopConfigOutputTypeDef",
-    {
-        "TaskAvailabilityLifetimeInSeconds": int,
-        "TaskTimeLimitInSeconds": int,
-        "TaskKeywords": List[str],
-        "PublicWorkforceTaskPrice": PublicWorkforceTaskPriceTypeDef,
-    },
-    total=False,
-)
-
-class HumanLoopConfigOutputTypeDef(
-    _RequiredHumanLoopConfigOutputTypeDef, _OptionalHumanLoopConfigOutputTypeDef
-):
-    pass
-
 _RequiredHumanLoopConfigTypeDef = TypedDict(
     "_RequiredHumanLoopConfigTypeDef",
     {
         "WorkteamArn": str,
         "HumanTaskUiArn": str,
         "TaskTitle": str,
         "TaskDescription": str,
@@ -16028,43 +14885,14 @@
     },
     total=False,
 )
 
 class HumanLoopConfigTypeDef(_RequiredHumanLoopConfigTypeDef, _OptionalHumanLoopConfigTypeDef):
     pass
 
-_RequiredHumanTaskConfigOutputTypeDef = TypedDict(
-    "_RequiredHumanTaskConfigOutputTypeDef",
-    {
-        "WorkteamArn": str,
-        "UiConfig": UiConfigTypeDef,
-        "PreHumanTaskLambdaArn": str,
-        "TaskTitle": str,
-        "TaskDescription": str,
-        "NumberOfHumanWorkersPerDataObject": int,
-        "TaskTimeLimitInSeconds": int,
-        "AnnotationConsolidationConfig": AnnotationConsolidationConfigTypeDef,
-    },
-)
-_OptionalHumanTaskConfigOutputTypeDef = TypedDict(
-    "_OptionalHumanTaskConfigOutputTypeDef",
-    {
-        "TaskKeywords": List[str],
-        "TaskAvailabilityLifetimeInSeconds": int,
-        "MaxConcurrentTaskCount": int,
-        "PublicWorkforceTaskPrice": PublicWorkforceTaskPriceTypeDef,
-    },
-    total=False,
-)
-
-class HumanTaskConfigOutputTypeDef(
-    _RequiredHumanTaskConfigOutputTypeDef, _OptionalHumanTaskConfigOutputTypeDef
-):
-    pass
-
 _RequiredHumanTaskConfigTypeDef = TypedDict(
     "_RequiredHumanTaskConfigTypeDef",
     {
         "WorkteamArn": str,
         "UiConfig": UiConfigTypeDef,
         "PreHumanTaskLambdaArn": str,
         "TaskTitle": str,
@@ -16099,15 +14927,15 @@
         "PipelineExperimentConfig": PipelineExperimentConfigTypeDef,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedBy": UserContextTypeDef,
         "ParallelismConfiguration": ParallelismConfigurationTypeDef,
-        "SelectiveExecutionConfig": SelectiveExecutionConfigOutputTypeDef,
+        "SelectiveExecutionConfig": SelectiveExecutionConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PipelineExecutionTypeDef = TypedDict(
     "PipelineExecutionTypeDef",
     {
@@ -16120,22 +14948,19 @@
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "CreatedBy": UserContextTypeDef,
         "LastModifiedBy": UserContextTypeDef,
         "ParallelismConfiguration": ParallelismConfigurationTypeDef,
         "PipelineParameters": List[ParameterTypeDef],
-        "SelectiveExecutionConfig": SelectiveExecutionConfigOutputTypeDef,
+        "SelectiveExecutionConfig": SelectiveExecutionConfigTypeDef,
     },
     total=False,
 )
 
-SelectiveExecutionConfigUnionTypeDef = Union[
-    SelectiveExecutionConfigTypeDef, SelectiveExecutionConfigOutputTypeDef
-]
 _RequiredStartPipelineExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartPipelineExecutionRequestRequestTypeDef",
     {
         "PipelineName": str,
         "ClientRequestToken": str,
     },
 )
@@ -16153,43 +14978,14 @@
 
 class StartPipelineExecutionRequestRequestTypeDef(
     _RequiredStartPipelineExecutionRequestRequestTypeDef,
     _OptionalStartPipelineExecutionRequestRequestTypeDef,
 ):
     pass
 
-ShadowModeConfigUnionTypeDef = Union[ShadowModeConfigTypeDef, ShadowModeConfigOutputTypeDef]
-SourceAlgorithmSpecificationUnionTypeDef = Union[
-    SourceAlgorithmSpecificationTypeDef, SourceAlgorithmSpecificationOutputTypeDef
-]
-_RequiredAlgorithmSpecificationOutputTypeDef = TypedDict(
-    "_RequiredAlgorithmSpecificationOutputTypeDef",
-    {
-        "TrainingInputMode": TrainingInputModeType,
-    },
-)
-_OptionalAlgorithmSpecificationOutputTypeDef = TypedDict(
-    "_OptionalAlgorithmSpecificationOutputTypeDef",
-    {
-        "TrainingImage": str,
-        "AlgorithmName": str,
-        "MetricDefinitions": List[MetricDefinitionTypeDef],
-        "EnableSageMakerMetricsTimeSeries": bool,
-        "ContainerEntrypoint": List[str],
-        "ContainerArguments": List[str],
-        "TrainingImageConfig": TrainingImageConfigTypeDef,
-    },
-    total=False,
-)
-
-class AlgorithmSpecificationOutputTypeDef(
-    _RequiredAlgorithmSpecificationOutputTypeDef, _OptionalAlgorithmSpecificationOutputTypeDef
-):
-    pass
-
 _RequiredAlgorithmSpecificationTypeDef = TypedDict(
     "_RequiredAlgorithmSpecificationTypeDef",
     {
         "TrainingInputMode": TrainingInputModeType,
     },
 )
 _OptionalAlgorithmSpecificationTypeDef = TypedDict(
@@ -16260,38 +15056,25 @@
     {
         "ArtifactSummaries": List[ArtifactSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AsyncInferenceConfigUnionTypeDef = Union[
-    AsyncInferenceConfigTypeDef, AsyncInferenceConfigOutputTypeDef
-]
-AutoMLProblemTypeConfigOutputTypeDef = TypedDict(
-    "AutoMLProblemTypeConfigOutputTypeDef",
-    {
-        "ImageClassificationJobConfig": ImageClassificationJobConfigTypeDef,
-        "TextClassificationJobConfig": TextClassificationJobConfigTypeDef,
-        "TabularJobConfig": TabularJobConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 AutoMLProblemTypeConfigTypeDef = TypedDict(
     "AutoMLProblemTypeConfigTypeDef",
     {
         "ImageClassificationJobConfig": ImageClassificationJobConfigTypeDef,
         "TextClassificationJobConfig": TextClassificationJobConfigTypeDef,
         "TabularJobConfig": TabularJobConfigTypeDef,
+        "TimeSeriesForecastingJobConfig": TimeSeriesForecastingJobConfigTypeDef,
     },
     total=False,
 )
 
-AutoMLJobConfigUnionTypeDef = Union[AutoMLJobConfigTypeDef, AutoMLJobConfigOutputTypeDef]
 _RequiredCreateAutoMLJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoMLJobRequestRequestTypeDef",
     {
         "AutoMLJobName": str,
         "InputDataConfig": Sequence[AutoMLChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
@@ -16311,17 +15094,14 @@
 )
 
 class CreateAutoMLJobRequestRequestTypeDef(
     _RequiredCreateAutoMLJobRequestRequestTypeDef, _OptionalCreateAutoMLJobRequestRequestTypeDef
 ):
     pass
 
-LabelingJobAlgorithmsConfigUnionTypeDef = Union[
-    LabelingJobAlgorithmsConfigTypeDef, LabelingJobAlgorithmsConfigOutputTypeDef
-]
 PipelineExecutionStepTypeDef = TypedDict(
     "PipelineExecutionStepTypeDef",
     {
         "StepName": str,
         "StepDisplayName": str,
         "StepDescription": str,
         "StartTime": datetime,
@@ -16342,15 +15122,15 @@
         "AutoMLJobName": str,
         "AutoMLJobArn": str,
         "InputDataConfig": List[AutoMLChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "RoleArn": str,
         "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
         "ProblemType": ProblemTypeType,
-        "AutoMLJobConfig": AutoMLJobConfigOutputTypeDef,
+        "AutoMLJobConfig": AutoMLJobConfigTypeDef,
         "CreationTime": datetime,
         "EndTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
         "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
         "BestCandidate": AutoMLCandidateTypeDef,
         "AutoMLJobStatus": AutoMLJobStatusType,
@@ -16369,63 +15149,20 @@
     {
         "Candidates": List[AutoMLCandidateTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDeploymentConfigOutputTypeDef = TypedDict(
-    "_RequiredDeploymentConfigOutputTypeDef",
-    {
-        "BlueGreenUpdatePolicy": BlueGreenUpdatePolicyTypeDef,
-    },
-)
-_OptionalDeploymentConfigOutputTypeDef = TypedDict(
-    "_OptionalDeploymentConfigOutputTypeDef",
-    {
-        "AutoRollbackConfiguration": AutoRollbackConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class DeploymentConfigOutputTypeDef(
-    _RequiredDeploymentConfigOutputTypeDef, _OptionalDeploymentConfigOutputTypeDef
-):
-    pass
-
-_RequiredDeploymentConfigTypeDef = TypedDict(
-    "_RequiredDeploymentConfigTypeDef",
+DeploymentConfigTypeDef = TypedDict(
+    "DeploymentConfigTypeDef",
     {
         "BlueGreenUpdatePolicy": BlueGreenUpdatePolicyTypeDef,
-    },
-)
-_OptionalDeploymentConfigTypeDef = TypedDict(
-    "_OptionalDeploymentConfigTypeDef",
-    {
         "AutoRollbackConfiguration": AutoRollbackConfigTypeDef,
-    },
-    total=False,
-)
-
-class DeploymentConfigTypeDef(_RequiredDeploymentConfigTypeDef, _OptionalDeploymentConfigTypeDef):
-    pass
-
-RecommendationJobInputConfigOutputTypeDef = TypedDict(
-    "RecommendationJobInputConfigOutputTypeDef",
-    {
-        "ModelPackageVersionArn": str,
-        "JobDurationInSeconds": int,
-        "TrafficPattern": TrafficPatternOutputTypeDef,
-        "ResourceLimit": RecommendationJobResourceLimitTypeDef,
-        "EndpointConfigurations": List[EndpointInputConfigurationOutputTypeDef],
-        "VolumeKmsKeyId": str,
-        "ContainerConfig": RecommendationJobContainerConfigOutputTypeDef,
-        "Endpoints": List[EndpointInfoTypeDef],
-        "VpcConfig": RecommendationJobVpcConfigOutputTypeDef,
-        "ModelName": str,
+        "RollingUpdatePolicy": RollingUpdatePolicyTypeDef,
     },
     total=False,
 )
 
 RecommendationJobInputConfigTypeDef = TypedDict(
     "RecommendationJobInputConfigTypeDef",
     {
@@ -16439,50 +15176,31 @@
         "Endpoints": Sequence[EndpointInfoTypeDef],
         "VpcConfig": RecommendationJobVpcConfigTypeDef,
         "ModelName": str,
     },
     total=False,
 )
 
-ExplainerConfigOutputTypeDef = TypedDict(
-    "ExplainerConfigOutputTypeDef",
-    {
-        "ClarifyExplainerConfig": ClarifyExplainerConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ExplainerConfigTypeDef = TypedDict(
     "ExplainerConfigTypeDef",
     {
         "ClarifyExplainerConfig": ClarifyExplainerConfigTypeDef,
     },
     total=False,
 )
 
-DomainSettingsUnionTypeDef = Union[DomainSettingsTypeDef, DomainSettingsOutputTypeDef]
-DescribeSpaceResponseTypeDef = TypedDict(
-    "DescribeSpaceResponseTypeDef",
+ListInferenceExperimentsResponseTypeDef = TypedDict(
+    "ListInferenceExperimentsResponseTypeDef",
     {
-        "DomainId": str,
-        "SpaceArn": str,
-        "SpaceName": str,
-        "HomeEfsFileSystemUid": str,
-        "Status": SpaceStatusType,
-        "LastModifiedTime": datetime,
-        "CreationTime": datetime,
-        "FailureReason": str,
-        "SpaceSettings": SpaceSettingsOutputTypeDef,
+        "InferenceExperiments": List[InferenceExperimentSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DefaultSpaceSettingsUnionTypeDef = Union[
-    DefaultSpaceSettingsTypeDef, DefaultSpaceSettingsOutputTypeDef
-]
 _RequiredCreateSpaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSpaceRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpaceName": str,
     },
 )
@@ -16496,15 +15214,30 @@
 )
 
 class CreateSpaceRequestRequestTypeDef(
     _RequiredCreateSpaceRequestRequestTypeDef, _OptionalCreateSpaceRequestRequestTypeDef
 ):
     pass
 
-SpaceSettingsUnionTypeDef = Union[SpaceSettingsTypeDef, SpaceSettingsOutputTypeDef]
+DescribeSpaceResponseTypeDef = TypedDict(
+    "DescribeSpaceResponseTypeDef",
+    {
+        "DomainId": str,
+        "SpaceArn": str,
+        "SpaceName": str,
+        "HomeEfsFileSystemUid": str,
+        "Status": SpaceStatusType,
+        "LastModifiedTime": datetime,
+        "CreationTime": datetime,
+        "FailureReason": str,
+        "SpaceSettings": SpaceSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateSpaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSpaceRequestRequestTypeDef",
     {
         "DomainId": str,
         "SpaceName": str,
     },
 )
@@ -16517,60 +15250,14 @@
 )
 
 class UpdateSpaceRequestRequestTypeDef(
     _RequiredUpdateSpaceRequestRequestTypeDef, _OptionalUpdateSpaceRequestRequestTypeDef
 ):
     pass
 
-DescribeDomainResponseTypeDef = TypedDict(
-    "DescribeDomainResponseTypeDef",
-    {
-        "DomainArn": str,
-        "DomainId": str,
-        "DomainName": str,
-        "HomeEfsFileSystemId": str,
-        "SingleSignOnManagedApplicationInstanceId": str,
-        "Status": DomainStatusType,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "AuthMode": AuthModeType,
-        "DefaultUserSettings": UserSettingsOutputTypeDef,
-        "AppNetworkAccessType": AppNetworkAccessTypeType,
-        "HomeEfsFileSystemKmsKeyId": str,
-        "SubnetIds": List[str],
-        "Url": str,
-        "VpcId": str,
-        "KmsKeyId": str,
-        "DomainSettings": DomainSettingsOutputTypeDef,
-        "AppSecurityGroupManagement": AppSecurityGroupManagementType,
-        "SecurityGroupIdForDomainBoundary": str,
-        "DefaultSpaceSettings": DefaultSpaceSettingsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeUserProfileResponseTypeDef = TypedDict(
-    "DescribeUserProfileResponseTypeDef",
-    {
-        "DomainId": str,
-        "UserProfileArn": str,
-        "UserProfileName": str,
-        "HomeEfsFileSystemUid": str,
-        "Status": UserProfileStatusType,
-        "LastModifiedTime": datetime,
-        "CreationTime": datetime,
-        "FailureReason": str,
-        "SingleSignOnUserIdentifier": str,
-        "SingleSignOnUserValue": str,
-        "UserSettings": UserSettingsOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "AuthMode": AuthModeType,
         "DefaultUserSettings": UserSettingsTypeDef,
         "SubnetIds": Sequence[str],
@@ -16615,14 +15302,60 @@
 )
 
 class CreateUserProfileRequestRequestTypeDef(
     _RequiredCreateUserProfileRequestRequestTypeDef, _OptionalCreateUserProfileRequestRequestTypeDef
 ):
     pass
 
+DescribeDomainResponseTypeDef = TypedDict(
+    "DescribeDomainResponseTypeDef",
+    {
+        "DomainArn": str,
+        "DomainId": str,
+        "DomainName": str,
+        "HomeEfsFileSystemId": str,
+        "SingleSignOnManagedApplicationInstanceId": str,
+        "Status": DomainStatusType,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "AuthMode": AuthModeType,
+        "DefaultUserSettings": UserSettingsTypeDef,
+        "AppNetworkAccessType": AppNetworkAccessTypeType,
+        "HomeEfsFileSystemKmsKeyId": str,
+        "SubnetIds": List[str],
+        "Url": str,
+        "VpcId": str,
+        "KmsKeyId": str,
+        "DomainSettings": DomainSettingsTypeDef,
+        "AppSecurityGroupManagement": AppSecurityGroupManagementType,
+        "SecurityGroupIdForDomainBoundary": str,
+        "DefaultSpaceSettings": DefaultSpaceSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeUserProfileResponseTypeDef = TypedDict(
+    "DescribeUserProfileResponseTypeDef",
+    {
+        "DomainId": str,
+        "UserProfileArn": str,
+        "UserProfileName": str,
+        "HomeEfsFileSystemUid": str,
+        "Status": UserProfileStatusType,
+        "LastModifiedTime": datetime,
+        "CreationTime": datetime,
+        "FailureReason": str,
+        "SingleSignOnUserIdentifier": str,
+        "SingleSignOnUserValue": str,
+        "UserSettings": UserSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDomainRequestRequestTypeDef",
     {
         "DomainId": str,
     },
 )
 _OptionalUpdateDomainRequestRequestTypeDef = TypedDict(
@@ -16657,75 +15390,14 @@
 )
 
 class UpdateUserProfileRequestRequestTypeDef(
     _RequiredUpdateUserProfileRequestRequestTypeDef, _OptionalUpdateUserProfileRequestRequestTypeDef
 ):
     pass
 
-UserSettingsUnionTypeDef = Union[UserSettingsTypeDef, UserSettingsOutputTypeDef]
-_RequiredHyperParameterTrainingJobDefinitionOutputTypeDef = TypedDict(
-    "_RequiredHyperParameterTrainingJobDefinitionOutputTypeDef",
-    {
-        "AlgorithmSpecification": HyperParameterAlgorithmSpecificationOutputTypeDef,
-        "RoleArn": str,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "StoppingCondition": StoppingConditionTypeDef,
-    },
-)
-_OptionalHyperParameterTrainingJobDefinitionOutputTypeDef = TypedDict(
-    "_OptionalHyperParameterTrainingJobDefinitionOutputTypeDef",
-    {
-        "DefinitionName": str,
-        "TuningObjective": HyperParameterTuningJobObjectiveTypeDef,
-        "HyperParameterRanges": ParameterRangesOutputTypeDef,
-        "StaticHyperParameters": Dict[str, str],
-        "InputDataConfig": List[ChannelOutputTypeDef],
-        "VpcConfig": VpcConfigOutputTypeDef,
-        "ResourceConfig": ResourceConfigOutputTypeDef,
-        "EnableNetworkIsolation": bool,
-        "EnableInterContainerTrafficEncryption": bool,
-        "EnableManagedSpotTraining": bool,
-        "CheckpointConfig": CheckpointConfigTypeDef,
-        "RetryStrategy": RetryStrategyTypeDef,
-        "HyperParameterTuningResourceConfig": HyperParameterTuningResourceConfigOutputTypeDef,
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-class HyperParameterTrainingJobDefinitionOutputTypeDef(
-    _RequiredHyperParameterTrainingJobDefinitionOutputTypeDef,
-    _OptionalHyperParameterTrainingJobDefinitionOutputTypeDef,
-):
-    pass
-
-_RequiredTrainingJobDefinitionOutputTypeDef = TypedDict(
-    "_RequiredTrainingJobDefinitionOutputTypeDef",
-    {
-        "TrainingInputMode": TrainingInputModeType,
-        "InputDataConfig": List[ChannelOutputTypeDef],
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigOutputTypeDef,
-        "StoppingCondition": StoppingConditionTypeDef,
-    },
-)
-_OptionalTrainingJobDefinitionOutputTypeDef = TypedDict(
-    "_OptionalTrainingJobDefinitionOutputTypeDef",
-    {
-        "HyperParameters": Dict[str, str],
-    },
-    total=False,
-)
-
-class TrainingJobDefinitionOutputTypeDef(
-    _RequiredTrainingJobDefinitionOutputTypeDef, _OptionalTrainingJobDefinitionOutputTypeDef
-):
-    pass
-
-ChannelUnionTypeDef = Union[ChannelTypeDef, ChannelOutputTypeDef]
 _RequiredHyperParameterTrainingJobDefinitionTypeDef = TypedDict(
     "_RequiredHyperParameterTrainingJobDefinitionTypeDef",
     {
         "AlgorithmSpecification": HyperParameterAlgorithmSpecificationTypeDef,
         "RoleArn": str,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
@@ -16835,39 +15507,14 @@
     {
         "TrialComponentSummaries": List[TrialComponentSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTrainingSpecificationOutputTypeDef = TypedDict(
-    "_RequiredTrainingSpecificationOutputTypeDef",
-    {
-        "TrainingImage": str,
-        "SupportedTrainingInstanceTypes": List[TrainingInstanceTypeType],
-        "TrainingChannels": List[ChannelSpecificationOutputTypeDef],
-    },
-)
-_OptionalTrainingSpecificationOutputTypeDef = TypedDict(
-    "_OptionalTrainingSpecificationOutputTypeDef",
-    {
-        "TrainingImageDigest": str,
-        "SupportedHyperParameters": List[HyperParameterSpecificationOutputTypeDef],
-        "SupportsDistributedTraining": bool,
-        "MetricDefinitions": List[MetricDefinitionTypeDef],
-        "SupportedTuningJobObjectiveMetrics": List[HyperParameterTuningJobObjectiveTypeDef],
-    },
-    total=False,
-)
-
-class TrainingSpecificationOutputTypeDef(
-    _RequiredTrainingSpecificationOutputTypeDef, _OptionalTrainingSpecificationOutputTypeDef
-):
-    pass
-
 _RequiredTrainingSpecificationTypeDef = TypedDict(
     "_RequiredTrainingSpecificationTypeDef",
     {
         "TrainingImage": str,
         "SupportedTrainingInstanceTypes": Sequence[TrainingInstanceTypeType],
         "TrainingChannels": Sequence[ChannelSpecificationTypeDef],
     },
@@ -16885,17 +15532,14 @@
 )
 
 class TrainingSpecificationTypeDef(
     _RequiredTrainingSpecificationTypeDef, _OptionalTrainingSpecificationTypeDef
 ):
     pass
 
-HyperParameterTuningJobConfigUnionTypeDef = Union[
-    HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
-]
 ListAppImageConfigsResponseTypeDef = TypedDict(
     "ListAppImageConfigsResponseTypeDef",
     {
         "NextToken": str,
         "AppImageConfigs": List[AppImageConfigDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -16916,27 +15560,24 @@
 )
 _OptionalLabelingJobSummaryTypeDef = TypedDict(
     "_OptionalLabelingJobSummaryTypeDef",
     {
         "AnnotationConsolidationLambdaArn": str,
         "FailureReason": str,
         "LabelingJobOutput": LabelingJobOutputTypeDef,
-        "InputConfig": LabelingJobInputConfigOutputTypeDef,
+        "InputConfig": LabelingJobInputConfigTypeDef,
     },
     total=False,
 )
 
 class LabelingJobSummaryTypeDef(
     _RequiredLabelingJobSummaryTypeDef, _OptionalLabelingJobSummaryTypeDef
 ):
     pass
 
-LabelingJobInputConfigUnionTypeDef = Union[
-    LabelingJobInputConfigTypeDef, LabelingJobInputConfigOutputTypeDef
-]
 DescribeWorkteamResponseTypeDef = TypedDict(
     "DescribeWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -16954,123 +15595,109 @@
     "UpdateWorkteamResponseTypeDef",
     {
         "Workteam": WorkteamTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateWorkteamRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkteamRequestRequestTypeDef",
+ScalingPolicyTypeDef = TypedDict(
+    "ScalingPolicyTypeDef",
     {
-        "WorkteamName": str,
-        "MemberDefinitions": Sequence[MemberDefinitionUnionTypeDef],
-        "Description": str,
+        "TargetTracking": TargetTrackingScalingPolicyConfigurationTypeDef,
     },
+    total=False,
 )
-_OptionalCreateWorkteamRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkteamRequestRequestTypeDef",
+
+ListMonitoringAlertsResponseTypeDef = TypedDict(
+    "ListMonitoringAlertsResponseTypeDef",
     {
-        "WorkforceName": str,
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "Tags": Sequence[TagTypeDef],
+        "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateWorkteamRequestRequestTypeDef(
-    _RequiredCreateWorkteamRequestRequestTypeDef, _OptionalCreateWorkteamRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateWorkteamRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateWorkteamRequestRequestTypeDef",
+_RequiredCreateModelInputRequestTypeDef = TypedDict(
+    "_RequiredCreateModelInputRequestTypeDef",
     {
-        "WorkteamName": str,
+        "ModelName": str,
+        "ExecutionRoleArn": str,
     },
 )
-_OptionalUpdateWorkteamRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateWorkteamRequestRequestTypeDef",
+_OptionalCreateModelInputRequestTypeDef = TypedDict(
+    "_OptionalCreateModelInputRequestTypeDef",
     {
-        "MemberDefinitions": Sequence[MemberDefinitionUnionTypeDef],
-        "Description": str,
-        "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "PrimaryContainer": ContainerDefinitionTypeDef,
+        "Containers": Sequence[ContainerDefinitionTypeDef],
+        "InferenceExecutionConfig": InferenceExecutionConfigTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "VpcConfig": VpcConfigTypeDef,
+        "EnableNetworkIsolation": bool,
     },
     total=False,
 )
 
-class UpdateWorkteamRequestRequestTypeDef(
-    _RequiredUpdateWorkteamRequestRequestTypeDef, _OptionalUpdateWorkteamRequestRequestTypeDef
+class CreateModelInputRequestTypeDef(
+    _RequiredCreateModelInputRequestTypeDef, _OptionalCreateModelInputRequestTypeDef
 ):
     pass
 
-ListMonitoringAlertsResponseTypeDef = TypedDict(
-    "ListMonitoringAlertsResponseTypeDef",
-    {
-        "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeModelOutputTypeDef = TypedDict(
     "DescribeModelOutputTypeDef",
     {
         "ModelName": str,
-        "PrimaryContainer": ContainerDefinitionOutputTypeDef,
-        "Containers": List[ContainerDefinitionOutputTypeDef],
+        "PrimaryContainer": ContainerDefinitionTypeDef,
+        "Containers": List[ContainerDefinitionTypeDef],
         "InferenceExecutionConfig": InferenceExecutionConfigTypeDef,
         "ExecutionRoleArn": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "CreationTime": datetime,
         "ModelArn": str,
         "EnableNetworkIsolation": bool,
         "DeploymentRecommendation": DeploymentRecommendationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelTypeDef = TypedDict(
     "ModelTypeDef",
     {
         "ModelName": str,
-        "PrimaryContainer": ContainerDefinitionOutputTypeDef,
-        "Containers": List[ContainerDefinitionOutputTypeDef],
+        "PrimaryContainer": ContainerDefinitionTypeDef,
+        "Containers": List[ContainerDefinitionTypeDef],
         "InferenceExecutionConfig": InferenceExecutionConfigTypeDef,
         "ExecutionRoleArn": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "CreationTime": datetime,
         "ModelArn": str,
         "EnableNetworkIsolation": bool,
         "Tags": List[TagTypeDef],
         "DeploymentRecommendation": DeploymentRecommendationTypeDef,
     },
     total=False,
 )
 
-ContainerDefinitionUnionTypeDef = Union[
-    ContainerDefinitionTypeDef, ContainerDefinitionOutputTypeDef
-]
 DescribeInferenceExperimentResponseTypeDef = TypedDict(
     "DescribeInferenceExperimentResponseTypeDef",
     {
         "Arn": str,
         "Name": str,
         "Type": Literal["ShadowMode"],
-        "Schedule": InferenceExperimentScheduleOutputTypeDef,
+        "Schedule": InferenceExperimentScheduleTypeDef,
         "Status": InferenceExperimentStatusType,
         "StatusReason": str,
         "Description": str,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "LastModifiedTime": datetime,
         "RoleArn": str,
         "EndpointMetadata": EndpointMetadataTypeDef,
         "ModelVariants": List[ModelVariantConfigSummaryTypeDef],
-        "DataStorageConfig": InferenceExperimentDataStorageConfigOutputTypeDef,
-        "ShadowModeConfig": ShadowModeConfigOutputTypeDef,
+        "DataStorageConfig": InferenceExperimentDataStorageConfigTypeDef,
+        "ShadowModeConfig": ShadowModeConfigTypeDef,
         "KmsKey": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateInferenceExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInferenceExperimentRequestRequestTypeDef",
@@ -17144,21 +15771,46 @@
 
 class UpdateInferenceExperimentRequestRequestTypeDef(
     _RequiredUpdateInferenceExperimentRequestRequestTypeDef,
     _OptionalUpdateInferenceExperimentRequestRequestTypeDef,
 ):
     pass
 
+_RequiredUpdateModelPackageInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateModelPackageInputRequestTypeDef",
+    {
+        "ModelPackageArn": str,
+    },
+)
+_OptionalUpdateModelPackageInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateModelPackageInputRequestTypeDef",
+    {
+        "ModelApprovalStatus": ModelApprovalStatusType,
+        "ApprovalDescription": str,
+        "CustomerMetadataProperties": Mapping[str, str],
+        "CustomerMetadataPropertiesToRemove": Sequence[str],
+        "AdditionalInferenceSpecificationsToAdd": Sequence[
+            AdditionalInferenceSpecificationDefinitionTypeDef
+        ],
+    },
+    total=False,
+)
+
+class UpdateModelPackageInputRequestTypeDef(
+    _RequiredUpdateModelPackageInputRequestTypeDef, _OptionalUpdateModelPackageInputRequestTypeDef
+):
+    pass
+
 _RequiredBatchDescribeModelPackageSummaryTypeDef = TypedDict(
     "_RequiredBatchDescribeModelPackageSummaryTypeDef",
     {
         "ModelPackageGroupName": str,
         "ModelPackageArn": str,
         "CreationTime": datetime,
-        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
     },
 )
 _OptionalBatchDescribeModelPackageSummaryTypeDef = TypedDict(
     "_OptionalBatchDescribeModelPackageSummaryTypeDef",
     {
         "ModelPackageVersion": int,
@@ -17170,88 +15822,14 @@
 
 class BatchDescribeModelPackageSummaryTypeDef(
     _RequiredBatchDescribeModelPackageSummaryTypeDef,
     _OptionalBatchDescribeModelPackageSummaryTypeDef,
 ):
     pass
 
-AdditionalInferenceSpecificationDefinitionUnionTypeDef = Union[
-    AdditionalInferenceSpecificationDefinitionTypeDef,
-    AdditionalInferenceSpecificationDefinitionOutputTypeDef,
-]
-InferenceSpecificationUnionTypeDef = Union[
-    InferenceSpecificationTypeDef, InferenceSpecificationOutputTypeDef
-]
-DataQualityJobInputOutputTypeDef = TypedDict(
-    "DataQualityJobInputOutputTypeDef",
-    {
-        "EndpointInput": EndpointInputTypeDef,
-        "BatchTransformInput": BatchTransformInputOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredModelBiasJobInputOutputTypeDef = TypedDict(
-    "_RequiredModelBiasJobInputOutputTypeDef",
-    {
-        "GroundTruthS3Input": MonitoringGroundTruthS3InputTypeDef,
-    },
-)
-_OptionalModelBiasJobInputOutputTypeDef = TypedDict(
-    "_OptionalModelBiasJobInputOutputTypeDef",
-    {
-        "EndpointInput": EndpointInputTypeDef,
-        "BatchTransformInput": BatchTransformInputOutputTypeDef,
-    },
-    total=False,
-)
-
-class ModelBiasJobInputOutputTypeDef(
-    _RequiredModelBiasJobInputOutputTypeDef, _OptionalModelBiasJobInputOutputTypeDef
-):
-    pass
-
-ModelExplainabilityJobInputOutputTypeDef = TypedDict(
-    "ModelExplainabilityJobInputOutputTypeDef",
-    {
-        "EndpointInput": EndpointInputTypeDef,
-        "BatchTransformInput": BatchTransformInputOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredModelQualityJobInputOutputTypeDef = TypedDict(
-    "_RequiredModelQualityJobInputOutputTypeDef",
-    {
-        "GroundTruthS3Input": MonitoringGroundTruthS3InputTypeDef,
-    },
-)
-_OptionalModelQualityJobInputOutputTypeDef = TypedDict(
-    "_OptionalModelQualityJobInputOutputTypeDef",
-    {
-        "EndpointInput": EndpointInputTypeDef,
-        "BatchTransformInput": BatchTransformInputOutputTypeDef,
-    },
-    total=False,
-)
-
-class ModelQualityJobInputOutputTypeDef(
-    _RequiredModelQualityJobInputOutputTypeDef, _OptionalModelQualityJobInputOutputTypeDef
-):
-    pass
-
-MonitoringInputOutputTypeDef = TypedDict(
-    "MonitoringInputOutputTypeDef",
-    {
-        "EndpointInput": EndpointInputTypeDef,
-        "BatchTransformInput": BatchTransformInputOutputTypeDef,
-    },
-    total=False,
-)
-
 DataQualityJobInputTypeDef = TypedDict(
     "DataQualityJobInputTypeDef",
     {
         "EndpointInput": EndpointInputTypeDef,
         "BatchTransformInput": BatchTransformInputTypeDef,
     },
     total=False,
@@ -17311,28 +15889,54 @@
     {
         "EndpointInput": EndpointInputTypeDef,
         "BatchTransformInput": BatchTransformInputTypeDef,
     },
     total=False,
 )
 
-MonitoringOutputConfigUnionTypeDef = Union[
-    MonitoringOutputConfigTypeDef, MonitoringOutputConfigOutputTypeDef
-]
+_RequiredCreateProcessingJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProcessingJobRequestRequestTypeDef",
+    {
+        "ProcessingJobName": str,
+        "ProcessingResources": ProcessingResourcesTypeDef,
+        "AppSpecification": AppSpecificationTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateProcessingJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProcessingJobRequestRequestTypeDef",
+    {
+        "ProcessingInputs": Sequence[ProcessingInputTypeDef],
+        "ProcessingOutputConfig": ProcessingOutputConfigTypeDef,
+        "StoppingCondition": ProcessingStoppingConditionTypeDef,
+        "Environment": Mapping[str, str],
+        "NetworkConfig": NetworkConfigTypeDef,
+        "Tags": Sequence[TagTypeDef],
+        "ExperimentConfig": ExperimentConfigTypeDef,
+    },
+    total=False,
+)
+
+class CreateProcessingJobRequestRequestTypeDef(
+    _RequiredCreateProcessingJobRequestRequestTypeDef,
+    _OptionalCreateProcessingJobRequestRequestTypeDef,
+):
+    pass
+
 DescribeProcessingJobResponseTypeDef = TypedDict(
     "DescribeProcessingJobResponseTypeDef",
     {
         "ProcessingInputs": List[ProcessingInputTypeDef],
-        "ProcessingOutputConfig": ProcessingOutputConfigOutputTypeDef,
+        "ProcessingOutputConfig": ProcessingOutputConfigTypeDef,
         "ProcessingJobName": str,
         "ProcessingResources": ProcessingResourcesTypeDef,
         "StoppingCondition": ProcessingStoppingConditionTypeDef,
-        "AppSpecification": AppSpecificationOutputTypeDef,
+        "AppSpecification": AppSpecificationTypeDef,
         "Environment": Dict[str, str],
-        "NetworkConfig": NetworkConfigOutputTypeDef,
+        "NetworkConfig": NetworkConfigTypeDef,
         "RoleArn": str,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "ProcessingJobArn": str,
         "ProcessingJobStatus": ProcessingJobStatusType,
         "ExitMessage": str,
         "FailureReason": str,
         "ProcessingEndTime": datetime,
@@ -17346,21 +15950,21 @@
     },
 )
 
 ProcessingJobTypeDef = TypedDict(
     "ProcessingJobTypeDef",
     {
         "ProcessingInputs": List[ProcessingInputTypeDef],
-        "ProcessingOutputConfig": ProcessingOutputConfigOutputTypeDef,
+        "ProcessingOutputConfig": ProcessingOutputConfigTypeDef,
         "ProcessingJobName": str,
         "ProcessingResources": ProcessingResourcesTypeDef,
         "StoppingCondition": ProcessingStoppingConditionTypeDef,
-        "AppSpecification": AppSpecificationOutputTypeDef,
+        "AppSpecification": AppSpecificationTypeDef,
         "Environment": Dict[str, str],
-        "NetworkConfig": NetworkConfigOutputTypeDef,
+        "NetworkConfig": NetworkConfigTypeDef,
         "RoleArn": str,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "ProcessingJobArn": str,
         "ProcessingJobStatus": ProcessingJobStatusType,
         "ExitMessage": str,
         "FailureReason": str,
         "ProcessingEndTime": datetime,
@@ -17371,181 +15975,186 @@
         "AutoMLJobArn": str,
         "TrainingJobArn": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateProcessingJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProcessingJobRequestRequestTypeDef",
+_RequiredCreateFlowDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFlowDefinitionRequestRequestTypeDef",
     {
-        "ProcessingJobName": str,
-        "ProcessingResources": ProcessingResourcesTypeDef,
-        "AppSpecification": AppSpecificationTypeDef,
+        "FlowDefinitionName": str,
+        "HumanLoopConfig": HumanLoopConfigTypeDef,
+        "OutputConfig": FlowDefinitionOutputConfigTypeDef,
         "RoleArn": str,
     },
 )
-_OptionalCreateProcessingJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProcessingJobRequestRequestTypeDef",
+_OptionalCreateFlowDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFlowDefinitionRequestRequestTypeDef",
     {
-        "ProcessingInputs": Sequence[ProcessingInputTypeDef],
-        "ProcessingOutputConfig": ProcessingOutputConfigTypeDef,
-        "StoppingCondition": ProcessingStoppingConditionTypeDef,
-        "Environment": Mapping[str, str],
-        "NetworkConfig": NetworkConfigTypeDef,
+        "HumanLoopRequestSource": HumanLoopRequestSourceTypeDef,
+        "HumanLoopActivationConfig": HumanLoopActivationConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
-        "ExperimentConfig": ExperimentConfigTypeDef,
     },
     total=False,
 )
 
-class CreateProcessingJobRequestRequestTypeDef(
-    _RequiredCreateProcessingJobRequestRequestTypeDef,
-    _OptionalCreateProcessingJobRequestRequestTypeDef,
+class CreateFlowDefinitionRequestRequestTypeDef(
+    _RequiredCreateFlowDefinitionRequestRequestTypeDef,
+    _OptionalCreateFlowDefinitionRequestRequestTypeDef,
 ):
     pass
 
-ProcessingOutputConfigUnionTypeDef = Union[
-    ProcessingOutputConfigTypeDef, ProcessingOutputConfigOutputTypeDef
-]
 DescribeFlowDefinitionResponseTypeDef = TypedDict(
     "DescribeFlowDefinitionResponseTypeDef",
     {
         "FlowDefinitionArn": str,
         "FlowDefinitionName": str,
         "FlowDefinitionStatus": FlowDefinitionStatusType,
         "CreationTime": datetime,
         "HumanLoopRequestSource": HumanLoopRequestSourceTypeDef,
         "HumanLoopActivationConfig": HumanLoopActivationConfigTypeDef,
-        "HumanLoopConfig": HumanLoopConfigOutputTypeDef,
+        "HumanLoopConfig": HumanLoopConfigTypeDef,
         "OutputConfig": FlowDefinitionOutputConfigTypeDef,
         "RoleArn": str,
         "FailureReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateFlowDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFlowDefinitionRequestRequestTypeDef",
+_RequiredCreateLabelingJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLabelingJobRequestRequestTypeDef",
     {
-        "FlowDefinitionName": str,
-        "HumanLoopConfig": HumanLoopConfigTypeDef,
-        "OutputConfig": FlowDefinitionOutputConfigTypeDef,
+        "LabelingJobName": str,
+        "LabelAttributeName": str,
+        "InputConfig": LabelingJobInputConfigTypeDef,
+        "OutputConfig": LabelingJobOutputConfigTypeDef,
         "RoleArn": str,
+        "HumanTaskConfig": HumanTaskConfigTypeDef,
     },
 )
-_OptionalCreateFlowDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFlowDefinitionRequestRequestTypeDef",
+_OptionalCreateLabelingJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLabelingJobRequestRequestTypeDef",
     {
-        "HumanLoopRequestSource": HumanLoopRequestSourceTypeDef,
-        "HumanLoopActivationConfig": HumanLoopActivationConfigTypeDef,
+        "LabelCategoryConfigS3Uri": str,
+        "StoppingConditions": LabelingJobStoppingConditionsTypeDef,
+        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class CreateFlowDefinitionRequestRequestTypeDef(
-    _RequiredCreateFlowDefinitionRequestRequestTypeDef,
-    _OptionalCreateFlowDefinitionRequestRequestTypeDef,
+class CreateLabelingJobRequestRequestTypeDef(
+    _RequiredCreateLabelingJobRequestRequestTypeDef, _OptionalCreateLabelingJobRequestRequestTypeDef
 ):
     pass
 
-HumanLoopConfigUnionTypeDef = Union[HumanLoopConfigTypeDef, HumanLoopConfigOutputTypeDef]
 DescribeLabelingJobResponseTypeDef = TypedDict(
     "DescribeLabelingJobResponseTypeDef",
     {
         "LabelingJobStatus": LabelingJobStatusType,
         "LabelCounters": LabelCountersTypeDef,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "JobReferenceCode": str,
         "LabelingJobName": str,
         "LabelingJobArn": str,
         "LabelAttributeName": str,
-        "InputConfig": LabelingJobInputConfigOutputTypeDef,
+        "InputConfig": LabelingJobInputConfigTypeDef,
         "OutputConfig": LabelingJobOutputConfigTypeDef,
         "RoleArn": str,
         "LabelCategoryConfigS3Uri": str,
         "StoppingConditions": LabelingJobStoppingConditionsTypeDef,
-        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigOutputTypeDef,
-        "HumanTaskConfig": HumanTaskConfigOutputTypeDef,
+        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigTypeDef,
+        "HumanTaskConfig": HumanTaskConfigTypeDef,
         "Tags": List[TagTypeDef],
         "LabelingJobOutput": LabelingJobOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateLabelingJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLabelingJobRequestRequestTypeDef",
+_RequiredCreateTrainingJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTrainingJobRequestRequestTypeDef",
     {
-        "LabelingJobName": str,
-        "LabelAttributeName": str,
-        "InputConfig": LabelingJobInputConfigTypeDef,
-        "OutputConfig": LabelingJobOutputConfigTypeDef,
+        "TrainingJobName": str,
+        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
         "RoleArn": str,
-        "HumanTaskConfig": HumanTaskConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "ResourceConfig": ResourceConfigTypeDef,
+        "StoppingCondition": StoppingConditionTypeDef,
     },
 )
-_OptionalCreateLabelingJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLabelingJobRequestRequestTypeDef",
+_OptionalCreateTrainingJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTrainingJobRequestRequestTypeDef",
     {
-        "LabelCategoryConfigS3Uri": str,
-        "StoppingConditions": LabelingJobStoppingConditionsTypeDef,
-        "LabelingJobAlgorithmsConfig": LabelingJobAlgorithmsConfigTypeDef,
+        "HyperParameters": Mapping[str, str],
+        "InputDataConfig": Sequence[ChannelTypeDef],
+        "VpcConfig": VpcConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
+        "EnableNetworkIsolation": bool,
+        "EnableInterContainerTrafficEncryption": bool,
+        "EnableManagedSpotTraining": bool,
+        "CheckpointConfig": CheckpointConfigTypeDef,
+        "DebugHookConfig": DebugHookConfigTypeDef,
+        "DebugRuleConfigurations": Sequence[DebugRuleConfigurationTypeDef],
+        "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
+        "ExperimentConfig": ExperimentConfigTypeDef,
+        "ProfilerConfig": ProfilerConfigTypeDef,
+        "ProfilerRuleConfigurations": Sequence[ProfilerRuleConfigurationTypeDef],
+        "Environment": Mapping[str, str],
+        "RetryStrategy": RetryStrategyTypeDef,
     },
     total=False,
 )
 
-class CreateLabelingJobRequestRequestTypeDef(
-    _RequiredCreateLabelingJobRequestRequestTypeDef, _OptionalCreateLabelingJobRequestRequestTypeDef
+class CreateTrainingJobRequestRequestTypeDef(
+    _RequiredCreateTrainingJobRequestRequestTypeDef, _OptionalCreateTrainingJobRequestRequestTypeDef
 ):
     pass
 
-HumanTaskConfigUnionTypeDef = Union[HumanTaskConfigTypeDef, HumanTaskConfigOutputTypeDef]
 DescribeTrainingJobResponseTypeDef = TypedDict(
     "DescribeTrainingJobResponseTypeDef",
     {
         "TrainingJobName": str,
         "TrainingJobArn": str,
         "TuningJobArn": str,
         "LabelingJobArn": str,
         "AutoMLJobArn": str,
         "ModelArtifacts": ModelArtifactsTypeDef,
         "TrainingJobStatus": TrainingJobStatusType,
         "SecondaryStatus": SecondaryStatusType,
         "FailureReason": str,
         "HyperParameters": Dict[str, str],
-        "AlgorithmSpecification": AlgorithmSpecificationOutputTypeDef,
+        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
         "RoleArn": str,
-        "InputDataConfig": List[ChannelOutputTypeDef],
+        "InputDataConfig": List[ChannelTypeDef],
         "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigOutputTypeDef,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "ResourceConfig": ResourceConfigTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
         "CreationTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
         "LastModifiedTime": datetime,
         "SecondaryStatusTransitions": List[SecondaryStatusTransitionTypeDef],
         "FinalMetricDataList": List[MetricDataTypeDef],
         "EnableNetworkIsolation": bool,
         "EnableInterContainerTrafficEncryption": bool,
         "EnableManagedSpotTraining": bool,
         "CheckpointConfig": CheckpointConfigTypeDef,
         "TrainingTimeInSeconds": int,
         "BillableTimeInSeconds": int,
-        "DebugHookConfig": DebugHookConfigOutputTypeDef,
+        "DebugHookConfig": DebugHookConfigTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
-        "DebugRuleConfigurations": List[DebugRuleConfigurationOutputTypeDef],
+        "DebugRuleConfigurations": List[DebugRuleConfigurationTypeDef],
         "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
         "DebugRuleEvaluationStatuses": List[DebugRuleEvaluationStatusTypeDef],
-        "ProfilerConfig": ProfilerConfigOutputTypeDef,
-        "ProfilerRuleConfigurations": List[ProfilerRuleConfigurationOutputTypeDef],
+        "ProfilerConfig": ProfilerConfigTypeDef,
+        "ProfilerRuleConfigurations": List[ProfilerRuleConfigurationTypeDef],
         "ProfilerRuleEvaluationStatuses": List[ProfilerRuleEvaluationStatusTypeDef],
         "ProfilingStatus": ProfilingStatusType,
         "RetryStrategy": RetryStrategyTypeDef,
         "Environment": Dict[str, str],
         "WarmPoolStatus": WarmPoolStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -17560,48 +16169,46 @@
         "LabelingJobArn": str,
         "AutoMLJobArn": str,
         "ModelArtifacts": ModelArtifactsTypeDef,
         "TrainingJobStatus": TrainingJobStatusType,
         "SecondaryStatus": SecondaryStatusType,
         "FailureReason": str,
         "HyperParameters": Dict[str, str],
-        "AlgorithmSpecification": AlgorithmSpecificationOutputTypeDef,
+        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
         "RoleArn": str,
-        "InputDataConfig": List[ChannelOutputTypeDef],
+        "InputDataConfig": List[ChannelTypeDef],
         "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigOutputTypeDef,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "ResourceConfig": ResourceConfigTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "StoppingCondition": StoppingConditionTypeDef,
         "CreationTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
         "LastModifiedTime": datetime,
         "SecondaryStatusTransitions": List[SecondaryStatusTransitionTypeDef],
         "FinalMetricDataList": List[MetricDataTypeDef],
         "EnableNetworkIsolation": bool,
         "EnableInterContainerTrafficEncryption": bool,
         "EnableManagedSpotTraining": bool,
         "CheckpointConfig": CheckpointConfigTypeDef,
         "TrainingTimeInSeconds": int,
         "BillableTimeInSeconds": int,
-        "DebugHookConfig": DebugHookConfigOutputTypeDef,
+        "DebugHookConfig": DebugHookConfigTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
-        "DebugRuleConfigurations": List[DebugRuleConfigurationOutputTypeDef],
+        "DebugRuleConfigurations": List[DebugRuleConfigurationTypeDef],
         "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
         "DebugRuleEvaluationStatuses": List[DebugRuleEvaluationStatusTypeDef],
+        "ProfilerConfig": ProfilerConfigTypeDef,
         "Environment": Dict[str, str],
         "RetryStrategy": RetryStrategyTypeDef,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-AlgorithmSpecificationUnionTypeDef = Union[
-    AlgorithmSpecificationTypeDef, AlgorithmSpecificationOutputTypeDef
-]
 _RequiredCreateTransformJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTransformJobRequestRequestTypeDef",
     {
         "TransformJobName": str,
         "ModelName": str,
         "TransformInput": TransformInputTypeDef,
         "TransformOutput": TransformOutputTypeDef,
@@ -17654,38 +16261,14 @@
         "AutoMLJobArn": str,
         "DataProcessing": DataProcessingTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTransformJobDefinitionOutputTypeDef = TypedDict(
-    "_RequiredTransformJobDefinitionOutputTypeDef",
-    {
-        "TransformInput": TransformInputTypeDef,
-        "TransformOutput": TransformOutputTypeDef,
-        "TransformResources": TransformResourcesTypeDef,
-    },
-)
-_OptionalTransformJobDefinitionOutputTypeDef = TypedDict(
-    "_OptionalTransformJobDefinitionOutputTypeDef",
-    {
-        "MaxConcurrentTransforms": int,
-        "MaxPayloadInMB": int,
-        "BatchStrategy": BatchStrategyType,
-        "Environment": Dict[str, str],
-    },
-    total=False,
-)
-
-class TransformJobDefinitionOutputTypeDef(
-    _RequiredTransformJobDefinitionOutputTypeDef, _OptionalTransformJobDefinitionOutputTypeDef
-):
-    pass
-
 _RequiredTransformJobDefinitionTypeDef = TypedDict(
     "_RequiredTransformJobDefinitionTypeDef",
     {
         "TransformInput": TransformInputTypeDef,
         "TransformOutput": TransformOutputTypeDef,
         "TransformResources": TransformResourcesTypeDef,
     },
@@ -17730,46 +16313,14 @@
         "DataProcessing": DataProcessingTypeDef,
         "ExperimentConfig": ExperimentConfigTypeDef,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-DescribeAutoMLJobV2ResponseTypeDef = TypedDict(
-    "DescribeAutoMLJobV2ResponseTypeDef",
-    {
-        "AutoMLJobName": str,
-        "AutoMLJobArn": str,
-        "AutoMLJobInputDataConfig": List[AutoMLJobChannelTypeDef],
-        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
-        "RoleArn": str,
-        "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
-        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigOutputTypeDef,
-        "CreationTime": datetime,
-        "EndTime": datetime,
-        "LastModifiedTime": datetime,
-        "FailureReason": str,
-        "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
-        "BestCandidate": AutoMLCandidateTypeDef,
-        "AutoMLJobStatus": AutoMLJobStatusType,
-        "AutoMLJobSecondaryStatus": AutoMLJobSecondaryStatusType,
-        "ModelDeployConfig": ModelDeployConfigTypeDef,
-        "ModelDeployResult": ModelDeployResultTypeDef,
-        "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
-        "SecurityConfig": AutoMLSecurityConfigOutputTypeDef,
-        "AutoMLJobArtifacts": AutoMLJobArtifactsTypeDef,
-        "ResolvedAttributes": AutoMLResolvedAttributesTypeDef,
-        "AutoMLProblemTypeConfigName": AutoMLProblemTypeConfigNameType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AutoMLProblemTypeConfigUnionTypeDef = Union[
-    AutoMLProblemTypeConfigTypeDef, AutoMLProblemTypeConfigOutputTypeDef
-]
 _RequiredCreateAutoMLJobV2RequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoMLJobV2RequestRequestTypeDef",
     {
         "AutoMLJobName": str,
         "AutoMLJobInputDataConfig": Sequence[AutoMLJobChannelTypeDef],
         "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
         "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
@@ -17789,14 +16340,43 @@
 )
 
 class CreateAutoMLJobV2RequestRequestTypeDef(
     _RequiredCreateAutoMLJobV2RequestRequestTypeDef, _OptionalCreateAutoMLJobV2RequestRequestTypeDef
 ):
     pass
 
+DescribeAutoMLJobV2ResponseTypeDef = TypedDict(
+    "DescribeAutoMLJobV2ResponseTypeDef",
+    {
+        "AutoMLJobName": str,
+        "AutoMLJobArn": str,
+        "AutoMLJobInputDataConfig": List[AutoMLJobChannelTypeDef],
+        "OutputDataConfig": AutoMLOutputDataConfigTypeDef,
+        "RoleArn": str,
+        "AutoMLJobObjective": AutoMLJobObjectiveTypeDef,
+        "AutoMLProblemTypeConfig": AutoMLProblemTypeConfigTypeDef,
+        "CreationTime": datetime,
+        "EndTime": datetime,
+        "LastModifiedTime": datetime,
+        "FailureReason": str,
+        "PartialFailureReasons": List[AutoMLPartialFailureReasonTypeDef],
+        "BestCandidate": AutoMLCandidateTypeDef,
+        "AutoMLJobStatus": AutoMLJobStatusType,
+        "AutoMLJobSecondaryStatus": AutoMLJobSecondaryStatusType,
+        "ModelDeployConfig": ModelDeployConfigTypeDef,
+        "ModelDeployResult": ModelDeployResultTypeDef,
+        "DataSplitConfig": AutoMLDataSplitConfigTypeDef,
+        "SecurityConfig": AutoMLSecurityConfigTypeDef,
+        "AutoMLJobArtifacts": AutoMLJobArtifactsTypeDef,
+        "ResolvedAttributes": AutoMLResolvedAttributesTypeDef,
+        "AutoMLProblemTypeConfigName": AutoMLProblemTypeConfigNameType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListPipelineExecutionStepsResponseTypeDef = TypedDict(
     "ListPipelineExecutionStepsResponseTypeDef",
     {
         "PipelineExecutionSteps": List[PipelineExecutionStepTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -17819,15 +16399,14 @@
 )
 
 class CreateEndpointInputRequestTypeDef(
     _RequiredCreateEndpointInputRequestTypeDef, _OptionalCreateEndpointInputRequestTypeDef
 ):
     pass
 
-DeploymentConfigUnionTypeDef = Union[DeploymentConfigTypeDef, DeploymentConfigOutputTypeDef]
 _RequiredUpdateEndpointInputRequestTypeDef = TypedDict(
     "_RequiredUpdateEndpointInputRequestTypeDef",
     {
         "EndpointName": str,
         "EndpointConfigName": str,
     },
 )
@@ -17843,75 +16422,98 @@
 )
 
 class UpdateEndpointInputRequestTypeDef(
     _RequiredUpdateEndpointInputRequestTypeDef, _OptionalUpdateEndpointInputRequestTypeDef
 ):
     pass
 
+_RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef",
+    {
+        "JobName": str,
+        "JobType": RecommendationJobTypeType,
+        "RoleArn": str,
+        "InputConfig": RecommendationJobInputConfigTypeDef,
+    },
+)
+_OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef",
+    {
+        "JobDescription": str,
+        "StoppingConditions": RecommendationJobStoppingConditionsTypeDef,
+        "OutputConfig": RecommendationJobOutputConfigTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateInferenceRecommendationsJobRequestRequestTypeDef(
+    _RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef,
+    _OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef,
+):
+    pass
+
 DescribeInferenceRecommendationsJobResponseTypeDef = TypedDict(
     "DescribeInferenceRecommendationsJobResponseTypeDef",
     {
         "JobName": str,
         "JobDescription": str,
         "JobType": RecommendationJobTypeType,
         "JobArn": str,
         "RoleArn": str,
         "Status": RecommendationJobStatusType,
         "CreationTime": datetime,
         "CompletionTime": datetime,
         "LastModifiedTime": datetime,
         "FailureReason": str,
-        "InputConfig": RecommendationJobInputConfigOutputTypeDef,
-        "StoppingConditions": RecommendationJobStoppingConditionsOutputTypeDef,
+        "InputConfig": RecommendationJobInputConfigTypeDef,
+        "StoppingConditions": RecommendationJobStoppingConditionsTypeDef,
         "InferenceRecommendations": List[InferenceRecommendationTypeDef],
         "EndpointPerformances": List[EndpointPerformanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef",
+_RequiredCreateEndpointConfigInputRequestTypeDef = TypedDict(
+    "_RequiredCreateEndpointConfigInputRequestTypeDef",
     {
-        "JobName": str,
-        "JobType": RecommendationJobTypeType,
-        "RoleArn": str,
-        "InputConfig": RecommendationJobInputConfigTypeDef,
+        "EndpointConfigName": str,
+        "ProductionVariants": Sequence[ProductionVariantTypeDef],
     },
 )
-_OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef",
+_OptionalCreateEndpointConfigInputRequestTypeDef = TypedDict(
+    "_OptionalCreateEndpointConfigInputRequestTypeDef",
     {
-        "JobDescription": str,
-        "StoppingConditions": RecommendationJobStoppingConditionsTypeDef,
-        "OutputConfig": RecommendationJobOutputConfigTypeDef,
+        "DataCaptureConfig": DataCaptureConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
+        "ExplainerConfig": ExplainerConfigTypeDef,
+        "ShadowProductionVariants": Sequence[ProductionVariantTypeDef],
     },
     total=False,
 )
 
-class CreateInferenceRecommendationsJobRequestRequestTypeDef(
-    _RequiredCreateInferenceRecommendationsJobRequestRequestTypeDef,
-    _OptionalCreateInferenceRecommendationsJobRequestRequestTypeDef,
+class CreateEndpointConfigInputRequestTypeDef(
+    _RequiredCreateEndpointConfigInputRequestTypeDef,
+    _OptionalCreateEndpointConfigInputRequestTypeDef,
 ):
     pass
 
-RecommendationJobInputConfigUnionTypeDef = Union[
-    RecommendationJobInputConfigTypeDef, RecommendationJobInputConfigOutputTypeDef
-]
 DescribeEndpointConfigOutputTypeDef = TypedDict(
     "DescribeEndpointConfigOutputTypeDef",
     {
         "EndpointConfigName": str,
         "EndpointConfigArn": str,
         "ProductionVariants": List[ProductionVariantTypeDef],
-        "DataCaptureConfig": DataCaptureConfigOutputTypeDef,
+        "DataCaptureConfig": DataCaptureConfigTypeDef,
         "KmsKeyId": str,
         "CreationTime": datetime,
-        "AsyncInferenceConfig": AsyncInferenceConfigOutputTypeDef,
-        "ExplainerConfig": ExplainerConfigOutputTypeDef,
+        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
+        "ExplainerConfig": ExplainerConfigTypeDef,
         "ShadowProductionVariants": List[ProductionVariantTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointOutputTypeDef = TypedDict(
     "DescribeEndpointOutputTypeDef",
@@ -17921,320 +16523,137 @@
         "EndpointConfigName": str,
         "ProductionVariants": List[ProductionVariantSummaryTypeDef],
         "DataCaptureConfig": DataCaptureConfigSummaryTypeDef,
         "EndpointStatus": EndpointStatusType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "LastDeploymentConfig": DeploymentConfigOutputTypeDef,
-        "AsyncInferenceConfig": AsyncInferenceConfigOutputTypeDef,
+        "LastDeploymentConfig": DeploymentConfigTypeDef,
+        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
         "PendingDeploymentSummary": PendingDeploymentSummaryTypeDef,
-        "ExplainerConfig": ExplainerConfigOutputTypeDef,
+        "ExplainerConfig": ExplainerConfigTypeDef,
         "ShadowProductionVariants": List[ProductionVariantSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateEndpointConfigInputRequestTypeDef = TypedDict(
-    "_RequiredCreateEndpointConfigInputRequestTypeDef",
+_RequiredCreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHyperParameterTuningJobRequestRequestTypeDef",
     {
-        "EndpointConfigName": str,
-        "ProductionVariants": Sequence[ProductionVariantTypeDef],
+        "HyperParameterTuningJobName": str,
+        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
     },
 )
-_OptionalCreateEndpointConfigInputRequestTypeDef = TypedDict(
-    "_OptionalCreateEndpointConfigInputRequestTypeDef",
+_OptionalCreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHyperParameterTuningJobRequestRequestTypeDef",
     {
-        "DataCaptureConfig": DataCaptureConfigTypeDef,
+        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionTypeDef,
+        "TrainingJobDefinitions": Sequence[HyperParameterTrainingJobDefinitionTypeDef],
+        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
         "Tags": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "AsyncInferenceConfig": AsyncInferenceConfigTypeDef,
-        "ExplainerConfig": ExplainerConfigTypeDef,
-        "ShadowProductionVariants": Sequence[ProductionVariantTypeDef],
+        "Autotune": AutotuneTypeDef,
     },
     total=False,
 )
 
-class CreateEndpointConfigInputRequestTypeDef(
-    _RequiredCreateEndpointConfigInputRequestTypeDef,
-    _OptionalCreateEndpointConfigInputRequestTypeDef,
+class CreateHyperParameterTuningJobRequestRequestTypeDef(
+    _RequiredCreateHyperParameterTuningJobRequestRequestTypeDef,
+    _OptionalCreateHyperParameterTuningJobRequestRequestTypeDef,
 ):
     pass
 
-ExplainerConfigUnionTypeDef = Union[ExplainerConfigTypeDef, ExplainerConfigOutputTypeDef]
 DescribeHyperParameterTuningJobResponseTypeDef = TypedDict(
     "DescribeHyperParameterTuningJobResponseTypeDef",
     {
         "HyperParameterTuningJobName": str,
         "HyperParameterTuningJobArn": str,
-        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigOutputTypeDef,
-        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionOutputTypeDef,
-        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionOutputTypeDef],
+        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
+        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionTypeDef,
+        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionTypeDef],
         "HyperParameterTuningJobStatus": HyperParameterTuningJobStatusType,
         "CreationTime": datetime,
         "HyperParameterTuningEndTime": datetime,
         "LastModifiedTime": datetime,
         "TrainingJobStatusCounters": TrainingJobStatusCountersTypeDef,
         "ObjectiveStatusCounters": ObjectiveStatusCountersTypeDef,
         "BestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
         "OverallBestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
-        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigOutputTypeDef,
+        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
         "FailureReason": str,
         "TuningJobCompletionDetails": HyperParameterTuningJobCompletionDetailsTypeDef,
         "ConsumedResources": HyperParameterTuningJobConsumedResourcesTypeDef,
         "Autotune": AutotuneTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HyperParameterTuningJobSearchEntityTypeDef = TypedDict(
     "HyperParameterTuningJobSearchEntityTypeDef",
     {
         "HyperParameterTuningJobName": str,
         "HyperParameterTuningJobArn": str,
-        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigOutputTypeDef,
-        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionOutputTypeDef,
-        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionOutputTypeDef],
+        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
+        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionTypeDef,
+        "TrainingJobDefinitions": List[HyperParameterTrainingJobDefinitionTypeDef],
         "HyperParameterTuningJobStatus": HyperParameterTuningJobStatusType,
         "CreationTime": datetime,
         "HyperParameterTuningEndTime": datetime,
         "LastModifiedTime": datetime,
         "TrainingJobStatusCounters": TrainingJobStatusCountersTypeDef,
         "ObjectiveStatusCounters": ObjectiveStatusCountersTypeDef,
         "BestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
         "OverallBestTrainingJob": HyperParameterTrainingJobSummaryTypeDef,
-        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigOutputTypeDef,
+        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
         "FailureReason": str,
         "Tags": List[TagTypeDef],
         "TuningJobCompletionDetails": HyperParameterTuningJobCompletionDetailsTypeDef,
         "ConsumedResources": HyperParameterTuningJobConsumedResourcesTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateTrainingJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTrainingJobRequestRequestTypeDef",
-    {
-        "TrainingJobName": str,
-        "AlgorithmSpecification": AlgorithmSpecificationTypeDef,
-        "RoleArn": str,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "ResourceConfig": ResourceConfigTypeDef,
-        "StoppingCondition": StoppingConditionTypeDef,
-    },
-)
-_OptionalCreateTrainingJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTrainingJobRequestRequestTypeDef",
-    {
-        "HyperParameters": Mapping[str, str],
-        "InputDataConfig": Sequence[ChannelUnionTypeDef],
-        "VpcConfig": VpcConfigTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "EnableNetworkIsolation": bool,
-        "EnableInterContainerTrafficEncryption": bool,
-        "EnableManagedSpotTraining": bool,
-        "CheckpointConfig": CheckpointConfigTypeDef,
-        "DebugHookConfig": DebugHookConfigTypeDef,
-        "DebugRuleConfigurations": Sequence[DebugRuleConfigurationUnionTypeDef],
-        "TensorBoardOutputConfig": TensorBoardOutputConfigTypeDef,
-        "ExperimentConfig": ExperimentConfigTypeDef,
-        "ProfilerConfig": ProfilerConfigTypeDef,
-        "ProfilerRuleConfigurations": Sequence[ProfilerRuleConfigurationUnionTypeDef],
-        "Environment": Mapping[str, str],
-        "RetryStrategy": RetryStrategyTypeDef,
-    },
-    total=False,
-)
-
-class CreateTrainingJobRequestRequestTypeDef(
-    _RequiredCreateTrainingJobRequestRequestTypeDef, _OptionalCreateTrainingJobRequestRequestTypeDef
-):
-    pass
-
-HyperParameterTrainingJobDefinitionUnionTypeDef = Union[
-    HyperParameterTrainingJobDefinitionTypeDef, HyperParameterTrainingJobDefinitionOutputTypeDef
-]
 ListInferenceRecommendationsJobStepsResponseTypeDef = TypedDict(
     "ListInferenceRecommendationsJobStepsResponseTypeDef",
     {
         "Steps": List[InferenceRecommendationsJobStepTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TrainingSpecificationUnionTypeDef = Union[
-    TrainingSpecificationTypeDef, TrainingSpecificationOutputTypeDef
-]
 ListLabelingJobsResponseTypeDef = TypedDict(
     "ListLabelingJobsResponseTypeDef",
     {
         "LabelingJobSummaryList": List[LabelingJobSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateModelInputRequestTypeDef = TypedDict(
-    "_RequiredCreateModelInputRequestTypeDef",
+DynamicScalingConfigurationTypeDef = TypedDict(
+    "DynamicScalingConfigurationTypeDef",
     {
-        "ModelName": str,
-        "ExecutionRoleArn": str,
-    },
-)
-_OptionalCreateModelInputRequestTypeDef = TypedDict(
-    "_OptionalCreateModelInputRequestTypeDef",
-    {
-        "PrimaryContainer": ContainerDefinitionTypeDef,
-        "Containers": Sequence[ContainerDefinitionUnionTypeDef],
-        "InferenceExecutionConfig": InferenceExecutionConfigTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "VpcConfig": VpcConfigTypeDef,
-        "EnableNetworkIsolation": bool,
+        "MinCapacity": int,
+        "MaxCapacity": int,
+        "ScaleInCooldown": int,
+        "ScaleOutCooldown": int,
+        "ScalingPolicies": List[ScalingPolicyTypeDef],
     },
     total=False,
 )
 
-class CreateModelInputRequestTypeDef(
-    _RequiredCreateModelInputRequestTypeDef, _OptionalCreateModelInputRequestTypeDef
-):
-    pass
-
 BatchDescribeModelPackageOutputTypeDef = TypedDict(
     "BatchDescribeModelPackageOutputTypeDef",
     {
         "ModelPackageSummaries": Dict[str, BatchDescribeModelPackageSummaryTypeDef],
         "BatchDescribeModelPackageErrorMap": Dict[str, BatchDescribeModelPackageErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateModelPackageInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateModelPackageInputRequestTypeDef",
-    {
-        "ModelPackageArn": str,
-    },
-)
-_OptionalUpdateModelPackageInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateModelPackageInputRequestTypeDef",
-    {
-        "ModelApprovalStatus": ModelApprovalStatusType,
-        "ApprovalDescription": str,
-        "CustomerMetadataProperties": Mapping[str, str],
-        "CustomerMetadataPropertiesToRemove": Sequence[str],
-        "AdditionalInferenceSpecificationsToAdd": Sequence[
-            AdditionalInferenceSpecificationDefinitionUnionTypeDef
-        ],
-    },
-    total=False,
-)
-
-class UpdateModelPackageInputRequestTypeDef(
-    _RequiredUpdateModelPackageInputRequestTypeDef, _OptionalUpdateModelPackageInputRequestTypeDef
-):
-    pass
-
-DescribeDataQualityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeDataQualityJobDefinitionResponseTypeDef",
-    {
-        "JobDefinitionArn": str,
-        "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "DataQualityBaselineConfig": DataQualityBaselineConfigTypeDef,
-        "DataQualityAppSpecification": DataQualityAppSpecificationOutputTypeDef,
-        "DataQualityJobInput": DataQualityJobInputOutputTypeDef,
-        "DataQualityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
-        "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
-        "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeModelBiasJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelBiasJobDefinitionResponseTypeDef",
-    {
-        "JobDefinitionArn": str,
-        "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "ModelBiasBaselineConfig": ModelBiasBaselineConfigTypeDef,
-        "ModelBiasAppSpecification": ModelBiasAppSpecificationOutputTypeDef,
-        "ModelBiasJobInput": ModelBiasJobInputOutputTypeDef,
-        "ModelBiasJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
-        "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
-        "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeModelExplainabilityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
-    {
-        "JobDefinitionArn": str,
-        "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "ModelExplainabilityBaselineConfig": ModelExplainabilityBaselineConfigTypeDef,
-        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationOutputTypeDef,
-        "ModelExplainabilityJobInput": ModelExplainabilityJobInputOutputTypeDef,
-        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
-        "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
-        "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeModelQualityJobDefinitionResponseTypeDef = TypedDict(
-    "DescribeModelQualityJobDefinitionResponseTypeDef",
-    {
-        "JobDefinitionArn": str,
-        "JobDefinitionName": str,
-        "CreationTime": datetime,
-        "ModelQualityBaselineConfig": ModelQualityBaselineConfigTypeDef,
-        "ModelQualityAppSpecification": ModelQualityAppSpecificationOutputTypeDef,
-        "ModelQualityJobInput": ModelQualityJobInputOutputTypeDef,
-        "ModelQualityJobOutputConfig": MonitoringOutputConfigOutputTypeDef,
-        "JobResources": MonitoringResourcesTypeDef,
-        "NetworkConfig": MonitoringNetworkConfigOutputTypeDef,
-        "RoleArn": str,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredMonitoringJobDefinitionOutputTypeDef = TypedDict(
-    "_RequiredMonitoringJobDefinitionOutputTypeDef",
-    {
-        "MonitoringInputs": List[MonitoringInputOutputTypeDef],
-        "MonitoringOutputConfig": MonitoringOutputConfigOutputTypeDef,
-        "MonitoringResources": MonitoringResourcesTypeDef,
-        "MonitoringAppSpecification": MonitoringAppSpecificationOutputTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalMonitoringJobDefinitionOutputTypeDef = TypedDict(
-    "_OptionalMonitoringJobDefinitionOutputTypeDef",
-    {
-        "BaselineConfig": MonitoringBaselineConfigTypeDef,
-        "StoppingCondition": MonitoringStoppingConditionTypeDef,
-        "Environment": Dict[str, str],
-        "NetworkConfig": NetworkConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class MonitoringJobDefinitionOutputTypeDef(
-    _RequiredMonitoringJobDefinitionOutputTypeDef, _OptionalMonitoringJobDefinitionOutputTypeDef
-):
-    pass
-
 _RequiredCreateDataQualityJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataQualityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
         "DataQualityAppSpecification": DataQualityAppSpecificationTypeDef,
         "DataQualityJobInput": DataQualityJobInputTypeDef,
         "DataQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
@@ -18255,17 +16674,32 @@
 
 class CreateDataQualityJobDefinitionRequestRequestTypeDef(
     _RequiredCreateDataQualityJobDefinitionRequestRequestTypeDef,
     _OptionalCreateDataQualityJobDefinitionRequestRequestTypeDef,
 ):
     pass
 
-DataQualityJobInputUnionTypeDef = Union[
-    DataQualityJobInputTypeDef, DataQualityJobInputOutputTypeDef
-]
+DescribeDataQualityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeDataQualityJobDefinitionResponseTypeDef",
+    {
+        "JobDefinitionArn": str,
+        "JobDefinitionName": str,
+        "CreationTime": datetime,
+        "DataQualityBaselineConfig": DataQualityBaselineConfigTypeDef,
+        "DataQualityAppSpecification": DataQualityAppSpecificationTypeDef,
+        "DataQualityJobInput": DataQualityJobInputTypeDef,
+        "DataQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "RoleArn": str,
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateModelBiasJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelBiasJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
         "ModelBiasAppSpecification": ModelBiasAppSpecificationTypeDef,
         "ModelBiasJobInput": ModelBiasJobInputTypeDef,
         "ModelBiasJobOutputConfig": MonitoringOutputConfigTypeDef,
@@ -18286,15 +16720,32 @@
 
 class CreateModelBiasJobDefinitionRequestRequestTypeDef(
     _RequiredCreateModelBiasJobDefinitionRequestRequestTypeDef,
     _OptionalCreateModelBiasJobDefinitionRequestRequestTypeDef,
 ):
     pass
 
-ModelBiasJobInputUnionTypeDef = Union[ModelBiasJobInputTypeDef, ModelBiasJobInputOutputTypeDef]
+DescribeModelBiasJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelBiasJobDefinitionResponseTypeDef",
+    {
+        "JobDefinitionArn": str,
+        "JobDefinitionName": str,
+        "CreationTime": datetime,
+        "ModelBiasBaselineConfig": ModelBiasBaselineConfigTypeDef,
+        "ModelBiasAppSpecification": ModelBiasAppSpecificationTypeDef,
+        "ModelBiasJobInput": ModelBiasJobInputTypeDef,
+        "ModelBiasJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "RoleArn": str,
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateModelExplainabilityJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelExplainabilityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
         "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationTypeDef,
         "ModelExplainabilityJobInput": ModelExplainabilityJobInputTypeDef,
         "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigTypeDef,
@@ -18315,17 +16766,32 @@
 
 class CreateModelExplainabilityJobDefinitionRequestRequestTypeDef(
     _RequiredCreateModelExplainabilityJobDefinitionRequestRequestTypeDef,
     _OptionalCreateModelExplainabilityJobDefinitionRequestRequestTypeDef,
 ):
     pass
 
-ModelExplainabilityJobInputUnionTypeDef = Union[
-    ModelExplainabilityJobInputTypeDef, ModelExplainabilityJobInputOutputTypeDef
-]
+DescribeModelExplainabilityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelExplainabilityJobDefinitionResponseTypeDef",
+    {
+        "JobDefinitionArn": str,
+        "JobDefinitionName": str,
+        "CreationTime": datetime,
+        "ModelExplainabilityBaselineConfig": ModelExplainabilityBaselineConfigTypeDef,
+        "ModelExplainabilityAppSpecification": ModelExplainabilityAppSpecificationTypeDef,
+        "ModelExplainabilityJobInput": ModelExplainabilityJobInputTypeDef,
+        "ModelExplainabilityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "RoleArn": str,
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateModelQualityJobDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateModelQualityJobDefinitionRequestRequestTypeDef",
     {
         "JobDefinitionName": str,
         "ModelQualityAppSpecification": ModelQualityAppSpecificationTypeDef,
         "ModelQualityJobInput": ModelQualityJobInputTypeDef,
         "ModelQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
@@ -18346,17 +16812,32 @@
 
 class CreateModelQualityJobDefinitionRequestRequestTypeDef(
     _RequiredCreateModelQualityJobDefinitionRequestRequestTypeDef,
     _OptionalCreateModelQualityJobDefinitionRequestRequestTypeDef,
 ):
     pass
 
-ModelQualityJobInputUnionTypeDef = Union[
-    ModelQualityJobInputTypeDef, ModelQualityJobInputOutputTypeDef
-]
+DescribeModelQualityJobDefinitionResponseTypeDef = TypedDict(
+    "DescribeModelQualityJobDefinitionResponseTypeDef",
+    {
+        "JobDefinitionArn": str,
+        "JobDefinitionName": str,
+        "CreationTime": datetime,
+        "ModelQualityBaselineConfig": ModelQualityBaselineConfigTypeDef,
+        "ModelQualityAppSpecification": ModelQualityAppSpecificationTypeDef,
+        "ModelQualityJobInput": ModelQualityJobInputTypeDef,
+        "ModelQualityJobOutputConfig": MonitoringOutputConfigTypeDef,
+        "JobResources": MonitoringResourcesTypeDef,
+        "NetworkConfig": MonitoringNetworkConfigTypeDef,
+        "RoleArn": str,
+        "StoppingCondition": MonitoringStoppingConditionTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredMonitoringJobDefinitionTypeDef = TypedDict(
     "_RequiredMonitoringJobDefinitionTypeDef",
     {
         "MonitoringInputs": Sequence[MonitoringInputTypeDef],
         "MonitoringOutputConfig": MonitoringOutputConfigTypeDef,
         "MonitoringResources": MonitoringResourcesTypeDef,
         "MonitoringAppSpecification": MonitoringAppSpecificationTypeDef,
@@ -18375,43 +16856,14 @@
 )
 
 class MonitoringJobDefinitionTypeDef(
     _RequiredMonitoringJobDefinitionTypeDef, _OptionalMonitoringJobDefinitionTypeDef
 ):
     pass
 
-_RequiredAlgorithmValidationProfileOutputTypeDef = TypedDict(
-    "_RequiredAlgorithmValidationProfileOutputTypeDef",
-    {
-        "ProfileName": str,
-        "TrainingJobDefinition": TrainingJobDefinitionOutputTypeDef,
-    },
-)
-_OptionalAlgorithmValidationProfileOutputTypeDef = TypedDict(
-    "_OptionalAlgorithmValidationProfileOutputTypeDef",
-    {
-        "TransformJobDefinition": TransformJobDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
-class AlgorithmValidationProfileOutputTypeDef(
-    _RequiredAlgorithmValidationProfileOutputTypeDef,
-    _OptionalAlgorithmValidationProfileOutputTypeDef,
-):
-    pass
-
-ModelPackageValidationProfileOutputTypeDef = TypedDict(
-    "ModelPackageValidationProfileOutputTypeDef",
-    {
-        "ProfileName": str,
-        "TransformJobDefinition": TransformJobDefinitionOutputTypeDef,
-    },
-)
-
 _RequiredAlgorithmValidationProfileTypeDef = TypedDict(
     "_RequiredAlgorithmValidationProfileTypeDef",
     {
         "ProfileName": str,
         "TrainingJobDefinition": TrainingJobDefinitionTypeDef,
     },
 )
@@ -18443,77 +16895,39 @@
         "TrainingJob": TrainingJobTypeDef,
         "ProcessingJob": ProcessingJobTypeDef,
         "TransformJob": TransformJobTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHyperParameterTuningJobRequestRequestTypeDef",
-    {
-        "HyperParameterTuningJobName": str,
-        "HyperParameterTuningJobConfig": HyperParameterTuningJobConfigTypeDef,
-    },
-)
-_OptionalCreateHyperParameterTuningJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHyperParameterTuningJobRequestRequestTypeDef",
-    {
-        "TrainingJobDefinition": HyperParameterTrainingJobDefinitionTypeDef,
-        "TrainingJobDefinitions": Sequence[HyperParameterTrainingJobDefinitionUnionTypeDef],
-        "WarmStartConfig": HyperParameterTuningJobWarmStartConfigTypeDef,
-        "Tags": Sequence[TagTypeDef],
-        "Autotune": AutotuneTypeDef,
-    },
-    total=False,
-)
-
-class CreateHyperParameterTuningJobRequestRequestTypeDef(
-    _RequiredCreateHyperParameterTuningJobRequestRequestTypeDef,
-    _OptionalCreateHyperParameterTuningJobRequestRequestTypeDef,
-):
-    pass
-
-MonitoringScheduleConfigOutputTypeDef = TypedDict(
-    "MonitoringScheduleConfigOutputTypeDef",
+GetScalingConfigurationRecommendationResponseTypeDef = TypedDict(
+    "GetScalingConfigurationRecommendationResponseTypeDef",
     {
-        "ScheduleConfig": ScheduleConfigTypeDef,
-        "MonitoringJobDefinition": MonitoringJobDefinitionOutputTypeDef,
-        "MonitoringJobDefinitionName": str,
-        "MonitoringType": MonitoringTypeType,
+        "InferenceRecommendationsJobName": str,
+        "RecommendationId": str,
+        "EndpointName": str,
+        "TargetCpuUtilizationPerCore": int,
+        "ScalingPolicyObjective": ScalingPolicyObjectiveTypeDef,
+        "Metric": ScalingPolicyMetricTypeDef,
+        "DynamicScalingConfiguration": DynamicScalingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 MonitoringScheduleConfigTypeDef = TypedDict(
     "MonitoringScheduleConfigTypeDef",
     {
         "ScheduleConfig": ScheduleConfigTypeDef,
         "MonitoringJobDefinition": MonitoringJobDefinitionTypeDef,
         "MonitoringJobDefinitionName": str,
         "MonitoringType": MonitoringTypeType,
     },
     total=False,
 )
 
-AlgorithmValidationSpecificationOutputTypeDef = TypedDict(
-    "AlgorithmValidationSpecificationOutputTypeDef",
-    {
-        "ValidationRole": str,
-        "ValidationProfiles": List[AlgorithmValidationProfileOutputTypeDef],
-    },
-)
-
-ModelPackageValidationSpecificationOutputTypeDef = TypedDict(
-    "ModelPackageValidationSpecificationOutputTypeDef",
-    {
-        "ValidationRole": str,
-        "ValidationProfiles": List[ModelPackageValidationProfileOutputTypeDef],
-    },
-)
-
 AlgorithmValidationSpecificationTypeDef = TypedDict(
     "AlgorithmValidationSpecificationTypeDef",
     {
         "ValidationRole": str,
         "ValidationProfiles": Sequence[AlgorithmValidationProfileTypeDef],
     },
 )
@@ -18550,25 +16964,46 @@
         "Tags": List[TagTypeDef],
         "Parents": List[ParentTypeDef],
         "RunName": str,
     },
     total=False,
 )
 
+_RequiredCreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMonitoringScheduleRequestRequestTypeDef",
+    {
+        "MonitoringScheduleName": str,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
+    },
+)
+_OptionalCreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMonitoringScheduleRequestRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateMonitoringScheduleRequestRequestTypeDef(
+    _RequiredCreateMonitoringScheduleRequestRequestTypeDef,
+    _OptionalCreateMonitoringScheduleRequestRequestTypeDef,
+):
+    pass
+
 DescribeMonitoringScheduleResponseTypeDef = TypedDict(
     "DescribeMonitoringScheduleResponseTypeDef",
     {
         "MonitoringScheduleArn": str,
         "MonitoringScheduleName": str,
         "MonitoringScheduleStatus": ScheduleStatusType,
         "MonitoringType": MonitoringTypeType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigOutputTypeDef,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
         "EndpointName": str,
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelDashboardMonitoringScheduleTypeDef = TypedDict(
@@ -18577,15 +17012,15 @@
         "MonitoringScheduleArn": str,
         "MonitoringScheduleName": str,
         "MonitoringScheduleStatus": ScheduleStatusType,
         "MonitoringType": MonitoringTypeType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigOutputTypeDef,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
         "EndpointName": str,
         "MonitoringAlertSummaries": List[MonitoringAlertSummaryTypeDef],
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
     },
     total=False,
 )
 
@@ -18595,84 +17030,111 @@
         "MonitoringScheduleArn": str,
         "MonitoringScheduleName": str,
         "MonitoringScheduleStatus": ScheduleStatusType,
         "MonitoringType": MonitoringTypeType,
         "FailureReason": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigOutputTypeDef,
+        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
         "EndpointName": str,
         "LastMonitoringExecutionSummary": MonitoringExecutionSummaryTypeDef,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMonitoringScheduleRequestRequestTypeDef",
+UpdateMonitoringScheduleRequestRequestTypeDef = TypedDict(
+    "UpdateMonitoringScheduleRequestRequestTypeDef",
     {
         "MonitoringScheduleName": str,
         "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
     },
 )
-_OptionalCreateMonitoringScheduleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMonitoringScheduleRequestRequestTypeDef",
+
+_RequiredCreateAlgorithmInputRequestTypeDef = TypedDict(
+    "_RequiredCreateAlgorithmInputRequestTypeDef",
     {
+        "AlgorithmName": str,
+        "TrainingSpecification": TrainingSpecificationTypeDef,
+    },
+)
+_OptionalCreateAlgorithmInputRequestTypeDef = TypedDict(
+    "_OptionalCreateAlgorithmInputRequestTypeDef",
+    {
+        "AlgorithmDescription": str,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "ValidationSpecification": AlgorithmValidationSpecificationTypeDef,
+        "CertifyForMarketplace": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class CreateMonitoringScheduleRequestRequestTypeDef(
-    _RequiredCreateMonitoringScheduleRequestRequestTypeDef,
-    _OptionalCreateMonitoringScheduleRequestRequestTypeDef,
+class CreateAlgorithmInputRequestTypeDef(
+    _RequiredCreateAlgorithmInputRequestTypeDef, _OptionalCreateAlgorithmInputRequestTypeDef
 ):
     pass
 
-MonitoringScheduleConfigUnionTypeDef = Union[
-    MonitoringScheduleConfigTypeDef, MonitoringScheduleConfigOutputTypeDef
-]
-UpdateMonitoringScheduleRequestRequestTypeDef = TypedDict(
-    "UpdateMonitoringScheduleRequestRequestTypeDef",
-    {
-        "MonitoringScheduleName": str,
-        "MonitoringScheduleConfig": MonitoringScheduleConfigTypeDef,
-    },
-)
-
 DescribeAlgorithmOutputTypeDef = TypedDict(
     "DescribeAlgorithmOutputTypeDef",
     {
         "AlgorithmName": str,
         "AlgorithmArn": str,
         "AlgorithmDescription": str,
         "CreationTime": datetime,
-        "TrainingSpecification": TrainingSpecificationOutputTypeDef,
-        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
-        "ValidationSpecification": AlgorithmValidationSpecificationOutputTypeDef,
+        "TrainingSpecification": TrainingSpecificationTypeDef,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "ValidationSpecification": AlgorithmValidationSpecificationTypeDef,
         "AlgorithmStatus": AlgorithmStatusType,
         "AlgorithmStatusDetails": AlgorithmStatusDetailsTypeDef,
         "ProductId": str,
         "CertifyForMarketplace": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CreateModelPackageInputRequestTypeDef = TypedDict(
+    "CreateModelPackageInputRequestTypeDef",
+    {
+        "ModelPackageName": str,
+        "ModelPackageGroupName": str,
+        "ModelPackageDescription": str,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "ValidationSpecification": ModelPackageValidationSpecificationTypeDef,
+        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationTypeDef,
+        "CertifyForMarketplace": bool,
+        "Tags": Sequence[TagTypeDef],
+        "ModelApprovalStatus": ModelApprovalStatusType,
+        "MetadataProperties": MetadataPropertiesTypeDef,
+        "ModelMetrics": ModelMetricsTypeDef,
+        "ClientToken": str,
+        "CustomerMetadataProperties": Mapping[str, str],
+        "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
+        "Domain": str,
+        "Task": str,
+        "SamplePayloadUrl": str,
+        "AdditionalInferenceSpecifications": Sequence[
+            AdditionalInferenceSpecificationDefinitionTypeDef
+        ],
+    },
+    total=False,
+)
+
 DescribeModelPackageOutputTypeDef = TypedDict(
     "DescribeModelPackageOutputTypeDef",
     {
         "ModelPackageName": str,
         "ModelPackageGroupName": str,
         "ModelPackageVersion": int,
         "ModelPackageArn": str,
         "ModelPackageDescription": str,
         "CreationTime": datetime,
-        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
-        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationOutputTypeDef,
-        "ValidationSpecification": ModelPackageValidationSpecificationOutputTypeDef,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationTypeDef,
+        "ValidationSpecification": ModelPackageValidationSpecificationTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
         "ModelPackageStatusDetails": ModelPackageStatusDetailsTypeDef,
         "CertifyForMarketplace": bool,
         "ModelApprovalStatus": ModelApprovalStatusType,
         "CreatedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
         "ModelMetrics": ModelMetricsTypeDef,
@@ -18681,112 +17143,55 @@
         "ApprovalDescription": str,
         "CustomerMetadataProperties": Dict[str, str],
         "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
         "Domain": str,
         "Task": str,
         "SamplePayloadUrl": str,
         "AdditionalInferenceSpecifications": List[
-            AdditionalInferenceSpecificationDefinitionOutputTypeDef
+            AdditionalInferenceSpecificationDefinitionTypeDef
         ],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModelPackageTypeDef = TypedDict(
     "ModelPackageTypeDef",
     {
         "ModelPackageName": str,
         "ModelPackageGroupName": str,
         "ModelPackageVersion": int,
         "ModelPackageArn": str,
         "ModelPackageDescription": str,
         "CreationTime": datetime,
-        "InferenceSpecification": InferenceSpecificationOutputTypeDef,
-        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationOutputTypeDef,
-        "ValidationSpecification": ModelPackageValidationSpecificationOutputTypeDef,
+        "InferenceSpecification": InferenceSpecificationTypeDef,
+        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationTypeDef,
+        "ValidationSpecification": ModelPackageValidationSpecificationTypeDef,
         "ModelPackageStatus": ModelPackageStatusType,
         "ModelPackageStatusDetails": ModelPackageStatusDetailsTypeDef,
         "CertifyForMarketplace": bool,
         "ModelApprovalStatus": ModelApprovalStatusType,
         "CreatedBy": UserContextTypeDef,
         "MetadataProperties": MetadataPropertiesTypeDef,
         "ModelMetrics": ModelMetricsTypeDef,
         "LastModifiedTime": datetime,
         "LastModifiedBy": UserContextTypeDef,
         "ApprovalDescription": str,
         "Domain": str,
         "Task": str,
         "SamplePayloadUrl": str,
         "AdditionalInferenceSpecifications": List[
-            AdditionalInferenceSpecificationDefinitionOutputTypeDef
+            AdditionalInferenceSpecificationDefinitionTypeDef
         ],
         "Tags": List[TagTypeDef],
         "CustomerMetadataProperties": Dict[str, str],
         "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
     },
     total=False,
 )
 
-AlgorithmValidationSpecificationUnionTypeDef = Union[
-    AlgorithmValidationSpecificationTypeDef, AlgorithmValidationSpecificationOutputTypeDef
-]
-_RequiredCreateAlgorithmInputRequestTypeDef = TypedDict(
-    "_RequiredCreateAlgorithmInputRequestTypeDef",
-    {
-        "AlgorithmName": str,
-        "TrainingSpecification": TrainingSpecificationTypeDef,
-    },
-)
-_OptionalCreateAlgorithmInputRequestTypeDef = TypedDict(
-    "_OptionalCreateAlgorithmInputRequestTypeDef",
-    {
-        "AlgorithmDescription": str,
-        "InferenceSpecification": InferenceSpecificationTypeDef,
-        "ValidationSpecification": AlgorithmValidationSpecificationTypeDef,
-        "CertifyForMarketplace": bool,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateAlgorithmInputRequestTypeDef(
-    _RequiredCreateAlgorithmInputRequestTypeDef, _OptionalCreateAlgorithmInputRequestTypeDef
-):
-    pass
-
-CreateModelPackageInputRequestTypeDef = TypedDict(
-    "CreateModelPackageInputRequestTypeDef",
-    {
-        "ModelPackageName": str,
-        "ModelPackageGroupName": str,
-        "ModelPackageDescription": str,
-        "InferenceSpecification": InferenceSpecificationTypeDef,
-        "ValidationSpecification": ModelPackageValidationSpecificationTypeDef,
-        "SourceAlgorithmSpecification": SourceAlgorithmSpecificationTypeDef,
-        "CertifyForMarketplace": bool,
-        "Tags": Sequence[TagTypeDef],
-        "ModelApprovalStatus": ModelApprovalStatusType,
-        "MetadataProperties": MetadataPropertiesTypeDef,
-        "ModelMetrics": ModelMetricsTypeDef,
-        "ClientToken": str,
-        "CustomerMetadataProperties": Mapping[str, str],
-        "DriftCheckBaselines": DriftCheckBaselinesTypeDef,
-        "Domain": str,
-        "Task": str,
-        "SamplePayloadUrl": str,
-        "AdditionalInferenceSpecifications": Sequence[
-            AdditionalInferenceSpecificationDefinitionUnionTypeDef
-        ],
-    },
-    total=False,
-)
-
-ModelPackageValidationSpecificationUnionTypeDef = Union[
-    ModelPackageValidationSpecificationTypeDef, ModelPackageValidationSpecificationOutputTypeDef
-]
 ModelDashboardModelTypeDef = TypedDict(
     "ModelDashboardModelTypeDef",
     {
         "Model": ModelTypeDef,
         "Endpoints": List[ModelDashboardEndpointTypeDef],
         "LastBatchTransformJob": TransformJobTypeDef,
         "MonitoringSchedules": List[ModelDashboardMonitoringScheduleTypeDef],
```

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/waiter.py` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker/waiter.pyi` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.5.2.post1/types_aiobotocore_sagemaker.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-2.5.2.post2/types_aiobotocore_sagemaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

