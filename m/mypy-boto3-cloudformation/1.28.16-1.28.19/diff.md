# Comparing `tmp/mypy-boto3-cloudformation-1.28.16.tar.gz` & `tmp/mypy-boto3-cloudformation-1.28.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudformation-1.28.16.tar", last modified: Tue Aug  1 11:36:22 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudformation-1.28.19.tar", last modified: Fri Aug  4 11:22:32 2023, max compression
```

## Comparing `mypy-boto3-cloudformation-1.28.16.tar` & `mypy-boto3-cloudformation-1.28.19.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:22.236934 mypy-boto3-cloudformation-1.28.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-01 11:12:24.000000 mypy-boto3-cloudformation-1.28.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30157 2023-08-01 11:36:22.232934 mypy-boto3-cloudformation-1.28.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28645 2023-08-01 11:12:24.000000 mypy-boto3-cloudformation-1.28.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:22.228934 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-08-01 11:12:24.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-08-01 11:12:24.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 11:12:24.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66427 2023-08-01 11:12:25.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    66328 2023-08-01 11:12:25.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18517 2023-08-01 11:12:26.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18515 2023-08-01 11:12:26.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17280 2023-08-01 11:12:26.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-08-01 11:12:26.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:12:24.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22999 2023-08-01 11:12:26.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-08-01 11:12:26.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    94147 2023-08-01 11:12:30.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94030 2023-08-01 11:12:27.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 11:12:24.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-08-01 11:12:26.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8779 2023-08-01 11:12:26.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:22.232934 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30157 2023-08-01 11:36:21.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-01 11:36:22.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:21.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:21.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 11:36:21.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 11:36:21.000000 mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:22.236934 mypy-boto3-cloudformation-1.28.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-01 11:12:23.000000 mypy-boto3-cloudformation-1.28.16/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:22:32.346644 mypy-boto3-cloudformation-1.28.19/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 11:22:07.000000 mypy-boto3-cloudformation-1.28.19/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19219 2023-08-04 11:22:32.346644 mypy-boto3-cloudformation-1.28.19/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17707 2023-08-04 11:22:07.000000 mypy-boto3-cloudformation-1.28.19/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:22:32.346644 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5317 2023-08-04 11:22:07.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5315 2023-08-04 11:22:07.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      935 2023-08-04 11:22:07.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    66347 2023-08-04 11:22:08.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    66248 2023-08-04 11:22:08.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18537 2023-08-04 11:22:09.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18535 2023-08-04 11:22:09.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17400 2023-08-04 11:22:08.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17384 2023-08-04 11:22:08.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:22:07.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23020 2023-08-04 11:22:08.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22976 2023-08-04 11:22:08.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    97333 2023-08-04 11:22:11.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    97214 2023-08-04 11:22:10.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       61 2023-08-04 11:22:07.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8787 2023-08-04 11:22:08.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8779 2023-08-04 11:22:08.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 11:22:32.346644 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19219 2023-08-04 11:22:32.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      979 2023-08-04 11:22:32.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 11:22:32.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 11:22:32.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 11:22:32.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 11:22:32.000000 mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation.egg-info/top_level.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 11:22:32.346644 mypy-boto3-cloudformation-1.28.19/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2042 2023-08-04 11:22:07.000000 mypy-boto3-cloudformation-1.28.19/setup.py
```

### Comparing `mypy-boto3-cloudformation-1.28.16/LICENSE` & `mypy-boto3-cloudformation-1.28.19/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/__init__.py` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/__init__.pyi` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/client.py` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     AutoDeploymentTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     CreateChangeSetOutputTypeDef,
     CreateStackInstancesOutputTypeDef,
     CreateStackOutputTypeDef,
     CreateStackSetOutputTypeDef,
     DeleteStackInstancesOutputTypeDef,
-    DeploymentTargetsUnionTypeDef,
+    DeploymentTargetsTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeChangeSetHooksOutputTypeDef,
     DescribeChangeSetOutputTypeDef,
     DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusOutputTypeDef,
     DescribeStackEventsOutputTypeDef,
@@ -108,19 +108,19 @@
     ManagedExecutionTypeDef,
     OperationResultFilterTypeDef,
     ParameterTypeDef,
     PublishTypeOutputTypeDef,
     RegisterPublisherOutputTypeDef,
     RegisterTypeOutputTypeDef,
     ResourceToImportTypeDef,
-    RollbackConfigurationUnionTypeDef,
+    RollbackConfigurationTypeDef,
     RollbackStackOutputTypeDef,
     SetTypeConfigurationOutputTypeDef,
     StackInstanceFilterTypeDef,
-    StackSetOperationPreferencesUnionTypeDef,
+    StackSetOperationPreferencesTypeDef,
     TagTypeDef,
     TemplateSummaryConfigTypeDef,
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
@@ -290,15 +290,15 @@
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         Description: str = ...,
         ChangeSetType: ChangeSetTypeType = ...,
         ResourcesToImport: Sequence[ResourceToImportTypeDef] = ...,
         IncludeNestedStacks: bool = ...,
@@ -316,15 +316,15 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
@@ -343,17 +343,17 @@
 
     def create_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> CreateStackInstancesOutputTypeDef:
         """
         Creates stack instances for the specified accounts, within the specified Amazon
         Web Services Regions.
 
@@ -432,16 +432,16 @@
     def delete_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         RetainStacks: bool,
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DeleteStackInstancesOutputTypeDef:
         """
         Deletes stack instances for the specified accounts, in the specified Amazon Web
         Services Regions.
 
@@ -686,15 +686,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#detect_stack_resource_drift)
         """
 
     def detect_stack_set_drift(
         self,
         *,
         StackSetName: str,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DetectStackSetDriftOutputTypeDef:
         """
         Detect drift on a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_set_drift)
@@ -788,15 +788,15 @@
     def import_stacks_to_stack_set(
         self,
         *,
         StackSetName: str,
         StackIds: Sequence[str] = ...,
         StackIdsUrl: str = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> ImportStacksToStackSetOutputTypeDef:
         """
         Import existing stacks into a new stack sets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.import_stacks_to_stack_set)
@@ -1162,15 +1162,15 @@
         UsePreviousTemplate: bool = ...,
         StackPolicyDuringUpdateBody: str = ...,
         StackPolicyDuringUpdateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
         ClientRequestToken: str = ...,
         RetainExceptOnCreate: bool = ...
@@ -1184,17 +1184,17 @@
 
     def update_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> UpdateStackInstancesOutputTypeDef:
         """
         Updates the parameter values for stack instances for the specified accounts,
         within the specified Amazon Web Services Regions.
 
@@ -1209,18 +1209,18 @@
         Description: str = ...,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         AdministrationRoleARN: str = ...,
         ExecutionRoleName: str = ...,
-        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsTypeDef = ...,
         PermissionModel: PermissionModelsType = ...,
         AutoDeployment: AutoDeploymentTypeDef = ...,
         OperationId: str = ...,
         Accounts: Sequence[str] = ...,
         Regions: Sequence[str] = ...,
         CallAs: CallAsType = ...,
         ManagedExecution: ManagedExecutionTypeDef = ...
```

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/client.pyi` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     AutoDeploymentTypeDef,
     BatchDescribeTypeConfigurationsOutputTypeDef,
     CreateChangeSetOutputTypeDef,
     CreateStackInstancesOutputTypeDef,
     CreateStackOutputTypeDef,
     CreateStackSetOutputTypeDef,
     DeleteStackInstancesOutputTypeDef,
-    DeploymentTargetsUnionTypeDef,
+    DeploymentTargetsTypeDef,
     DescribeAccountLimitsOutputTypeDef,
     DescribeChangeSetHooksOutputTypeDef,
     DescribeChangeSetOutputTypeDef,
     DescribeOrganizationsAccessOutputTypeDef,
     DescribePublisherOutputTypeDef,
     DescribeStackDriftDetectionStatusOutputTypeDef,
     DescribeStackEventsOutputTypeDef,
@@ -108,19 +108,19 @@
     ManagedExecutionTypeDef,
     OperationResultFilterTypeDef,
     ParameterTypeDef,
     PublishTypeOutputTypeDef,
     RegisterPublisherOutputTypeDef,
     RegisterTypeOutputTypeDef,
     ResourceToImportTypeDef,
-    RollbackConfigurationUnionTypeDef,
+    RollbackConfigurationTypeDef,
     RollbackStackOutputTypeDef,
     SetTypeConfigurationOutputTypeDef,
     StackInstanceFilterTypeDef,
-    StackSetOperationPreferencesUnionTypeDef,
+    StackSetOperationPreferencesTypeDef,
     TagTypeDef,
     TemplateSummaryConfigTypeDef,
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
@@ -278,15 +278,15 @@
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientToken: str = ...,
         Description: str = ...,
         ChangeSetType: ChangeSetTypeType = ...,
         ResourcesToImport: Sequence[ResourceToImportTypeDef] = ...,
         IncludeNestedStacks: bool = ...,
@@ -303,15 +303,15 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
@@ -329,17 +329,17 @@
         """
     def create_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> CreateStackInstancesOutputTypeDef:
         """
         Creates stack instances for the specified accounts, within the specified Amazon
         Web Services Regions.
 
@@ -412,16 +412,16 @@
     def delete_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         RetainStacks: bool,
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DeleteStackInstancesOutputTypeDef:
         """
         Deletes stack instances for the specified accounts, in the specified Amazon Web
         Services Regions.
 
@@ -645,15 +645,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_resource_drift)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#detect_stack_resource_drift)
         """
     def detect_stack_set_drift(
         self,
         *,
         StackSetName: str,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> DetectStackSetDriftOutputTypeDef:
         """
         Detect drift on a stack set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_set_drift)
@@ -740,15 +740,15 @@
     def import_stacks_to_stack_set(
         self,
         *,
         StackSetName: str,
         StackIds: Sequence[str] = ...,
         StackIdsUrl: str = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> ImportStacksToStackSetOutputTypeDef:
         """
         Import existing stacks into a new stack sets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.import_stacks_to_stack_set)
@@ -1089,15 +1089,15 @@
         UsePreviousTemplate: bool = ...,
         StackPolicyDuringUpdateBody: str = ...,
         StackPolicyDuringUpdateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
-        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         StackPolicyBody: str = ...,
         StackPolicyURL: str = ...,
         NotificationARNs: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisableRollback: bool = ...,
         ClientRequestToken: str = ...,
         RetainExceptOnCreate: bool = ...
@@ -1110,17 +1110,17 @@
         """
     def update_stack_instances(
         self,
         *,
         StackSetName: str,
         Regions: Sequence[str],
         Accounts: Sequence[str] = ...,
-        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsTypeDef = ...,
         ParameterOverrides: Sequence[ParameterTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         OperationId: str = ...,
         CallAs: CallAsType = ...
     ) -> UpdateStackInstancesOutputTypeDef:
         """
         Updates the parameter values for stack instances for the specified accounts,
         within the specified Amazon Web Services Regions.
 
@@ -1134,18 +1134,18 @@
         Description: str = ...,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         UsePreviousTemplate: bool = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OperationPreferences: StackSetOperationPreferencesUnionTypeDef = ...,
+        OperationPreferences: StackSetOperationPreferencesTypeDef = ...,
         AdministrationRoleARN: str = ...,
         ExecutionRoleName: str = ...,
-        DeploymentTargets: DeploymentTargetsUnionTypeDef = ...,
+        DeploymentTargets: DeploymentTargetsTypeDef = ...,
         PermissionModel: PermissionModelsType = ...,
         AutoDeployment: AutoDeploymentTypeDef = ...,
         OperationId: str = ...,
         Accounts: Sequence[str] = ...,
         Regions: Sequence[str] = ...,
         CallAs: CallAsType = ...,
         ManagedExecution: ManagedExecutionTypeDef = ...
```

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/literals.py` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -703,14 +703,15 @@
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

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/literals.pyi` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -701,14 +701,15 @@
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

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/paginator.py` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,24 +56,24 @@
     RegistryTypeType,
     StackSetStatusType,
     StackStatusType,
     VisibilityType,
 )
 from .type_defs import (
     DescribeAccountLimitsOutputTypeDef,
-    DescribeChangeSetOutputTypeDef,
+    DescribeChangeSetOutputStackResourceSummaryTypeDef,
     DescribeStackEventsOutputTypeDef,
-    DescribeStacksOutputTypeDef,
+    DescribeStacksOutputStackResourceSummaryTypeDef,
     ListChangeSetsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListImportsOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     ListStackResourcesOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
-    ListStackSetOperationsOutputTypeDef,
+    ListStackSetOperationsOutputStackResourceSummaryTypeDef,
     ListStackSetsOutputTypeDef,
     ListStacksOutputTypeDef,
     ListTypesOutputTypeDef,
     OperationResultFilterTypeDef,
     PaginatorConfigTypeDef,
     StackInstanceFilterTypeDef,
     TypeFiltersTypeDef,
@@ -130,15 +130,15 @@
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeChangeSetOutputTypeDef]:
+    ) -> _PageIterator[DescribeChangeSetOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
         """
 
 
 class DescribeStackEventsPaginator(Paginator):
@@ -160,15 +160,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
         self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeStacksOutputTypeDef]:
+    ) -> _PageIterator[DescribeStacksOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
         """
 
 
 class ListChangeSetsPaginator(Paginator):
@@ -282,15 +282,15 @@
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListStackSetOperationsOutputTypeDef]:
+    ) -> _PageIterator[ListStackSetOperationsOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
 
 class ListStackSetsPaginator(Paginator):
```

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/paginator.pyi` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,24 +56,24 @@
     RegistryTypeType,
     StackSetStatusType,
     StackStatusType,
     VisibilityType,
 )
 from .type_defs import (
     DescribeAccountLimitsOutputTypeDef,
-    DescribeChangeSetOutputTypeDef,
+    DescribeChangeSetOutputStackResourceSummaryTypeDef,
     DescribeStackEventsOutputTypeDef,
-    DescribeStacksOutputTypeDef,
+    DescribeStacksOutputStackResourceSummaryTypeDef,
     ListChangeSetsOutputTypeDef,
     ListExportsOutputTypeDef,
     ListImportsOutputTypeDef,
     ListStackInstancesOutputTypeDef,
     ListStackResourcesOutputTypeDef,
     ListStackSetOperationResultsOutputTypeDef,
-    ListStackSetOperationsOutputTypeDef,
+    ListStackSetOperationsOutputStackResourceSummaryTypeDef,
     ListStackSetsOutputTypeDef,
     ListStacksOutputTypeDef,
     ListTypesOutputTypeDef,
     OperationResultFilterTypeDef,
     PaginatorConfigTypeDef,
     StackInstanceFilterTypeDef,
     TypeFiltersTypeDef,
@@ -126,15 +126,15 @@
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeChangeSetOutputTypeDef]:
+    ) -> _PageIterator[DescribeChangeSetOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
         """
 
 class DescribeStackEventsPaginator(Paginator):
     """
@@ -154,15 +154,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
         self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[DescribeStacksOutputTypeDef]:
+    ) -> _PageIterator[DescribeStacksOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describestackspaginator)
         """
 
 class ListChangeSetsPaginator(Paginator):
     """
@@ -269,15 +269,15 @@
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListStackSetOperationsOutputTypeDef]:
+    ) -> _PageIterator[ListStackSetOperationsOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
 class ListStackSetsPaginator(Paginator):
     """
```

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/service_resource.py` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,18 +34,19 @@
     HookStatusType,
     OnFailureType,
     ResourceStatusType,
     StackStatusType,
 )
 from .type_defs import (
     ModuleInfoResponseTypeDef,
+    ModuleInfoTypeDef,
     OutputTypeDef,
     ParameterTypeDef,
+    RollbackConfigurationResponseTypeDef,
     RollbackConfigurationTypeDef,
-    RollbackConfigurationUnionTypeDef,
     StackDriftInformationResponseTypeDef,
     StackResourceDriftInformationResponseTypeDef,
     StackResourceDriftInformationSummaryResponseTypeDef,
     TagTypeDef,
     UpdateStackOutputTypeDef,
 )
 
@@ -236,15 +237,15 @@
     stack_name: str
     change_set_id: str
     description: str
     parameters: List[ParameterTypeDef]
     creation_time: datetime
     deletion_time: datetime
     last_updated_time: datetime
-    rollback_configuration: RollbackConfigurationTypeDef
+    rollback_configuration: RollbackConfigurationResponseTypeDef
     stack_status: StackStatusType
     stack_status_reason: str
     disable_rollback: bool
     notification_arns: List[str]
     timeout_in_minutes: int
     capabilities: List[CapabilityType]
     outputs: List[OutputTypeDef]
@@ -359,15 +360,15 @@
     resource_type: str
     last_updated_timestamp: datetime
     resource_status: ResourceStatusType
     resource_status_reason: str
     description: str
     metadata: str
     drift_information: StackResourceDriftInformationResponseTypeDef
-    module_info: ModuleInfoResponseTypeDef
+    module_info: ModuleInfoTypeDef
     stack_name: str
     logical_id: str
 
     def Stack(self) -> _Stack:
         """
         Creates a Stack resource.
 
@@ -491,15 +492,15 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
```

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/service_resource.pyi` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -34,18 +34,19 @@
     HookStatusType,
     OnFailureType,
     ResourceStatusType,
     StackStatusType,
 )
 from .type_defs import (
     ModuleInfoResponseTypeDef,
+    ModuleInfoTypeDef,
     OutputTypeDef,
     ParameterTypeDef,
+    RollbackConfigurationResponseTypeDef,
     RollbackConfigurationTypeDef,
-    RollbackConfigurationUnionTypeDef,
     StackDriftInformationResponseTypeDef,
     StackResourceDriftInformationResponseTypeDef,
     StackResourceDriftInformationSummaryResponseTypeDef,
     TagTypeDef,
     UpdateStackOutputTypeDef,
 )
 
@@ -214,15 +215,15 @@
     stack_name: str
     change_set_id: str
     description: str
     parameters: List[ParameterTypeDef]
     creation_time: datetime
     deletion_time: datetime
     last_updated_time: datetime
-    rollback_configuration: RollbackConfigurationTypeDef
+    rollback_configuration: RollbackConfigurationResponseTypeDef
     stack_status: StackStatusType
     stack_status_reason: str
     disable_rollback: bool
     notification_arns: List[str]
     timeout_in_minutes: int
     capabilities: List[CapabilityType]
     outputs: List[OutputTypeDef]
@@ -329,15 +330,15 @@
     resource_type: str
     last_updated_timestamp: datetime
     resource_status: ResourceStatusType
     resource_status_reason: str
     description: str
     metadata: str
     drift_information: StackResourceDriftInformationResponseTypeDef
-    module_info: ModuleInfoResponseTypeDef
+    module_info: ModuleInfoTypeDef
     stack_name: str
     logical_id: str
 
     def Stack(self) -> _Stack:
         """
         Creates a Stack resource.
 
@@ -448,15 +449,15 @@
         self,
         *,
         StackName: str,
         TemplateBody: str = ...,
         TemplateURL: str = ...,
         Parameters: Sequence[ParameterTypeDef] = ...,
         DisableRollback: bool = ...,
-        RollbackConfiguration: RollbackConfigurationUnionTypeDef = ...,
+        RollbackConfiguration: RollbackConfigurationTypeDef = ...,
         TimeoutInMinutes: int = ...,
         NotificationARNs: Sequence[str] = ...,
         Capabilities: Sequence[CapabilityType] = ...,
         ResourceTypes: Sequence[str] = ...,
         RoleARN: str = ...,
         OnFailure: OnFailureType = ...,
         StackPolicyBody: str = ...,
```

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/type_defs.py` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_cloudformation.type_defs import AccountGateResultTypeDef
 
     data: AccountGateResultTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountFilterTypeType,
     AccountGateStatusType,
     CallAsType,
     CapabilityType,
     CategoryType,
@@ -99,15 +99,14 @@
     "StackSetOperationPreferencesTypeDef",
     "ManagedExecutionTypeDef",
     "DeactivateTypeInputRequestTypeDef",
     "DeleteChangeSetInputRequestTypeDef",
     "DeleteStackInputRequestTypeDef",
     "DeleteStackInputStackDeleteTypeDef",
     "DeleteStackSetInputRequestTypeDef",
-    "DeploymentTargetsOutputTypeDef",
     "DeregisterTypeInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "DescribeChangeSetHooksInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeChangeSetInputRequestTypeDef",
     "DescribeOrganizationsAccessInputRequestTypeDef",
@@ -145,15 +144,14 @@
     "ListStackSetsInputRequestTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
     "ListTypeVersionsInputRequestTypeDef",
     "TypeVersionSummaryTypeDef",
     "TypeFiltersTypeDef",
     "TypeSummaryTypeDef",
-    "ModuleInfoTypeDef",
     "OutputTypeDef",
     "ParameterConstraintsTypeDef",
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     "PropertyDifferenceTypeDef",
     "PublishTypeInputRequestTypeDef",
     "RecordHandlerProgressInputRequestTypeDef",
     "RegisterPublisherInputRequestTypeDef",
@@ -166,15 +164,15 @@
     "SignalResourceInputRequestTypeDef",
     "StackDriftInformationSummaryTypeDef",
     "StackDriftInformationTypeDef",
     "StackInstanceComprehensiveStatusTypeDef",
     "StackResourceDriftInformationTypeDef",
     "StackResourceDriftInformationSummaryTypeDef",
     "StackSetDriftDetectionDetailsTypeDef",
-    "StackSetOperationPreferencesOutputTypeDef",
+    "StackSetOperationPreferencesStackResourceSummaryTypeDef",
     "StackSetOperationStatusDetailsTypeDef",
     "StopStackSetOperationInputRequestTypeDef",
     "TemplateParameterTypeDef",
     "TestTypeInputRequestTypeDef",
     "UpdateTerminationProtectionInputRequestTypeDef",
     "ValidateTemplateInputRequestTypeDef",
     "StackSetOperationResultSummaryTypeDef",
@@ -197,14 +195,15 @@
     "EstimateTemplateCostOutputTypeDef",
     "GetStackPolicyOutputTypeDef",
     "GetTemplateOutputTypeDef",
     "ImportStacksToStackSetOutputTypeDef",
     "ListImportsOutputTypeDef",
     "ListTypeRegistrationsOutputTypeDef",
     "ModuleInfoResponseTypeDef",
+    "ModuleInfoTypeDef",
     "PublishTypeOutputTypeDef",
     "RegisterPublisherOutputTypeDef",
     "RegisterTypeOutputTypeDef",
     "RollbackStackOutputTypeDef",
     "SetTypeConfigurationOutputTypeDef",
     "StackDriftInformationResponseTypeDef",
     "StackResourceDriftInformationResponseTypeDef",
@@ -223,15 +222,14 @@
     "DeleteStackInstancesInputRequestTypeDef",
     "DetectStackSetDriftInputRequestTypeDef",
     "ImportStacksToStackSetInputRequestTypeDef",
     "UpdateStackInstancesInputRequestTypeDef",
     "CreateStackSetInputRequestTypeDef",
     "StackSetSummaryTypeDef",
     "UpdateStackSetInputRequestTypeDef",
-    "DeploymentTargetsUnionTypeDef",
     "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     "DescribeStacksInputDescribeStacksPaginateTypeDef",
     "ListChangeSetsInputListChangeSetsPaginateTypeDef",
     "ListExportsInputListExportsPaginateTypeDef",
     "ListImportsInputListImportsPaginateTypeDef",
@@ -257,57 +255,61 @@
     "ListStackSetOperationResultsInputRequestTypeDef",
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
     "ParameterDeclarationTypeDef",
     "StackInstanceResourceDriftsSummaryTypeDef",
-    "StackResourceDriftTypeDef",
     "ResourceChangeDetailTypeDef",
-    "RollbackConfigurationOutputTypeDef",
+    "RollbackConfigurationResponseTypeDef",
+    "RollbackConfigurationStackResourceSummaryTypeDef",
     "RollbackConfigurationTypeDef",
     "StackSummaryTypeDef",
     "StackInstanceSummaryTypeDef",
     "StackInstanceTypeDef",
-    "StackResourceDetailTypeDef",
-    "StackResourceTypeDef",
-    "StackResourceSummaryTypeDef",
     "StackSetTypeDef",
-    "StackSetOperationPreferencesUnionTypeDef",
+    "StackSetOperationSummaryStackResourceSummaryTypeDef",
     "StackSetOperationSummaryTypeDef",
     "StackSetOperationTypeDef",
     "ValidateTemplateOutputTypeDef",
     "ListStackSetOperationResultsOutputTypeDef",
+    "StackResourceDetailTypeDef",
+    "StackResourceDriftTypeDef",
+    "StackResourceSummaryTypeDef",
+    "StackResourceTypeDef",
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     "ChangeSetHookTypeDef",
     "ListStackSetsOutputTypeDef",
     "GetTemplateSummaryOutputTypeDef",
     "ListStackInstanceResourceDriftsOutputTypeDef",
-    "DescribeStackResourceDriftsOutputTypeDef",
-    "DetectStackResourceDriftOutputTypeDef",
     "ResourceChangeTypeDef",
-    "StackTypeDef",
+    "StackStackResourceSummaryTypeDef",
     "CreateChangeSetInputRequestTypeDef",
     "CreateStackInputRequestTypeDef",
     "CreateStackInputServiceResourceCreateStackTypeDef",
-    "RollbackConfigurationUnionTypeDef",
+    "StackTypeDef",
     "UpdateStackInputRequestTypeDef",
     "UpdateStackInputStackUpdateTypeDef",
     "ListStacksOutputTypeDef",
     "ListStackInstancesOutputTypeDef",
     "DescribeStackInstanceOutputTypeDef",
-    "DescribeStackResourceOutputTypeDef",
-    "DescribeStackResourcesOutputTypeDef",
-    "ListStackResourcesOutputTypeDef",
     "DescribeStackSetOutputTypeDef",
+    "ListStackSetOperationsOutputStackResourceSummaryTypeDef",
     "ListStackSetOperationsOutputTypeDef",
     "DescribeStackSetOperationOutputTypeDef",
+    "DescribeStackResourceOutputTypeDef",
+    "DescribeStackResourceDriftsOutputTypeDef",
+    "DetectStackResourceDriftOutputTypeDef",
+    "ListStackResourcesOutputTypeDef",
+    "DescribeStackResourcesOutputTypeDef",
     "DescribeChangeSetHooksOutputTypeDef",
     "ChangeTypeDef",
+    "DescribeStacksOutputStackResourceSummaryTypeDef",
     "DescribeStacksOutputTypeDef",
+    "DescribeChangeSetOutputStackResourceSummaryTypeDef",
     "DescribeChangeSetOutputTypeDef",
 )
 
 AccountGateResultTypeDef = TypedDict(
     "AccountGateResultTypeDef",
     {
         "Status": AccountGateStatusType,
@@ -602,25 +604,14 @@
 
 class DeleteStackSetInputRequestTypeDef(
     _RequiredDeleteStackSetInputRequestTypeDef, _OptionalDeleteStackSetInputRequestTypeDef
 ):
     pass
 
 
-DeploymentTargetsOutputTypeDef = TypedDict(
-    "DeploymentTargetsOutputTypeDef",
-    {
-        "Accounts": List[str],
-        "AccountsUrl": str,
-        "OrganizationalUnitIds": List[str],
-        "AccountFilterType": AccountFilterTypeType,
-    },
-    total=False,
-)
-
 DeregisterTypeInputRequestTypeDef = TypedDict(
     "DeregisterTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
@@ -1251,23 +1242,14 @@
         "PublisherIdentity": IdentityProviderType,
         "PublisherName": str,
         "IsActivated": bool,
     },
     total=False,
 )
 
-ModuleInfoTypeDef = TypedDict(
-    "ModuleInfoTypeDef",
-    {
-        "TypeHierarchy": str,
-        "LogicalIdHierarchy": str,
-    },
-    total=False,
-)
-
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "OutputKey": str,
         "OutputValue": str,
         "Description": str,
         "ExportName": str,
@@ -1561,16 +1543,16 @@
         "InSyncStackInstancesCount": int,
         "InProgressStackInstancesCount": int,
         "FailedStackInstancesCount": int,
     },
     total=False,
 )
 
-StackSetOperationPreferencesOutputTypeDef = TypedDict(
-    "StackSetOperationPreferencesOutputTypeDef",
+StackSetOperationPreferencesStackResourceSummaryTypeDef = TypedDict(
+    "StackSetOperationPreferencesStackResourceSummaryTypeDef",
     {
         "RegionConcurrencyType": RegionConcurrencyTypeType,
         "RegionOrder": List[str],
         "FailureToleranceCount": int,
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
@@ -1885,14 +1867,23 @@
     {
         "TypeHierarchy": str,
         "LogicalIdHierarchy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ModuleInfoTypeDef = TypedDict(
+    "ModuleInfoTypeDef",
+    {
+        "TypeHierarchy": str,
+        "LogicalIdHierarchy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PublishTypeOutputTypeDef = TypedDict(
     "PublishTypeOutputTypeDef",
     {
         "PublicTypeArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2259,15 +2250,14 @@
 
 class UpdateStackSetInputRequestTypeDef(
     _RequiredUpdateStackSetInputRequestTypeDef, _OptionalUpdateStackSetInputRequestTypeDef
 ):
     pass
 
 
-DeploymentTargetsUnionTypeDef = Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef]
 DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
     "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2785,57 +2775,36 @@
 class StackInstanceResourceDriftsSummaryTypeDef(
     _RequiredStackInstanceResourceDriftsSummaryTypeDef,
     _OptionalStackInstanceResourceDriftsSummaryTypeDef,
 ):
     pass
 
 
-_RequiredStackResourceDriftTypeDef = TypedDict(
-    "_RequiredStackResourceDriftTypeDef",
-    {
-        "StackId": str,
-        "LogicalResourceId": str,
-        "ResourceType": str,
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "Timestamp": datetime,
-    },
-)
-_OptionalStackResourceDriftTypeDef = TypedDict(
-    "_OptionalStackResourceDriftTypeDef",
-    {
-        "PhysicalResourceId": str,
-        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
-        "ExpectedProperties": str,
-        "ActualProperties": str,
-        "PropertyDifferences": List[PropertyDifferenceTypeDef],
-        "ModuleInfo": ModuleInfoTypeDef,
-    },
-    total=False,
-)
-
-
-class StackResourceDriftTypeDef(
-    _RequiredStackResourceDriftTypeDef, _OptionalStackResourceDriftTypeDef
-):
-    pass
-
-
 ResourceChangeDetailTypeDef = TypedDict(
     "ResourceChangeDetailTypeDef",
     {
         "Target": ResourceTargetDefinitionTypeDef,
         "Evaluation": EvaluationTypeType,
         "ChangeSource": ChangeSourceType,
         "CausingEntity": str,
     },
     total=False,
 )
 
-RollbackConfigurationOutputTypeDef = TypedDict(
-    "RollbackConfigurationOutputTypeDef",
+RollbackConfigurationResponseTypeDef = TypedDict(
+    "RollbackConfigurationResponseTypeDef",
+    {
+        "RollbackTriggers": List[RollbackTriggerTypeDef],
+        "MonitoringTimeInMinutes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackConfigurationStackResourceSummaryTypeDef = TypedDict(
+    "RollbackConfigurationStackResourceSummaryTypeDef",
     {
         "RollbackTriggers": List[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
     },
     total=False,
 )
 
@@ -2909,14 +2878,110 @@
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
     },
     total=False,
 )
 
+StackSetTypeDef = TypedDict(
+    "StackSetTypeDef",
+    {
+        "StackSetName": str,
+        "StackSetId": str,
+        "Description": str,
+        "Status": StackSetStatusType,
+        "TemplateBody": str,
+        "Parameters": List[ParameterTypeDef],
+        "Capabilities": List[CapabilityType],
+        "Tags": List[TagTypeDef],
+        "StackSetARN": str,
+        "AdministrationRoleARN": str,
+        "ExecutionRoleName": str,
+        "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
+        "AutoDeployment": AutoDeploymentTypeDef,
+        "PermissionModel": PermissionModelsType,
+        "OrganizationalUnitIds": List[str],
+        "ManagedExecution": ManagedExecutionTypeDef,
+        "Regions": List[str],
+    },
+    total=False,
+)
+
+StackSetOperationSummaryStackResourceSummaryTypeDef = TypedDict(
+    "StackSetOperationSummaryStackResourceSummaryTypeDef",
+    {
+        "OperationId": str,
+        "Action": StackSetOperationActionType,
+        "Status": StackSetOperationStatusType,
+        "CreationTimestamp": datetime,
+        "EndTimestamp": datetime,
+        "StatusReason": str,
+        "StatusDetails": StackSetOperationStatusDetailsTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesStackResourceSummaryTypeDef,
+    },
+    total=False,
+)
+
+StackSetOperationSummaryTypeDef = TypedDict(
+    "StackSetOperationSummaryTypeDef",
+    {
+        "OperationId": str,
+        "Action": StackSetOperationActionType,
+        "Status": StackSetOperationStatusType,
+        "CreationTimestamp": datetime,
+        "EndTimestamp": datetime,
+        "StatusReason": str,
+        "StatusDetails": StackSetOperationStatusDetailsTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesTypeDef,
+    },
+    total=False,
+)
+
+StackSetOperationTypeDef = TypedDict(
+    "StackSetOperationTypeDef",
+    {
+        "OperationId": str,
+        "StackSetId": str,
+        "Action": StackSetOperationActionType,
+        "Status": StackSetOperationStatusType,
+        "OperationPreferences": StackSetOperationPreferencesTypeDef,
+        "RetainStacks": bool,
+        "AdministrationRoleARN": str,
+        "ExecutionRoleName": str,
+        "CreationTimestamp": datetime,
+        "EndTimestamp": datetime,
+        "DeploymentTargets": DeploymentTargetsTypeDef,
+        "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
+        "StatusReason": str,
+        "StatusDetails": StackSetOperationStatusDetailsTypeDef,
+    },
+    total=False,
+)
+
+ValidateTemplateOutputTypeDef = TypedDict(
+    "ValidateTemplateOutputTypeDef",
+    {
+        "Parameters": List[TemplateParameterTypeDef],
+        "Description": str,
+        "Capabilities": List[CapabilityType],
+        "CapabilitiesReason": str,
+        "DeclaredTransforms": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListStackSetOperationResultsOutputTypeDef = TypedDict(
+    "ListStackSetOperationResultsOutputTypeDef",
+    {
+        "Summaries": List[StackSetOperationResultSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredStackResourceDetailTypeDef = TypedDict(
     "_RequiredStackResourceDetailTypeDef",
     {
         "LogicalResourceId": str,
         "ResourceType": str,
         "LastUpdatedTimestamp": datetime,
         "ResourceStatus": ResourceStatusType,
@@ -2940,39 +3005,41 @@
 
 class StackResourceDetailTypeDef(
     _RequiredStackResourceDetailTypeDef, _OptionalStackResourceDetailTypeDef
 ):
     pass
 
 
-_RequiredStackResourceTypeDef = TypedDict(
-    "_RequiredStackResourceTypeDef",
+_RequiredStackResourceDriftTypeDef = TypedDict(
+    "_RequiredStackResourceDriftTypeDef",
     {
+        "StackId": str,
         "LogicalResourceId": str,
         "ResourceType": str,
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
         "Timestamp": datetime,
-        "ResourceStatus": ResourceStatusType,
     },
 )
-_OptionalStackResourceTypeDef = TypedDict(
-    "_OptionalStackResourceTypeDef",
+_OptionalStackResourceDriftTypeDef = TypedDict(
+    "_OptionalStackResourceDriftTypeDef",
     {
-        "StackName": str,
-        "StackId": str,
         "PhysicalResourceId": str,
-        "ResourceStatusReason": str,
-        "Description": str,
-        "DriftInformation": StackResourceDriftInformationTypeDef,
+        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
+        "ExpectedProperties": str,
+        "ActualProperties": str,
+        "PropertyDifferences": List[PropertyDifferenceTypeDef],
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
 
-class StackResourceTypeDef(_RequiredStackResourceTypeDef, _OptionalStackResourceTypeDef):
+class StackResourceDriftTypeDef(
+    _RequiredStackResourceDriftTypeDef, _OptionalStackResourceDriftTypeDef
+):
     pass
 
 
 _RequiredStackResourceSummaryTypeDef = TypedDict(
     "_RequiredStackResourceSummaryTypeDef",
     {
         "LogicalResourceId": str,
@@ -2995,97 +3062,41 @@
 
 class StackResourceSummaryTypeDef(
     _RequiredStackResourceSummaryTypeDef, _OptionalStackResourceSummaryTypeDef
 ):
     pass
 
 
-StackSetTypeDef = TypedDict(
-    "StackSetTypeDef",
+_RequiredStackResourceTypeDef = TypedDict(
+    "_RequiredStackResourceTypeDef",
     {
-        "StackSetName": str,
-        "StackSetId": str,
-        "Description": str,
-        "Status": StackSetStatusType,
-        "TemplateBody": str,
-        "Parameters": List[ParameterTypeDef],
-        "Capabilities": List[CapabilityType],
-        "Tags": List[TagTypeDef],
-        "StackSetARN": str,
-        "AdministrationRoleARN": str,
-        "ExecutionRoleName": str,
-        "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
-        "AutoDeployment": AutoDeploymentTypeDef,
-        "PermissionModel": PermissionModelsType,
-        "OrganizationalUnitIds": List[str],
-        "ManagedExecution": ManagedExecutionTypeDef,
-        "Regions": List[str],
+        "LogicalResourceId": str,
+        "ResourceType": str,
+        "Timestamp": datetime,
+        "ResourceStatus": ResourceStatusType,
     },
-    total=False,
 )
-
-StackSetOperationPreferencesUnionTypeDef = Union[
-    StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
-]
-StackSetOperationSummaryTypeDef = TypedDict(
-    "StackSetOperationSummaryTypeDef",
+_OptionalStackResourceTypeDef = TypedDict(
+    "_OptionalStackResourceTypeDef",
     {
-        "OperationId": str,
-        "Action": StackSetOperationActionType,
-        "Status": StackSetOperationStatusType,
-        "CreationTimestamp": datetime,
-        "EndTimestamp": datetime,
-        "StatusReason": str,
-        "StatusDetails": StackSetOperationStatusDetailsTypeDef,
-        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
+        "StackName": str,
+        "StackId": str,
+        "PhysicalResourceId": str,
+        "ResourceStatusReason": str,
+        "Description": str,
+        "DriftInformation": StackResourceDriftInformationTypeDef,
+        "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
-StackSetOperationTypeDef = TypedDict(
-    "StackSetOperationTypeDef",
-    {
-        "OperationId": str,
-        "StackSetId": str,
-        "Action": StackSetOperationActionType,
-        "Status": StackSetOperationStatusType,
-        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
-        "RetainStacks": bool,
-        "AdministrationRoleARN": str,
-        "ExecutionRoleName": str,
-        "CreationTimestamp": datetime,
-        "EndTimestamp": datetime,
-        "DeploymentTargets": DeploymentTargetsOutputTypeDef,
-        "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
-        "StatusReason": str,
-        "StatusDetails": StackSetOperationStatusDetailsTypeDef,
-    },
-    total=False,
-)
 
-ValidateTemplateOutputTypeDef = TypedDict(
-    "ValidateTemplateOutputTypeDef",
-    {
-        "Parameters": List[TemplateParameterTypeDef],
-        "Description": str,
-        "Capabilities": List[CapabilityType],
-        "CapabilitiesReason": str,
-        "DeclaredTransforms": List[str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class StackResourceTypeDef(_RequiredStackResourceTypeDef, _OptionalStackResourceTypeDef):
+    pass
 
-ListStackSetOperationResultsOutputTypeDef = TypedDict(
-    "ListStackSetOperationResultsOutputTypeDef",
-    {
-        "Summaries": List[StackSetOperationResultSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 BatchDescribeTypeConfigurationsOutputTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     {
         "Errors": List[BatchDescribeTypeConfigurationsErrorTypeDef],
         "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierTypeDef],
         "TypeConfigurations": List[TypeConfigurationDetailsTypeDef],
@@ -3137,31 +3148,14 @@
     {
         "Summaries": List[StackInstanceResourceDriftsSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStackResourceDriftsOutputTypeDef = TypedDict(
-    "DescribeStackResourceDriftsOutputTypeDef",
-    {
-        "StackResourceDrifts": List[StackResourceDriftTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetectStackResourceDriftOutputTypeDef = TypedDict(
-    "DetectStackResourceDriftOutputTypeDef",
-    {
-        "StackResourceDrift": StackResourceDriftTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
         "LogicalResourceId": str,
         "PhysicalResourceId": str,
         "ResourceType": str,
@@ -3170,32 +3164,32 @@
         "Details": List[ResourceChangeDetailTypeDef],
         "ChangeSetId": str,
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
-_RequiredStackTypeDef = TypedDict(
-    "_RequiredStackTypeDef",
+_RequiredStackStackResourceSummaryTypeDef = TypedDict(
+    "_RequiredStackStackResourceSummaryTypeDef",
     {
         "StackName": str,
         "CreationTime": datetime,
         "StackStatus": StackStatusType,
     },
 )
-_OptionalStackTypeDef = TypedDict(
-    "_OptionalStackTypeDef",
+_OptionalStackStackResourceSummaryTypeDef = TypedDict(
+    "_OptionalStackStackResourceSummaryTypeDef",
     {
         "StackId": str,
         "ChangeSetId": str,
         "Description": str,
         "Parameters": List[ParameterTypeDef],
         "DeletionTime": datetime,
         "LastUpdatedTime": datetime,
-        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
+        "RollbackConfiguration": RollbackConfigurationStackResourceSummaryTypeDef,
         "StackStatusReason": str,
         "DisableRollback": bool,
         "NotificationARNs": List[str],
         "TimeoutInMinutes": int,
         "Capabilities": List[CapabilityType],
         "Outputs": List[OutputTypeDef],
         "RoleARN": str,
@@ -3206,15 +3200,17 @@
         "DriftInformation": StackDriftInformationTypeDef,
         "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
 
-class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
+class StackStackResourceSummaryTypeDef(
+    _RequiredStackStackResourceSummaryTypeDef, _OptionalStackStackResourceSummaryTypeDef
+):
     pass
 
 
 _RequiredCreateChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateChangeSetInputRequestTypeDef",
     {
         "StackName": str,
@@ -3322,17 +3318,54 @@
 class CreateStackInputServiceResourceCreateStackTypeDef(
     _RequiredCreateStackInputServiceResourceCreateStackTypeDef,
     _OptionalCreateStackInputServiceResourceCreateStackTypeDef,
 ):
     pass
 
 
-RollbackConfigurationUnionTypeDef = Union[
-    RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
-]
+_RequiredStackTypeDef = TypedDict(
+    "_RequiredStackTypeDef",
+    {
+        "StackName": str,
+        "CreationTime": datetime,
+        "StackStatus": StackStatusType,
+    },
+)
+_OptionalStackTypeDef = TypedDict(
+    "_OptionalStackTypeDef",
+    {
+        "StackId": str,
+        "ChangeSetId": str,
+        "Description": str,
+        "Parameters": List[ParameterTypeDef],
+        "DeletionTime": datetime,
+        "LastUpdatedTime": datetime,
+        "RollbackConfiguration": RollbackConfigurationTypeDef,
+        "StackStatusReason": str,
+        "DisableRollback": bool,
+        "NotificationARNs": List[str],
+        "TimeoutInMinutes": int,
+        "Capabilities": List[CapabilityType],
+        "Outputs": List[OutputTypeDef],
+        "RoleARN": str,
+        "Tags": List[TagTypeDef],
+        "EnableTerminationProtection": bool,
+        "ParentId": str,
+        "RootId": str,
+        "DriftInformation": StackDriftInformationTypeDef,
+        "RetainExceptOnCreate": bool,
+    },
+    total=False,
+)
+
+
+class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
+    pass
+
+
 _RequiredUpdateStackInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalUpdateStackInputRequestTypeDef = TypedDict(
@@ -3412,60 +3445,86 @@
     "DescribeStackInstanceOutputTypeDef",
     {
         "StackInstance": StackInstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStackResourceOutputTypeDef = TypedDict(
-    "DescribeStackResourceOutputTypeDef",
+DescribeStackSetOutputTypeDef = TypedDict(
+    "DescribeStackSetOutputTypeDef",
     {
-        "StackResourceDetail": StackResourceDetailTypeDef,
+        "StackSet": StackSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStackResourcesOutputTypeDef = TypedDict(
-    "DescribeStackResourcesOutputTypeDef",
+ListStackSetOperationsOutputStackResourceSummaryTypeDef = TypedDict(
+    "ListStackSetOperationsOutputStackResourceSummaryTypeDef",
     {
-        "StackResources": List[StackResourceTypeDef],
+        "Summaries": List[StackSetOperationSummaryStackResourceSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListStackResourcesOutputTypeDef = TypedDict(
-    "ListStackResourcesOutputTypeDef",
+ListStackSetOperationsOutputTypeDef = TypedDict(
+    "ListStackSetOperationsOutputTypeDef",
     {
-        "StackResourceSummaries": List[StackResourceSummaryTypeDef],
+        "Summaries": List[StackSetOperationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStackSetOutputTypeDef = TypedDict(
-    "DescribeStackSetOutputTypeDef",
+DescribeStackSetOperationOutputTypeDef = TypedDict(
+    "DescribeStackSetOperationOutputTypeDef",
     {
-        "StackSet": StackSetTypeDef,
+        "StackSetOperation": StackSetOperationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListStackSetOperationsOutputTypeDef = TypedDict(
-    "ListStackSetOperationsOutputTypeDef",
+DescribeStackResourceOutputTypeDef = TypedDict(
+    "DescribeStackResourceOutputTypeDef",
     {
-        "Summaries": List[StackSetOperationSummaryTypeDef],
+        "StackResourceDetail": StackResourceDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackResourceDriftsOutputTypeDef = TypedDict(
+    "DescribeStackResourceDriftsOutputTypeDef",
+    {
+        "StackResourceDrifts": List[StackResourceDriftTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStackSetOperationOutputTypeDef = TypedDict(
-    "DescribeStackSetOperationOutputTypeDef",
+DetectStackResourceDriftOutputTypeDef = TypedDict(
+    "DetectStackResourceDriftOutputTypeDef",
     {
-        "StackSetOperation": StackSetOperationTypeDef,
+        "StackResourceDrift": StackResourceDriftTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListStackResourcesOutputTypeDef = TypedDict(
+    "ListStackResourcesOutputTypeDef",
+    {
+        "StackResourceSummaries": List[StackResourceSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackResourcesOutputTypeDef = TypedDict(
+    "DescribeStackResourcesOutputTypeDef",
+    {
+        "StackResources": List[StackResourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetHooksOutputTypeDef = TypedDict(
     "DescribeChangeSetHooksOutputTypeDef",
     {
@@ -3486,38 +3545,74 @@
         "Type": Literal["Resource"],
         "HookInvocationCount": int,
         "ResourceChange": ResourceChangeTypeDef,
     },
     total=False,
 )
 
+DescribeStacksOutputStackResourceSummaryTypeDef = TypedDict(
+    "DescribeStacksOutputStackResourceSummaryTypeDef",
+    {
+        "Stacks": List[StackStackResourceSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeStacksOutputTypeDef = TypedDict(
     "DescribeStacksOutputTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeChangeSetOutputStackResourceSummaryTypeDef = TypedDict(
+    "DescribeChangeSetOutputStackResourceSummaryTypeDef",
+    {
+        "ChangeSetName": str,
+        "ChangeSetId": str,
+        "StackId": str,
+        "StackName": str,
+        "Description": str,
+        "Parameters": List[ParameterTypeDef],
+        "CreationTime": datetime,
+        "ExecutionStatus": ExecutionStatusType,
+        "Status": ChangeSetStatusType,
+        "StatusReason": str,
+        "NotificationARNs": List[str],
+        "RollbackConfiguration": RollbackConfigurationStackResourceSummaryTypeDef,
+        "Capabilities": List[CapabilityType],
+        "Tags": List[TagTypeDef],
+        "Changes": List[ChangeTypeDef],
+        "NextToken": str,
+        "IncludeNestedStacks": bool,
+        "ParentChangeSetId": str,
+        "RootChangeSetId": str,
+        "OnStackFailure": OnStackFailureType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeChangeSetOutputTypeDef = TypedDict(
     "DescribeChangeSetOutputTypeDef",
     {
         "ChangeSetName": str,
         "ChangeSetId": str,
         "StackId": str,
         "StackName": str,
         "Description": str,
         "Parameters": List[ParameterTypeDef],
         "CreationTime": datetime,
         "ExecutionStatus": ExecutionStatusType,
         "Status": ChangeSetStatusType,
         "StatusReason": str,
         "NotificationARNs": List[str],
-        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
+        "RollbackConfiguration": RollbackConfigurationTypeDef,
         "Capabilities": List[CapabilityType],
         "Tags": List[TagTypeDef],
         "Changes": List[ChangeTypeDef],
         "NextToken": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
```

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/type_defs.pyi` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from mypy_boto3_cloudformation.type_defs import AccountGateResultTypeDef
 
     data: AccountGateResultTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountFilterTypeType,
     AccountGateStatusType,
     CallAsType,
     CapabilityType,
     CategoryType,
@@ -98,15 +98,14 @@
     "StackSetOperationPreferencesTypeDef",
     "ManagedExecutionTypeDef",
     "DeactivateTypeInputRequestTypeDef",
     "DeleteChangeSetInputRequestTypeDef",
     "DeleteStackInputRequestTypeDef",
     "DeleteStackInputStackDeleteTypeDef",
     "DeleteStackSetInputRequestTypeDef",
-    "DeploymentTargetsOutputTypeDef",
     "DeregisterTypeInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeAccountLimitsInputRequestTypeDef",
     "DescribeChangeSetHooksInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeChangeSetInputRequestTypeDef",
     "DescribeOrganizationsAccessInputRequestTypeDef",
@@ -144,15 +143,14 @@
     "ListStackSetsInputRequestTypeDef",
     "ListStacksInputRequestTypeDef",
     "ListTypeRegistrationsInputRequestTypeDef",
     "ListTypeVersionsInputRequestTypeDef",
     "TypeVersionSummaryTypeDef",
     "TypeFiltersTypeDef",
     "TypeSummaryTypeDef",
-    "ModuleInfoTypeDef",
     "OutputTypeDef",
     "ParameterConstraintsTypeDef",
     "PhysicalResourceIdContextKeyValuePairTypeDef",
     "PropertyDifferenceTypeDef",
     "PublishTypeInputRequestTypeDef",
     "RecordHandlerProgressInputRequestTypeDef",
     "RegisterPublisherInputRequestTypeDef",
@@ -165,15 +163,15 @@
     "SignalResourceInputRequestTypeDef",
     "StackDriftInformationSummaryTypeDef",
     "StackDriftInformationTypeDef",
     "StackInstanceComprehensiveStatusTypeDef",
     "StackResourceDriftInformationTypeDef",
     "StackResourceDriftInformationSummaryTypeDef",
     "StackSetDriftDetectionDetailsTypeDef",
-    "StackSetOperationPreferencesOutputTypeDef",
+    "StackSetOperationPreferencesStackResourceSummaryTypeDef",
     "StackSetOperationStatusDetailsTypeDef",
     "StopStackSetOperationInputRequestTypeDef",
     "TemplateParameterTypeDef",
     "TestTypeInputRequestTypeDef",
     "UpdateTerminationProtectionInputRequestTypeDef",
     "ValidateTemplateInputRequestTypeDef",
     "StackSetOperationResultSummaryTypeDef",
@@ -196,14 +194,15 @@
     "EstimateTemplateCostOutputTypeDef",
     "GetStackPolicyOutputTypeDef",
     "GetTemplateOutputTypeDef",
     "ImportStacksToStackSetOutputTypeDef",
     "ListImportsOutputTypeDef",
     "ListTypeRegistrationsOutputTypeDef",
     "ModuleInfoResponseTypeDef",
+    "ModuleInfoTypeDef",
     "PublishTypeOutputTypeDef",
     "RegisterPublisherOutputTypeDef",
     "RegisterTypeOutputTypeDef",
     "RollbackStackOutputTypeDef",
     "SetTypeConfigurationOutputTypeDef",
     "StackDriftInformationResponseTypeDef",
     "StackResourceDriftInformationResponseTypeDef",
@@ -222,15 +221,14 @@
     "DeleteStackInstancesInputRequestTypeDef",
     "DetectStackSetDriftInputRequestTypeDef",
     "ImportStacksToStackSetInputRequestTypeDef",
     "UpdateStackInstancesInputRequestTypeDef",
     "CreateStackSetInputRequestTypeDef",
     "StackSetSummaryTypeDef",
     "UpdateStackSetInputRequestTypeDef",
-    "DeploymentTargetsUnionTypeDef",
     "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     "DescribeStacksInputDescribeStacksPaginateTypeDef",
     "ListChangeSetsInputListChangeSetsPaginateTypeDef",
     "ListExportsInputListExportsPaginateTypeDef",
     "ListImportsInputListImportsPaginateTypeDef",
@@ -256,57 +254,61 @@
     "ListStackSetOperationResultsInputRequestTypeDef",
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
     "ParameterDeclarationTypeDef",
     "StackInstanceResourceDriftsSummaryTypeDef",
-    "StackResourceDriftTypeDef",
     "ResourceChangeDetailTypeDef",
-    "RollbackConfigurationOutputTypeDef",
+    "RollbackConfigurationResponseTypeDef",
+    "RollbackConfigurationStackResourceSummaryTypeDef",
     "RollbackConfigurationTypeDef",
     "StackSummaryTypeDef",
     "StackInstanceSummaryTypeDef",
     "StackInstanceTypeDef",
-    "StackResourceDetailTypeDef",
-    "StackResourceTypeDef",
-    "StackResourceSummaryTypeDef",
     "StackSetTypeDef",
-    "StackSetOperationPreferencesUnionTypeDef",
+    "StackSetOperationSummaryStackResourceSummaryTypeDef",
     "StackSetOperationSummaryTypeDef",
     "StackSetOperationTypeDef",
     "ValidateTemplateOutputTypeDef",
     "ListStackSetOperationResultsOutputTypeDef",
+    "StackResourceDetailTypeDef",
+    "StackResourceDriftTypeDef",
+    "StackResourceSummaryTypeDef",
+    "StackResourceTypeDef",
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     "ChangeSetHookTypeDef",
     "ListStackSetsOutputTypeDef",
     "GetTemplateSummaryOutputTypeDef",
     "ListStackInstanceResourceDriftsOutputTypeDef",
-    "DescribeStackResourceDriftsOutputTypeDef",
-    "DetectStackResourceDriftOutputTypeDef",
     "ResourceChangeTypeDef",
-    "StackTypeDef",
+    "StackStackResourceSummaryTypeDef",
     "CreateChangeSetInputRequestTypeDef",
     "CreateStackInputRequestTypeDef",
     "CreateStackInputServiceResourceCreateStackTypeDef",
-    "RollbackConfigurationUnionTypeDef",
+    "StackTypeDef",
     "UpdateStackInputRequestTypeDef",
     "UpdateStackInputStackUpdateTypeDef",
     "ListStacksOutputTypeDef",
     "ListStackInstancesOutputTypeDef",
     "DescribeStackInstanceOutputTypeDef",
-    "DescribeStackResourceOutputTypeDef",
-    "DescribeStackResourcesOutputTypeDef",
-    "ListStackResourcesOutputTypeDef",
     "DescribeStackSetOutputTypeDef",
+    "ListStackSetOperationsOutputStackResourceSummaryTypeDef",
     "ListStackSetOperationsOutputTypeDef",
     "DescribeStackSetOperationOutputTypeDef",
+    "DescribeStackResourceOutputTypeDef",
+    "DescribeStackResourceDriftsOutputTypeDef",
+    "DetectStackResourceDriftOutputTypeDef",
+    "ListStackResourcesOutputTypeDef",
+    "DescribeStackResourcesOutputTypeDef",
     "DescribeChangeSetHooksOutputTypeDef",
     "ChangeTypeDef",
+    "DescribeStacksOutputStackResourceSummaryTypeDef",
     "DescribeStacksOutputTypeDef",
+    "DescribeChangeSetOutputStackResourceSummaryTypeDef",
     "DescribeChangeSetOutputTypeDef",
 )
 
 AccountGateResultTypeDef = TypedDict(
     "AccountGateResultTypeDef",
     {
         "Status": AccountGateStatusType,
@@ -591,25 +593,14 @@
 )
 
 class DeleteStackSetInputRequestTypeDef(
     _RequiredDeleteStackSetInputRequestTypeDef, _OptionalDeleteStackSetInputRequestTypeDef
 ):
     pass
 
-DeploymentTargetsOutputTypeDef = TypedDict(
-    "DeploymentTargetsOutputTypeDef",
-    {
-        "Accounts": List[str],
-        "AccountsUrl": str,
-        "OrganizationalUnitIds": List[str],
-        "AccountFilterType": AccountFilterTypeType,
-    },
-    total=False,
-)
-
 DeregisterTypeInputRequestTypeDef = TypedDict(
     "DeregisterTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": RegistryTypeType,
         "TypeName": str,
         "VersionId": str,
@@ -1212,23 +1203,14 @@
         "PublisherIdentity": IdentityProviderType,
         "PublisherName": str,
         "IsActivated": bool,
     },
     total=False,
 )
 
-ModuleInfoTypeDef = TypedDict(
-    "ModuleInfoTypeDef",
-    {
-        "TypeHierarchy": str,
-        "LogicalIdHierarchy": str,
-    },
-    total=False,
-)
-
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "OutputKey": str,
         "OutputValue": str,
         "Description": str,
         "ExportName": str,
@@ -1506,16 +1488,16 @@
         "InSyncStackInstancesCount": int,
         "InProgressStackInstancesCount": int,
         "FailedStackInstancesCount": int,
     },
     total=False,
 )
 
-StackSetOperationPreferencesOutputTypeDef = TypedDict(
-    "StackSetOperationPreferencesOutputTypeDef",
+StackSetOperationPreferencesStackResourceSummaryTypeDef = TypedDict(
+    "StackSetOperationPreferencesStackResourceSummaryTypeDef",
     {
         "RegionConcurrencyType": RegionConcurrencyTypeType,
         "RegionOrder": List[str],
         "FailureToleranceCount": int,
         "FailureTolerancePercentage": int,
         "MaxConcurrentCount": int,
         "MaxConcurrentPercentage": int,
@@ -1826,14 +1808,23 @@
     {
         "TypeHierarchy": str,
         "LogicalIdHierarchy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ModuleInfoTypeDef = TypedDict(
+    "ModuleInfoTypeDef",
+    {
+        "TypeHierarchy": str,
+        "LogicalIdHierarchy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PublishTypeOutputTypeDef = TypedDict(
     "PublishTypeOutputTypeDef",
     {
         "PublicTypeArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2186,15 +2177,14 @@
 )
 
 class UpdateStackSetInputRequestTypeDef(
     _RequiredUpdateStackSetInputRequestTypeDef, _OptionalUpdateStackSetInputRequestTypeDef
 ):
     pass
 
-DeploymentTargetsUnionTypeDef = Union[DeploymentTargetsTypeDef, DeploymentTargetsOutputTypeDef]
 DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef = TypedDict(
     "DescribeAccountLimitsInputDescribeAccountLimitsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2688,55 +2678,36 @@
 
 class StackInstanceResourceDriftsSummaryTypeDef(
     _RequiredStackInstanceResourceDriftsSummaryTypeDef,
     _OptionalStackInstanceResourceDriftsSummaryTypeDef,
 ):
     pass
 
-_RequiredStackResourceDriftTypeDef = TypedDict(
-    "_RequiredStackResourceDriftTypeDef",
-    {
-        "StackId": str,
-        "LogicalResourceId": str,
-        "ResourceType": str,
-        "StackResourceDriftStatus": StackResourceDriftStatusType,
-        "Timestamp": datetime,
-    },
-)
-_OptionalStackResourceDriftTypeDef = TypedDict(
-    "_OptionalStackResourceDriftTypeDef",
-    {
-        "PhysicalResourceId": str,
-        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
-        "ExpectedProperties": str,
-        "ActualProperties": str,
-        "PropertyDifferences": List[PropertyDifferenceTypeDef],
-        "ModuleInfo": ModuleInfoTypeDef,
-    },
-    total=False,
-)
-
-class StackResourceDriftTypeDef(
-    _RequiredStackResourceDriftTypeDef, _OptionalStackResourceDriftTypeDef
-):
-    pass
-
 ResourceChangeDetailTypeDef = TypedDict(
     "ResourceChangeDetailTypeDef",
     {
         "Target": ResourceTargetDefinitionTypeDef,
         "Evaluation": EvaluationTypeType,
         "ChangeSource": ChangeSourceType,
         "CausingEntity": str,
     },
     total=False,
 )
 
-RollbackConfigurationOutputTypeDef = TypedDict(
-    "RollbackConfigurationOutputTypeDef",
+RollbackConfigurationResponseTypeDef = TypedDict(
+    "RollbackConfigurationResponseTypeDef",
+    {
+        "RollbackTriggers": List[RollbackTriggerTypeDef],
+        "MonitoringTimeInMinutes": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RollbackConfigurationStackResourceSummaryTypeDef = TypedDict(
+    "RollbackConfigurationStackResourceSummaryTypeDef",
     {
         "RollbackTriggers": List[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
     },
     total=False,
 )
 
@@ -2808,94 +2779,14 @@
         "DriftStatus": StackDriftStatusType,
         "LastDriftCheckTimestamp": datetime,
         "LastOperationId": str,
     },
     total=False,
 )
 
-_RequiredStackResourceDetailTypeDef = TypedDict(
-    "_RequiredStackResourceDetailTypeDef",
-    {
-        "LogicalResourceId": str,
-        "ResourceType": str,
-        "LastUpdatedTimestamp": datetime,
-        "ResourceStatus": ResourceStatusType,
-    },
-)
-_OptionalStackResourceDetailTypeDef = TypedDict(
-    "_OptionalStackResourceDetailTypeDef",
-    {
-        "StackName": str,
-        "StackId": str,
-        "PhysicalResourceId": str,
-        "ResourceStatusReason": str,
-        "Description": str,
-        "Metadata": str,
-        "DriftInformation": StackResourceDriftInformationTypeDef,
-        "ModuleInfo": ModuleInfoTypeDef,
-    },
-    total=False,
-)
-
-class StackResourceDetailTypeDef(
-    _RequiredStackResourceDetailTypeDef, _OptionalStackResourceDetailTypeDef
-):
-    pass
-
-_RequiredStackResourceTypeDef = TypedDict(
-    "_RequiredStackResourceTypeDef",
-    {
-        "LogicalResourceId": str,
-        "ResourceType": str,
-        "Timestamp": datetime,
-        "ResourceStatus": ResourceStatusType,
-    },
-)
-_OptionalStackResourceTypeDef = TypedDict(
-    "_OptionalStackResourceTypeDef",
-    {
-        "StackName": str,
-        "StackId": str,
-        "PhysicalResourceId": str,
-        "ResourceStatusReason": str,
-        "Description": str,
-        "DriftInformation": StackResourceDriftInformationTypeDef,
-        "ModuleInfo": ModuleInfoTypeDef,
-    },
-    total=False,
-)
-
-class StackResourceTypeDef(_RequiredStackResourceTypeDef, _OptionalStackResourceTypeDef):
-    pass
-
-_RequiredStackResourceSummaryTypeDef = TypedDict(
-    "_RequiredStackResourceSummaryTypeDef",
-    {
-        "LogicalResourceId": str,
-        "ResourceType": str,
-        "LastUpdatedTimestamp": datetime,
-        "ResourceStatus": ResourceStatusType,
-    },
-)
-_OptionalStackResourceSummaryTypeDef = TypedDict(
-    "_OptionalStackResourceSummaryTypeDef",
-    {
-        "PhysicalResourceId": str,
-        "ResourceStatusReason": str,
-        "DriftInformation": StackResourceDriftInformationSummaryTypeDef,
-        "ModuleInfo": ModuleInfoTypeDef,
-    },
-    total=False,
-)
-
-class StackResourceSummaryTypeDef(
-    _RequiredStackResourceSummaryTypeDef, _OptionalStackResourceSummaryTypeDef
-):
-    pass
-
 StackSetTypeDef = TypedDict(
     "StackSetTypeDef",
     {
         "StackSetName": str,
         "StackSetId": str,
         "Description": str,
         "Status": StackSetStatusType,
@@ -2912,46 +2803,58 @@
         "OrganizationalUnitIds": List[str],
         "ManagedExecution": ManagedExecutionTypeDef,
         "Regions": List[str],
     },
     total=False,
 )
 
-StackSetOperationPreferencesUnionTypeDef = Union[
-    StackSetOperationPreferencesTypeDef, StackSetOperationPreferencesOutputTypeDef
-]
+StackSetOperationSummaryStackResourceSummaryTypeDef = TypedDict(
+    "StackSetOperationSummaryStackResourceSummaryTypeDef",
+    {
+        "OperationId": str,
+        "Action": StackSetOperationActionType,
+        "Status": StackSetOperationStatusType,
+        "CreationTimestamp": datetime,
+        "EndTimestamp": datetime,
+        "StatusReason": str,
+        "StatusDetails": StackSetOperationStatusDetailsTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesStackResourceSummaryTypeDef,
+    },
+    total=False,
+)
+
 StackSetOperationSummaryTypeDef = TypedDict(
     "StackSetOperationSummaryTypeDef",
     {
         "OperationId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
-        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesTypeDef,
     },
     total=False,
 )
 
 StackSetOperationTypeDef = TypedDict(
     "StackSetOperationTypeDef",
     {
         "OperationId": str,
         "StackSetId": str,
         "Action": StackSetOperationActionType,
         "Status": StackSetOperationStatusType,
-        "OperationPreferences": StackSetOperationPreferencesOutputTypeDef,
+        "OperationPreferences": StackSetOperationPreferencesTypeDef,
         "RetainStacks": bool,
         "AdministrationRoleARN": str,
         "ExecutionRoleName": str,
         "CreationTimestamp": datetime,
         "EndTimestamp": datetime,
-        "DeploymentTargets": DeploymentTargetsOutputTypeDef,
+        "DeploymentTargets": DeploymentTargetsTypeDef,
         "StackSetDriftDetectionDetails": StackSetDriftDetectionDetailsTypeDef,
         "StatusReason": str,
         "StatusDetails": StackSetOperationStatusDetailsTypeDef,
     },
     total=False,
 )
 
@@ -2972,14 +2875,122 @@
     {
         "Summaries": List[StackSetOperationResultSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredStackResourceDetailTypeDef = TypedDict(
+    "_RequiredStackResourceDetailTypeDef",
+    {
+        "LogicalResourceId": str,
+        "ResourceType": str,
+        "LastUpdatedTimestamp": datetime,
+        "ResourceStatus": ResourceStatusType,
+    },
+)
+_OptionalStackResourceDetailTypeDef = TypedDict(
+    "_OptionalStackResourceDetailTypeDef",
+    {
+        "StackName": str,
+        "StackId": str,
+        "PhysicalResourceId": str,
+        "ResourceStatusReason": str,
+        "Description": str,
+        "Metadata": str,
+        "DriftInformation": StackResourceDriftInformationTypeDef,
+        "ModuleInfo": ModuleInfoTypeDef,
+    },
+    total=False,
+)
+
+class StackResourceDetailTypeDef(
+    _RequiredStackResourceDetailTypeDef, _OptionalStackResourceDetailTypeDef
+):
+    pass
+
+_RequiredStackResourceDriftTypeDef = TypedDict(
+    "_RequiredStackResourceDriftTypeDef",
+    {
+        "StackId": str,
+        "LogicalResourceId": str,
+        "ResourceType": str,
+        "StackResourceDriftStatus": StackResourceDriftStatusType,
+        "Timestamp": datetime,
+    },
+)
+_OptionalStackResourceDriftTypeDef = TypedDict(
+    "_OptionalStackResourceDriftTypeDef",
+    {
+        "PhysicalResourceId": str,
+        "PhysicalResourceIdContext": List[PhysicalResourceIdContextKeyValuePairTypeDef],
+        "ExpectedProperties": str,
+        "ActualProperties": str,
+        "PropertyDifferences": List[PropertyDifferenceTypeDef],
+        "ModuleInfo": ModuleInfoTypeDef,
+    },
+    total=False,
+)
+
+class StackResourceDriftTypeDef(
+    _RequiredStackResourceDriftTypeDef, _OptionalStackResourceDriftTypeDef
+):
+    pass
+
+_RequiredStackResourceSummaryTypeDef = TypedDict(
+    "_RequiredStackResourceSummaryTypeDef",
+    {
+        "LogicalResourceId": str,
+        "ResourceType": str,
+        "LastUpdatedTimestamp": datetime,
+        "ResourceStatus": ResourceStatusType,
+    },
+)
+_OptionalStackResourceSummaryTypeDef = TypedDict(
+    "_OptionalStackResourceSummaryTypeDef",
+    {
+        "PhysicalResourceId": str,
+        "ResourceStatusReason": str,
+        "DriftInformation": StackResourceDriftInformationSummaryTypeDef,
+        "ModuleInfo": ModuleInfoTypeDef,
+    },
+    total=False,
+)
+
+class StackResourceSummaryTypeDef(
+    _RequiredStackResourceSummaryTypeDef, _OptionalStackResourceSummaryTypeDef
+):
+    pass
+
+_RequiredStackResourceTypeDef = TypedDict(
+    "_RequiredStackResourceTypeDef",
+    {
+        "LogicalResourceId": str,
+        "ResourceType": str,
+        "Timestamp": datetime,
+        "ResourceStatus": ResourceStatusType,
+    },
+)
+_OptionalStackResourceTypeDef = TypedDict(
+    "_OptionalStackResourceTypeDef",
+    {
+        "StackName": str,
+        "StackId": str,
+        "PhysicalResourceId": str,
+        "ResourceStatusReason": str,
+        "Description": str,
+        "DriftInformation": StackResourceDriftInformationTypeDef,
+        "ModuleInfo": ModuleInfoTypeDef,
+    },
+    total=False,
+)
+
+class StackResourceTypeDef(_RequiredStackResourceTypeDef, _OptionalStackResourceTypeDef):
+    pass
+
 BatchDescribeTypeConfigurationsOutputTypeDef = TypedDict(
     "BatchDescribeTypeConfigurationsOutputTypeDef",
     {
         "Errors": List[BatchDescribeTypeConfigurationsErrorTypeDef],
         "UnprocessedTypeConfigurations": List[TypeConfigurationIdentifierTypeDef],
         "TypeConfigurations": List[TypeConfigurationDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3030,31 +3041,14 @@
     {
         "Summaries": List[StackInstanceResourceDriftsSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStackResourceDriftsOutputTypeDef = TypedDict(
-    "DescribeStackResourceDriftsOutputTypeDef",
-    {
-        "StackResourceDrifts": List[StackResourceDriftTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DetectStackResourceDriftOutputTypeDef = TypedDict(
-    "DetectStackResourceDriftOutputTypeDef",
-    {
-        "StackResourceDrift": StackResourceDriftTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ResourceChangeTypeDef = TypedDict(
     "ResourceChangeTypeDef",
     {
         "Action": ChangeActionType,
         "LogicalResourceId": str,
         "PhysicalResourceId": str,
         "ResourceType": str,
@@ -3063,32 +3057,32 @@
         "Details": List[ResourceChangeDetailTypeDef],
         "ChangeSetId": str,
         "ModuleInfo": ModuleInfoTypeDef,
     },
     total=False,
 )
 
-_RequiredStackTypeDef = TypedDict(
-    "_RequiredStackTypeDef",
+_RequiredStackStackResourceSummaryTypeDef = TypedDict(
+    "_RequiredStackStackResourceSummaryTypeDef",
     {
         "StackName": str,
         "CreationTime": datetime,
         "StackStatus": StackStatusType,
     },
 )
-_OptionalStackTypeDef = TypedDict(
-    "_OptionalStackTypeDef",
+_OptionalStackStackResourceSummaryTypeDef = TypedDict(
+    "_OptionalStackStackResourceSummaryTypeDef",
     {
         "StackId": str,
         "ChangeSetId": str,
         "Description": str,
         "Parameters": List[ParameterTypeDef],
         "DeletionTime": datetime,
         "LastUpdatedTime": datetime,
-        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
+        "RollbackConfiguration": RollbackConfigurationStackResourceSummaryTypeDef,
         "StackStatusReason": str,
         "DisableRollback": bool,
         "NotificationARNs": List[str],
         "TimeoutInMinutes": int,
         "Capabilities": List[CapabilityType],
         "Outputs": List[OutputTypeDef],
         "RoleARN": str,
@@ -3098,15 +3092,17 @@
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
         "RetainExceptOnCreate": bool,
     },
     total=False,
 )
 
-class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
+class StackStackResourceSummaryTypeDef(
+    _RequiredStackStackResourceSummaryTypeDef, _OptionalStackStackResourceSummaryTypeDef
+):
     pass
 
 _RequiredCreateChangeSetInputRequestTypeDef = TypedDict(
     "_RequiredCreateChangeSetInputRequestTypeDef",
     {
         "StackName": str,
         "ChangeSetName": str,
@@ -3207,17 +3203,52 @@
 
 class CreateStackInputServiceResourceCreateStackTypeDef(
     _RequiredCreateStackInputServiceResourceCreateStackTypeDef,
     _OptionalCreateStackInputServiceResourceCreateStackTypeDef,
 ):
     pass
 
-RollbackConfigurationUnionTypeDef = Union[
-    RollbackConfigurationTypeDef, RollbackConfigurationOutputTypeDef
-]
+_RequiredStackTypeDef = TypedDict(
+    "_RequiredStackTypeDef",
+    {
+        "StackName": str,
+        "CreationTime": datetime,
+        "StackStatus": StackStatusType,
+    },
+)
+_OptionalStackTypeDef = TypedDict(
+    "_OptionalStackTypeDef",
+    {
+        "StackId": str,
+        "ChangeSetId": str,
+        "Description": str,
+        "Parameters": List[ParameterTypeDef],
+        "DeletionTime": datetime,
+        "LastUpdatedTime": datetime,
+        "RollbackConfiguration": RollbackConfigurationTypeDef,
+        "StackStatusReason": str,
+        "DisableRollback": bool,
+        "NotificationARNs": List[str],
+        "TimeoutInMinutes": int,
+        "Capabilities": List[CapabilityType],
+        "Outputs": List[OutputTypeDef],
+        "RoleARN": str,
+        "Tags": List[TagTypeDef],
+        "EnableTerminationProtection": bool,
+        "ParentId": str,
+        "RootId": str,
+        "DriftInformation": StackDriftInformationTypeDef,
+        "RetainExceptOnCreate": bool,
+    },
+    total=False,
+)
+
+class StackTypeDef(_RequiredStackTypeDef, _OptionalStackTypeDef):
+    pass
+
 _RequiredUpdateStackInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStackInputRequestTypeDef",
     {
         "StackName": str,
     },
 )
 _OptionalUpdateStackInputRequestTypeDef = TypedDict(
@@ -3295,60 +3326,86 @@
     "DescribeStackInstanceOutputTypeDef",
     {
         "StackInstance": StackInstanceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStackResourceOutputTypeDef = TypedDict(
-    "DescribeStackResourceOutputTypeDef",
+DescribeStackSetOutputTypeDef = TypedDict(
+    "DescribeStackSetOutputTypeDef",
     {
-        "StackResourceDetail": StackResourceDetailTypeDef,
+        "StackSet": StackSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStackResourcesOutputTypeDef = TypedDict(
-    "DescribeStackResourcesOutputTypeDef",
+ListStackSetOperationsOutputStackResourceSummaryTypeDef = TypedDict(
+    "ListStackSetOperationsOutputStackResourceSummaryTypeDef",
     {
-        "StackResources": List[StackResourceTypeDef],
+        "Summaries": List[StackSetOperationSummaryStackResourceSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListStackResourcesOutputTypeDef = TypedDict(
-    "ListStackResourcesOutputTypeDef",
+ListStackSetOperationsOutputTypeDef = TypedDict(
+    "ListStackSetOperationsOutputTypeDef",
     {
-        "StackResourceSummaries": List[StackResourceSummaryTypeDef],
+        "Summaries": List[StackSetOperationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStackSetOutputTypeDef = TypedDict(
-    "DescribeStackSetOutputTypeDef",
+DescribeStackSetOperationOutputTypeDef = TypedDict(
+    "DescribeStackSetOperationOutputTypeDef",
     {
-        "StackSet": StackSetTypeDef,
+        "StackSetOperation": StackSetOperationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListStackSetOperationsOutputTypeDef = TypedDict(
-    "ListStackSetOperationsOutputTypeDef",
+DescribeStackResourceOutputTypeDef = TypedDict(
+    "DescribeStackResourceOutputTypeDef",
     {
-        "Summaries": List[StackSetOperationSummaryTypeDef],
+        "StackResourceDetail": StackResourceDetailTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackResourceDriftsOutputTypeDef = TypedDict(
+    "DescribeStackResourceDriftsOutputTypeDef",
+    {
+        "StackResourceDrifts": List[StackResourceDriftTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeStackSetOperationOutputTypeDef = TypedDict(
-    "DescribeStackSetOperationOutputTypeDef",
+DetectStackResourceDriftOutputTypeDef = TypedDict(
+    "DetectStackResourceDriftOutputTypeDef",
     {
-        "StackSetOperation": StackSetOperationTypeDef,
+        "StackResourceDrift": StackResourceDriftTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListStackResourcesOutputTypeDef = TypedDict(
+    "ListStackResourcesOutputTypeDef",
+    {
+        "StackResourceSummaries": List[StackResourceSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeStackResourcesOutputTypeDef = TypedDict(
+    "DescribeStackResourcesOutputTypeDef",
+    {
+        "StackResources": List[StackResourceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeChangeSetHooksOutputTypeDef = TypedDict(
     "DescribeChangeSetHooksOutputTypeDef",
     {
@@ -3369,38 +3426,74 @@
         "Type": Literal["Resource"],
         "HookInvocationCount": int,
         "ResourceChange": ResourceChangeTypeDef,
     },
     total=False,
 )
 
+DescribeStacksOutputStackResourceSummaryTypeDef = TypedDict(
+    "DescribeStacksOutputStackResourceSummaryTypeDef",
+    {
+        "Stacks": List[StackStackResourceSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeStacksOutputTypeDef = TypedDict(
     "DescribeStacksOutputTypeDef",
     {
         "Stacks": List[StackTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeChangeSetOutputStackResourceSummaryTypeDef = TypedDict(
+    "DescribeChangeSetOutputStackResourceSummaryTypeDef",
+    {
+        "ChangeSetName": str,
+        "ChangeSetId": str,
+        "StackId": str,
+        "StackName": str,
+        "Description": str,
+        "Parameters": List[ParameterTypeDef],
+        "CreationTime": datetime,
+        "ExecutionStatus": ExecutionStatusType,
+        "Status": ChangeSetStatusType,
+        "StatusReason": str,
+        "NotificationARNs": List[str],
+        "RollbackConfiguration": RollbackConfigurationStackResourceSummaryTypeDef,
+        "Capabilities": List[CapabilityType],
+        "Tags": List[TagTypeDef],
+        "Changes": List[ChangeTypeDef],
+        "NextToken": str,
+        "IncludeNestedStacks": bool,
+        "ParentChangeSetId": str,
+        "RootChangeSetId": str,
+        "OnStackFailure": OnStackFailureType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeChangeSetOutputTypeDef = TypedDict(
     "DescribeChangeSetOutputTypeDef",
     {
         "ChangeSetName": str,
         "ChangeSetId": str,
         "StackId": str,
         "StackName": str,
         "Description": str,
         "Parameters": List[ParameterTypeDef],
         "CreationTime": datetime,
         "ExecutionStatus": ExecutionStatusType,
         "Status": ChangeSetStatusType,
         "StatusReason": str,
         "NotificationARNs": List[str],
-        "RollbackConfiguration": RollbackConfigurationOutputTypeDef,
+        "RollbackConfiguration": RollbackConfigurationTypeDef,
         "Capabilities": List[CapabilityType],
         "Tags": List[TagTypeDef],
         "Changes": List[ChangeTypeDef],
         "NextToken": str,
         "IncludeNestedStacks": bool,
         "ParentChangeSetId": str,
         "RootChangeSetId": str,
```

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/waiter.py` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation/waiter.pyi` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.16/mypy_boto3_cloudformation.egg-info/SOURCES.txt` & `mypy-boto3-cloudformation-1.28.19/mypy_boto3_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.28.16/setup.py` & `mypy-boto3-cloudformation-1.28.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudformation",
-    version="1.28.16",
+    version="1.28.19",
     packages=["mypy_boto3_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudFormation 1.28.16 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        "Type annotations for boto3.CloudFormation 1.28.19 service generated with"
+        " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

