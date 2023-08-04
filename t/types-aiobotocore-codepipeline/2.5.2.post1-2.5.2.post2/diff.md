# Comparing `tmp/types-aiobotocore-codepipeline-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codepipeline-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codepipeline-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-codepipeline-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:38 2023, max compression
```

## Comparing `types-aiobotocore-codepipeline-2.5.2.post1.tar` & `types-aiobotocore-codepipeline-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.677619 types-aiobotocore-codepipeline-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20005 2023-08-02 14:52:04.677619 types-aiobotocore-codepipeline-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18467 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.677619 types-aiobotocore-codepipeline-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:35:11.000000 types-aiobotocore-codepipeline-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.673619 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34423 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34369 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    51697 2023-08-02 14:35:14.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    51626 2023-08-02 14:35:13.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:12.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.677619 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20005 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:04.000000 types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:38.971629 types-aiobotocore-codepipeline-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:28.000000 types-aiobotocore-codepipeline-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-08-04 12:00:38.971629 types-aiobotocore-codepipeline-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-08-04 11:42:28.000000 types-aiobotocore-codepipeline-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:38.971629 types-aiobotocore-codepipeline-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:42:28.000000 types-aiobotocore-codepipeline-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:38.963629 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-04 11:42:28.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-08-04 11:42:28.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:42:28.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-08-04 11:42:29.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34324 2023-08-04 11:42:28.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-08-04 11:42:30.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-08-04 11:42:29.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-08-04 11:42:29.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-08-04 11:42:29.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:28.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46257 2023-08-04 11:42:31.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46196 2023-08-04 11:42:30.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:28.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:38.971629 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-08-04 12:00:38.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:00:38.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:38.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:38.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:38.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:38.000000 types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/LICENSE` & `types-aiobotocore-codepipeline-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/setup.py` & `types-aiobotocore-codepipeline-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codepipeline",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codepipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodePipeline 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__init__.py` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__init__.pyi` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/__main__.py` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodePipeline 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CodePipeline 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline\nOther"
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

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/client.py` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     ListWebhooksPaginator,
 )
 from .type_defs import (
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionExecutionFilterTypeDef,
-    ActionRevisionUnionTypeDef,
-    ActionTypeDeclarationUnionTypeDef,
+    ActionRevisionTypeDef,
+    ActionTypeDeclarationTypeDef,
     ActionTypeIdTypeDef,
     ActionTypeSettingsTypeDef,
     ApprovalResultTypeDef,
     ArtifactDetailsTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     CreatePipelineOutputTypeDef,
     CurrentRevisionTypeDef,
@@ -54,26 +54,26 @@
     GetThirdPartyJobDetailsOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListPipelinesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWebhooksOutputTypeDef,
-    PipelineDeclarationUnionTypeDef,
+    PipelineDeclarationTypeDef,
     PollForJobsOutputTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     PutActionRevisionOutputTypeDef,
     PutApprovalResultOutputTypeDef,
     PutWebhookOutputTypeDef,
     RetryStageExecutionOutputTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionOutputTypeDef,
     TagTypeDef,
     UpdatePipelineOutputTypeDef,
-    WebhookDefinitionUnionTypeDef,
+    WebhookDefinitionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -199,15 +199,15 @@
         the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#create_custom_action_type)
         """
 
     async def create_pipeline(
-        self, *, pipeline: PipelineDeclarationUnionTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, pipeline: PipelineDeclarationTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#create_pipeline)
         """
@@ -443,15 +443,15 @@
 
     async def put_action_revision(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
-        actionRevision: ActionRevisionUnionTypeDef
+        actionRevision: ActionRevisionTypeDef
     ) -> PutActionRevisionOutputTypeDef:
         """
         Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_action_revision)
         """
@@ -523,15 +523,15 @@
         worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_third_party_job_success_result)
         """
 
     async def put_webhook(
-        self, *, webhook: WebhookDefinitionUnionTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, webhook: WebhookDefinitionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> PutWebhookOutputTypeDef:
         """
         Defines a webhook and returns a unique webhook URL generated by CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_webhook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_webhook)
         """
@@ -593,26 +593,26 @@
         Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#untag_resource)
         """
 
     async def update_action_type(
-        self, *, actionType: ActionTypeDeclarationUnionTypeDef
+        self, *, actionType: ActionTypeDeclarationTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an action type that was created with any supported integration model,
         where the action type is to be used by customers of the action type provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_action_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#update_action_type)
         """
 
     async def update_pipeline(
-        self, *, pipeline: PipelineDeclarationUnionTypeDef
+        self, *, pipeline: PipelineDeclarationTypeDef
     ) -> UpdatePipelineOutputTypeDef:
         """
         Updates a specified pipeline with edits or changes to its structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/client.pyi` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     ListWebhooksPaginator,
 )
 from .type_defs import (
     AcknowledgeJobOutputTypeDef,
     AcknowledgeThirdPartyJobOutputTypeDef,
     ActionConfigurationPropertyTypeDef,
     ActionExecutionFilterTypeDef,
-    ActionRevisionUnionTypeDef,
-    ActionTypeDeclarationUnionTypeDef,
+    ActionRevisionTypeDef,
+    ActionTypeDeclarationTypeDef,
     ActionTypeIdTypeDef,
     ActionTypeSettingsTypeDef,
     ApprovalResultTypeDef,
     ArtifactDetailsTypeDef,
     CreateCustomActionTypeOutputTypeDef,
     CreatePipelineOutputTypeDef,
     CurrentRevisionTypeDef,
@@ -54,26 +54,26 @@
     GetThirdPartyJobDetailsOutputTypeDef,
     ListActionExecutionsOutputTypeDef,
     ListActionTypesOutputTypeDef,
     ListPipelineExecutionsOutputTypeDef,
     ListPipelinesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListWebhooksOutputTypeDef,
-    PipelineDeclarationUnionTypeDef,
+    PipelineDeclarationTypeDef,
     PollForJobsOutputTypeDef,
     PollForThirdPartyJobsOutputTypeDef,
     PutActionRevisionOutputTypeDef,
     PutApprovalResultOutputTypeDef,
     PutWebhookOutputTypeDef,
     RetryStageExecutionOutputTypeDef,
     StartPipelineExecutionOutputTypeDef,
     StopPipelineExecutionOutputTypeDef,
     TagTypeDef,
     UpdatePipelineOutputTypeDef,
-    WebhookDefinitionUnionTypeDef,
+    WebhookDefinitionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -189,15 +189,15 @@
         Creates a new custom action that can be used in all pipelines associated with
         the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#create_custom_action_type)
         """
     async def create_pipeline(
-        self, *, pipeline: PipelineDeclarationUnionTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, pipeline: PipelineDeclarationTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineOutputTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#create_pipeline)
         """
@@ -411,15 +411,15 @@
         """
     async def put_action_revision(
         self,
         *,
         pipelineName: str,
         stageName: str,
         actionName: str,
-        actionRevision: ActionRevisionUnionTypeDef
+        actionRevision: ActionRevisionTypeDef
     ) -> PutActionRevisionOutputTypeDef:
         """
         Provides information to CodePipeline about new revisions to a source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_action_revision)
         """
@@ -485,15 +485,15 @@
         Represents the success of a third party job as returned to the pipeline by a job
         worker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_third_party_job_success_result)
         """
     async def put_webhook(
-        self, *, webhook: WebhookDefinitionUnionTypeDef, tags: Sequence[TagTypeDef] = ...
+        self, *, webhook: WebhookDefinitionTypeDef, tags: Sequence[TagTypeDef] = ...
     ) -> PutWebhookOutputTypeDef:
         """
         Defines a webhook and returns a unique webhook URL generated by CodePipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_webhook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#put_webhook)
         """
@@ -548,25 +548,25 @@
         """
         Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#untag_resource)
         """
     async def update_action_type(
-        self, *, actionType: ActionTypeDeclarationUnionTypeDef
+        self, *, actionType: ActionTypeDeclarationTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an action type that was created with any supported integration model,
         where the action type is to be used by customers of the action type provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_action_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#update_action_type)
         """
     async def update_pipeline(
-        self, *, pipeline: PipelineDeclarationUnionTypeDef
+        self, *, pipeline: PipelineDeclarationTypeDef
     ) -> UpdatePipelineOutputTypeDef:
         """
         Updates a specified pipeline with edits or changes to its structure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codepipeline/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/literals.py` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/literals.pyi` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/paginator.py` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/paginator.pyi` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/type_defs.py` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,42 +51,40 @@
     "ActionContextTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ErrorDetailsTypeDef",
-    "ActionRevisionOutputTypeDef",
-    "TimestampTypeDef",
+    "ActionRevisionTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
     "ActionTypeIdentifierTypeDef",
-    "ActionTypePermissionsOutputTypeDef",
+    "ActionTypePermissionsTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
-    "ActionTypePermissionsTypeDef",
     "ActionTypeSettingsTypeDef",
     "ArtifactDetailsTypeDef",
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
     "EncryptionKeyTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
+    "TimestampTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
-    "JobWorkerExecutorConfigurationOutputTypeDef",
-    "LambdaExecutorConfigurationTypeDef",
     "JobWorkerExecutorConfigurationTypeDef",
+    "LambdaExecutorConfigurationTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
     "PipelineMetadataTypeDef",
     "GetPipelineStateInputRequestTypeDef",
@@ -117,87 +115,75 @@
     "PutActionRevisionOutputTypeDef",
     "PutApprovalResultOutputTypeDef",
     "RetryStageExecutionOutputTypeDef",
     "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
-    "ActionDeclarationOutputTypeDef",
     "ActionDeclarationTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
-    "ActionRevisionTypeDef",
-    "CurrentRevisionTypeDef",
+    "PutActionRevisionInputRequestTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "PipelineExecutionTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
-    "ExecutorConfigurationOutputTypeDef",
+    "CurrentRevisionTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
     "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionTypesInputListActionTypesPaginateTypeDef",
     "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
-    "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
-    "StageDeclarationOutputTypeDef",
     "StageDeclarationTypeDef",
     "ActionStateTypeDef",
-    "ActionRevisionUnionTypeDef",
-    "PutActionRevisionInputRequestTypeDef",
-    "PutJobSuccessResultInputRequestTypeDef",
-    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "CreateCustomActionTypeOutputTypeDef",
     "ListActionTypesOutputTypeDef",
     "ActionExecutionInputTypeDef",
     "ActionExecutionOutputTypeDef",
     "ArtifactTypeDef",
     "GetPipelineExecutionOutputTypeDef",
-    "ActionTypeExecutorOutputTypeDef",
+    "PutJobSuccessResultInputRequestTypeDef",
+    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "ActionTypeExecutorTypeDef",
     "ListPipelineExecutionsOutputTypeDef",
     "ListWebhookItemTypeDef",
     "PutWebhookInputRequestTypeDef",
-    "WebhookDefinitionUnionTypeDef",
-    "PipelineDeclarationOutputTypeDef",
     "PipelineDeclarationTypeDef",
     "StageStateTypeDef",
     "ActionExecutionDetailTypeDef",
     "JobDataTypeDef",
     "ThirdPartyJobDataTypeDef",
-    "ActionTypeDeclarationOutputTypeDef",
     "ActionTypeDeclarationTypeDef",
     "ListWebhooksOutputTypeDef",
     "PutWebhookOutputTypeDef",
+    "CreatePipelineInputRequestTypeDef",
     "CreatePipelineOutputTypeDef",
     "GetPipelineOutputTypeDef",
-    "UpdatePipelineOutputTypeDef",
-    "CreatePipelineInputRequestTypeDef",
-    "PipelineDeclarationUnionTypeDef",
     "UpdatePipelineInputRequestTypeDef",
+    "UpdatePipelineOutputTypeDef",
     "GetPipelineStateOutputTypeDef",
     "ListActionExecutionsOutputTypeDef",
     "JobDetailsTypeDef",
     "JobTypeDef",
     "ThirdPartyJobDetailsTypeDef",
     "GetActionTypeOutputTypeDef",
-    "ActionTypeDeclarationUnionTypeDef",
     "UpdateActionTypeInputRequestTypeDef",
     "GetJobDetailsOutputTypeDef",
     "PollForJobsOutputTypeDef",
     "GetThirdPartyJobDetailsOutputTypeDef",
 )
 
 AWSSessionCredentialsTypeDef = TypedDict(
@@ -327,24 +313,23 @@
     {
         "code": str,
         "message": str,
     },
     total=False,
 )
 
-ActionRevisionOutputTypeDef = TypedDict(
-    "ActionRevisionOutputTypeDef",
+ActionRevisionTypeDef = TypedDict(
+    "ActionRevisionTypeDef",
     {
         "revisionId": str,
         "revisionChangeId": str,
         "created": datetime,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
@@ -355,16 +340,16 @@
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
     },
 )
 
-ActionTypePermissionsOutputTypeDef = TypedDict(
-    "ActionTypePermissionsOutputTypeDef",
+ActionTypePermissionsTypeDef = TypedDict(
+    "ActionTypePermissionsTypeDef",
     {
         "allowedAccounts": List[str],
     },
 )
 
 _RequiredActionTypePropertyTypeDef = TypedDict(
     "_RequiredActionTypePropertyTypeDef",
@@ -398,21 +383,14 @@
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
-ActionTypePermissionsTypeDef = TypedDict(
-    "ActionTypePermissionsTypeDef",
-    {
-        "allowedAccounts": Sequence[str],
-    },
-)
-
 ActionTypeSettingsTypeDef = TypedDict(
     "ActionTypeSettingsTypeDef",
     {
         "thirdPartyConfigurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
@@ -486,14 +464,15 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -555,39 +534,30 @@
     {
         "triggerType": TriggerTypeType,
         "triggerDetail": str,
     },
     total=False,
 )
 
-JobWorkerExecutorConfigurationOutputTypeDef = TypedDict(
-    "JobWorkerExecutorConfigurationOutputTypeDef",
+JobWorkerExecutorConfigurationTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationTypeDef",
     {
         "pollingAccounts": List[str],
         "pollingServicePrincipals": List[str],
     },
     total=False,
 )
 
 LambdaExecutorConfigurationTypeDef = TypedDict(
     "LambdaExecutorConfigurationTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
 
-JobWorkerExecutorConfigurationTypeDef = TypedDict(
-    "JobWorkerExecutorConfigurationTypeDef",
-    {
-        "pollingAccounts": Sequence[str],
-        "pollingServicePrincipals": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredFailureDetailsTypeDef = TypedDict(
     "_RequiredFailureDetailsTypeDef",
     {
         "type": FailureTypeType,
         "message": str,
     },
 )
@@ -1041,42 +1011,14 @@
 class PollForThirdPartyJobsInputRequestTypeDef(
     _RequiredPollForThirdPartyJobsInputRequestTypeDef,
     _OptionalPollForThirdPartyJobsInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredActionDeclarationOutputTypeDef = TypedDict(
-    "_RequiredActionDeclarationOutputTypeDef",
-    {
-        "name": str,
-        "actionTypeId": ActionTypeIdTypeDef,
-    },
-)
-_OptionalActionDeclarationOutputTypeDef = TypedDict(
-    "_OptionalActionDeclarationOutputTypeDef",
-    {
-        "runOrder": int,
-        "configuration": Dict[str, str],
-        "outputArtifacts": List[OutputArtifactTypeDef],
-        "inputArtifacts": List[InputArtifactTypeDef],
-        "roleArn": str,
-        "region": str,
-        "namespace": str,
-    },
-    total=False,
-)
-
-
-class ActionDeclarationOutputTypeDef(
-    _RequiredActionDeclarationOutputTypeDef, _OptionalActionDeclarationOutputTypeDef
-):
-    pass
-
-
 _RequiredActionDeclarationTypeDef = TypedDict(
     "_RequiredActionDeclarationTypeDef",
     {
         "name": str,
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
@@ -1138,44 +1080,24 @@
         "externalExecutionUrl": str,
         "percentComplete": int,
         "errorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-ActionRevisionTypeDef = TypedDict(
-    "ActionRevisionTypeDef",
-    {
-        "revisionId": str,
-        "revisionChangeId": str,
-        "created": TimestampTypeDef,
-    },
-)
-
-_RequiredCurrentRevisionTypeDef = TypedDict(
-    "_RequiredCurrentRevisionTypeDef",
-    {
-        "revision": str,
-        "changeIdentifier": str,
-    },
-)
-_OptionalCurrentRevisionTypeDef = TypedDict(
-    "_OptionalCurrentRevisionTypeDef",
+PutActionRevisionInputRequestTypeDef = TypedDict(
+    "PutActionRevisionInputRequestTypeDef",
     {
-        "created": TimestampTypeDef,
-        "revisionSummary": str,
+        "pipelineName": str,
+        "stageName": str,
+        "actionName": str,
+        "actionRevision": ActionRevisionTypeDef,
     },
-    total=False,
 )
 
-
-class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
-    pass
-
-
 _RequiredActionTypeTypeDef = TypedDict(
     "_RequiredActionTypeTypeDef",
     {
         "id": ActionTypeIdTypeDef,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
         "outputArtifactDetails": ArtifactDetailsTypeDef,
     },
@@ -1297,23 +1219,35 @@
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
-ExecutorConfigurationOutputTypeDef = TypedDict(
-    "ExecutorConfigurationOutputTypeDef",
+_RequiredCurrentRevisionTypeDef = TypedDict(
+    "_RequiredCurrentRevisionTypeDef",
     {
-        "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
-        "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationOutputTypeDef,
+        "revision": str,
+        "changeIdentifier": str,
+    },
+)
+_OptionalCurrentRevisionTypeDef = TypedDict(
+    "_OptionalCurrentRevisionTypeDef",
+    {
+        "created": TimestampTypeDef,
+        "revisionSummary": str,
     },
     total=False,
 )
 
+
+class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
+    pass
+
+
 ExecutorConfigurationTypeDef = TypedDict(
     "ExecutorConfigurationTypeDef",
     {
         "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
         "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationTypeDef,
     },
     total=False,
@@ -1468,60 +1402,26 @@
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WebhookDefinitionOutputTypeDef = TypedDict(
-    "WebhookDefinitionOutputTypeDef",
-    {
-        "name": str,
-        "targetPipeline": str,
-        "targetAction": str,
-        "filters": List[WebhookFilterRuleTypeDef],
-        "authentication": WebhookAuthenticationTypeType,
-        "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
-    },
-)
-
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
         "targetPipeline": str,
         "targetAction": str,
-        "filters": Sequence[WebhookFilterRuleTypeDef],
+        "filters": List[WebhookFilterRuleTypeDef],
         "authentication": WebhookAuthenticationTypeType,
         "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
 
-_RequiredStageDeclarationOutputTypeDef = TypedDict(
-    "_RequiredStageDeclarationOutputTypeDef",
-    {
-        "name": str,
-        "actions": List[ActionDeclarationOutputTypeDef],
-    },
-)
-_OptionalStageDeclarationOutputTypeDef = TypedDict(
-    "_OptionalStageDeclarationOutputTypeDef",
-    {
-        "blockers": List[BlockerDeclarationTypeDef],
-    },
-    total=False,
-)
-
-
-class StageDeclarationOutputTypeDef(
-    _RequiredStageDeclarationOutputTypeDef, _OptionalStageDeclarationOutputTypeDef
-):
-    pass
-
-
 _RequiredStageDeclarationTypeDef = TypedDict(
     "_RequiredStageDeclarationTypeDef",
     {
         "name": str,
         "actions": Sequence[ActionDeclarationTypeDef],
     },
 )
@@ -1538,82 +1438,22 @@
     pass
 
 
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": str,
-        "currentRevision": ActionRevisionOutputTypeDef,
+        "currentRevision": ActionRevisionTypeDef,
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
-ActionRevisionUnionTypeDef = Union[ActionRevisionTypeDef, ActionRevisionOutputTypeDef]
-PutActionRevisionInputRequestTypeDef = TypedDict(
-    "PutActionRevisionInputRequestTypeDef",
-    {
-        "pipelineName": str,
-        "stageName": str,
-        "actionName": str,
-        "actionRevision": ActionRevisionTypeDef,
-    },
-)
-
-_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutJobSuccessResultInputRequestTypeDef",
-    {
-        "jobId": str,
-    },
-)
-_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutJobSuccessResultInputRequestTypeDef",
-    {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
-        "outputVariables": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class PutJobSuccessResultInputRequestTypeDef(
-    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
-):
-    pass
-
-
-_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
-    {
-        "jobId": str,
-        "clientToken": str,
-    },
-)
-_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
-    {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
-    },
-    total=False,
-)
-
-
-class PutThirdPartyJobSuccessResultInputRequestTypeDef(
-    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
-    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
-):
-    pass
-
-
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1666,33 +1506,59 @@
     "GetPipelineExecutionOutputTypeDef",
     {
         "pipelineExecution": PipelineExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredActionTypeExecutorOutputTypeDef = TypedDict(
-    "_RequiredActionTypeExecutorOutputTypeDef",
+_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutJobSuccessResultInputRequestTypeDef",
     {
-        "configuration": ExecutorConfigurationOutputTypeDef,
-        "type": ExecutorTypeType,
+        "jobId": str,
+    },
+)
+_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
+        "outputVariables": Mapping[str, str],
     },
+    total=False,
 )
-_OptionalActionTypeExecutorOutputTypeDef = TypedDict(
-    "_OptionalActionTypeExecutorOutputTypeDef",
+
+
+class PutJobSuccessResultInputRequestTypeDef(
+    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
+):
+    pass
+
+
+_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
     {
-        "policyStatementsTemplate": str,
-        "jobTimeout": int,
+        "jobId": str,
+        "clientToken": str,
+    },
+)
+_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
     },
     total=False,
 )
 
 
-class ActionTypeExecutorOutputTypeDef(
-    _RequiredActionTypeExecutorOutputTypeDef, _OptionalActionTypeExecutorOutputTypeDef
+class PutThirdPartyJobSuccessResultInputRequestTypeDef(
+    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
+    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
 ):
     pass
 
 
 _RequiredActionTypeExecutorTypeDef = TypedDict(
     "_RequiredActionTypeExecutorTypeDef",
     {
@@ -1724,15 +1590,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListWebhookItemTypeDef = TypedDict(
     "_RequiredListWebhookItemTypeDef",
     {
-        "definition": WebhookDefinitionOutputTypeDef,
+        "definition": WebhookDefinitionTypeDef,
         "url": str,
     },
 )
 _OptionalListWebhookItemTypeDef = TypedDict(
     "_OptionalListWebhookItemTypeDef",
     {
         "errorMessage": str,
@@ -1766,40 +1632,14 @@
 
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
 
-WebhookDefinitionUnionTypeDef = Union[WebhookDefinitionTypeDef, WebhookDefinitionOutputTypeDef]
-_RequiredPipelineDeclarationOutputTypeDef = TypedDict(
-    "_RequiredPipelineDeclarationOutputTypeDef",
-    {
-        "name": str,
-        "roleArn": str,
-        "stages": List[StageDeclarationOutputTypeDef],
-    },
-)
-_OptionalPipelineDeclarationOutputTypeDef = TypedDict(
-    "_OptionalPipelineDeclarationOutputTypeDef",
-    {
-        "artifactStore": ArtifactStoreTypeDef,
-        "artifactStores": Dict[str, ArtifactStoreTypeDef],
-        "version": int,
-    },
-    total=False,
-)
-
-
-class PipelineDeclarationOutputTypeDef(
-    _RequiredPipelineDeclarationOutputTypeDef, _OptionalPipelineDeclarationOutputTypeDef
-):
-    pass
-
-
 _RequiredPipelineDeclarationTypeDef = TypedDict(
     "_RequiredPipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
     },
@@ -1876,56 +1716,29 @@
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
         "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
-_RequiredActionTypeDeclarationOutputTypeDef = TypedDict(
-    "_RequiredActionTypeDeclarationOutputTypeDef",
-    {
-        "executor": ActionTypeExecutorOutputTypeDef,
-        "id": ActionTypeIdentifierTypeDef,
-        "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
-        "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
-    },
-)
-_OptionalActionTypeDeclarationOutputTypeDef = TypedDict(
-    "_OptionalActionTypeDeclarationOutputTypeDef",
-    {
-        "description": str,
-        "permissions": ActionTypePermissionsOutputTypeDef,
-        "properties": List[ActionTypePropertyTypeDef],
-        "urls": ActionTypeUrlsTypeDef,
-    },
-    total=False,
-)
-
-
-class ActionTypeDeclarationOutputTypeDef(
-    _RequiredActionTypeDeclarationOutputTypeDef, _OptionalActionTypeDeclarationOutputTypeDef
-):
-    pass
-
-
 _RequiredActionTypeDeclarationTypeDef = TypedDict(
     "_RequiredActionTypeDeclarationTypeDef",
     {
         "executor": ActionTypeExecutorTypeDef,
         "id": ActionTypeIdentifierTypeDef,
         "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
     },
 )
 _OptionalActionTypeDeclarationTypeDef = TypedDict(
     "_OptionalActionTypeDeclarationTypeDef",
     {
         "description": str,
         "permissions": ActionTypePermissionsTypeDef,
-        "properties": Sequence[ActionTypePropertyTypeDef],
+        "properties": List[ActionTypePropertyTypeDef],
         "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
 
 class ActionTypeDeclarationTypeDef(
@@ -1947,40 +1760,14 @@
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreatePipelineOutputTypeDef = TypedDict(
-    "CreatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationOutputTypeDef,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPipelineOutputTypeDef = TypedDict(
-    "GetPipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationOutputTypeDef,
-        "metadata": PipelineMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePipelineOutputTypeDef = TypedDict(
-    "UpdatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 _OptionalCreatePipelineInputRequestTypeDef = TypedDict(
@@ -1994,24 +1781,47 @@
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
 
-PipelineDeclarationUnionTypeDef = Union[
-    PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef
-]
+CreatePipelineOutputTypeDef = TypedDict(
+    "CreatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationTypeDef,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPipelineOutputTypeDef = TypedDict(
+    "GetPipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationTypeDef,
+        "metadata": PipelineMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
+UpdatePipelineOutputTypeDef = TypedDict(
+    "UpdatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetPipelineStateOutputTypeDef = TypedDict(
     "GetPipelineStateOutputTypeDef",
     {
         "pipelineName": str,
         "pipelineVersion": int,
         "stageStates": List[StageStateTypeDef],
         "created": datetime,
@@ -2059,22 +1869,19 @@
     },
     total=False,
 )
 
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
-        "actionType": ActionTypeDeclarationOutputTypeDef,
+        "actionType": ActionTypeDeclarationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActionTypeDeclarationUnionTypeDef = Union[
-    ActionTypeDeclarationTypeDef, ActionTypeDeclarationOutputTypeDef
-]
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline/type_defs.pyi` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -50,42 +50,40 @@
     "ActionContextTypeDef",
     "ActionTypeIdTypeDef",
     "InputArtifactTypeDef",
     "OutputArtifactTypeDef",
     "ActionExecutionFilterTypeDef",
     "ActionExecutionResultTypeDef",
     "ErrorDetailsTypeDef",
-    "ActionRevisionOutputTypeDef",
-    "TimestampTypeDef",
+    "ActionRevisionTypeDef",
     "ActionTypeArtifactDetailsTypeDef",
     "ActionTypeIdentifierTypeDef",
-    "ActionTypePermissionsOutputTypeDef",
+    "ActionTypePermissionsTypeDef",
     "ActionTypePropertyTypeDef",
     "ActionTypeUrlsTypeDef",
-    "ActionTypePermissionsTypeDef",
     "ActionTypeSettingsTypeDef",
     "ArtifactDetailsTypeDef",
     "ApprovalResultTypeDef",
     "S3LocationTypeDef",
     "S3ArtifactLocationTypeDef",
     "ArtifactRevisionTypeDef",
     "EncryptionKeyTypeDef",
     "BlockerDeclarationTypeDef",
     "TagTypeDef",
+    "TimestampTypeDef",
     "DeleteCustomActionTypeInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
     "DeleteWebhookInputRequestTypeDef",
     "DeregisterWebhookWithThirdPartyInputRequestTypeDef",
     "DisableStageTransitionInputRequestTypeDef",
     "EnableStageTransitionInputRequestTypeDef",
     "ExecutionDetailsTypeDef",
     "ExecutionTriggerTypeDef",
-    "JobWorkerExecutorConfigurationOutputTypeDef",
-    "LambdaExecutorConfigurationTypeDef",
     "JobWorkerExecutorConfigurationTypeDef",
+    "LambdaExecutorConfigurationTypeDef",
     "FailureDetailsTypeDef",
     "GetActionTypeInputRequestTypeDef",
     "GetJobDetailsInputRequestTypeDef",
     "GetPipelineExecutionInputRequestTypeDef",
     "GetPipelineInputRequestTypeDef",
     "PipelineMetadataTypeDef",
     "GetPipelineStateInputRequestTypeDef",
@@ -116,87 +114,75 @@
     "PutActionRevisionOutputTypeDef",
     "PutApprovalResultOutputTypeDef",
     "RetryStageExecutionOutputTypeDef",
     "StartPipelineExecutionOutputTypeDef",
     "StopPipelineExecutionOutputTypeDef",
     "PollForJobsInputRequestTypeDef",
     "PollForThirdPartyJobsInputRequestTypeDef",
-    "ActionDeclarationOutputTypeDef",
     "ActionDeclarationTypeDef",
     "ListActionExecutionsInputRequestTypeDef",
     "ActionExecutionTypeDef",
-    "ActionRevisionTypeDef",
-    "CurrentRevisionTypeDef",
+    "PutActionRevisionInputRequestTypeDef",
     "ActionTypeTypeDef",
     "PutApprovalResultInputRequestTypeDef",
     "ArtifactDetailTypeDef",
     "ArtifactLocationTypeDef",
     "PipelineExecutionTypeDef",
     "ArtifactStoreTypeDef",
     "CreateCustomActionTypeInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
-    "ExecutorConfigurationOutputTypeDef",
+    "CurrentRevisionTypeDef",
     "ExecutorConfigurationTypeDef",
     "PutJobFailureResultInputRequestTypeDef",
     "PutThirdPartyJobFailureResultInputRequestTypeDef",
     "ListActionExecutionsInputListActionExecutionsPaginateTypeDef",
     "ListActionTypesInputListActionTypesPaginateTypeDef",
     "ListPipelineExecutionsInputListPipelineExecutionsPaginateTypeDef",
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListWebhooksInputListWebhooksPaginateTypeDef",
     "ListPipelinesOutputTypeDef",
     "PipelineContextTypeDef",
     "PipelineExecutionSummaryTypeDef",
     "PollForThirdPartyJobsOutputTypeDef",
-    "WebhookDefinitionOutputTypeDef",
     "WebhookDefinitionTypeDef",
-    "StageDeclarationOutputTypeDef",
     "StageDeclarationTypeDef",
     "ActionStateTypeDef",
-    "ActionRevisionUnionTypeDef",
-    "PutActionRevisionInputRequestTypeDef",
-    "PutJobSuccessResultInputRequestTypeDef",
-    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "CreateCustomActionTypeOutputTypeDef",
     "ListActionTypesOutputTypeDef",
     "ActionExecutionInputTypeDef",
     "ActionExecutionOutputTypeDef",
     "ArtifactTypeDef",
     "GetPipelineExecutionOutputTypeDef",
-    "ActionTypeExecutorOutputTypeDef",
+    "PutJobSuccessResultInputRequestTypeDef",
+    "PutThirdPartyJobSuccessResultInputRequestTypeDef",
     "ActionTypeExecutorTypeDef",
     "ListPipelineExecutionsOutputTypeDef",
     "ListWebhookItemTypeDef",
     "PutWebhookInputRequestTypeDef",
-    "WebhookDefinitionUnionTypeDef",
-    "PipelineDeclarationOutputTypeDef",
     "PipelineDeclarationTypeDef",
     "StageStateTypeDef",
     "ActionExecutionDetailTypeDef",
     "JobDataTypeDef",
     "ThirdPartyJobDataTypeDef",
-    "ActionTypeDeclarationOutputTypeDef",
     "ActionTypeDeclarationTypeDef",
     "ListWebhooksOutputTypeDef",
     "PutWebhookOutputTypeDef",
+    "CreatePipelineInputRequestTypeDef",
     "CreatePipelineOutputTypeDef",
     "GetPipelineOutputTypeDef",
-    "UpdatePipelineOutputTypeDef",
-    "CreatePipelineInputRequestTypeDef",
-    "PipelineDeclarationUnionTypeDef",
     "UpdatePipelineInputRequestTypeDef",
+    "UpdatePipelineOutputTypeDef",
     "GetPipelineStateOutputTypeDef",
     "ListActionExecutionsOutputTypeDef",
     "JobDetailsTypeDef",
     "JobTypeDef",
     "ThirdPartyJobDetailsTypeDef",
     "GetActionTypeOutputTypeDef",
-    "ActionTypeDeclarationUnionTypeDef",
     "UpdateActionTypeInputRequestTypeDef",
     "GetJobDetailsOutputTypeDef",
     "PollForJobsOutputTypeDef",
     "GetThirdPartyJobDetailsOutputTypeDef",
 )
 
 AWSSessionCredentialsTypeDef = TypedDict(
@@ -324,24 +310,23 @@
     {
         "code": str,
         "message": str,
     },
     total=False,
 )
 
-ActionRevisionOutputTypeDef = TypedDict(
-    "ActionRevisionOutputTypeDef",
+ActionRevisionTypeDef = TypedDict(
+    "ActionRevisionTypeDef",
     {
         "revisionId": str,
         "revisionChangeId": str,
         "created": datetime,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 ActionTypeArtifactDetailsTypeDef = TypedDict(
     "ActionTypeArtifactDetailsTypeDef",
     {
         "minimumCount": int,
         "maximumCount": int,
     },
 )
@@ -352,16 +337,16 @@
         "category": ActionCategoryType,
         "owner": str,
         "provider": str,
         "version": str,
     },
 )
 
-ActionTypePermissionsOutputTypeDef = TypedDict(
-    "ActionTypePermissionsOutputTypeDef",
+ActionTypePermissionsTypeDef = TypedDict(
+    "ActionTypePermissionsTypeDef",
     {
         "allowedAccounts": List[str],
     },
 )
 
 _RequiredActionTypePropertyTypeDef = TypedDict(
     "_RequiredActionTypePropertyTypeDef",
@@ -393,21 +378,14 @@
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
     },
     total=False,
 )
 
-ActionTypePermissionsTypeDef = TypedDict(
-    "ActionTypePermissionsTypeDef",
-    {
-        "allowedAccounts": Sequence[str],
-    },
-)
-
 ActionTypeSettingsTypeDef = TypedDict(
     "ActionTypeSettingsTypeDef",
     {
         "thirdPartyConfigurationUrl": str,
         "entityUrlTemplate": str,
         "executionUrlTemplate": str,
         "revisionUrlTemplate": str,
@@ -481,14 +459,15 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 DeleteCustomActionTypeInputRequestTypeDef = TypedDict(
     "DeleteCustomActionTypeInputRequestTypeDef",
     {
         "category": ActionCategoryType,
         "provider": str,
         "version": str,
     },
@@ -550,39 +529,30 @@
     {
         "triggerType": TriggerTypeType,
         "triggerDetail": str,
     },
     total=False,
 )
 
-JobWorkerExecutorConfigurationOutputTypeDef = TypedDict(
-    "JobWorkerExecutorConfigurationOutputTypeDef",
+JobWorkerExecutorConfigurationTypeDef = TypedDict(
+    "JobWorkerExecutorConfigurationTypeDef",
     {
         "pollingAccounts": List[str],
         "pollingServicePrincipals": List[str],
     },
     total=False,
 )
 
 LambdaExecutorConfigurationTypeDef = TypedDict(
     "LambdaExecutorConfigurationTypeDef",
     {
         "lambdaFunctionArn": str,
     },
 )
 
-JobWorkerExecutorConfigurationTypeDef = TypedDict(
-    "JobWorkerExecutorConfigurationTypeDef",
-    {
-        "pollingAccounts": Sequence[str],
-        "pollingServicePrincipals": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredFailureDetailsTypeDef = TypedDict(
     "_RequiredFailureDetailsTypeDef",
     {
         "type": FailureTypeType,
         "message": str,
     },
 )
@@ -1016,40 +986,14 @@
 
 class PollForThirdPartyJobsInputRequestTypeDef(
     _RequiredPollForThirdPartyJobsInputRequestTypeDef,
     _OptionalPollForThirdPartyJobsInputRequestTypeDef,
 ):
     pass
 
-_RequiredActionDeclarationOutputTypeDef = TypedDict(
-    "_RequiredActionDeclarationOutputTypeDef",
-    {
-        "name": str,
-        "actionTypeId": ActionTypeIdTypeDef,
-    },
-)
-_OptionalActionDeclarationOutputTypeDef = TypedDict(
-    "_OptionalActionDeclarationOutputTypeDef",
-    {
-        "runOrder": int,
-        "configuration": Dict[str, str],
-        "outputArtifacts": List[OutputArtifactTypeDef],
-        "inputArtifacts": List[InputArtifactTypeDef],
-        "roleArn": str,
-        "region": str,
-        "namespace": str,
-    },
-    total=False,
-)
-
-class ActionDeclarationOutputTypeDef(
-    _RequiredActionDeclarationOutputTypeDef, _OptionalActionDeclarationOutputTypeDef
-):
-    pass
-
 _RequiredActionDeclarationTypeDef = TypedDict(
     "_RequiredActionDeclarationTypeDef",
     {
         "name": str,
         "actionTypeId": ActionTypeIdTypeDef,
     },
 )
@@ -1107,42 +1051,24 @@
         "externalExecutionUrl": str,
         "percentComplete": int,
         "errorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-ActionRevisionTypeDef = TypedDict(
-    "ActionRevisionTypeDef",
-    {
-        "revisionId": str,
-        "revisionChangeId": str,
-        "created": TimestampTypeDef,
-    },
-)
-
-_RequiredCurrentRevisionTypeDef = TypedDict(
-    "_RequiredCurrentRevisionTypeDef",
-    {
-        "revision": str,
-        "changeIdentifier": str,
-    },
-)
-_OptionalCurrentRevisionTypeDef = TypedDict(
-    "_OptionalCurrentRevisionTypeDef",
+PutActionRevisionInputRequestTypeDef = TypedDict(
+    "PutActionRevisionInputRequestTypeDef",
     {
-        "created": TimestampTypeDef,
-        "revisionSummary": str,
+        "pipelineName": str,
+        "stageName": str,
+        "actionName": str,
+        "actionRevision": ActionRevisionTypeDef,
     },
-    total=False,
 )
 
-class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
-    pass
-
 _RequiredActionTypeTypeDef = TypedDict(
     "_RequiredActionTypeTypeDef",
     {
         "id": ActionTypeIdTypeDef,
         "inputArtifactDetails": ArtifactDetailsTypeDef,
         "outputArtifactDetails": ArtifactDetailsTypeDef,
     },
@@ -1258,23 +1184,33 @@
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
-ExecutorConfigurationOutputTypeDef = TypedDict(
-    "ExecutorConfigurationOutputTypeDef",
+_RequiredCurrentRevisionTypeDef = TypedDict(
+    "_RequiredCurrentRevisionTypeDef",
     {
-        "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
-        "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationOutputTypeDef,
+        "revision": str,
+        "changeIdentifier": str,
+    },
+)
+_OptionalCurrentRevisionTypeDef = TypedDict(
+    "_OptionalCurrentRevisionTypeDef",
+    {
+        "created": TimestampTypeDef,
+        "revisionSummary": str,
     },
     total=False,
 )
 
+class CurrentRevisionTypeDef(_RequiredCurrentRevisionTypeDef, _OptionalCurrentRevisionTypeDef):
+    pass
+
 ExecutorConfigurationTypeDef = TypedDict(
     "ExecutorConfigurationTypeDef",
     {
         "lambdaExecutorConfiguration": LambdaExecutorConfigurationTypeDef,
         "jobWorkerExecutorConfiguration": JobWorkerExecutorConfigurationTypeDef,
     },
     total=False,
@@ -1423,58 +1359,26 @@
     "PollForThirdPartyJobsOutputTypeDef",
     {
         "jobs": List[ThirdPartyJobTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WebhookDefinitionOutputTypeDef = TypedDict(
-    "WebhookDefinitionOutputTypeDef",
-    {
-        "name": str,
-        "targetPipeline": str,
-        "targetAction": str,
-        "filters": List[WebhookFilterRuleTypeDef],
-        "authentication": WebhookAuthenticationTypeType,
-        "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
-    },
-)
-
 WebhookDefinitionTypeDef = TypedDict(
     "WebhookDefinitionTypeDef",
     {
         "name": str,
         "targetPipeline": str,
         "targetAction": str,
-        "filters": Sequence[WebhookFilterRuleTypeDef],
+        "filters": List[WebhookFilterRuleTypeDef],
         "authentication": WebhookAuthenticationTypeType,
         "authenticationConfiguration": WebhookAuthConfigurationTypeDef,
     },
 )
 
-_RequiredStageDeclarationOutputTypeDef = TypedDict(
-    "_RequiredStageDeclarationOutputTypeDef",
-    {
-        "name": str,
-        "actions": List[ActionDeclarationOutputTypeDef],
-    },
-)
-_OptionalStageDeclarationOutputTypeDef = TypedDict(
-    "_OptionalStageDeclarationOutputTypeDef",
-    {
-        "blockers": List[BlockerDeclarationTypeDef],
-    },
-    total=False,
-)
-
-class StageDeclarationOutputTypeDef(
-    _RequiredStageDeclarationOutputTypeDef, _OptionalStageDeclarationOutputTypeDef
-):
-    pass
-
 _RequiredStageDeclarationTypeDef = TypedDict(
     "_RequiredStageDeclarationTypeDef",
     {
         "name": str,
         "actions": Sequence[ActionDeclarationTypeDef],
     },
 )
@@ -1489,78 +1393,22 @@
 class StageDeclarationTypeDef(_RequiredStageDeclarationTypeDef, _OptionalStageDeclarationTypeDef):
     pass
 
 ActionStateTypeDef = TypedDict(
     "ActionStateTypeDef",
     {
         "actionName": str,
-        "currentRevision": ActionRevisionOutputTypeDef,
+        "currentRevision": ActionRevisionTypeDef,
         "latestExecution": ActionExecutionTypeDef,
         "entityUrl": str,
         "revisionUrl": str,
     },
     total=False,
 )
 
-ActionRevisionUnionTypeDef = Union[ActionRevisionTypeDef, ActionRevisionOutputTypeDef]
-PutActionRevisionInputRequestTypeDef = TypedDict(
-    "PutActionRevisionInputRequestTypeDef",
-    {
-        "pipelineName": str,
-        "stageName": str,
-        "actionName": str,
-        "actionRevision": ActionRevisionTypeDef,
-    },
-)
-
-_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutJobSuccessResultInputRequestTypeDef",
-    {
-        "jobId": str,
-    },
-)
-_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutJobSuccessResultInputRequestTypeDef",
-    {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
-        "outputVariables": Mapping[str, str],
-    },
-    total=False,
-)
-
-class PutJobSuccessResultInputRequestTypeDef(
-    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
-):
-    pass
-
-_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
-    {
-        "jobId": str,
-        "clientToken": str,
-    },
-)
-_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
-    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
-    {
-        "currentRevision": CurrentRevisionTypeDef,
-        "continuationToken": str,
-        "executionDetails": ExecutionDetailsTypeDef,
-    },
-    total=False,
-)
-
-class PutThirdPartyJobSuccessResultInputRequestTypeDef(
-    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
-    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
-):
-    pass
-
 CreateCustomActionTypeOutputTypeDef = TypedDict(
     "CreateCustomActionTypeOutputTypeDef",
     {
         "actionType": ActionTypeTypeDef,
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1613,32 +1461,56 @@
     "GetPipelineExecutionOutputTypeDef",
     {
         "pipelineExecution": PipelineExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredActionTypeExecutorOutputTypeDef = TypedDict(
-    "_RequiredActionTypeExecutorOutputTypeDef",
+_RequiredPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutJobSuccessResultInputRequestTypeDef",
     {
-        "configuration": ExecutorConfigurationOutputTypeDef,
-        "type": ExecutorTypeType,
+        "jobId": str,
     },
 )
-_OptionalActionTypeExecutorOutputTypeDef = TypedDict(
-    "_OptionalActionTypeExecutorOutputTypeDef",
+_OptionalPutJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutJobSuccessResultInputRequestTypeDef",
     {
-        "policyStatementsTemplate": str,
-        "jobTimeout": int,
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
+        "outputVariables": Mapping[str, str],
+    },
+    total=False,
+)
+
+class PutJobSuccessResultInputRequestTypeDef(
+    _RequiredPutJobSuccessResultInputRequestTypeDef, _OptionalPutJobSuccessResultInputRequestTypeDef
+):
+    pass
+
+_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "jobId": str,
+        "clientToken": str,
+    },
+)
+_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef = TypedDict(
+    "_OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef",
+    {
+        "currentRevision": CurrentRevisionTypeDef,
+        "continuationToken": str,
+        "executionDetails": ExecutionDetailsTypeDef,
     },
     total=False,
 )
 
-class ActionTypeExecutorOutputTypeDef(
-    _RequiredActionTypeExecutorOutputTypeDef, _OptionalActionTypeExecutorOutputTypeDef
+class PutThirdPartyJobSuccessResultInputRequestTypeDef(
+    _RequiredPutThirdPartyJobSuccessResultInputRequestTypeDef,
+    _OptionalPutThirdPartyJobSuccessResultInputRequestTypeDef,
 ):
     pass
 
 _RequiredActionTypeExecutorTypeDef = TypedDict(
     "_RequiredActionTypeExecutorTypeDef",
     {
         "configuration": ExecutorConfigurationTypeDef,
@@ -1667,15 +1539,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListWebhookItemTypeDef = TypedDict(
     "_RequiredListWebhookItemTypeDef",
     {
-        "definition": WebhookDefinitionOutputTypeDef,
+        "definition": WebhookDefinitionTypeDef,
         "url": str,
     },
 )
 _OptionalListWebhookItemTypeDef = TypedDict(
     "_OptionalListWebhookItemTypeDef",
     {
         "errorMessage": str,
@@ -1705,38 +1577,14 @@
 )
 
 class PutWebhookInputRequestTypeDef(
     _RequiredPutWebhookInputRequestTypeDef, _OptionalPutWebhookInputRequestTypeDef
 ):
     pass
 
-WebhookDefinitionUnionTypeDef = Union[WebhookDefinitionTypeDef, WebhookDefinitionOutputTypeDef]
-_RequiredPipelineDeclarationOutputTypeDef = TypedDict(
-    "_RequiredPipelineDeclarationOutputTypeDef",
-    {
-        "name": str,
-        "roleArn": str,
-        "stages": List[StageDeclarationOutputTypeDef],
-    },
-)
-_OptionalPipelineDeclarationOutputTypeDef = TypedDict(
-    "_OptionalPipelineDeclarationOutputTypeDef",
-    {
-        "artifactStore": ArtifactStoreTypeDef,
-        "artifactStores": Dict[str, ArtifactStoreTypeDef],
-        "version": int,
-    },
-    total=False,
-)
-
-class PipelineDeclarationOutputTypeDef(
-    _RequiredPipelineDeclarationOutputTypeDef, _OptionalPipelineDeclarationOutputTypeDef
-):
-    pass
-
 _RequiredPipelineDeclarationTypeDef = TypedDict(
     "_RequiredPipelineDeclarationTypeDef",
     {
         "name": str,
         "roleArn": str,
         "stages": Sequence[StageDeclarationTypeDef],
     },
@@ -1811,54 +1659,29 @@
         "artifactCredentials": AWSSessionCredentialsTypeDef,
         "continuationToken": str,
         "encryptionKey": EncryptionKeyTypeDef,
     },
     total=False,
 )
 
-_RequiredActionTypeDeclarationOutputTypeDef = TypedDict(
-    "_RequiredActionTypeDeclarationOutputTypeDef",
-    {
-        "executor": ActionTypeExecutorOutputTypeDef,
-        "id": ActionTypeIdentifierTypeDef,
-        "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
-        "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
-    },
-)
-_OptionalActionTypeDeclarationOutputTypeDef = TypedDict(
-    "_OptionalActionTypeDeclarationOutputTypeDef",
-    {
-        "description": str,
-        "permissions": ActionTypePermissionsOutputTypeDef,
-        "properties": List[ActionTypePropertyTypeDef],
-        "urls": ActionTypeUrlsTypeDef,
-    },
-    total=False,
-)
-
-class ActionTypeDeclarationOutputTypeDef(
-    _RequiredActionTypeDeclarationOutputTypeDef, _OptionalActionTypeDeclarationOutputTypeDef
-):
-    pass
-
 _RequiredActionTypeDeclarationTypeDef = TypedDict(
     "_RequiredActionTypeDeclarationTypeDef",
     {
         "executor": ActionTypeExecutorTypeDef,
         "id": ActionTypeIdentifierTypeDef,
         "inputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
         "outputArtifactDetails": ActionTypeArtifactDetailsTypeDef,
     },
 )
 _OptionalActionTypeDeclarationTypeDef = TypedDict(
     "_OptionalActionTypeDeclarationTypeDef",
     {
         "description": str,
         "permissions": ActionTypePermissionsTypeDef,
-        "properties": Sequence[ActionTypePropertyTypeDef],
+        "properties": List[ActionTypePropertyTypeDef],
         "urls": ActionTypeUrlsTypeDef,
     },
     total=False,
 )
 
 class ActionTypeDeclarationTypeDef(
     _RequiredActionTypeDeclarationTypeDef, _OptionalActionTypeDeclarationTypeDef
@@ -1878,40 +1701,14 @@
     "PutWebhookOutputTypeDef",
     {
         "webhook": ListWebhookItemTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreatePipelineOutputTypeDef = TypedDict(
-    "CreatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationOutputTypeDef,
-        "tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPipelineOutputTypeDef = TypedDict(
-    "GetPipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationOutputTypeDef,
-        "metadata": PipelineMetadataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UpdatePipelineOutputTypeDef = TypedDict(
-    "UpdatePipelineOutputTypeDef",
-    {
-        "pipeline": PipelineDeclarationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 _OptionalCreatePipelineInputRequestTypeDef = TypedDict(
@@ -1923,24 +1720,47 @@
 )
 
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
-PipelineDeclarationUnionTypeDef = Union[
-    PipelineDeclarationTypeDef, PipelineDeclarationOutputTypeDef
-]
+CreatePipelineOutputTypeDef = TypedDict(
+    "CreatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationTypeDef,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPipelineOutputTypeDef = TypedDict(
+    "GetPipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationTypeDef,
+        "metadata": PipelineMetadataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdatePipelineInputRequestTypeDef = TypedDict(
     "UpdatePipelineInputRequestTypeDef",
     {
         "pipeline": PipelineDeclarationTypeDef,
     },
 )
 
+UpdatePipelineOutputTypeDef = TypedDict(
+    "UpdatePipelineOutputTypeDef",
+    {
+        "pipeline": PipelineDeclarationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetPipelineStateOutputTypeDef = TypedDict(
     "GetPipelineStateOutputTypeDef",
     {
         "pipelineName": str,
         "pipelineVersion": int,
         "stageStates": List[StageStateTypeDef],
         "created": datetime,
@@ -1988,22 +1808,19 @@
     },
     total=False,
 )
 
 GetActionTypeOutputTypeDef = TypedDict(
     "GetActionTypeOutputTypeDef",
     {
-        "actionType": ActionTypeDeclarationOutputTypeDef,
+        "actionType": ActionTypeDeclarationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActionTypeDeclarationUnionTypeDef = Union[
-    ActionTypeDeclarationTypeDef, ActionTypeDeclarationOutputTypeDef
-]
 UpdateActionTypeInputRequestTypeDef = TypedDict(
     "UpdateActionTypeInputRequestTypeDef",
     {
         "actionType": ActionTypeDeclarationTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-codepipeline-2.5.2.post1/types_aiobotocore_codepipeline.egg-info/SOURCES.txt` & `types-aiobotocore-codepipeline-2.5.2.post2/types_aiobotocore_codepipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

