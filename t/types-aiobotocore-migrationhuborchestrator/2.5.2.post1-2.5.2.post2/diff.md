# Comparing `tmp/types-aiobotocore-migrationhuborchestrator-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-migrationhuborchestrator-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-migrationhuborchestrator-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-migrationhuborchestrator-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1.tar` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:41.369519 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18475 2023-08-02 14:52:41.365519 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16889 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:41.369519 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:41.365519 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27093 2023-08-02 14:43:43.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27049 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9988 2023-08-02 14:43:43.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9986 2023-08-02 14:43:43.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-08-02 14:43:43.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-08-02 14:43:43.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    32650 2023-08-02 14:43:43.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32622 2023-08-02 14:43:43.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:41.365519 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18475 2023-08-02 14:52:41.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-02 14:52:41.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:41.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:41.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:41.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 14:52:41.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.076643 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14781 2023-08-04 13:59:19.076643 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13195 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.076643 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:58:46.126642 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.076643 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2061 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2060 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1011 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27081 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27037 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10083 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10081 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9801 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9792 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31838 2023-08-04 13:45:10.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31810 2023-08-04 13:45:09.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:08.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.076643 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14781 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1136 2023-08-04 13:59:19.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       43 2023-08-04 13:59:19.000000 types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/LICENSE` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/__init__.py` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/__init__.pyi` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/__main__.py` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.MigrationHubOrchestrator 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator\nOther"
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

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/client.py` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,21 +47,21 @@
     ListTagsForResourceResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
-    StepInputUnionTypeDef,
+    StepInputTypeDef,
     StopMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepResponseTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
-    WorkflowStepUnionTypeDef,
+    WorkflowStepOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -121,15 +121,15 @@
 
     async def create_workflow(
         self,
         *,
         name: str,
         templateId: str,
         applicationConfigurationId: str,
-        inputParameters: Mapping[str, StepInputUnionTypeDef],
+        inputParameters: Mapping[str, StepInputTypeDef],
         description: str = ...,
         stepTargets: Sequence[str] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateMigrationWorkflowResponseTypeDef:
         """
         Create a workflow to orchestrate your migrations.
 
@@ -143,15 +143,15 @@
         name: str,
         stepGroupId: str,
         workflowId: str,
         stepActionType: StepActionTypeType,
         description: str = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[WorkflowStepUnionTypeDef] = ...,
+        outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...
     ) -> CreateWorkflowStepResponseTypeDef:
         """
         Create a step in the migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step)
@@ -402,15 +402,15 @@
 
     async def update_workflow(
         self,
         *,
         id: str,
         name: str = ...,
         description: str = ...,
-        inputParameters: Mapping[str, StepInputUnionTypeDef] = ...,
+        inputParameters: Mapping[str, StepInputTypeDef] = ...,
         stepTargets: Sequence[str] = ...
     ) -> UpdateMigrationWorkflowResponseTypeDef:
         """
         Update a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#update_workflow)
@@ -423,15 +423,15 @@
         stepGroupId: str,
         workflowId: str,
         name: str = ...,
         description: str = ...,
         stepActionType: StepActionTypeType = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[WorkflowStepUnionTypeDef] = ...,
+        outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...,
         status: StepStatusType = ...
     ) -> UpdateWorkflowStepResponseTypeDef:
         """
         Update a step in a migration workflow.
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/client.pyi` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -47,21 +47,21 @@
     ListTagsForResourceResponseTypeDef,
     ListTemplateStepGroupsResponseTypeDef,
     ListTemplateStepsResponseTypeDef,
     ListWorkflowStepGroupsResponseTypeDef,
     ListWorkflowStepsResponseTypeDef,
     RetryWorkflowStepResponseTypeDef,
     StartMigrationWorkflowResponseTypeDef,
-    StepInputUnionTypeDef,
+    StepInputTypeDef,
     StopMigrationWorkflowResponseTypeDef,
     UpdateMigrationWorkflowResponseTypeDef,
     UpdateWorkflowStepGroupResponseTypeDef,
     UpdateWorkflowStepResponseTypeDef,
     WorkflowStepAutomationConfigurationTypeDef,
-    WorkflowStepUnionTypeDef,
+    WorkflowStepOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -114,15 +114,15 @@
         """
     async def create_workflow(
         self,
         *,
         name: str,
         templateId: str,
         applicationConfigurationId: str,
-        inputParameters: Mapping[str, StepInputUnionTypeDef],
+        inputParameters: Mapping[str, StepInputTypeDef],
         description: str = ...,
         stepTargets: Sequence[str] = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateMigrationWorkflowResponseTypeDef:
         """
         Create a workflow to orchestrate your migrations.
 
@@ -135,15 +135,15 @@
         name: str,
         stepGroupId: str,
         workflowId: str,
         stepActionType: StepActionTypeType,
         description: str = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[WorkflowStepUnionTypeDef] = ...,
+        outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...
     ) -> CreateWorkflowStepResponseTypeDef:
         """
         Create a step in the migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.create_workflow_step)
@@ -369,15 +369,15 @@
         """
     async def update_workflow(
         self,
         *,
         id: str,
         name: str = ...,
         description: str = ...,
-        inputParameters: Mapping[str, StepInputUnionTypeDef] = ...,
+        inputParameters: Mapping[str, StepInputTypeDef] = ...,
         stepTargets: Sequence[str] = ...
     ) -> UpdateMigrationWorkflowResponseTypeDef:
         """
         Update a migration workflow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#MigrationHubOrchestrator.Client.update_workflow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/client/#update_workflow)
@@ -389,15 +389,15 @@
         stepGroupId: str,
         workflowId: str,
         name: str = ...,
         description: str = ...,
         stepActionType: StepActionTypeType = ...,
         workflowStepAutomationConfiguration: WorkflowStepAutomationConfigurationTypeDef = ...,
         stepTarget: Sequence[str] = ...,
-        outputs: Sequence[WorkflowStepUnionTypeDef] = ...,
+        outputs: Sequence[WorkflowStepOutputTypeDef] = ...,
         previous: Sequence[str] = ...,
         next: Sequence[str] = ...,
         status: StepStatusType = ...
     ) -> UpdateWorkflowStepResponseTypeDef:
         """
         Update a step in a migration workflow.
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/literals.py` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
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
@@ -209,14 +210,15 @@
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
@@ -295,26 +297,28 @@
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

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/literals.pyi` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
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
@@ -207,14 +208,15 @@
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
@@ -293,26 +295,28 @@
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

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/paginator.py` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/paginator.pyi` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/type_defs.py` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for migrationhuborchestrator service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_migrationhuborchestrator.type_defs import ResponseMetadataTypeDef
+    from types_aiobotocore_migrationhuborchestrator.type_defs import StepInputTypeDef
 
-    data: ResponseMetadataTypeDef = ...
+    data: StepInputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     DataTypeType,
     MigrationWorkflowStatusEnumType,
     OwnerType,
     PluginHealthType,
     RunEnvironmentType,
@@ -34,16 +34,16 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "StepInputTypeDef",
     "ResponseMetadataTypeDef",
-    "StepInputOutputTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
     "GetMigrationWorkflowRequestRequestTypeDef",
     "GetMigrationWorkflowTemplateRequestRequestTypeDef",
@@ -69,30 +69,30 @@
     "WorkflowStepGroupSummaryTypeDef",
     "ListWorkflowStepsRequestRequestTypeDef",
     "WorkflowStepSummaryTypeDef",
     "PlatformCommandTypeDef",
     "PlatformScriptKeyTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
-    "StepInputTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
-    "WorkflowStepOutputUnionOutputTypeDef",
     "WorkflowStepOutputUnionTypeDef",
+    "CreateMigrationWorkflowRequestRequestTypeDef",
+    "UpdateMigrationWorkflowRequestRequestTypeDef",
+    "CreateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowResponseTypeDef",
-    "UpdateWorkflowStepResponseTypeDef",
-    "CreateMigrationWorkflowResponseTypeDef",
     "UpdateMigrationWorkflowResponseTypeDef",
+    "UpdateWorkflowStepResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
     "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
@@ -107,47 +107,43 @@
     "ListPluginsResponseTypeDef",
     "ListTemplateStepGroupsResponseTypeDef",
     "ListTemplateStepsResponseTypeDef",
     "ListWorkflowStepGroupsResponseTypeDef",
     "ListWorkflowStepsResponseTypeDef",
     "StepAutomationConfigurationTypeDef",
     "WorkflowStepAutomationConfigurationTypeDef",
-    "StepInputUnionTypeDef",
     "WorkflowStepOutputTypeDef",
     "GetTemplateStepResponseTypeDef",
-    "CreateMigrationWorkflowRequestRequestTypeDef",
-    "UpdateMigrationWorkflowRequestRequestTypeDef",
-    "GetWorkflowStepResponseTypeDef",
-    "WorkflowStepUnionTypeDef",
     "CreateWorkflowStepRequestRequestTypeDef",
+    "GetWorkflowStepResponseTypeDef",
     "UpdateWorkflowStepRequestRequestTypeDef",
 )
 
+StepInputTypeDef = TypedDict(
+    "StepInputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringsValue": Sequence[str],
+        "mapOfStringValue": Mapping[str, str],
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-StepInputOutputTypeDef = TypedDict(
-    "StepInputOutputTypeDef",
-    {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringsValue": List[str],
-        "mapOfStringValue": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredCreateWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "name": str,
     },
 )
@@ -542,25 +538,14 @@
 StartMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StartMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-StepInputTypeDef = TypedDict(
-    "StepInputTypeDef",
-    {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringsValue": Sequence[str],
-        "mapOfStringValue": Mapping[str, str],
-    },
-    total=False,
-)
-
 StopMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StopMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -602,34 +587,94 @@
 class UpdateWorkflowStepGroupRequestRequestTypeDef(
     _RequiredUpdateWorkflowStepGroupRequestRequestTypeDef,
     _OptionalUpdateWorkflowStepGroupRequestRequestTypeDef,
 ):
     pass
 
 
-WorkflowStepOutputUnionOutputTypeDef = TypedDict(
-    "WorkflowStepOutputUnionOutputTypeDef",
+WorkflowStepOutputUnionTypeDef = TypedDict(
+    "WorkflowStepOutputUnionTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
-        "listOfStringValue": List[str],
+        "listOfStringValue": Sequence[str],
     },
     total=False,
 )
 
-WorkflowStepOutputUnionTypeDef = TypedDict(
-    "WorkflowStepOutputUnionTypeDef",
+_RequiredCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMigrationWorkflowRequestRequestTypeDef",
     {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringValue": Sequence[str],
+        "name": str,
+        "templateId": str,
+        "applicationConfigurationId": str,
+        "inputParameters": Mapping[str, StepInputTypeDef],
+    },
+)
+_OptionalCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMigrationWorkflowRequestRequestTypeDef",
+    {
+        "description": str,
+        "stepTargets": Sequence[str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
+class CreateMigrationWorkflowRequestRequestTypeDef(
+    _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
+    _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "inputParameters": Mapping[str, StepInputTypeDef],
+        "stepTargets": Sequence[str],
+    },
+    total=False,
+)
+
+
+class UpdateMigrationWorkflowRequestRequestTypeDef(
+    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
+    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
+):
+    pass
+
+
+CreateMigrationWorkflowResponseTypeDef = TypedDict(
+    "CreateMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "templateId": str,
+        "adsApplicationConfigurationId": str,
+        "workflowInputs": Dict[str, StepInputTypeDef],
+        "stepTargets": List[str],
+        "status": MigrationWorkflowStatusEnumType,
+        "creationTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateWorkflowStepResponseTypeDef = TypedDict(
     "CreateWorkflowStepResponseTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "workflowId": str,
         "name": str,
@@ -686,58 +731,40 @@
         "status": MigrationWorkflowStatusEnumType,
         "statusMessage": str,
         "lastStopTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWorkflowStepResponseTypeDef = TypedDict(
-    "UpdateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMigrationWorkflowResponseTypeDef = TypedDict(
-    "CreateMigrationWorkflowResponseTypeDef",
+UpdateMigrationWorkflowResponseTypeDef = TypedDict(
+    "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputOutputTypeDef],
+        "workflowInputs": Dict[str, StepInputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
+        "lastModifiedTime": datetime,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateMigrationWorkflowResponseTypeDef = TypedDict(
-    "UpdateMigrationWorkflowResponseTypeDef",
+UpdateWorkflowStepResponseTypeDef = TypedDict(
+    "UpdateWorkflowStepResponseTypeDef",
     {
         "id": str,
-        "arn": str,
+        "stepGroupId": str,
+        "workflowId": str,
         "name": str,
-        "description": str,
-        "templateId": str,
-        "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputOutputTypeDef],
-        "stepTargets": List[str],
-        "status": MigrationWorkflowStatusEnumType,
-        "creationTime": datetime,
-        "lastModifiedTime": datetime,
-        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkflowStepGroupResponseTypeDef = TypedDict(
     "CreateWorkflowStepGroupResponseTypeDef",
     {
@@ -769,15 +796,15 @@
         "lastStartTime": datetime,
         "lastStopTime": datetime,
         "lastModifiedTime": datetime,
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "totalSteps": int,
         "completedSteps": int,
-        "workflowInputs": Dict[str, StepInputOutputTypeDef],
+        "workflowInputs": Dict[str, StepInputTypeDef],
         "tags": Dict[str, str],
         "workflowBucket": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateStepGroupResponseTypeDef = TypedDict(
@@ -1047,22 +1074,21 @@
         "command": PlatformCommandTypeDef,
         "runEnvironment": RunEnvironmentType,
         "targetType": TargetTypeType,
     },
     total=False,
 )
 
-StepInputUnionTypeDef = Union[StepInputTypeDef, StepInputOutputTypeDef]
 WorkflowStepOutputTypeDef = TypedDict(
     "WorkflowStepOutputTypeDef",
     {
         "name": str,
         "dataType": DataTypeType,
         "required": bool,
-        "value": WorkflowStepOutputUnionOutputTypeDef,
+        "value": WorkflowStepOutputUnionTypeDef,
     },
     total=False,
 )
 
 GetTemplateStepResponseTypeDef = TypedDict(
     "GetTemplateStepResponseTypeDef",
     {
@@ -1077,62 +1103,40 @@
         "next": List[str],
         "outputs": List[StepOutputTypeDef],
         "stepAutomationConfiguration": StepAutomationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMigrationWorkflowRequestRequestTypeDef",
+_RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
-        "templateId": str,
-        "applicationConfigurationId": str,
-        "inputParameters": Mapping[str, StepInputUnionTypeDef],
-    },
-)
-_OptionalCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "description": str,
-        "stepTargets": Sequence[str],
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateMigrationWorkflowRequestRequestTypeDef(
-    _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
-    _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "stepActionType": StepActionTypeType,
     },
 )
-_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
+_OptionalCreateWorkflowStepRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkflowStepRequestRequestTypeDef",
     {
-        "name": str,
         "description": str,
-        "inputParameters": Mapping[str, StepInputUnionTypeDef],
-        "stepTargets": Sequence[str],
+        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
+        "stepTarget": Sequence[str],
+        "outputs": Sequence[WorkflowStepOutputTypeDef],
+        "previous": Sequence[str],
+        "next": Sequence[str],
     },
     total=False,
 )
 
 
-class UpdateMigrationWorkflowRequestRequestTypeDef(
-    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
-    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
+class CreateWorkflowStepRequestRequestTypeDef(
+    _RequiredCreateWorkflowStepRequestRequestTypeDef,
+    _OptionalCreateWorkflowStepRequestRequestTypeDef,
 ):
     pass
 
 
 GetWorkflowStepResponseTypeDef = TypedDict(
     "GetWorkflowStepResponseTypeDef",
     {
@@ -1157,45 +1161,14 @@
         "noOfSrvCompleted": int,
         "noOfSrvFailed": int,
         "totalNoOfSrv": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WorkflowStepUnionTypeDef = Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]
-_RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkflowStepRequestRequestTypeDef",
-    {
-        "name": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "stepActionType": StepActionTypeType,
-    },
-)
-_OptionalCreateWorkflowStepRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkflowStepRequestRequestTypeDef",
-    {
-        "description": str,
-        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
-        "stepTarget": Sequence[str],
-        "outputs": Sequence[WorkflowStepUnionTypeDef],
-        "previous": Sequence[str],
-        "next": Sequence[str],
-    },
-    total=False,
-)
-
-
-class CreateWorkflowStepRequestRequestTypeDef(
-    _RequiredCreateWorkflowStepRequestRequestTypeDef,
-    _OptionalCreateWorkflowStepRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredUpdateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkflowStepRequestRequestTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "workflowId": str,
     },
@@ -1204,15 +1177,15 @@
     "_OptionalUpdateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
         "stepActionType": StepActionTypeType,
         "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
         "stepTarget": Sequence[str],
-        "outputs": Sequence[WorkflowStepUnionTypeDef],
+        "outputs": Sequence[WorkflowStepOutputTypeDef],
         "previous": Sequence[str],
         "next": Sequence[str],
         "status": StepStatusType,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator/type_defs.pyi` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for migrationhuborchestrator service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhuborchestrator/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_migrationhuborchestrator.type_defs import ResponseMetadataTypeDef
+    from types_aiobotocore_migrationhuborchestrator.type_defs import StepInputTypeDef
 
-    data: ResponseMetadataTypeDef = ...
+    data: StepInputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     DataTypeType,
     MigrationWorkflowStatusEnumType,
     OwnerType,
     PluginHealthType,
     RunEnvironmentType,
@@ -33,16 +33,16 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "StepInputTypeDef",
     "ResponseMetadataTypeDef",
-    "StepInputOutputTypeDef",
     "CreateWorkflowStepGroupRequestRequestTypeDef",
     "ToolTypeDef",
     "DeleteMigrationWorkflowRequestRequestTypeDef",
     "DeleteWorkflowStepGroupRequestRequestTypeDef",
     "DeleteWorkflowStepRequestRequestTypeDef",
     "GetMigrationWorkflowRequestRequestTypeDef",
     "GetMigrationWorkflowTemplateRequestRequestTypeDef",
@@ -68,30 +68,30 @@
     "WorkflowStepGroupSummaryTypeDef",
     "ListWorkflowStepsRequestRequestTypeDef",
     "WorkflowStepSummaryTypeDef",
     "PlatformCommandTypeDef",
     "PlatformScriptKeyTypeDef",
     "RetryWorkflowStepRequestRequestTypeDef",
     "StartMigrationWorkflowRequestRequestTypeDef",
-    "StepInputTypeDef",
     "StopMigrationWorkflowRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateWorkflowStepGroupRequestRequestTypeDef",
-    "WorkflowStepOutputUnionOutputTypeDef",
     "WorkflowStepOutputUnionTypeDef",
+    "CreateMigrationWorkflowRequestRequestTypeDef",
+    "UpdateMigrationWorkflowRequestRequestTypeDef",
+    "CreateMigrationWorkflowResponseTypeDef",
     "CreateWorkflowStepResponseTypeDef",
     "DeleteMigrationWorkflowResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RetryWorkflowStepResponseTypeDef",
     "StartMigrationWorkflowResponseTypeDef",
     "StopMigrationWorkflowResponseTypeDef",
-    "UpdateWorkflowStepResponseTypeDef",
-    "CreateMigrationWorkflowResponseTypeDef",
     "UpdateMigrationWorkflowResponseTypeDef",
+    "UpdateWorkflowStepResponseTypeDef",
     "CreateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowResponseTypeDef",
     "GetTemplateStepGroupResponseTypeDef",
     "GetWorkflowStepGroupResponseTypeDef",
     "UpdateWorkflowStepGroupResponseTypeDef",
     "GetMigrationWorkflowTemplateResponseTypeDef",
     "ListMigrationWorkflowTemplatesRequestListTemplatesPaginateTypeDef",
@@ -106,47 +106,43 @@
     "ListPluginsResponseTypeDef",
     "ListTemplateStepGroupsResponseTypeDef",
     "ListTemplateStepsResponseTypeDef",
     "ListWorkflowStepGroupsResponseTypeDef",
     "ListWorkflowStepsResponseTypeDef",
     "StepAutomationConfigurationTypeDef",
     "WorkflowStepAutomationConfigurationTypeDef",
-    "StepInputUnionTypeDef",
     "WorkflowStepOutputTypeDef",
     "GetTemplateStepResponseTypeDef",
-    "CreateMigrationWorkflowRequestRequestTypeDef",
-    "UpdateMigrationWorkflowRequestRequestTypeDef",
-    "GetWorkflowStepResponseTypeDef",
-    "WorkflowStepUnionTypeDef",
     "CreateWorkflowStepRequestRequestTypeDef",
+    "GetWorkflowStepResponseTypeDef",
     "UpdateWorkflowStepRequestRequestTypeDef",
 )
 
+StepInputTypeDef = TypedDict(
+    "StepInputTypeDef",
+    {
+        "integerValue": int,
+        "stringValue": str,
+        "listOfStringsValue": Sequence[str],
+        "mapOfStringValue": Mapping[str, str],
+    },
+    total=False,
+)
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-StepInputOutputTypeDef = TypedDict(
-    "StepInputOutputTypeDef",
-    {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringsValue": List[str],
-        "mapOfStringValue": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredCreateWorkflowStepGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkflowStepGroupRequestRequestTypeDef",
     {
         "workflowId": str,
         "name": str,
     },
 )
@@ -531,25 +527,14 @@
 StartMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StartMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-StepInputTypeDef = TypedDict(
-    "StepInputTypeDef",
-    {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringsValue": Sequence[str],
-        "mapOfStringValue": Mapping[str, str],
-    },
-    total=False,
-)
-
 StopMigrationWorkflowRequestRequestTypeDef = TypedDict(
     "StopMigrationWorkflowRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -589,34 +574,90 @@
 
 class UpdateWorkflowStepGroupRequestRequestTypeDef(
     _RequiredUpdateWorkflowStepGroupRequestRequestTypeDef,
     _OptionalUpdateWorkflowStepGroupRequestRequestTypeDef,
 ):
     pass
 
-WorkflowStepOutputUnionOutputTypeDef = TypedDict(
-    "WorkflowStepOutputUnionOutputTypeDef",
+WorkflowStepOutputUnionTypeDef = TypedDict(
+    "WorkflowStepOutputUnionTypeDef",
     {
         "integerValue": int,
         "stringValue": str,
-        "listOfStringValue": List[str],
+        "listOfStringValue": Sequence[str],
     },
     total=False,
 )
 
-WorkflowStepOutputUnionTypeDef = TypedDict(
-    "WorkflowStepOutputUnionTypeDef",
+_RequiredCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMigrationWorkflowRequestRequestTypeDef",
     {
-        "integerValue": int,
-        "stringValue": str,
-        "listOfStringValue": Sequence[str],
+        "name": str,
+        "templateId": str,
+        "applicationConfigurationId": str,
+        "inputParameters": Mapping[str, StepInputTypeDef],
+    },
+)
+_OptionalCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMigrationWorkflowRequestRequestTypeDef",
+    {
+        "description": str,
+        "stepTargets": Sequence[str],
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+class CreateMigrationWorkflowRequestRequestTypeDef(
+    _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
+    _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
+    {
+        "name": str,
+        "description": str,
+        "inputParameters": Mapping[str, StepInputTypeDef],
+        "stepTargets": Sequence[str],
+    },
+    total=False,
+)
+
+class UpdateMigrationWorkflowRequestRequestTypeDef(
+    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
+    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
+):
+    pass
+
+CreateMigrationWorkflowResponseTypeDef = TypedDict(
+    "CreateMigrationWorkflowResponseTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "name": str,
+        "description": str,
+        "templateId": str,
+        "adsApplicationConfigurationId": str,
+        "workflowInputs": Dict[str, StepInputTypeDef],
+        "stepTargets": List[str],
+        "status": MigrationWorkflowStatusEnumType,
+        "creationTime": datetime,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateWorkflowStepResponseTypeDef = TypedDict(
     "CreateWorkflowStepResponseTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "workflowId": str,
         "name": str,
@@ -673,58 +714,40 @@
         "status": MigrationWorkflowStatusEnumType,
         "statusMessage": str,
         "lastStopTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateWorkflowStepResponseTypeDef = TypedDict(
-    "UpdateWorkflowStepResponseTypeDef",
-    {
-        "id": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "name": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateMigrationWorkflowResponseTypeDef = TypedDict(
-    "CreateMigrationWorkflowResponseTypeDef",
+UpdateMigrationWorkflowResponseTypeDef = TypedDict(
+    "UpdateMigrationWorkflowResponseTypeDef",
     {
         "id": str,
         "arn": str,
         "name": str,
         "description": str,
         "templateId": str,
         "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputOutputTypeDef],
+        "workflowInputs": Dict[str, StepInputTypeDef],
         "stepTargets": List[str],
         "status": MigrationWorkflowStatusEnumType,
         "creationTime": datetime,
+        "lastModifiedTime": datetime,
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateMigrationWorkflowResponseTypeDef = TypedDict(
-    "UpdateMigrationWorkflowResponseTypeDef",
+UpdateWorkflowStepResponseTypeDef = TypedDict(
+    "UpdateWorkflowStepResponseTypeDef",
     {
         "id": str,
-        "arn": str,
+        "stepGroupId": str,
+        "workflowId": str,
         "name": str,
-        "description": str,
-        "templateId": str,
-        "adsApplicationConfigurationId": str,
-        "workflowInputs": Dict[str, StepInputOutputTypeDef],
-        "stepTargets": List[str],
-        "status": MigrationWorkflowStatusEnumType,
-        "creationTime": datetime,
-        "lastModifiedTime": datetime,
-        "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateWorkflowStepGroupResponseTypeDef = TypedDict(
     "CreateWorkflowStepGroupResponseTypeDef",
     {
@@ -756,15 +779,15 @@
         "lastStartTime": datetime,
         "lastStopTime": datetime,
         "lastModifiedTime": datetime,
         "endTime": datetime,
         "tools": List[ToolTypeDef],
         "totalSteps": int,
         "completedSteps": int,
-        "workflowInputs": Dict[str, StepInputOutputTypeDef],
+        "workflowInputs": Dict[str, StepInputTypeDef],
         "tags": Dict[str, str],
         "workflowBucket": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTemplateStepGroupResponseTypeDef = TypedDict(
@@ -1026,22 +1049,21 @@
         "command": PlatformCommandTypeDef,
         "runEnvironment": RunEnvironmentType,
         "targetType": TargetTypeType,
     },
     total=False,
 )
 
-StepInputUnionTypeDef = Union[StepInputTypeDef, StepInputOutputTypeDef]
 WorkflowStepOutputTypeDef = TypedDict(
     "WorkflowStepOutputTypeDef",
     {
         "name": str,
         "dataType": DataTypeType,
         "required": bool,
-        "value": WorkflowStepOutputUnionOutputTypeDef,
+        "value": WorkflowStepOutputUnionTypeDef,
     },
     total=False,
 )
 
 GetTemplateStepResponseTypeDef = TypedDict(
     "GetTemplateStepResponseTypeDef",
     {
@@ -1056,59 +1078,39 @@
         "next": List[str],
         "outputs": List[StepOutputTypeDef],
         "stepAutomationConfiguration": StepAutomationConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMigrationWorkflowRequestRequestTypeDef",
+_RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
-        "templateId": str,
-        "applicationConfigurationId": str,
-        "inputParameters": Mapping[str, StepInputUnionTypeDef],
-    },
-)
-_OptionalCreateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "description": str,
-        "stepTargets": Sequence[str],
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateMigrationWorkflowRequestRequestTypeDef(
-    _RequiredCreateMigrationWorkflowRequestRequestTypeDef,
-    _OptionalCreateMigrationWorkflowRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateMigrationWorkflowRequestRequestTypeDef",
-    {
-        "id": str,
+        "stepGroupId": str,
+        "workflowId": str,
+        "stepActionType": StepActionTypeType,
     },
 )
-_OptionalUpdateMigrationWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateMigrationWorkflowRequestRequestTypeDef",
+_OptionalCreateWorkflowStepRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkflowStepRequestRequestTypeDef",
     {
-        "name": str,
         "description": str,
-        "inputParameters": Mapping[str, StepInputUnionTypeDef],
-        "stepTargets": Sequence[str],
+        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
+        "stepTarget": Sequence[str],
+        "outputs": Sequence[WorkflowStepOutputTypeDef],
+        "previous": Sequence[str],
+        "next": Sequence[str],
     },
     total=False,
 )
 
-class UpdateMigrationWorkflowRequestRequestTypeDef(
-    _RequiredUpdateMigrationWorkflowRequestRequestTypeDef,
-    _OptionalUpdateMigrationWorkflowRequestRequestTypeDef,
+class CreateWorkflowStepRequestRequestTypeDef(
+    _RequiredCreateWorkflowStepRequestRequestTypeDef,
+    _OptionalCreateWorkflowStepRequestRequestTypeDef,
 ):
     pass
 
 GetWorkflowStepResponseTypeDef = TypedDict(
     "GetWorkflowStepResponseTypeDef",
     {
         "name": str,
@@ -1132,43 +1134,14 @@
         "noOfSrvCompleted": int,
         "noOfSrvFailed": int,
         "totalNoOfSrv": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WorkflowStepUnionTypeDef = Union[WorkflowStepOutputTypeDef, WorkflowStepOutputTypeDef]
-_RequiredCreateWorkflowStepRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkflowStepRequestRequestTypeDef",
-    {
-        "name": str,
-        "stepGroupId": str,
-        "workflowId": str,
-        "stepActionType": StepActionTypeType,
-    },
-)
-_OptionalCreateWorkflowStepRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkflowStepRequestRequestTypeDef",
-    {
-        "description": str,
-        "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
-        "stepTarget": Sequence[str],
-        "outputs": Sequence[WorkflowStepUnionTypeDef],
-        "previous": Sequence[str],
-        "next": Sequence[str],
-    },
-    total=False,
-)
-
-class CreateWorkflowStepRequestRequestTypeDef(
-    _RequiredCreateWorkflowStepRequestRequestTypeDef,
-    _OptionalCreateWorkflowStepRequestRequestTypeDef,
-):
-    pass
-
 _RequiredUpdateWorkflowStepRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkflowStepRequestRequestTypeDef",
     {
         "id": str,
         "stepGroupId": str,
         "workflowId": str,
     },
@@ -1177,15 +1150,15 @@
     "_OptionalUpdateWorkflowStepRequestRequestTypeDef",
     {
         "name": str,
         "description": str,
         "stepActionType": StepActionTypeType,
         "workflowStepAutomationConfiguration": WorkflowStepAutomationConfigurationTypeDef,
         "stepTarget": Sequence[str],
-        "outputs": Sequence[WorkflowStepUnionTypeDef],
+        "outputs": Sequence[WorkflowStepOutputTypeDef],
         "previous": Sequence[str],
         "next": Sequence[str],
         "status": StepStatusType,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-migrationhuborchestrator-2.5.2.post1/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt` & `types-aiobotocore-migrationhuborchestrator-2.5.2.post2/types_aiobotocore_migrationhuborchestrator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

