# Comparing `tmp/types-aiobotocore-codebuild-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codebuild-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codebuild-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-codebuild-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:36 2023, max compression
```

## Comparing `types-aiobotocore-codebuild-2.5.2.post1.tar` & `types-aiobotocore-codebuild-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.441626 types-aiobotocore-codebuild-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21759 2023-08-02 14:52:02.441626 types-aiobotocore-codebuild-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20233 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.441626 types-aiobotocore-codebuild-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.433626 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43834 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43768 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-02 14:34:56.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59885 2023-08-02 14:34:57.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59822 2023-08-02 14:34:56.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:55.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.441626 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21759 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:02.000000 types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.575537 types-aiobotocore-codebuild-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:10.000000 types-aiobotocore-codebuild-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 2023-08-04 12:00:36.575537 types-aiobotocore-codebuild-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-08-04 11:42:10.000000 types-aiobotocore-codebuild-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:36.575537 types-aiobotocore-codebuild-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-04 11:42:10.000000 types-aiobotocore-codebuild-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.575537 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-04 11:42:10.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-04 11:42:10.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-04 11:42:10.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43759 2023-08-04 11:42:11.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43693 2023-08-04 11:42:10.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-08-04 11:42:11.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-08-04 11:42:11.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-08-04 11:42:11.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-08-04 11:42:11.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:10.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57197 2023-08-04 11:42:13.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57138 2023-08-04 11:42:12.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:10.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.575537 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 2023-08-04 12:00:36.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 12:00:36.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:36.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:00:36.000000 types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/LICENSE` & `types-aiobotocore-codebuild-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/setup.py` & `types-aiobotocore-codebuild-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codebuild",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codebuild"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeBuild 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__init__.py` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__init__.pyi` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/__main__.py` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeBuild 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CodeBuild 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild\nOther"
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

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/client.py` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,17 @@
     ListReportsForReportGroupOutputTypeDef,
     ListReportsOutputTypeDef,
     ListSharedProjectsOutputTypeDef,
     ListSharedReportGroupsOutputTypeDef,
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     ProjectArtifactsTypeDef,
-    ProjectBuildBatchConfigUnionTypeDef,
-    ProjectCacheUnionTypeDef,
-    ProjectEnvironmentUnionTypeDef,
+    ProjectBuildBatchConfigTypeDef,
+    ProjectCacheTypeDef,
+    ProjectEnvironmentTypeDef,
     ProjectFileSystemLocationTypeDef,
     ProjectSourceTypeDef,
     ProjectSourceVersionTypeDef,
     PutResourcePolicyOutputTypeDef,
     RegistryCredentialTypeDef,
     ReportExportConfigTypeDef,
     ReportFilterTypeDef,
@@ -106,15 +106,15 @@
     StopBuildOutputTypeDef,
     TagTypeDef,
     TestCaseFilterTypeDef,
     UpdateProjectOutputTypeDef,
     UpdateProjectVisibilityOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     UpdateWebhookOutputTypeDef,
-    VpcConfigUnionTypeDef,
+    VpcConfigTypeDef,
     WebhookFilterTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -227,31 +227,31 @@
 
     async def create_project(
         self,
         *,
         name: str,
         source: ProjectSourceTypeDef,
         artifacts: ProjectArtifactsTypeDef,
-        environment: ProjectEnvironmentUnionTypeDef,
+        environment: ProjectEnvironmentTypeDef,
         serviceRole: str,
         description: str = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: ProjectCacheUnionTypeDef = ...,
+        cache: ProjectCacheTypeDef = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: VpcConfigUnionTypeDef = ...,
+        vpcConfig: VpcConfigTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
+        buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#create_project)
@@ -657,15 +657,15 @@
         insecureSslOverride: bool = ...,
         reportBuildStatusOverride: bool = ...,
         buildStatusConfigOverride: BuildStatusConfigTypeDef = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: ProjectCacheUnionTypeDef = ...,
+        cacheOverride: ProjectCacheTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         timeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
@@ -698,25 +698,25 @@
         buildspecOverride: str = ...,
         insecureSslOverride: bool = ...,
         reportBuildBatchStatusOverride: bool = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: ProjectCacheUnionTypeDef = ...,
+        cacheOverride: ProjectCacheTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         buildTimeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
         registryCredentialOverride: RegistryCredentialTypeDef = ...,
         imagePullCredentialsTypeOverride: ImagePullCredentialsTypeType = ...,
-        buildBatchConfigOverride: ProjectBuildBatchConfigUnionTypeDef = ...,
+        buildBatchConfigOverride: ProjectBuildBatchConfigTypeDef = ...,
         debugSessionEnabled: bool = ...
     ) -> StartBuildBatchOutputTypeDef:
         """
         Starts a batch build for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.start_build_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#start_build_batch)
@@ -745,26 +745,26 @@
         description: str = ...,
         source: ProjectSourceTypeDef = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         artifacts: ProjectArtifactsTypeDef = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: ProjectCacheUnionTypeDef = ...,
-        environment: ProjectEnvironmentUnionTypeDef = ...,
+        cache: ProjectCacheTypeDef = ...,
+        environment: ProjectEnvironmentTypeDef = ...,
         serviceRole: str = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: VpcConfigUnionTypeDef = ...,
+        vpcConfig: VpcConfigTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
+        buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> UpdateProjectOutputTypeDef:
         """
         Changes the settings of a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_project)
```

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/client.pyi` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,17 @@
     ListReportsForReportGroupOutputTypeDef,
     ListReportsOutputTypeDef,
     ListSharedProjectsOutputTypeDef,
     ListSharedReportGroupsOutputTypeDef,
     ListSourceCredentialsOutputTypeDef,
     LogsConfigTypeDef,
     ProjectArtifactsTypeDef,
-    ProjectBuildBatchConfigUnionTypeDef,
-    ProjectCacheUnionTypeDef,
-    ProjectEnvironmentUnionTypeDef,
+    ProjectBuildBatchConfigTypeDef,
+    ProjectCacheTypeDef,
+    ProjectEnvironmentTypeDef,
     ProjectFileSystemLocationTypeDef,
     ProjectSourceTypeDef,
     ProjectSourceVersionTypeDef,
     PutResourcePolicyOutputTypeDef,
     RegistryCredentialTypeDef,
     ReportExportConfigTypeDef,
     ReportFilterTypeDef,
@@ -106,15 +106,15 @@
     StopBuildOutputTypeDef,
     TagTypeDef,
     TestCaseFilterTypeDef,
     UpdateProjectOutputTypeDef,
     UpdateProjectVisibilityOutputTypeDef,
     UpdateReportGroupOutputTypeDef,
     UpdateWebhookOutputTypeDef,
-    VpcConfigUnionTypeDef,
+    VpcConfigTypeDef,
     WebhookFilterTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -214,31 +214,31 @@
         """
     async def create_project(
         self,
         *,
         name: str,
         source: ProjectSourceTypeDef,
         artifacts: ProjectArtifactsTypeDef,
-        environment: ProjectEnvironmentUnionTypeDef,
+        environment: ProjectEnvironmentTypeDef,
         serviceRole: str,
         description: str = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: ProjectCacheUnionTypeDef = ...,
+        cache: ProjectCacheTypeDef = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: VpcConfigUnionTypeDef = ...,
+        vpcConfig: VpcConfigTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
+        buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#create_project)
@@ -612,15 +612,15 @@
         insecureSslOverride: bool = ...,
         reportBuildStatusOverride: bool = ...,
         buildStatusConfigOverride: BuildStatusConfigTypeDef = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: ProjectCacheUnionTypeDef = ...,
+        cacheOverride: ProjectCacheTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         timeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
@@ -652,25 +652,25 @@
         buildspecOverride: str = ...,
         insecureSslOverride: bool = ...,
         reportBuildBatchStatusOverride: bool = ...,
         environmentTypeOverride: EnvironmentTypeType = ...,
         imageOverride: str = ...,
         computeTypeOverride: ComputeTypeType = ...,
         certificateOverride: str = ...,
-        cacheOverride: ProjectCacheUnionTypeDef = ...,
+        cacheOverride: ProjectCacheTypeDef = ...,
         serviceRoleOverride: str = ...,
         privilegedModeOverride: bool = ...,
         buildTimeoutInMinutesOverride: int = ...,
         queuedTimeoutInMinutesOverride: int = ...,
         encryptionKeyOverride: str = ...,
         idempotencyToken: str = ...,
         logsConfigOverride: LogsConfigTypeDef = ...,
         registryCredentialOverride: RegistryCredentialTypeDef = ...,
         imagePullCredentialsTypeOverride: ImagePullCredentialsTypeType = ...,
-        buildBatchConfigOverride: ProjectBuildBatchConfigUnionTypeDef = ...,
+        buildBatchConfigOverride: ProjectBuildBatchConfigTypeDef = ...,
         debugSessionEnabled: bool = ...
     ) -> StartBuildBatchOutputTypeDef:
         """
         Starts a batch build for a project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.start_build_batch)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#start_build_batch)
@@ -696,26 +696,26 @@
         description: str = ...,
         source: ProjectSourceTypeDef = ...,
         secondarySources: Sequence[ProjectSourceTypeDef] = ...,
         sourceVersion: str = ...,
         secondarySourceVersions: Sequence[ProjectSourceVersionTypeDef] = ...,
         artifacts: ProjectArtifactsTypeDef = ...,
         secondaryArtifacts: Sequence[ProjectArtifactsTypeDef] = ...,
-        cache: ProjectCacheUnionTypeDef = ...,
-        environment: ProjectEnvironmentUnionTypeDef = ...,
+        cache: ProjectCacheTypeDef = ...,
+        environment: ProjectEnvironmentTypeDef = ...,
         serviceRole: str = ...,
         timeoutInMinutes: int = ...,
         queuedTimeoutInMinutes: int = ...,
         encryptionKey: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        vpcConfig: VpcConfigUnionTypeDef = ...,
+        vpcConfig: VpcConfigTypeDef = ...,
         badgeEnabled: bool = ...,
         logsConfig: LogsConfigTypeDef = ...,
         fileSystemLocations: Sequence[ProjectFileSystemLocationTypeDef] = ...,
-        buildBatchConfig: ProjectBuildBatchConfigUnionTypeDef = ...,
+        buildBatchConfig: ProjectBuildBatchConfigTypeDef = ...,
         concurrentBuildLimit: int = ...
     ) -> UpdateProjectOutputTypeDef:
         """
         Changes the settings of a build project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#CodeBuild.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codebuild/client/#update_project)
```

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/literals.py` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/literals.pyi` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/paginator.py` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/paginator.pyi` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/type_defs.py` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_codebuild.type_defs import BatchDeleteBuildsInputRequestTypeDef
 
     data: BatchDeleteBuildsInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ArtifactNamespaceType,
     ArtifactPackagingType,
     ArtifactsTypeType,
     AuthTypeType,
     BatchReportModeTypeType,
@@ -58,45 +58,41 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
     "BatchGetReportGroupsInputRequestTypeDef",
     "BatchGetReportsInputRequestTypeDef",
-    "BatchRestrictionsOutputTypeDef",
     "BatchRestrictionsTypeDef",
     "BuildArtifactsTypeDef",
     "BuildBatchFilterTypeDef",
     "PhaseContextTypeDef",
-    "ProjectCacheOutputTypeDef",
+    "ProjectCacheTypeDef",
     "ProjectFileSystemLocationTypeDef",
     "ProjectSourceVersionTypeDef",
-    "VpcConfigOutputTypeDef",
+    "VpcConfigTypeDef",
     "BuildStatusConfigTypeDef",
     "ResolvedArtifactTypeDef",
     "DebugSessionTypeDef",
     "ExportedEnvironmentVariableTypeDef",
     "NetworkInterfaceTypeDef",
     "CloudWatchLogsConfigTypeDef",
     "CodeCoverageReportSummaryTypeDef",
     "CodeCoverageTypeDef",
     "ProjectArtifactsTypeDef",
-    "ProjectCacheTypeDef",
     "TagTypeDef",
-    "VpcConfigTypeDef",
     "WebhookFilterTypeDef",
     "DeleteBuildBatchInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteReportGroupInputRequestTypeDef",
     "DeleteReportInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteSourceCredentialsInputRequestTypeDef",
@@ -147,24 +143,21 @@
     "ListReportGroupsOutputTypeDef",
     "ListReportsForReportGroupOutputTypeDef",
     "ListReportsOutputTypeDef",
     "ListSharedProjectsOutputTypeDef",
     "ListSharedReportGroupsOutputTypeDef",
     "PutResourcePolicyOutputTypeDef",
     "UpdateProjectVisibilityOutputTypeDef",
-    "ProjectBuildBatchConfigOutputTypeDef",
     "ProjectBuildBatchConfigTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
-    "ProjectCacheUnionTypeDef",
-    "VpcConfigUnionTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
     "WebhookTypeDef",
     "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
     "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
@@ -181,24 +174,21 @@
     "ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     "ListReportsForReportGroupInputRequestTypeDef",
     "ListReportsInputListReportsPaginateTypeDef",
     "ListReportsInputRequestTypeDef",
     "ListSourceCredentialsOutputTypeDef",
     "LogsConfigTypeDef",
     "LogsLocationTypeDef",
-    "ProjectEnvironmentOutputTypeDef",
     "ProjectEnvironmentTypeDef",
     "ProjectSourceTypeDef",
     "ReportExportConfigTypeDef",
-    "ProjectBuildBatchConfigUnionTypeDef",
     "BuildGroupTypeDef",
     "CreateWebhookOutputTypeDef",
     "UpdateWebhookOutputTypeDef",
     "EnvironmentPlatformTypeDef",
-    "ProjectEnvironmentUnionTypeDef",
     "BuildTypeDef",
     "CreateProjectInputRequestTypeDef",
     "ProjectTypeDef",
     "StartBuildBatchInputRequestTypeDef",
     "StartBuildInputRequestTypeDef",
     "UpdateProjectInputRequestTypeDef",
     "CreateReportGroupInputRequestTypeDef",
@@ -282,28 +272,19 @@
 BatchGetReportsInputRequestTypeDef = TypedDict(
     "BatchGetReportsInputRequestTypeDef",
     {
         "reportArns": Sequence[str],
     },
 )
 
-BatchRestrictionsOutputTypeDef = TypedDict(
-    "BatchRestrictionsOutputTypeDef",
-    {
-        "maximumBuildsAllowed": int,
-        "computeTypesAllowed": List[str],
-    },
-    total=False,
-)
-
 BatchRestrictionsTypeDef = TypedDict(
     "BatchRestrictionsTypeDef",
     {
         "maximumBuildsAllowed": int,
-        "computeTypesAllowed": Sequence[str],
+        "computeTypesAllowed": List[str],
     },
     total=False,
 )
 
 BuildArtifactsTypeDef = TypedDict(
     "BuildArtifactsTypeDef",
     {
@@ -331,36 +312,32 @@
     {
         "statusCode": str,
         "message": str,
     },
     total=False,
 )
 
-_RequiredProjectCacheOutputTypeDef = TypedDict(
-    "_RequiredProjectCacheOutputTypeDef",
+_RequiredProjectCacheTypeDef = TypedDict(
+    "_RequiredProjectCacheTypeDef",
     {
         "type": CacheTypeType,
     },
 )
-_OptionalProjectCacheOutputTypeDef = TypedDict(
-    "_OptionalProjectCacheOutputTypeDef",
+_OptionalProjectCacheTypeDef = TypedDict(
+    "_OptionalProjectCacheTypeDef",
     {
         "location": str,
         "modes": List[CacheModeType],
     },
     total=False,
 )
 
-
-class ProjectCacheOutputTypeDef(
-    _RequiredProjectCacheOutputTypeDef, _OptionalProjectCacheOutputTypeDef
-):
+class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
     pass
 
-
 ProjectFileSystemLocationTypeDef = TypedDict(
     "ProjectFileSystemLocationTypeDef",
     {
         "type": Literal["EFS"],
         "location": str,
         "mountPoint": str,
         "identifier": str,
@@ -373,16 +350,16 @@
     "ProjectSourceVersionTypeDef",
     {
         "sourceIdentifier": str,
         "sourceVersion": str,
     },
 )
 
-VpcConfigOutputTypeDef = TypedDict(
-    "VpcConfigOutputTypeDef",
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
     {
         "vpcId": str,
         "subnets": List[str],
         "securityGroupIds": List[str],
     },
     total=False,
 )
@@ -444,21 +421,19 @@
     {
         "groupName": str,
         "streamName": str,
     },
     total=False,
 )
 
-
 class CloudWatchLogsConfigTypeDef(
     _RequiredCloudWatchLogsConfigTypeDef, _OptionalCloudWatchLogsConfigTypeDef
 ):
     pass
 
-
 CodeCoverageReportSummaryTypeDef = TypedDict(
     "CodeCoverageReportSummaryTypeDef",
     {
         "lineCoveragePercentage": float,
         "linesCovered": int,
         "linesMissed": int,
         "branchCoveragePercentage": float,
@@ -503,58 +478,26 @@
         "encryptionDisabled": bool,
         "artifactIdentifier": str,
         "bucketOwnerAccess": BucketOwnerAccessType,
     },
     total=False,
 )
 
-
 class ProjectArtifactsTypeDef(_RequiredProjectArtifactsTypeDef, _OptionalProjectArtifactsTypeDef):
     pass
 
-
-_RequiredProjectCacheTypeDef = TypedDict(
-    "_RequiredProjectCacheTypeDef",
-    {
-        "type": CacheTypeType,
-    },
-)
-_OptionalProjectCacheTypeDef = TypedDict(
-    "_OptionalProjectCacheTypeDef",
-    {
-        "location": str,
-        "modes": Sequence[CacheModeType],
-    },
-    total=False,
-)
-
-
-class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
-    pass
-
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
-    {
-        "vpcId": str,
-        "subnets": Sequence[str],
-        "securityGroupIds": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredWebhookFilterTypeDef = TypedDict(
     "_RequiredWebhookFilterTypeDef",
     {
         "type": WebhookFilterTypeType,
         "pattern": str,
     },
 )
@@ -562,19 +505,17 @@
     "_OptionalWebhookFilterTypeDef",
     {
         "excludeMatchedPattern": bool,
     },
     total=False,
 )
 
-
 class WebhookFilterTypeDef(_RequiredWebhookFilterTypeDef, _OptionalWebhookFilterTypeDef):
     pass
 
-
 DeleteBuildBatchInputRequestTypeDef = TypedDict(
     "DeleteBuildBatchInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -595,21 +536,19 @@
     "_OptionalDeleteReportGroupInputRequestTypeDef",
     {
         "deleteReports": bool,
     },
     total=False,
 )
 
-
 class DeleteReportGroupInputRequestTypeDef(
     _RequiredDeleteReportGroupInputRequestTypeDef, _OptionalDeleteReportGroupInputRequestTypeDef
 ):
     pass
 
-
 DeleteReportInputRequestTypeDef = TypedDict(
     "DeleteReportInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -659,22 +598,20 @@
         "sortBy": ReportCodeCoverageSortByTypeType,
         "minLineCoveragePercentage": float,
         "maxLineCoveragePercentage": float,
     },
     total=False,
 )
 
-
 class DescribeCodeCoveragesInputRequestTypeDef(
     _RequiredDescribeCodeCoveragesInputRequestTypeDef,
     _OptionalDescribeCodeCoveragesInputRequestTypeDef,
 ):
     pass
 
-
 TestCaseFilterTypeDef = TypedDict(
     "TestCaseFilterTypeDef",
     {
         "status": str,
         "keyword": str,
     },
     total=False,
@@ -716,21 +653,19 @@
     "_OptionalEnvironmentVariableTypeDef",
     {
         "type": EnvironmentVariableTypeType,
     },
     total=False,
 )
 
-
 class EnvironmentVariableTypeDef(
     _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
 ):
     pass
 
-
 _RequiredGetReportGroupTrendInputRequestTypeDef = TypedDict(
     "_RequiredGetReportGroupTrendInputRequestTypeDef",
     {
         "reportGroupArn": str,
         "trendField": ReportGroupTrendFieldTypeType,
     },
 )
@@ -738,21 +673,19 @@
     "_OptionalGetReportGroupTrendInputRequestTypeDef",
     {
         "numOfReports": int,
     },
     total=False,
 )
 
-
 class GetReportGroupTrendInputRequestTypeDef(
     _RequiredGetReportGroupTrendInputRequestTypeDef, _OptionalGetReportGroupTrendInputRequestTypeDef
 ):
     pass
 
-
 ReportGroupTrendStatsTypeDef = TypedDict(
     "ReportGroupTrendStatsTypeDef",
     {
         "average": str,
         "max": str,
         "min": str,
     },
@@ -795,22 +728,20 @@
     {
         "username": str,
         "shouldOverwrite": bool,
     },
     total=False,
 )
 
-
 class ImportSourceCredentialsInputRequestTypeDef(
     _RequiredImportSourceCredentialsInputRequestTypeDef,
     _OptionalImportSourceCredentialsInputRequestTypeDef,
 ):
     pass
 
-
 InvalidateProjectCacheInputRequestTypeDef = TypedDict(
     "InvalidateProjectCacheInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
@@ -825,22 +756,20 @@
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListBuildsForProjectInputRequestTypeDef(
     _RequiredListBuildsForProjectInputRequestTypeDef,
     _OptionalListBuildsForProjectInputRequestTypeDef,
 ):
     pass
 
-
 ListBuildsInputRequestTypeDef = TypedDict(
     "ListBuildsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
@@ -919,19 +848,17 @@
         "location": str,
         "encryptionDisabled": bool,
         "bucketOwnerAccess": BucketOwnerAccessType,
     },
     total=False,
 )
 
-
 class S3LogsConfigTypeDef(_RequiredS3LogsConfigTypeDef, _OptionalS3LogsConfigTypeDef):
     pass
 
-
 ProjectBadgeTypeDef = TypedDict(
     "ProjectBadgeTypeDef",
     {
         "badgeEnabled": bool,
         "badgeRequestUrl": str,
     },
     total=False,
@@ -955,19 +882,17 @@
     "_OptionalSourceAuthTypeDef",
     {
         "resource": str,
     },
     total=False,
 )
 
-
 class SourceAuthTypeDef(_RequiredSourceAuthTypeDef, _OptionalSourceAuthTypeDef):
     pass
 
-
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
@@ -1038,22 +963,20 @@
     "_OptionalUpdateProjectVisibilityInputRequestTypeDef",
     {
         "resourceAccessRole": str,
     },
     total=False,
 )
 
-
 class UpdateProjectVisibilityInputRequestTypeDef(
     _RequiredUpdateProjectVisibilityInputRequestTypeDef,
     _OptionalUpdateProjectVisibilityInputRequestTypeDef,
 ):
     pass
 
-
 BatchDeleteBuildsOutputTypeDef = TypedDict(
     "BatchDeleteBuildsOutputTypeDef",
     {
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1197,26 +1120,14 @@
         "projectArn": str,
         "publicProjectAlias": str,
         "projectVisibility": ProjectVisibilityTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProjectBuildBatchConfigOutputTypeDef = TypedDict(
-    "ProjectBuildBatchConfigOutputTypeDef",
-    {
-        "serviceRole": str,
-        "combineArtifacts": bool,
-        "restrictions": BatchRestrictionsOutputTypeDef,
-        "timeoutInMins": int,
-        "batchReportMode": BatchReportModeTypeType,
-    },
-    total=False,
-)
-
 ProjectBuildBatchConfigTypeDef = TypedDict(
     "ProjectBuildBatchConfigTypeDef",
     {
         "serviceRole": str,
         "combineArtifacts": bool,
         "restrictions": BatchRestrictionsTypeDef,
         "timeoutInMins": int,
@@ -1291,16 +1202,14 @@
     {
         "nextToken": str,
         "codeCoverages": List[CodeCoverageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProjectCacheUnionTypeDef = Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef]
-VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredCreateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredCreateWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalCreateWebhookInputRequestTypeDef = TypedDict(
@@ -1309,21 +1218,19 @@
         "branchFilter": str,
         "filterGroups": Sequence[Sequence[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
     },
     total=False,
 )
 
-
 class CreateWebhookInputRequestTypeDef(
     _RequiredCreateWebhookInputRequestTypeDef, _OptionalCreateWebhookInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredUpdateWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateWebhookInputRequestTypeDef = TypedDict(
@@ -1333,21 +1240,19 @@
         "rotateSecret": bool,
         "filterGroups": Sequence[Sequence[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
     },
     total=False,
 )
 
-
 class UpdateWebhookInputRequestTypeDef(
     _RequiredUpdateWebhookInputRequestTypeDef, _OptionalUpdateWebhookInputRequestTypeDef
 ):
     pass
 
-
 WebhookTypeDef = TypedDict(
     "WebhookTypeDef",
     {
         "url": str,
         "payloadUrl": str,
         "secret": str,
         "branchFilter": str,
@@ -1372,22 +1277,20 @@
         "minLineCoveragePercentage": float,
         "maxLineCoveragePercentage": float,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
     _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
 ):
     pass
 
-
 ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
     "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     {
         "projectName": str,
         "filter": BuildBatchFilterTypeDef,
         "sortOrder": SortOrderTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -1416,22 +1319,20 @@
     {
         "sortOrder": SortOrderTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
     _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
 ):
     pass
 
-
 ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
     "ListBuildsInputListBuildsPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1488,22 +1389,20 @@
     {
         "filter": TestCaseFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTestCasesInputDescribeTestCasesPaginateTypeDef(
     _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeTestCasesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputRequestTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputRequestTypeDef = TypedDict(
@@ -1512,21 +1411,19 @@
         "nextToken": str,
         "maxResults": int,
         "filter": TestCaseFilterTypeDef,
     },
     total=False,
 )
 
-
 class DescribeTestCasesInputRequestTypeDef(
     _RequiredDescribeTestCasesInputRequestTypeDef, _OptionalDescribeTestCasesInputRequestTypeDef
 ):
     pass
 
-
 DescribeTestCasesOutputTypeDef = TypedDict(
     "DescribeTestCasesOutputTypeDef",
     {
         "nextToken": str,
         "testCases": List[TestCaseTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1562,22 +1459,20 @@
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef(
     _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListReportsForReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredListReportsForReportGroupInputRequestTypeDef",
     {
         "reportGroupArn": str,
     },
 )
 _OptionalListReportsForReportGroupInputRequestTypeDef = TypedDict(
@@ -1587,22 +1482,20 @@
         "sortOrder": SortOrderTypeType,
         "maxResults": int,
         "filter": ReportFilterTypeDef,
     },
     total=False,
 )
 
-
 class ListReportsForReportGroupInputRequestTypeDef(
     _RequiredListReportsForReportGroupInputRequestTypeDef,
     _OptionalListReportsForReportGroupInputRequestTypeDef,
 ):
     pass
 
-
 ListReportsInputListReportsPaginateTypeDef = TypedDict(
     "ListReportsInputListReportsPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1648,68 +1541,39 @@
         "s3LogsArn": str,
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
         "s3Logs": S3LogsConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredProjectEnvironmentOutputTypeDef = TypedDict(
-    "_RequiredProjectEnvironmentOutputTypeDef",
-    {
-        "type": EnvironmentTypeType,
-        "image": str,
-        "computeType": ComputeTypeType,
-    },
-)
-_OptionalProjectEnvironmentOutputTypeDef = TypedDict(
-    "_OptionalProjectEnvironmentOutputTypeDef",
-    {
-        "environmentVariables": List[EnvironmentVariableTypeDef],
-        "privilegedMode": bool,
-        "certificate": str,
-        "registryCredential": RegistryCredentialTypeDef,
-        "imagePullCredentialsType": ImagePullCredentialsTypeType,
-    },
-    total=False,
-)
-
-
-class ProjectEnvironmentOutputTypeDef(
-    _RequiredProjectEnvironmentOutputTypeDef, _OptionalProjectEnvironmentOutputTypeDef
-):
-    pass
-
-
 _RequiredProjectEnvironmentTypeDef = TypedDict(
     "_RequiredProjectEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "image": str,
         "computeType": ComputeTypeType,
     },
 )
 _OptionalProjectEnvironmentTypeDef = TypedDict(
     "_OptionalProjectEnvironmentTypeDef",
     {
-        "environmentVariables": Sequence[EnvironmentVariableTypeDef],
+        "environmentVariables": List[EnvironmentVariableTypeDef],
         "privilegedMode": bool,
         "certificate": str,
         "registryCredential": RegistryCredentialTypeDef,
         "imagePullCredentialsType": ImagePullCredentialsTypeType,
     },
     total=False,
 )
 
-
 class ProjectEnvironmentTypeDef(
     _RequiredProjectEnvironmentTypeDef, _OptionalProjectEnvironmentTypeDef
 ):
     pass
 
-
 _RequiredProjectSourceTypeDef = TypedDict(
     "_RequiredProjectSourceTypeDef",
     {
         "type": SourceTypeType,
     },
 )
 _OptionalProjectSourceTypeDef = TypedDict(
@@ -1724,31 +1588,26 @@
         "buildStatusConfig": BuildStatusConfigTypeDef,
         "insecureSsl": bool,
         "sourceIdentifier": str,
     },
     total=False,
 )
 
-
 class ProjectSourceTypeDef(_RequiredProjectSourceTypeDef, _OptionalProjectSourceTypeDef):
     pass
 
-
 ReportExportConfigTypeDef = TypedDict(
     "ReportExportConfigTypeDef",
     {
         "exportConfigType": ReportExportConfigTypeType,
         "s3Destination": S3ReportExportConfigTypeDef,
     },
     total=False,
 )
 
-ProjectBuildBatchConfigUnionTypeDef = Union[
-    ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
-]
 BuildGroupTypeDef = TypedDict(
     "BuildGroupTypeDef",
     {
         "identifier": str,
         "dependsOn": List[str],
         "ignoreFailure": bool,
         "currentBuildSummary": BuildSummaryTypeDef,
@@ -1778,15 +1637,14 @@
     {
         "platform": PlatformTypeType,
         "languages": List[EnvironmentLanguageTypeDef],
     },
     total=False,
 )
 
-ProjectEnvironmentUnionTypeDef = Union[ProjectEnvironmentTypeDef, ProjectEnvironmentOutputTypeDef]
 BuildTypeDef = TypedDict(
     "BuildTypeDef",
     {
         "id": str,
         "arn": str,
         "buildNumber": int,
         "startTime": datetime,
@@ -1798,23 +1656,23 @@
         "projectName": str,
         "phases": List[BuildPhaseTypeDef],
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheOutputTypeDef,
-        "environment": ProjectEnvironmentOutputTypeDef,
+        "cache": ProjectCacheTypeDef,
+        "environment": ProjectEnvironmentTypeDef,
         "serviceRole": str,
         "logs": LogsLocationTypeDef,
         "timeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "buildComplete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigOutputTypeDef,
+        "vpcConfig": VpcConfigTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "encryptionKey": str,
         "exportedEnvironmentVariables": List[ExportedEnvironmentVariableTypeDef],
         "reportArns": List[str],
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
         "debugSession": DebugSessionTypeDef,
         "buildBatchArn": str,
@@ -1851,48 +1709,46 @@
         "fileSystemLocations": Sequence[ProjectFileSystemLocationTypeDef],
         "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "concurrentBuildLimit": int,
     },
     total=False,
 )
 
-
 class CreateProjectInputRequestTypeDef(
     _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
 ):
     pass
 
-
 ProjectTypeDef = TypedDict(
     "ProjectTypeDef",
     {
         "name": str,
         "arn": str,
         "description": str,
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "sourceVersion": str,
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": ProjectArtifactsTypeDef,
         "secondaryArtifacts": List[ProjectArtifactsTypeDef],
-        "cache": ProjectCacheOutputTypeDef,
-        "environment": ProjectEnvironmentOutputTypeDef,
+        "cache": ProjectCacheTypeDef,
+        "environment": ProjectEnvironmentTypeDef,
         "serviceRole": str,
         "timeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "encryptionKey": str,
         "tags": List[TagTypeDef],
         "created": datetime,
         "lastModified": datetime,
         "webhook": WebhookTypeDef,
-        "vpcConfig": VpcConfigOutputTypeDef,
+        "vpcConfig": VpcConfigTypeDef,
         "badge": ProjectBadgeTypeDef,
         "logsConfig": LogsConfigTypeDef,
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
+        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "concurrentBuildLimit": int,
         "projectVisibility": ProjectVisibilityTypeType,
         "publicProjectAlias": str,
         "resourceAccessRole": str,
     },
     total=False,
 )
@@ -1936,21 +1792,19 @@
         "imagePullCredentialsTypeOverride": ImagePullCredentialsTypeType,
         "buildBatchConfigOverride": ProjectBuildBatchConfigTypeDef,
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
-
 class StartBuildBatchInputRequestTypeDef(
     _RequiredStartBuildBatchInputRequestTypeDef, _OptionalStartBuildBatchInputRequestTypeDef
 ):
     pass
 
-
 _RequiredStartBuildInputRequestTypeDef = TypedDict(
     "_RequiredStartBuildInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalStartBuildInputRequestTypeDef = TypedDict(
@@ -1986,21 +1840,19 @@
         "registryCredentialOverride": RegistryCredentialTypeDef,
         "imagePullCredentialsTypeOverride": ImagePullCredentialsTypeType,
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
-
 class StartBuildInputRequestTypeDef(
     _RequiredStartBuildInputRequestTypeDef, _OptionalStartBuildInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateProjectInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateProjectInputRequestTypeDef = TypedDict(
@@ -2026,21 +1878,19 @@
         "fileSystemLocations": Sequence[ProjectFileSystemLocationTypeDef],
         "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "concurrentBuildLimit": int,
     },
     total=False,
 )
 
-
 class UpdateProjectInputRequestTypeDef(
     _RequiredUpdateProjectInputRequestTypeDef, _OptionalUpdateProjectInputRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateReportGroupInputRequestTypeDef",
     {
         "name": str,
         "type": ReportTypeType,
         "exportConfig": ReportExportConfigTypeDef,
     },
@@ -2049,21 +1899,19 @@
     "_OptionalCreateReportGroupInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateReportGroupInputRequestTypeDef(
     _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
 ):
     pass
 
-
 ReportGroupTypeDef = TypedDict(
     "ReportGroupTypeDef",
     {
         "arn": str,
         "name": str,
         "type": ReportTypeType,
         "exportConfig": ReportExportConfigTypeDef,
@@ -2105,21 +1953,19 @@
     {
         "exportConfig": ReportExportConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class UpdateReportGroupInputRequestTypeDef(
     _RequiredUpdateReportGroupInputRequestTypeDef, _OptionalUpdateReportGroupInputRequestTypeDef
 ):
     pass
 
-
 BuildBatchTypeDef = TypedDict(
     "BuildBatchTypeDef",
     {
         "id": str,
         "arn": str,
         "startTime": datetime,
         "endTime": datetime,
@@ -2130,27 +1976,27 @@
         "projectName": str,
         "phases": List[BuildBatchPhaseTypeDef],
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheOutputTypeDef,
-        "environment": ProjectEnvironmentOutputTypeDef,
+        "cache": ProjectCacheTypeDef,
+        "environment": ProjectEnvironmentTypeDef,
         "serviceRole": str,
         "logConfig": LogsConfigTypeDef,
         "buildTimeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "complete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigOutputTypeDef,
+        "vpcConfig": VpcConfigTypeDef,
         "encryptionKey": str,
         "buildBatchNumber": int,
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
+        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "buildGroups": List[BuildGroupTypeDef],
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
 ListCuratedEnvironmentImagesOutputTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild/type_defs.pyi` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_codebuild.type_defs import BatchDeleteBuildsInputRequestTypeDef
 
     data: BatchDeleteBuildsInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ArtifactNamespaceType,
     ArtifactPackagingType,
     ArtifactsTypeType,
     AuthTypeType,
     BatchReportModeTypeType,
@@ -58,44 +58,42 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchDeleteBuildsInputRequestTypeDef",
     "BuildNotDeletedTypeDef",
     "ResponseMetadataTypeDef",
     "BatchGetBuildBatchesInputRequestTypeDef",
     "BatchGetBuildsInputRequestTypeDef",
     "BatchGetProjectsInputRequestTypeDef",
     "BatchGetReportGroupsInputRequestTypeDef",
     "BatchGetReportsInputRequestTypeDef",
-    "BatchRestrictionsOutputTypeDef",
     "BatchRestrictionsTypeDef",
     "BuildArtifactsTypeDef",
     "BuildBatchFilterTypeDef",
     "PhaseContextTypeDef",
-    "ProjectCacheOutputTypeDef",
+    "ProjectCacheTypeDef",
     "ProjectFileSystemLocationTypeDef",
     "ProjectSourceVersionTypeDef",
-    "VpcConfigOutputTypeDef",
+    "VpcConfigTypeDef",
     "BuildStatusConfigTypeDef",
     "ResolvedArtifactTypeDef",
     "DebugSessionTypeDef",
     "ExportedEnvironmentVariableTypeDef",
     "NetworkInterfaceTypeDef",
     "CloudWatchLogsConfigTypeDef",
     "CodeCoverageReportSummaryTypeDef",
     "CodeCoverageTypeDef",
     "ProjectArtifactsTypeDef",
-    "ProjectCacheTypeDef",
     "TagTypeDef",
-    "VpcConfigTypeDef",
     "WebhookFilterTypeDef",
     "DeleteBuildBatchInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteReportGroupInputRequestTypeDef",
     "DeleteReportInputRequestTypeDef",
     "DeleteResourcePolicyInputRequestTypeDef",
     "DeleteSourceCredentialsInputRequestTypeDef",
@@ -146,24 +144,21 @@
     "ListReportGroupsOutputTypeDef",
     "ListReportsForReportGroupOutputTypeDef",
     "ListReportsOutputTypeDef",
     "ListSharedProjectsOutputTypeDef",
     "ListSharedReportGroupsOutputTypeDef",
     "PutResourcePolicyOutputTypeDef",
     "UpdateProjectVisibilityOutputTypeDef",
-    "ProjectBuildBatchConfigOutputTypeDef",
     "ProjectBuildBatchConfigTypeDef",
     "ListBuildBatchesForProjectInputRequestTypeDef",
     "ListBuildBatchesInputRequestTypeDef",
     "BuildBatchPhaseTypeDef",
     "BuildPhaseTypeDef",
     "BuildSummaryTypeDef",
     "DescribeCodeCoveragesOutputTypeDef",
-    "ProjectCacheUnionTypeDef",
-    "VpcConfigUnionTypeDef",
     "CreateWebhookInputRequestTypeDef",
     "UpdateWebhookInputRequestTypeDef",
     "WebhookTypeDef",
     "DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef",
     "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     "ListBuildBatchesInputListBuildBatchesPaginateTypeDef",
     "ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef",
@@ -180,24 +175,21 @@
     "ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef",
     "ListReportsForReportGroupInputRequestTypeDef",
     "ListReportsInputListReportsPaginateTypeDef",
     "ListReportsInputRequestTypeDef",
     "ListSourceCredentialsOutputTypeDef",
     "LogsConfigTypeDef",
     "LogsLocationTypeDef",
-    "ProjectEnvironmentOutputTypeDef",
     "ProjectEnvironmentTypeDef",
     "ProjectSourceTypeDef",
     "ReportExportConfigTypeDef",
-    "ProjectBuildBatchConfigUnionTypeDef",
     "BuildGroupTypeDef",
     "CreateWebhookOutputTypeDef",
     "UpdateWebhookOutputTypeDef",
     "EnvironmentPlatformTypeDef",
-    "ProjectEnvironmentUnionTypeDef",
     "BuildTypeDef",
     "CreateProjectInputRequestTypeDef",
     "ProjectTypeDef",
     "StartBuildBatchInputRequestTypeDef",
     "StartBuildInputRequestTypeDef",
     "UpdateProjectInputRequestTypeDef",
     "CreateReportGroupInputRequestTypeDef",
@@ -281,28 +273,19 @@
 BatchGetReportsInputRequestTypeDef = TypedDict(
     "BatchGetReportsInputRequestTypeDef",
     {
         "reportArns": Sequence[str],
     },
 )
 
-BatchRestrictionsOutputTypeDef = TypedDict(
-    "BatchRestrictionsOutputTypeDef",
-    {
-        "maximumBuildsAllowed": int,
-        "computeTypesAllowed": List[str],
-    },
-    total=False,
-)
-
 BatchRestrictionsTypeDef = TypedDict(
     "BatchRestrictionsTypeDef",
     {
         "maximumBuildsAllowed": int,
-        "computeTypesAllowed": Sequence[str],
+        "computeTypesAllowed": List[str],
     },
     total=False,
 )
 
 BuildArtifactsTypeDef = TypedDict(
     "BuildArtifactsTypeDef",
     {
@@ -330,34 +313,34 @@
     {
         "statusCode": str,
         "message": str,
     },
     total=False,
 )
 
-_RequiredProjectCacheOutputTypeDef = TypedDict(
-    "_RequiredProjectCacheOutputTypeDef",
+_RequiredProjectCacheTypeDef = TypedDict(
+    "_RequiredProjectCacheTypeDef",
     {
         "type": CacheTypeType,
     },
 )
-_OptionalProjectCacheOutputTypeDef = TypedDict(
-    "_OptionalProjectCacheOutputTypeDef",
+_OptionalProjectCacheTypeDef = TypedDict(
+    "_OptionalProjectCacheTypeDef",
     {
         "location": str,
         "modes": List[CacheModeType],
     },
     total=False,
 )
 
-class ProjectCacheOutputTypeDef(
-    _RequiredProjectCacheOutputTypeDef, _OptionalProjectCacheOutputTypeDef
-):
+
+class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
     pass
 
+
 ProjectFileSystemLocationTypeDef = TypedDict(
     "ProjectFileSystemLocationTypeDef",
     {
         "type": Literal["EFS"],
         "location": str,
         "mountPoint": str,
         "identifier": str,
@@ -370,16 +353,16 @@
     "ProjectSourceVersionTypeDef",
     {
         "sourceIdentifier": str,
         "sourceVersion": str,
     },
 )
 
-VpcConfigOutputTypeDef = TypedDict(
-    "VpcConfigOutputTypeDef",
+VpcConfigTypeDef = TypedDict(
+    "VpcConfigTypeDef",
     {
         "vpcId": str,
         "subnets": List[str],
         "securityGroupIds": List[str],
     },
     total=False,
 )
@@ -441,19 +424,21 @@
     {
         "groupName": str,
         "streamName": str,
     },
     total=False,
 )
 
+
 class CloudWatchLogsConfigTypeDef(
     _RequiredCloudWatchLogsConfigTypeDef, _OptionalCloudWatchLogsConfigTypeDef
 ):
     pass
 
+
 CodeCoverageReportSummaryTypeDef = TypedDict(
     "CodeCoverageReportSummaryTypeDef",
     {
         "lineCoveragePercentage": float,
         "linesCovered": int,
         "linesMissed": int,
         "branchCoveragePercentage": float,
@@ -498,54 +483,28 @@
         "encryptionDisabled": bool,
         "artifactIdentifier": str,
         "bucketOwnerAccess": BucketOwnerAccessType,
     },
     total=False,
 )
 
+
 class ProjectArtifactsTypeDef(_RequiredProjectArtifactsTypeDef, _OptionalProjectArtifactsTypeDef):
     pass
 
-_RequiredProjectCacheTypeDef = TypedDict(
-    "_RequiredProjectCacheTypeDef",
-    {
-        "type": CacheTypeType,
-    },
-)
-_OptionalProjectCacheTypeDef = TypedDict(
-    "_OptionalProjectCacheTypeDef",
-    {
-        "location": str,
-        "modes": Sequence[CacheModeType],
-    },
-    total=False,
-)
-
-class ProjectCacheTypeDef(_RequiredProjectCacheTypeDef, _OptionalProjectCacheTypeDef):
-    pass
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
-VpcConfigTypeDef = TypedDict(
-    "VpcConfigTypeDef",
-    {
-        "vpcId": str,
-        "subnets": Sequence[str],
-        "securityGroupIds": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredWebhookFilterTypeDef = TypedDict(
     "_RequiredWebhookFilterTypeDef",
     {
         "type": WebhookFilterTypeType,
         "pattern": str,
     },
 )
@@ -553,17 +512,19 @@
     "_OptionalWebhookFilterTypeDef",
     {
         "excludeMatchedPattern": bool,
     },
     total=False,
 )
 
+
 class WebhookFilterTypeDef(_RequiredWebhookFilterTypeDef, _OptionalWebhookFilterTypeDef):
     pass
 
+
 DeleteBuildBatchInputRequestTypeDef = TypedDict(
     "DeleteBuildBatchInputRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -584,19 +545,21 @@
     "_OptionalDeleteReportGroupInputRequestTypeDef",
     {
         "deleteReports": bool,
     },
     total=False,
 )
 
+
 class DeleteReportGroupInputRequestTypeDef(
     _RequiredDeleteReportGroupInputRequestTypeDef, _OptionalDeleteReportGroupInputRequestTypeDef
 ):
     pass
 
+
 DeleteReportInputRequestTypeDef = TypedDict(
     "DeleteReportInputRequestTypeDef",
     {
         "arn": str,
     },
 )
 
@@ -646,20 +609,22 @@
         "sortBy": ReportCodeCoverageSortByTypeType,
         "minLineCoveragePercentage": float,
         "maxLineCoveragePercentage": float,
     },
     total=False,
 )
 
+
 class DescribeCodeCoveragesInputRequestTypeDef(
     _RequiredDescribeCodeCoveragesInputRequestTypeDef,
     _OptionalDescribeCodeCoveragesInputRequestTypeDef,
 ):
     pass
 
+
 TestCaseFilterTypeDef = TypedDict(
     "TestCaseFilterTypeDef",
     {
         "status": str,
         "keyword": str,
     },
     total=False,
@@ -701,19 +666,21 @@
     "_OptionalEnvironmentVariableTypeDef",
     {
         "type": EnvironmentVariableTypeType,
     },
     total=False,
 )
 
+
 class EnvironmentVariableTypeDef(
     _RequiredEnvironmentVariableTypeDef, _OptionalEnvironmentVariableTypeDef
 ):
     pass
 
+
 _RequiredGetReportGroupTrendInputRequestTypeDef = TypedDict(
     "_RequiredGetReportGroupTrendInputRequestTypeDef",
     {
         "reportGroupArn": str,
         "trendField": ReportGroupTrendFieldTypeType,
     },
 )
@@ -721,19 +688,21 @@
     "_OptionalGetReportGroupTrendInputRequestTypeDef",
     {
         "numOfReports": int,
     },
     total=False,
 )
 
+
 class GetReportGroupTrendInputRequestTypeDef(
     _RequiredGetReportGroupTrendInputRequestTypeDef, _OptionalGetReportGroupTrendInputRequestTypeDef
 ):
     pass
 
+
 ReportGroupTrendStatsTypeDef = TypedDict(
     "ReportGroupTrendStatsTypeDef",
     {
         "average": str,
         "max": str,
         "min": str,
     },
@@ -776,20 +745,22 @@
     {
         "username": str,
         "shouldOverwrite": bool,
     },
     total=False,
 )
 
+
 class ImportSourceCredentialsInputRequestTypeDef(
     _RequiredImportSourceCredentialsInputRequestTypeDef,
     _OptionalImportSourceCredentialsInputRequestTypeDef,
 ):
     pass
 
+
 InvalidateProjectCacheInputRequestTypeDef = TypedDict(
     "InvalidateProjectCacheInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
@@ -804,20 +775,22 @@
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListBuildsForProjectInputRequestTypeDef(
     _RequiredListBuildsForProjectInputRequestTypeDef,
     _OptionalListBuildsForProjectInputRequestTypeDef,
 ):
     pass
 
+
 ListBuildsInputRequestTypeDef = TypedDict(
     "ListBuildsInputRequestTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "nextToken": str,
     },
     total=False,
@@ -896,17 +869,19 @@
         "location": str,
         "encryptionDisabled": bool,
         "bucketOwnerAccess": BucketOwnerAccessType,
     },
     total=False,
 )
 
+
 class S3LogsConfigTypeDef(_RequiredS3LogsConfigTypeDef, _OptionalS3LogsConfigTypeDef):
     pass
 
+
 ProjectBadgeTypeDef = TypedDict(
     "ProjectBadgeTypeDef",
     {
         "badgeEnabled": bool,
         "badgeRequestUrl": str,
     },
     total=False,
@@ -930,17 +905,19 @@
     "_OptionalSourceAuthTypeDef",
     {
         "resource": str,
     },
     total=False,
 )
 
+
 class SourceAuthTypeDef(_RequiredSourceAuthTypeDef, _OptionalSourceAuthTypeDef):
     pass
 
+
 PutResourcePolicyInputRequestTypeDef = TypedDict(
     "PutResourcePolicyInputRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
     },
 )
@@ -1011,20 +988,22 @@
     "_OptionalUpdateProjectVisibilityInputRequestTypeDef",
     {
         "resourceAccessRole": str,
     },
     total=False,
 )
 
+
 class UpdateProjectVisibilityInputRequestTypeDef(
     _RequiredUpdateProjectVisibilityInputRequestTypeDef,
     _OptionalUpdateProjectVisibilityInputRequestTypeDef,
 ):
     pass
 
+
 BatchDeleteBuildsOutputTypeDef = TypedDict(
     "BatchDeleteBuildsOutputTypeDef",
     {
         "buildsDeleted": List[str],
         "buildsNotDeleted": List[BuildNotDeletedTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1168,26 +1147,14 @@
         "projectArn": str,
         "publicProjectAlias": str,
         "projectVisibility": ProjectVisibilityTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProjectBuildBatchConfigOutputTypeDef = TypedDict(
-    "ProjectBuildBatchConfigOutputTypeDef",
-    {
-        "serviceRole": str,
-        "combineArtifacts": bool,
-        "restrictions": BatchRestrictionsOutputTypeDef,
-        "timeoutInMins": int,
-        "batchReportMode": BatchReportModeTypeType,
-    },
-    total=False,
-)
-
 ProjectBuildBatchConfigTypeDef = TypedDict(
     "ProjectBuildBatchConfigTypeDef",
     {
         "serviceRole": str,
         "combineArtifacts": bool,
         "restrictions": BatchRestrictionsTypeDef,
         "timeoutInMins": int,
@@ -1262,16 +1229,14 @@
     {
         "nextToken": str,
         "codeCoverages": List[CodeCoverageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProjectCacheUnionTypeDef = Union[ProjectCacheTypeDef, ProjectCacheOutputTypeDef]
-VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredCreateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredCreateWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalCreateWebhookInputRequestTypeDef = TypedDict(
@@ -1280,19 +1245,21 @@
         "branchFilter": str,
         "filterGroups": Sequence[Sequence[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
     },
     total=False,
 )
 
+
 class CreateWebhookInputRequestTypeDef(
     _RequiredCreateWebhookInputRequestTypeDef, _OptionalCreateWebhookInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateWebhookInputRequestTypeDef = TypedDict(
     "_RequiredUpdateWebhookInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateWebhookInputRequestTypeDef = TypedDict(
@@ -1302,19 +1269,21 @@
         "rotateSecret": bool,
         "filterGroups": Sequence[Sequence[WebhookFilterTypeDef]],
         "buildType": WebhookBuildTypeType,
     },
     total=False,
 )
 
+
 class UpdateWebhookInputRequestTypeDef(
     _RequiredUpdateWebhookInputRequestTypeDef, _OptionalUpdateWebhookInputRequestTypeDef
 ):
     pass
 
+
 WebhookTypeDef = TypedDict(
     "WebhookTypeDef",
     {
         "url": str,
         "payloadUrl": str,
         "secret": str,
         "branchFilter": str,
@@ -1339,20 +1308,22 @@
         "minLineCoveragePercentage": float,
         "maxLineCoveragePercentage": float,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef(
     _RequiredDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
     _OptionalDescribeCodeCoveragesInputDescribeCodeCoveragesPaginateTypeDef,
 ):
     pass
 
+
 ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef = TypedDict(
     "ListBuildBatchesForProjectInputListBuildBatchesForProjectPaginateTypeDef",
     {
         "projectName": str,
         "filter": BuildBatchFilterTypeDef,
         "sortOrder": SortOrderTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
@@ -1381,20 +1352,22 @@
     {
         "sortOrder": SortOrderTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListBuildsForProjectInputListBuildsForProjectPaginateTypeDef(
     _RequiredListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
     _OptionalListBuildsForProjectInputListBuildsForProjectPaginateTypeDef,
 ):
     pass
 
+
 ListBuildsInputListBuildsPaginateTypeDef = TypedDict(
     "ListBuildsInputListBuildsPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1451,20 +1424,22 @@
     {
         "filter": TestCaseFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTestCasesInputDescribeTestCasesPaginateTypeDef(
     _RequiredDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
     _OptionalDescribeTestCasesInputDescribeTestCasesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeTestCasesInputRequestTypeDef = TypedDict(
     "_RequiredDescribeTestCasesInputRequestTypeDef",
     {
         "reportArn": str,
     },
 )
 _OptionalDescribeTestCasesInputRequestTypeDef = TypedDict(
@@ -1473,19 +1448,21 @@
         "nextToken": str,
         "maxResults": int,
         "filter": TestCaseFilterTypeDef,
     },
     total=False,
 )
 
+
 class DescribeTestCasesInputRequestTypeDef(
     _RequiredDescribeTestCasesInputRequestTypeDef, _OptionalDescribeTestCasesInputRequestTypeDef
 ):
     pass
 
+
 DescribeTestCasesOutputTypeDef = TypedDict(
     "DescribeTestCasesOutputTypeDef",
     {
         "nextToken": str,
         "testCases": List[TestCaseTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1521,20 +1498,22 @@
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef(
     _RequiredListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
     _OptionalListReportsForReportGroupInputListReportsForReportGroupPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListReportsForReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredListReportsForReportGroupInputRequestTypeDef",
     {
         "reportGroupArn": str,
     },
 )
 _OptionalListReportsForReportGroupInputRequestTypeDef = TypedDict(
@@ -1544,20 +1523,22 @@
         "sortOrder": SortOrderTypeType,
         "maxResults": int,
         "filter": ReportFilterTypeDef,
     },
     total=False,
 )
 
+
 class ListReportsForReportGroupInputRequestTypeDef(
     _RequiredListReportsForReportGroupInputRequestTypeDef,
     _OptionalListReportsForReportGroupInputRequestTypeDef,
 ):
     pass
 
+
 ListReportsInputListReportsPaginateTypeDef = TypedDict(
     "ListReportsInputListReportsPaginateTypeDef",
     {
         "sortOrder": SortOrderTypeType,
         "filter": ReportFilterTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1603,64 +1584,41 @@
         "s3LogsArn": str,
         "cloudWatchLogs": CloudWatchLogsConfigTypeDef,
         "s3Logs": S3LogsConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredProjectEnvironmentOutputTypeDef = TypedDict(
-    "_RequiredProjectEnvironmentOutputTypeDef",
-    {
-        "type": EnvironmentTypeType,
-        "image": str,
-        "computeType": ComputeTypeType,
-    },
-)
-_OptionalProjectEnvironmentOutputTypeDef = TypedDict(
-    "_OptionalProjectEnvironmentOutputTypeDef",
-    {
-        "environmentVariables": List[EnvironmentVariableTypeDef],
-        "privilegedMode": bool,
-        "certificate": str,
-        "registryCredential": RegistryCredentialTypeDef,
-        "imagePullCredentialsType": ImagePullCredentialsTypeType,
-    },
-    total=False,
-)
-
-class ProjectEnvironmentOutputTypeDef(
-    _RequiredProjectEnvironmentOutputTypeDef, _OptionalProjectEnvironmentOutputTypeDef
-):
-    pass
-
 _RequiredProjectEnvironmentTypeDef = TypedDict(
     "_RequiredProjectEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "image": str,
         "computeType": ComputeTypeType,
     },
 )
 _OptionalProjectEnvironmentTypeDef = TypedDict(
     "_OptionalProjectEnvironmentTypeDef",
     {
-        "environmentVariables": Sequence[EnvironmentVariableTypeDef],
+        "environmentVariables": List[EnvironmentVariableTypeDef],
         "privilegedMode": bool,
         "certificate": str,
         "registryCredential": RegistryCredentialTypeDef,
         "imagePullCredentialsType": ImagePullCredentialsTypeType,
     },
     total=False,
 )
 
+
 class ProjectEnvironmentTypeDef(
     _RequiredProjectEnvironmentTypeDef, _OptionalProjectEnvironmentTypeDef
 ):
     pass
 
+
 _RequiredProjectSourceTypeDef = TypedDict(
     "_RequiredProjectSourceTypeDef",
     {
         "type": SourceTypeType,
     },
 )
 _OptionalProjectSourceTypeDef = TypedDict(
@@ -1675,29 +1633,28 @@
         "buildStatusConfig": BuildStatusConfigTypeDef,
         "insecureSsl": bool,
         "sourceIdentifier": str,
     },
     total=False,
 )
 
+
 class ProjectSourceTypeDef(_RequiredProjectSourceTypeDef, _OptionalProjectSourceTypeDef):
     pass
 
+
 ReportExportConfigTypeDef = TypedDict(
     "ReportExportConfigTypeDef",
     {
         "exportConfigType": ReportExportConfigTypeType,
         "s3Destination": S3ReportExportConfigTypeDef,
     },
     total=False,
 )
 
-ProjectBuildBatchConfigUnionTypeDef = Union[
-    ProjectBuildBatchConfigTypeDef, ProjectBuildBatchConfigOutputTypeDef
-]
 BuildGroupTypeDef = TypedDict(
     "BuildGroupTypeDef",
     {
         "identifier": str,
         "dependsOn": List[str],
         "ignoreFailure": bool,
         "currentBuildSummary": BuildSummaryTypeDef,
@@ -1727,15 +1684,14 @@
     {
         "platform": PlatformTypeType,
         "languages": List[EnvironmentLanguageTypeDef],
     },
     total=False,
 )
 
-ProjectEnvironmentUnionTypeDef = Union[ProjectEnvironmentTypeDef, ProjectEnvironmentOutputTypeDef]
 BuildTypeDef = TypedDict(
     "BuildTypeDef",
     {
         "id": str,
         "arn": str,
         "buildNumber": int,
         "startTime": datetime,
@@ -1747,23 +1703,23 @@
         "projectName": str,
         "phases": List[BuildPhaseTypeDef],
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheOutputTypeDef,
-        "environment": ProjectEnvironmentOutputTypeDef,
+        "cache": ProjectCacheTypeDef,
+        "environment": ProjectEnvironmentTypeDef,
         "serviceRole": str,
         "logs": LogsLocationTypeDef,
         "timeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "buildComplete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigOutputTypeDef,
+        "vpcConfig": VpcConfigTypeDef,
         "networkInterface": NetworkInterfaceTypeDef,
         "encryptionKey": str,
         "exportedEnvironmentVariables": List[ExportedEnvironmentVariableTypeDef],
         "reportArns": List[str],
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
         "debugSession": DebugSessionTypeDef,
         "buildBatchArn": str,
@@ -1800,46 +1756,48 @@
         "fileSystemLocations": Sequence[ProjectFileSystemLocationTypeDef],
         "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "concurrentBuildLimit": int,
     },
     total=False,
 )
 
+
 class CreateProjectInputRequestTypeDef(
     _RequiredCreateProjectInputRequestTypeDef, _OptionalCreateProjectInputRequestTypeDef
 ):
     pass
 
+
 ProjectTypeDef = TypedDict(
     "ProjectTypeDef",
     {
         "name": str,
         "arn": str,
         "description": str,
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "sourceVersion": str,
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": ProjectArtifactsTypeDef,
         "secondaryArtifacts": List[ProjectArtifactsTypeDef],
-        "cache": ProjectCacheOutputTypeDef,
-        "environment": ProjectEnvironmentOutputTypeDef,
+        "cache": ProjectCacheTypeDef,
+        "environment": ProjectEnvironmentTypeDef,
         "serviceRole": str,
         "timeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "encryptionKey": str,
         "tags": List[TagTypeDef],
         "created": datetime,
         "lastModified": datetime,
         "webhook": WebhookTypeDef,
-        "vpcConfig": VpcConfigOutputTypeDef,
+        "vpcConfig": VpcConfigTypeDef,
         "badge": ProjectBadgeTypeDef,
         "logsConfig": LogsConfigTypeDef,
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
+        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "concurrentBuildLimit": int,
         "projectVisibility": ProjectVisibilityTypeType,
         "publicProjectAlias": str,
         "resourceAccessRole": str,
     },
     total=False,
 )
@@ -1883,19 +1841,21 @@
         "imagePullCredentialsTypeOverride": ImagePullCredentialsTypeType,
         "buildBatchConfigOverride": ProjectBuildBatchConfigTypeDef,
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
+
 class StartBuildBatchInputRequestTypeDef(
     _RequiredStartBuildBatchInputRequestTypeDef, _OptionalStartBuildBatchInputRequestTypeDef
 ):
     pass
 
+
 _RequiredStartBuildInputRequestTypeDef = TypedDict(
     "_RequiredStartBuildInputRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalStartBuildInputRequestTypeDef = TypedDict(
@@ -1931,19 +1891,21 @@
         "registryCredentialOverride": RegistryCredentialTypeDef,
         "imagePullCredentialsTypeOverride": ImagePullCredentialsTypeType,
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
+
 class StartBuildInputRequestTypeDef(
     _RequiredStartBuildInputRequestTypeDef, _OptionalStartBuildInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateProjectInputRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectInputRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateProjectInputRequestTypeDef = TypedDict(
@@ -1969,19 +1931,21 @@
         "fileSystemLocations": Sequence[ProjectFileSystemLocationTypeDef],
         "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "concurrentBuildLimit": int,
     },
     total=False,
 )
 
+
 class UpdateProjectInputRequestTypeDef(
     _RequiredUpdateProjectInputRequestTypeDef, _OptionalUpdateProjectInputRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateReportGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateReportGroupInputRequestTypeDef",
     {
         "name": str,
         "type": ReportTypeType,
         "exportConfig": ReportExportConfigTypeDef,
     },
@@ -1990,19 +1954,21 @@
     "_OptionalCreateReportGroupInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateReportGroupInputRequestTypeDef(
     _RequiredCreateReportGroupInputRequestTypeDef, _OptionalCreateReportGroupInputRequestTypeDef
 ):
     pass
 
+
 ReportGroupTypeDef = TypedDict(
     "ReportGroupTypeDef",
     {
         "arn": str,
         "name": str,
         "type": ReportTypeType,
         "exportConfig": ReportExportConfigTypeDef,
@@ -2044,19 +2010,21 @@
     {
         "exportConfig": ReportExportConfigTypeDef,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class UpdateReportGroupInputRequestTypeDef(
     _RequiredUpdateReportGroupInputRequestTypeDef, _OptionalUpdateReportGroupInputRequestTypeDef
 ):
     pass
 
+
 BuildBatchTypeDef = TypedDict(
     "BuildBatchTypeDef",
     {
         "id": str,
         "arn": str,
         "startTime": datetime,
         "endTime": datetime,
@@ -2067,27 +2035,27 @@
         "projectName": str,
         "phases": List[BuildBatchPhaseTypeDef],
         "source": ProjectSourceTypeDef,
         "secondarySources": List[ProjectSourceTypeDef],
         "secondarySourceVersions": List[ProjectSourceVersionTypeDef],
         "artifacts": BuildArtifactsTypeDef,
         "secondaryArtifacts": List[BuildArtifactsTypeDef],
-        "cache": ProjectCacheOutputTypeDef,
-        "environment": ProjectEnvironmentOutputTypeDef,
+        "cache": ProjectCacheTypeDef,
+        "environment": ProjectEnvironmentTypeDef,
         "serviceRole": str,
         "logConfig": LogsConfigTypeDef,
         "buildTimeoutInMinutes": int,
         "queuedTimeoutInMinutes": int,
         "complete": bool,
         "initiator": str,
-        "vpcConfig": VpcConfigOutputTypeDef,
+        "vpcConfig": VpcConfigTypeDef,
         "encryptionKey": str,
         "buildBatchNumber": int,
         "fileSystemLocations": List[ProjectFileSystemLocationTypeDef],
-        "buildBatchConfig": ProjectBuildBatchConfigOutputTypeDef,
+        "buildBatchConfig": ProjectBuildBatchConfigTypeDef,
         "buildGroups": List[BuildGroupTypeDef],
         "debugSessionEnabled": bool,
     },
     total=False,
 )
 
 ListCuratedEnvironmentImagesOutputTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-codebuild-2.5.2.post1/types_aiobotocore_codebuild.egg-info/SOURCES.txt` & `types-aiobotocore-codebuild-2.5.2.post2/types_aiobotocore_codebuild.egg-info/SOURCES.txt`

 * *Files identical despite different names*

