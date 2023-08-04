# Comparing `tmp/types-aiobotocore-cloudformation-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cloudformation-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudformation-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudformation-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:33 2023, max compression
```

## Comparing `types-aiobotocore-cloudformation-2.5.2.post1.tar` & `types-aiobotocore-cloudformation-2.5.2.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.989637 types-aiobotocore-cloudformation-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    30136 2023-08-02 14:51:59.985637 types-aiobotocore-cloudformation-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28590 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:59.989637 types-aiobotocore-cloudformation-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.981637 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68373 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    68273 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18030 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    25423 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    91368 2023-08-02 14:34:30.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    91255 2023-08-02 14:34:29.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:26.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-08-02 14:34:27.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.985637 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    30136 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:51:59.000000 types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.759431 types-aiobotocore-cloudformation-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:39.000000 types-aiobotocore-cloudformation-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-08-04 12:00:33.759431 types-aiobotocore-cloudformation-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17886 2023-08-04 11:41:39.000000 types-aiobotocore-cloudformation-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:33.759431 types-aiobotocore-cloudformation-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-04 11:41:39.000000 types-aiobotocore-cloudformation-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.759431 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-04 11:41:39.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-08-04 11:41:39.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 11:41:39.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68293 2023-08-04 11:41:41.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68193 2023-08-04 11:41:40.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18426 2023-08-04 11:41:42.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-08-04 11:41:41.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18150 2023-08-04 11:41:41.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-08-04 11:41:41.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:39.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25491 2023-08-04 11:41:41.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25444 2023-08-04 11:41:41.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    94484 2023-08-04 11:41:45.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94369 2023-08-04 11:41:43.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:39.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-08-04 11:41:41.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-08-04 11:41:41.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.759431 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-08-04 12:00:33.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-08-04 12:00:33.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:33.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:00:33.000000 types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/LICENSE` & `types-aiobotocore-cloudformation-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/setup.py` & `types-aiobotocore-cloudformation-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudformation",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudFormation 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__init__.py` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__init__.pyi` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/__main__.py` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudFormation 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation\nOther"
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/client.py` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
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
@@ -109,19 +109,19 @@
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
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
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
@@ -342,17 +342,17 @@
 
     async def create_stack_instances(
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
 
@@ -433,16 +433,16 @@
     async def delete_stack_instances(
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
 
@@ -689,15 +689,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#detect_stack_resource_drift)
         """
 
     async def detect_stack_set_drift(
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
@@ -789,15 +789,15 @@
     async def import_stacks_to_stack_set(
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
@@ -1141,15 +1141,15 @@
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
         ClientRequestToken: str = ...
     ) -> UpdateStackOutputTypeDef:
@@ -1162,17 +1162,17 @@
 
     async def update_stack_instances(
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
 
@@ -1187,18 +1187,18 @@
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/client.pyi` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
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
@@ -109,19 +109,19 @@
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
     TestTypeOutputTypeDef,
     TypeConfigurationIdentifierTypeDef,
     TypeFiltersTypeDef,
     UpdateStackInstancesOutputTypeDef,
     UpdateStackOutputTypeDef,
     UpdateStackSetOutputTypeDef,
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
@@ -328,17 +328,17 @@
         """
     async def create_stack_instances(
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
 
@@ -413,16 +413,16 @@
     async def delete_stack_instances(
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
 
@@ -648,15 +648,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.detect_stack_resource_drift)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/client/#detect_stack_resource_drift)
         """
     async def detect_stack_set_drift(
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
@@ -741,15 +741,15 @@
     async def import_stacks_to_stack_set(
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
@@ -1069,15 +1069,15 @@
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
         ClientRequestToken: str = ...
     ) -> UpdateStackOutputTypeDef:
@@ -1089,17 +1089,17 @@
         """
     async def update_stack_instances(
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
 
@@ -1113,18 +1113,18 @@
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/literals.py` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/literals.pyi` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/paginator.py` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,24 +58,24 @@
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
@@ -132,15 +132,15 @@
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[DescribeChangeSetOutputTypeDef]:
+    ) -> AsyncIterator[DescribeChangeSetOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describechangesetpaginator)
         """
 
 
 class DescribeStackEventsPaginator(AioPaginator):
@@ -162,15 +162,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
         self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[DescribeStacksOutputTypeDef]:
+    ) -> AsyncIterator[DescribeStacksOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
         """
 
 
 class ListChangeSetsPaginator(AioPaginator):
@@ -284,15 +284,15 @@
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ListStackSetOperationsOutputTypeDef]:
+    ) -> AsyncIterator[ListStackSetOperationsOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
 
 class ListStackSetsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/paginator.pyi` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -58,24 +58,24 @@
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
@@ -128,15 +128,15 @@
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[DescribeChangeSetOutputTypeDef]:
+    ) -> AsyncIterator[DescribeChangeSetOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describechangesetpaginator)
         """
 
 class DescribeStackEventsPaginator(AioPaginator):
     """
@@ -156,15 +156,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
     """
 
     def paginate(
         self, *, StackName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[DescribeStacksOutputTypeDef]:
+    ) -> AsyncIterator[DescribeStacksOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeStacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#describestackspaginator)
         """
 
 class ListChangeSetsPaginator(AioPaginator):
     """
@@ -271,15 +271,15 @@
 
     def paginate(
         self,
         *,
         StackSetName: str,
         CallAs: CallAsType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[ListStackSetOperationsOutputTypeDef]:
+    ) -> AsyncIterator[ListStackSetOperationsOutputStackResourceSummaryTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.ListStackSetOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/paginators/#liststacksetoperationspaginator)
         """
 
 class ListStackSetsPaginator(AioPaginator):
     """
```

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/service_resource.py` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,19 @@
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
 
@@ -264,15 +265,15 @@
     stack_name: Awaitable[str]
     change_set_id: Awaitable[str]
     description: Awaitable[str]
     parameters: Awaitable[List[ParameterTypeDef]]
     creation_time: Awaitable[datetime]
     deletion_time: Awaitable[datetime]
     last_updated_time: Awaitable[datetime]
-    rollback_configuration: Awaitable[RollbackConfigurationTypeDef]
+    rollback_configuration: Awaitable[RollbackConfigurationResponseTypeDef]
     stack_status: Awaitable[StackStatusType]
     stack_status_reason: Awaitable[str]
     disable_rollback: Awaitable[bool]
     notification_arns: Awaitable[List[str]]
     timeout_in_minutes: Awaitable[int]
     capabilities: Awaitable[List[CapabilityType]]
     outputs: Awaitable[List[OutputTypeDef]]
@@ -385,15 +386,15 @@
     resource_type: Awaitable[str]
     last_updated_timestamp: Awaitable[datetime]
     resource_status: Awaitable[ResourceStatusType]
     resource_status_reason: Awaitable[str]
     description: Awaitable[str]
     metadata: Awaitable[str]
     drift_information: Awaitable[StackResourceDriftInformationResponseTypeDef]
-    module_info: Awaitable[ModuleInfoResponseTypeDef]
+    module_info: Awaitable[ModuleInfoTypeDef]
     stack_name: str
     logical_id: str
 
     async def Stack(self) -> _Stack:
         """
         Creates a Stack resource.
 
@@ -517,15 +518,15 @@
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/service_resource.pyi` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -32,18 +32,19 @@
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
 
@@ -239,15 +240,15 @@
     stack_name: Awaitable[str]
     change_set_id: Awaitable[str]
     description: Awaitable[str]
     parameters: Awaitable[List[ParameterTypeDef]]
     creation_time: Awaitable[datetime]
     deletion_time: Awaitable[datetime]
     last_updated_time: Awaitable[datetime]
-    rollback_configuration: Awaitable[RollbackConfigurationTypeDef]
+    rollback_configuration: Awaitable[RollbackConfigurationResponseTypeDef]
     stack_status: Awaitable[StackStatusType]
     stack_status_reason: Awaitable[str]
     disable_rollback: Awaitable[bool]
     notification_arns: Awaitable[List[str]]
     timeout_in_minutes: Awaitable[int]
     capabilities: Awaitable[List[CapabilityType]]
     outputs: Awaitable[List[OutputTypeDef]]
@@ -352,15 +353,15 @@
     resource_type: Awaitable[str]
     last_updated_timestamp: Awaitable[datetime]
     resource_status: Awaitable[ResourceStatusType]
     resource_status_reason: Awaitable[str]
     description: Awaitable[str]
     metadata: Awaitable[str]
     drift_information: Awaitable[StackResourceDriftInformationResponseTypeDef]
-    module_info: Awaitable[ModuleInfoResponseTypeDef]
+    module_info: Awaitable[ModuleInfoTypeDef]
     stack_name: str
     logical_id: str
 
     async def Stack(self) -> _Stack:
         """
         Creates a Stack resource.
 
@@ -471,15 +472,15 @@
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/type_defs.py` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_cloudformation.type_defs import AccountGateResultTypeDef
 
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
@@ -143,15 +142,14 @@
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
@@ -164,15 +162,15 @@
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
@@ -195,14 +193,15 @@
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
@@ -221,15 +220,14 @@
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
@@ -253,56 +251,60 @@
     "ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     "ListStackSetOperationResultsInputRequestTypeDef",
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
     "ParameterDeclarationTypeDef",
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
@@ -597,25 +599,14 @@
 
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
@@ -1213,23 +1204,14 @@
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
@@ -1522,16 +1504,16 @@
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
@@ -1846,14 +1828,23 @@
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
@@ -2220,15 +2211,14 @@
 
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
@@ -2705,71 +2695,50 @@
         "NoEcho": bool,
         "Description": str,
         "ParameterConstraints": ParameterConstraintsTypeDef,
     },
     total=False,
 )
 
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
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
-        "RollbackTriggers": List[RollbackTriggerTypeDef],
+        "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
 _RequiredStackSummaryTypeDef = TypedDict(
     "_RequiredStackSummaryTypeDef",
     {
         "StackName": str,
         "CreationTime": datetime,
@@ -2829,14 +2798,110 @@
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
@@ -2860,39 +2925,41 @@
 
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
@@ -2915,97 +2982,41 @@
 
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
@@ -3047,31 +3058,14 @@
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
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
@@ -3080,32 +3074,32 @@
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
@@ -3115,15 +3109,17 @@
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
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
@@ -3229,17 +3225,53 @@
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
@@ -3317,60 +3349,86 @@
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
@@ -3391,38 +3449,74 @@
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/type_defs.pyi` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_cloudformation.type_defs import AccountGateResultTypeDef
 
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
@@ -142,15 +141,14 @@
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
@@ -163,15 +161,15 @@
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
@@ -194,14 +192,15 @@
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
@@ -220,15 +219,14 @@
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
@@ -252,56 +250,60 @@
     "ListStackSetOperationResultsInputListStackSetOperationResultsPaginateTypeDef",
     "ListStackSetOperationResultsInputRequestTypeDef",
     "ListTypeVersionsOutputTypeDef",
     "ListTypesInputListTypesPaginateTypeDef",
     "ListTypesInputRequestTypeDef",
     "ListTypesOutputTypeDef",
     "ParameterDeclarationTypeDef",
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
@@ -586,25 +588,14 @@
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
@@ -1176,23 +1167,14 @@
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
@@ -1469,16 +1451,16 @@
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
@@ -1789,14 +1771,23 @@
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
@@ -2149,15 +2140,14 @@
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
@@ -2612,69 +2602,50 @@
         "NoEcho": bool,
         "Description": str,
         "ParameterConstraints": ParameterConstraintsTypeDef,
     },
     total=False,
 )
 
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
 
 RollbackConfigurationTypeDef = TypedDict(
     "RollbackConfigurationTypeDef",
     {
-        "RollbackTriggers": List[RollbackTriggerTypeDef],
+        "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
         "MonitoringTimeInMinutes": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
 _RequiredStackSummaryTypeDef = TypedDict(
     "_RequiredStackSummaryTypeDef",
     {
         "StackName": str,
         "CreationTime": datetime,
@@ -2732,94 +2703,14 @@
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
@@ -2836,46 +2727,58 @@
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
 
@@ -2896,14 +2799,122 @@
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
@@ -2944,31 +2955,14 @@
         "Metadata": str,
         "DeclaredTransforms": List[str],
         "ResourceIdentifierSummaries": List[ResourceIdentifierSummaryTypeDef],
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
@@ -2977,32 +2971,32 @@
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
@@ -3011,15 +3005,17 @@
         "ParentId": str,
         "RootId": str,
         "DriftInformation": StackDriftInformationTypeDef,
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
@@ -3118,17 +3114,51 @@
 
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
@@ -3204,60 +3234,86 @@
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
@@ -3278,38 +3334,74 @@
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

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/waiter.py` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation/waiter.pyi` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudformation-2.5.2.post1/types_aiobotocore_cloudformation.egg-info/SOURCES.txt` & `types-aiobotocore-cloudformation-2.5.2.post2/types_aiobotocore_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

