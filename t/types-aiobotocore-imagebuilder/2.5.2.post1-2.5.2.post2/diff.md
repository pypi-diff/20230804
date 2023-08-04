# Comparing `tmp/types-aiobotocore-imagebuilder-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-imagebuilder-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-imagebuilder-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-imagebuilder-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
```

## Comparing `types-aiobotocore-imagebuilder-2.5.2.post1.tar` & `types-aiobotocore-imagebuilder-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.033570 types-aiobotocore-imagebuilder-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-08-02 14:52:24.033570 types-aiobotocore-imagebuilder-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18770 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.033570 types-aiobotocore-imagebuilder-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.033570 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44344 2023-08-02 14:40:09.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44279 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-08-02 14:40:10.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9688 2023-08-02 14:40:10.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71029 2023-08-02 14:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    70968 2023-08-02 14:40:11.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:08.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.033570 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:23.000000 types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.286642 types-aiobotocore-imagebuilder-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12443 2023-08-04 13:59:11.286642 types-aiobotocore-imagebuilder-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10905 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.286642 types-aiobotocore-imagebuilder-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.286642 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      482 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      481 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    44284 2023-08-04 13:40:13.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    44219 2023-08-04 13:40:13.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9785 2023-08-04 13:40:13.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9783 2023-08-04 13:40:13.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    66585 2023-08-04 13:40:15.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    66530 2023-08-04 13:40:14.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:12.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.286642 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12443 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:11.000000 types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post1/LICENSE` & `types-aiobotocore-imagebuilder-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post1/setup.py` & `types-aiobotocore-imagebuilder-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-imagebuilder",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_imagebuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.imagebuilder 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/__main__.py` & `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.imagebuilder 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.imagebuilder 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder\nOther"
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

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/client.py` & `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ComponentTypeType, OwnershipType, PipelineStatusType, PlatformType
 from .type_defs import (
     AdditionalInstanceConfigurationTypeDef,
     CancelImageCreationResponseTypeDef,
-    ComponentConfigurationUnionTypeDef,
+    ComponentConfigurationTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
     CreateImagePipelineResponseTypeDef,
     CreateImageRecipeResponseTypeDef,
     CreateImageResponseTypeDef,
     CreateInfrastructureConfigurationResponseTypeDef,
     DeleteComponentResponseTypeDef,
     DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
-    DistributionUnionTypeDef,
+    DistributionTypeDef,
     FilterTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentResponseTypeDef,
     GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     GetImagePipelineResponseTypeDef,
@@ -51,20 +51,20 @@
     GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeResponseTypeDef,
     GetImageResponseTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImageScanFindingsFilterTypeDef,
-    ImageScanningConfigurationUnionTypeDef,
+    ImageScanningConfigurationTypeDef,
     ImageTestsConfigurationTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
-    InstanceConfigurationUnionTypeDef,
+    InstanceConfigurationTypeDef,
     InstanceMetadataOptionsTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListContainerRecipesResponseTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePackagesResponseTypeDef,
@@ -197,20 +197,20 @@
 
     async def create_container_recipe(
         self,
         *,
         containerType: Literal["DOCKER"],
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationUnionTypeDef],
+        components: Sequence[ComponentConfigurationTypeDef],
         parentImage: str,
         targetRepository: TargetContainerRepositoryTypeDef,
         clientToken: str,
         description: str = ...,
-        instanceConfiguration: InstanceConfigurationUnionTypeDef = ...,
+        instanceConfiguration: InstanceConfigurationTypeDef = ...,
         dockerfileTemplateData: str = ...,
         dockerfileTemplateUri: str = ...,
         platformOverride: PlatformType = ...,
         imageOsVersionOverride: str = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         kmsKeyId: str = ...
@@ -222,15 +222,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_container_recipe)
         """
 
     async def create_distribution_configuration(
         self,
         *,
         name: str,
-        distributions: Sequence[DistributionUnionTypeDef],
+        distributions: Sequence[DistributionTypeDef],
         clientToken: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDistributionConfigurationResponseTypeDef:
         """
         Creates a new distribution configuration.
 
@@ -245,15 +245,15 @@
         clientToken: str,
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
     ) -> CreateImageResponseTypeDef:
         """
         Creates a new image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image)
         """
@@ -269,29 +269,29 @@
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
     ) -> CreateImagePipelineResponseTypeDef:
         """
         Creates a new image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image_pipeline)
         """
 
     async def create_image_recipe(
         self,
         *,
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationUnionTypeDef],
+        components: Sequence[ComponentConfigurationTypeDef],
         parentImage: str,
         clientToken: str,
         description: str = ...,
         blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...
@@ -839,15 +839,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#untag_resource)
         """
 
     async def update_distribution_configuration(
         self,
         *,
         distributionConfigurationArn: str,
-        distributions: Sequence[DistributionUnionTypeDef],
+        distributions: Sequence[DistributionTypeDef],
         clientToken: str,
         description: str = ...
     ) -> UpdateDistributionConfigurationResponseTypeDef:
         """
         Updates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_distribution_configuration)
@@ -864,15 +864,15 @@
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
-        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
     ) -> UpdateImagePipelineResponseTypeDef:
         """
         Updates an image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_image_pipeline)
         """
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/client.pyi` & `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ComponentTypeType, OwnershipType, PipelineStatusType, PlatformType
 from .type_defs import (
     AdditionalInstanceConfigurationTypeDef,
     CancelImageCreationResponseTypeDef,
-    ComponentConfigurationUnionTypeDef,
+    ComponentConfigurationTypeDef,
     CreateComponentResponseTypeDef,
     CreateContainerRecipeResponseTypeDef,
     CreateDistributionConfigurationResponseTypeDef,
     CreateImagePipelineResponseTypeDef,
     CreateImageRecipeResponseTypeDef,
     CreateImageResponseTypeDef,
     CreateInfrastructureConfigurationResponseTypeDef,
     DeleteComponentResponseTypeDef,
     DeleteContainerRecipeResponseTypeDef,
     DeleteDistributionConfigurationResponseTypeDef,
     DeleteImagePipelineResponseTypeDef,
     DeleteImageRecipeResponseTypeDef,
     DeleteImageResponseTypeDef,
     DeleteInfrastructureConfigurationResponseTypeDef,
-    DistributionUnionTypeDef,
+    DistributionTypeDef,
     FilterTypeDef,
     GetComponentPolicyResponseTypeDef,
     GetComponentResponseTypeDef,
     GetContainerRecipePolicyResponseTypeDef,
     GetContainerRecipeResponseTypeDef,
     GetDistributionConfigurationResponseTypeDef,
     GetImagePipelineResponseTypeDef,
@@ -51,20 +51,20 @@
     GetImageRecipePolicyResponseTypeDef,
     GetImageRecipeResponseTypeDef,
     GetImageResponseTypeDef,
     GetInfrastructureConfigurationResponseTypeDef,
     GetWorkflowExecutionResponseTypeDef,
     GetWorkflowStepExecutionResponseTypeDef,
     ImageScanFindingsFilterTypeDef,
-    ImageScanningConfigurationUnionTypeDef,
+    ImageScanningConfigurationTypeDef,
     ImageTestsConfigurationTypeDef,
     ImportComponentResponseTypeDef,
     ImportVmImageResponseTypeDef,
     InstanceBlockDeviceMappingTypeDef,
-    InstanceConfigurationUnionTypeDef,
+    InstanceConfigurationTypeDef,
     InstanceMetadataOptionsTypeDef,
     ListComponentBuildVersionsResponseTypeDef,
     ListComponentsResponseTypeDef,
     ListContainerRecipesResponseTypeDef,
     ListDistributionConfigurationsResponseTypeDef,
     ListImageBuildVersionsResponseTypeDef,
     ListImagePackagesResponseTypeDef,
@@ -188,20 +188,20 @@
         """
     async def create_container_recipe(
         self,
         *,
         containerType: Literal["DOCKER"],
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationUnionTypeDef],
+        components: Sequence[ComponentConfigurationTypeDef],
         parentImage: str,
         targetRepository: TargetContainerRepositoryTypeDef,
         clientToken: str,
         description: str = ...,
-        instanceConfiguration: InstanceConfigurationUnionTypeDef = ...,
+        instanceConfiguration: InstanceConfigurationTypeDef = ...,
         dockerfileTemplateData: str = ...,
         dockerfileTemplateUri: str = ...,
         platformOverride: PlatformType = ...,
         imageOsVersionOverride: str = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         kmsKeyId: str = ...
@@ -212,15 +212,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_container_recipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_container_recipe)
         """
     async def create_distribution_configuration(
         self,
         *,
         name: str,
-        distributions: Sequence[DistributionUnionTypeDef],
+        distributions: Sequence[DistributionTypeDef],
         clientToken: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateDistributionConfigurationResponseTypeDef:
         """
         Creates a new distribution configuration.
 
@@ -234,15 +234,15 @@
         clientToken: str,
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
     ) -> CreateImageResponseTypeDef:
         """
         Creates a new image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image)
         """
@@ -257,28 +257,28 @@
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
         tags: Mapping[str, str] = ...,
-        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
     ) -> CreateImagePipelineResponseTypeDef:
         """
         Creates a new image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.create_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#create_image_pipeline)
         """
     async def create_image_recipe(
         self,
         *,
         name: str,
         semanticVersion: str,
-        components: Sequence[ComponentConfigurationUnionTypeDef],
+        components: Sequence[ComponentConfigurationTypeDef],
         parentImage: str,
         clientToken: str,
         description: str = ...,
         blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         workingDirectory: str = ...,
         additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...
@@ -778,15 +778,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#untag_resource)
         """
     async def update_distribution_configuration(
         self,
         *,
         distributionConfigurationArn: str,
-        distributions: Sequence[DistributionUnionTypeDef],
+        distributions: Sequence[DistributionTypeDef],
         clientToken: str,
         description: str = ...
     ) -> UpdateDistributionConfigurationResponseTypeDef:
         """
         Updates a new distribution configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_distribution_configuration)
@@ -802,15 +802,15 @@
         imageRecipeArn: str = ...,
         containerRecipeArn: str = ...,
         distributionConfigurationArn: str = ...,
         imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,
         enhancedImageMetadataEnabled: bool = ...,
         schedule: ScheduleTypeDef = ...,
         status: PipelineStatusType = ...,
-        imageScanningConfiguration: ImageScanningConfigurationUnionTypeDef = ...
+        imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...
     ) -> UpdateImagePipelineResponseTypeDef:
         """
         Updates an image pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder.Client.update_image_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_imagebuilder/client/#update_image_pipeline)
         """
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/literals.py` & `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
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
@@ -205,14 +206,15 @@
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
@@ -291,26 +293,28 @@
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

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/literals.pyi` & `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
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
@@ -203,14 +204,15 @@
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
@@ -289,26 +291,28 @@
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

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/type_defs.py` & `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_imagebuilder.type_defs import SeverityCountsTypeDef
 
     data: SeverityCountsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     BuildTypeType,
     ComponentTypeType,
     DiskImageFormatType,
     EbsVolumeTypeType,
     ImageScanStatusType,
@@ -43,20 +43,18 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "SeverityCountsTypeDef",
     "SystemsManagerAgentTypeDef",
-    "LaunchPermissionConfigurationOutputTypeDef",
     "LaunchPermissionConfigurationTypeDef",
     "ImageStateTypeDef",
     "CancelImageCreationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "ComponentParameterOutputTypeDef",
     "ComponentParameterTypeDef",
     "ComponentParameterDetailTypeDef",
     "ComponentStateTypeDef",
     "ComponentVersionTypeDef",
     "TargetContainerRepositoryTypeDef",
     "ContainerRecipeSummaryTypeDef",
     "ContainerTypeDef",
@@ -73,15 +71,14 @@
     "DeleteImageRecipeRequestRequestTypeDef",
     "DeleteImageRequestRequestTypeDef",
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
     "DistributionConfigurationSummaryTypeDef",
     "LaunchTemplateConfigurationTypeDef",
     "S3ExportConfigurationTypeDef",
     "EbsInstanceBlockDeviceSpecificationTypeDef",
-    "EcrConfigurationOutputTypeDef",
     "EcrConfigurationTypeDef",
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     "FastLaunchSnapshotConfigurationTypeDef",
     "FilterTypeDef",
     "GetComponentPolicyRequestRequestTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetContainerRecipePolicyRequestRequestTypeDef",
@@ -121,15 +118,14 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AccountAggregationTypeDef",
     "ImageAggregationTypeDef",
     "ImagePipelineAggregationTypeDef",
     "VulnerabilityIdAggregationTypeDef",
     "AdditionalInstanceConfigurationTypeDef",
-    "AmiDistributionConfigurationOutputTypeDef",
     "AmiDistributionConfigurationTypeDef",
     "AmiTypeDef",
     "CancelImageCreationResponseTypeDef",
     "CreateComponentResponseTypeDef",
     "CreateContainerRecipeResponseTypeDef",
     "CreateDistributionConfigurationResponseTypeDef",
     "CreateImagePipelineResponseTypeDef",
@@ -156,26 +152,23 @@
     "PutContainerRecipePolicyResponseTypeDef",
     "PutImagePolicyResponseTypeDef",
     "PutImageRecipePolicyResponseTypeDef",
     "StartImagePipelineExecutionResponseTypeDef",
     "UpdateDistributionConfigurationResponseTypeDef",
     "UpdateImagePipelineResponseTypeDef",
     "UpdateInfrastructureConfigurationResponseTypeDef",
-    "ComponentConfigurationOutputTypeDef",
     "ComponentConfigurationTypeDef",
     "ComponentSummaryTypeDef",
     "ComponentTypeDef",
     "ListComponentsResponseTypeDef",
-    "ContainerDistributionConfigurationOutputTypeDef",
     "ContainerDistributionConfigurationTypeDef",
     "ListContainerRecipesResponseTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDistributionConfigurationsResponseTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
-    "ImageScanningConfigurationOutputTypeDef",
     "ImageScanningConfigurationTypeDef",
     "FastLaunchConfigurationTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListContainerRecipesRequestRequestTypeDef",
     "ListDistributionConfigurationsRequestRequestTypeDef",
     "ListImageBuildVersionsRequestRequestTypeDef",
     "ListImagePipelineImagesRequestRequestTypeDef",
@@ -192,52 +185,46 @@
     "ListWorkflowExecutionsResponseTypeDef",
     "ListWorkflowStepExecutionsResponseTypeDef",
     "LoggingTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ImageScanFindingAggregationTypeDef",
     "OutputResourcesTypeDef",
-    "ComponentConfigurationUnionTypeDef",
     "ListComponentBuildVersionsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
+    "CreateImageRecipeRequestRequestTypeDef",
     "ImageRecipeTypeDef",
-    "InstanceConfigurationOutputTypeDef",
     "InstanceConfigurationTypeDef",
-    "ImagePipelineTypeDef",
     "CreateImagePipelineRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
-    "ImageScanningConfigurationUnionTypeDef",
+    "ImagePipelineTypeDef",
     "UpdateImagePipelineRequestRequestTypeDef",
-    "DistributionOutputTypeDef",
     "DistributionTypeDef",
     "CreateInfrastructureConfigurationRequestRequestTypeDef",
     "InfrastructureConfigurationTypeDef",
     "UpdateInfrastructureConfigurationRequestRequestTypeDef",
     "ListImageScanFindingAggregationsResponseTypeDef",
     "ImageSummaryTypeDef",
-    "CreateImageRecipeRequestRequestTypeDef",
     "ImageScanFindingTypeDef",
     "GetImageRecipeResponseTypeDef",
     "ContainerRecipeTypeDef",
     "CreateContainerRecipeRequestRequestTypeDef",
-    "InstanceConfigurationUnionTypeDef",
     "GetImagePipelineResponseTypeDef",
     "ListImagePipelinesResponseTypeDef",
+    "CreateDistributionConfigurationRequestRequestTypeDef",
     "DistributionConfigurationTypeDef",
-    "DistributionUnionTypeDef",
+    "UpdateDistributionConfigurationRequestRequestTypeDef",
     "GetInfrastructureConfigurationResponseTypeDef",
     "ListImageBuildVersionsResponseTypeDef",
     "ListImagePipelineImagesResponseTypeDef",
     "ListImageScanFindingsResponseTypeDef",
     "GetContainerRecipeResponseTypeDef",
     "GetDistributionConfigurationResponseTypeDef",
     "ImageTypeDef",
-    "CreateDistributionConfigurationRequestRequestTypeDef",
-    "UpdateDistributionConfigurationRequestRequestTypeDef",
     "GetImageResponseTypeDef",
 )
 
 SeverityCountsTypeDef = TypedDict(
     "SeverityCountsTypeDef",
     {
         "all": int,
@@ -252,25 +239,14 @@
     "SystemsManagerAgentTypeDef",
     {
         "uninstallAfterBuild": bool,
     },
     total=False,
 )
 
-LaunchPermissionConfigurationOutputTypeDef = TypedDict(
-    "LaunchPermissionConfigurationOutputTypeDef",
-    {
-        "userIds": List[str],
-        "userGroups": List[str],
-        "organizationArns": List[str],
-        "organizationalUnitArns": List[str],
-    },
-    total=False,
-)
-
 LaunchPermissionConfigurationTypeDef = TypedDict(
     "LaunchPermissionConfigurationTypeDef",
     {
         "userIds": Sequence[str],
         "userGroups": Sequence[str],
         "organizationArns": Sequence[str],
         "organizationalUnitArns": Sequence[str],
@@ -302,22 +278,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ComponentParameterOutputTypeDef = TypedDict(
-    "ComponentParameterOutputTypeDef",
-    {
-        "name": str,
-        "value": List[str],
-    },
-)
-
 ComponentParameterTypeDef = TypedDict(
     "ComponentParameterTypeDef",
     {
         "name": str,
         "value": Sequence[str],
     },
 )
@@ -599,23 +567,14 @@
         "volumeSize": int,
         "volumeType": EbsVolumeTypeType,
         "throughput": int,
     },
     total=False,
 )
 
-EcrConfigurationOutputTypeDef = TypedDict(
-    "EcrConfigurationOutputTypeDef",
-    {
-        "repositoryName": str,
-        "containerTags": List[str],
-    },
-    total=False,
-)
-
 EcrConfigurationTypeDef = TypedDict(
     "EcrConfigurationTypeDef",
     {
         "repositoryName": str,
         "containerTags": Sequence[str],
     },
     total=False,
@@ -1137,27 +1096,14 @@
     {
         "systemsManagerAgent": SystemsManagerAgentTypeDef,
         "userDataOverride": str,
     },
     total=False,
 )
 
-AmiDistributionConfigurationOutputTypeDef = TypedDict(
-    "AmiDistributionConfigurationOutputTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "targetAccountIds": List[str],
-        "amiTags": Dict[str, str],
-        "kmsKeyId": str,
-        "launchPermission": LaunchPermissionConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 AmiDistributionConfigurationTypeDef = TypedDict(
     "AmiDistributionConfigurationTypeDef",
     {
         "name": str,
         "description": str,
         "targetAccountIds": Sequence[str],
         "amiTags": Mapping[str, str],
@@ -1503,35 +1449,14 @@
         "requestId": str,
         "clientToken": str,
         "infrastructureConfigurationArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredComponentConfigurationOutputTypeDef = TypedDict(
-    "_RequiredComponentConfigurationOutputTypeDef",
-    {
-        "componentArn": str,
-    },
-)
-_OptionalComponentConfigurationOutputTypeDef = TypedDict(
-    "_OptionalComponentConfigurationOutputTypeDef",
-    {
-        "parameters": List[ComponentParameterOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class ComponentConfigurationOutputTypeDef(
-    _RequiredComponentConfigurationOutputTypeDef, _OptionalComponentConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredComponentConfigurationTypeDef = TypedDict(
     "_RequiredComponentConfigurationTypeDef",
     {
         "componentArn": str,
     },
 )
 _OptionalComponentConfigurationTypeDef = TypedDict(
@@ -1601,37 +1526,14 @@
         "requestId": str,
         "componentVersionList": List[ComponentVersionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredContainerDistributionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredContainerDistributionConfigurationOutputTypeDef",
-    {
-        "targetRepository": TargetContainerRepositoryTypeDef,
-    },
-)
-_OptionalContainerDistributionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalContainerDistributionConfigurationOutputTypeDef",
-    {
-        "description": str,
-        "containerTags": List[str],
-    },
-    total=False,
-)
-
-
-class ContainerDistributionConfigurationOutputTypeDef(
-    _RequiredContainerDistributionConfigurationOutputTypeDef,
-    _OptionalContainerDistributionConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredContainerDistributionConfigurationTypeDef = TypedDict(
     "_RequiredContainerDistributionConfigurationTypeDef",
     {
         "targetRepository": TargetContainerRepositoryTypeDef,
     },
 )
 _OptionalContainerDistributionConfigurationTypeDef = TypedDict(
@@ -1691,23 +1593,14 @@
         "ebs": EbsInstanceBlockDeviceSpecificationTypeDef,
         "virtualName": str,
         "noDevice": str,
     },
     total=False,
 )
 
-ImageScanningConfigurationOutputTypeDef = TypedDict(
-    "ImageScanningConfigurationOutputTypeDef",
-    {
-        "imageScanningEnabled": bool,
-        "ecrConfiguration": EcrConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "imageScanningEnabled": bool,
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
     total=False,
@@ -2008,17 +1901,14 @@
     {
         "amis": List[AmiTypeDef],
         "containers": List[ContainerTypeDef],
     },
     total=False,
 )
 
-ComponentConfigurationUnionTypeDef = Union[
-    ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef
-]
 ListComponentBuildVersionsResponseTypeDef = TypedDict(
     "ListComponentBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "componentSummaryList": List[ComponentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2038,78 +1928,73 @@
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": CvssScoreDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImageRecipeRequestRequestTypeDef",
+    {
+        "name": str,
+        "semanticVersion": str,
+        "components": Sequence[ComponentConfigurationTypeDef],
+        "parentImage": str,
+        "clientToken": str,
+    },
+)
+_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImageRecipeRequestRequestTypeDef",
+    {
+        "description": str,
+        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
+        "tags": Mapping[str, str],
+        "workingDirectory": str,
+        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateImageRecipeRequestRequestTypeDef(
+    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
+):
+    pass
+
+
 ImageRecipeTypeDef = TypedDict(
     "ImageRecipeTypeDef",
     {
         "arn": str,
         "type": ImageTypeType,
         "name": str,
         "description": str,
         "platform": PlatformType,
         "owner": str,
         "version": str,
-        "components": List[ComponentConfigurationOutputTypeDef],
+        "components": List[ComponentConfigurationTypeDef],
         "parentImage": str,
         "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
         "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
     },
     total=False,
 )
 
-InstanceConfigurationOutputTypeDef = TypedDict(
-    "InstanceConfigurationOutputTypeDef",
-    {
-        "image": str,
-        "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
-    },
-    total=False,
-)
-
 InstanceConfigurationTypeDef = TypedDict(
     "InstanceConfigurationTypeDef",
     {
         "image": str,
         "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
     },
     total=False,
 )
 
-ImagePipelineTypeDef = TypedDict(
-    "ImagePipelineTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "platform": PlatformType,
-        "enhancedImageMetadataEnabled": bool,
-        "imageRecipeArn": str,
-        "containerRecipeArn": str,
-        "infrastructureConfigurationArn": str,
-        "distributionConfigurationArn": str,
-        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
-        "schedule": ScheduleTypeDef,
-        "status": PipelineStatusType,
-        "dateCreated": str,
-        "dateUpdated": str,
-        "dateLastRun": str,
-        "dateNextRun": str,
-        "tags": Dict[str, str],
-        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImagePipelineRequestRequestTypeDef",
     {
         "name": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2163,17 +2048,39 @@
 
 class CreateImageRequestRequestTypeDef(
     _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
 ):
     pass
 
 
-ImageScanningConfigurationUnionTypeDef = Union[
-    ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
-]
+ImagePipelineTypeDef = TypedDict(
+    "ImagePipelineTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "platform": PlatformType,
+        "enhancedImageMetadataEnabled": bool,
+        "imageRecipeArn": str,
+        "containerRecipeArn": str,
+        "infrastructureConfigurationArn": str,
+        "distributionConfigurationArn": str,
+        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
+        "schedule": ScheduleTypeDef,
+        "status": PipelineStatusType,
+        "dateCreated": str,
+        "dateUpdated": str,
+        "dateLastRun": str,
+        "dateNextRun": str,
+        "tags": Dict[str, str],
+        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2198,40 +2105,14 @@
 class UpdateImagePipelineRequestRequestTypeDef(
     _RequiredUpdateImagePipelineRequestRequestTypeDef,
     _OptionalUpdateImagePipelineRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDistributionOutputTypeDef = TypedDict(
-    "_RequiredDistributionOutputTypeDef",
-    {
-        "region": str,
-    },
-)
-_OptionalDistributionOutputTypeDef = TypedDict(
-    "_OptionalDistributionOutputTypeDef",
-    {
-        "amiDistributionConfiguration": AmiDistributionConfigurationOutputTypeDef,
-        "containerDistributionConfiguration": ContainerDistributionConfigurationOutputTypeDef,
-        "licenseConfigurationArns": List[str],
-        "launchTemplateConfigurations": List[LaunchTemplateConfigurationTypeDef],
-        "s3ExportConfiguration": S3ExportConfigurationTypeDef,
-        "fastLaunchConfigurations": List[FastLaunchConfigurationTypeDef],
-    },
-    total=False,
-)
-
-
-class DistributionOutputTypeDef(
-    _RequiredDistributionOutputTypeDef, _OptionalDistributionOutputTypeDef
-):
-    pass
-
-
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "region": str,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
@@ -2369,43 +2250,14 @@
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
     },
     total=False,
 )
 
-_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImageRecipeRequestRequestTypeDef",
-    {
-        "name": str,
-        "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationUnionTypeDef],
-        "parentImage": str,
-        "clientToken": str,
-    },
-)
-_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImageRecipeRequestRequestTypeDef",
-    {
-        "description": str,
-        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
-        "tags": Mapping[str, str],
-        "workingDirectory": str,
-        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateImageRecipeRequestRequestTypeDef(
-    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
-):
-    pass
-
-
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "awsAccountId": str,
         "imageBuildVersionArn": str,
         "imagePipelineArn": str,
         "type": str,
@@ -2438,16 +2290,16 @@
         "arn": str,
         "containerType": Literal["DOCKER"],
         "name": str,
         "description": str,
         "platform": PlatformType,
         "owner": str,
         "version": str,
-        "components": List[ComponentConfigurationOutputTypeDef],
-        "instanceConfiguration": InstanceConfigurationOutputTypeDef,
+        "components": List[ComponentConfigurationTypeDef],
+        "instanceConfiguration": InstanceConfigurationTypeDef,
         "dockerfileTemplateData": str,
         "kmsKeyId": str,
         "encrypted": bool,
         "parentImage": str,
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
@@ -2458,15 +2310,15 @@
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
         "containerType": Literal["DOCKER"],
         "name": str,
         "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationUnionTypeDef],
+        "components": Sequence[ComponentConfigurationTypeDef],
         "parentImage": str,
         "targetRepository": TargetContainerRepositoryTypeDef,
         "clientToken": str,
     },
 )
 _OptionalCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerRecipeRequestRequestTypeDef",
@@ -2488,17 +2340,14 @@
 class CreateContainerRecipeRequestRequestTypeDef(
     _RequiredCreateContainerRecipeRequestRequestTypeDef,
     _OptionalCreateContainerRecipeRequestRequestTypeDef,
 ):
     pass
 
 
-InstanceConfigurationUnionTypeDef = Union[
-    InstanceConfigurationTypeDef, InstanceConfigurationOutputTypeDef
-]
 GetImagePipelineResponseTypeDef = TypedDict(
     "GetImagePipelineResponseTypeDef",
     {
         "requestId": str,
         "imagePipeline": ImagePipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2510,42 +2359,90 @@
         "requestId": str,
         "imagePipelineList": List[ImagePipelineTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "distributions": Sequence[DistributionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredDistributionConfigurationTypeDef = TypedDict(
     "_RequiredDistributionConfigurationTypeDef",
     {
         "timeoutMinutes": int,
     },
 )
 _OptionalDistributionConfigurationTypeDef = TypedDict(
     "_OptionalDistributionConfigurationTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
-        "distributions": List[DistributionOutputTypeDef],
+        "distributions": List[DistributionTypeDef],
         "dateCreated": str,
         "dateUpdated": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
 class DistributionConfigurationTypeDef(
     _RequiredDistributionConfigurationTypeDef, _OptionalDistributionConfigurationTypeDef
 ):
     pass
 
 
-DistributionUnionTypeDef = Union[DistributionTypeDef, DistributionOutputTypeDef]
+_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "distributionConfigurationArn": str,
+        "distributions": Sequence[DistributionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+
+class UpdateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 GetInfrastructureConfigurationResponseTypeDef = TypedDict(
     "GetInfrastructureConfigurationResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2619,68 +2516,19 @@
         "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
         "dateCreated": str,
         "outputResources": OutputResourcesTypeDef,
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
         "scanState": ImageScanStateTypeDef,
-        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "distributions": Sequence[DistributionUnionTypeDef],
-        "clientToken": str,
-    },
-)
-_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "distributionConfigurationArn": str,
-        "distributions": Sequence[DistributionUnionTypeDef],
-        "clientToken": str,
-    },
-)
-_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
+        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class UpdateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 GetImageResponseTypeDef = TypedDict(
     "GetImageResponseTypeDef",
     {
         "requestId": str,
         "image": ImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder/type_defs.pyi` & `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_imagebuilder.type_defs import SeverityCountsTypeDef
 
     data: SeverityCountsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     BuildTypeType,
     ComponentTypeType,
     DiskImageFormatType,
     EbsVolumeTypeType,
     ImageScanStatusType,
@@ -42,20 +42,18 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "SeverityCountsTypeDef",
     "SystemsManagerAgentTypeDef",
-    "LaunchPermissionConfigurationOutputTypeDef",
     "LaunchPermissionConfigurationTypeDef",
     "ImageStateTypeDef",
     "CancelImageCreationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "ComponentParameterOutputTypeDef",
     "ComponentParameterTypeDef",
     "ComponentParameterDetailTypeDef",
     "ComponentStateTypeDef",
     "ComponentVersionTypeDef",
     "TargetContainerRepositoryTypeDef",
     "ContainerRecipeSummaryTypeDef",
     "ContainerTypeDef",
@@ -72,15 +70,14 @@
     "DeleteImageRecipeRequestRequestTypeDef",
     "DeleteImageRequestRequestTypeDef",
     "DeleteInfrastructureConfigurationRequestRequestTypeDef",
     "DistributionConfigurationSummaryTypeDef",
     "LaunchTemplateConfigurationTypeDef",
     "S3ExportConfigurationTypeDef",
     "EbsInstanceBlockDeviceSpecificationTypeDef",
-    "EcrConfigurationOutputTypeDef",
     "EcrConfigurationTypeDef",
     "FastLaunchLaunchTemplateSpecificationTypeDef",
     "FastLaunchSnapshotConfigurationTypeDef",
     "FilterTypeDef",
     "GetComponentPolicyRequestRequestTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetContainerRecipePolicyRequestRequestTypeDef",
@@ -120,15 +117,14 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AccountAggregationTypeDef",
     "ImageAggregationTypeDef",
     "ImagePipelineAggregationTypeDef",
     "VulnerabilityIdAggregationTypeDef",
     "AdditionalInstanceConfigurationTypeDef",
-    "AmiDistributionConfigurationOutputTypeDef",
     "AmiDistributionConfigurationTypeDef",
     "AmiTypeDef",
     "CancelImageCreationResponseTypeDef",
     "CreateComponentResponseTypeDef",
     "CreateContainerRecipeResponseTypeDef",
     "CreateDistributionConfigurationResponseTypeDef",
     "CreateImagePipelineResponseTypeDef",
@@ -155,26 +151,23 @@
     "PutContainerRecipePolicyResponseTypeDef",
     "PutImagePolicyResponseTypeDef",
     "PutImageRecipePolicyResponseTypeDef",
     "StartImagePipelineExecutionResponseTypeDef",
     "UpdateDistributionConfigurationResponseTypeDef",
     "UpdateImagePipelineResponseTypeDef",
     "UpdateInfrastructureConfigurationResponseTypeDef",
-    "ComponentConfigurationOutputTypeDef",
     "ComponentConfigurationTypeDef",
     "ComponentSummaryTypeDef",
     "ComponentTypeDef",
     "ListComponentsResponseTypeDef",
-    "ContainerDistributionConfigurationOutputTypeDef",
     "ContainerDistributionConfigurationTypeDef",
     "ListContainerRecipesResponseTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDistributionConfigurationsResponseTypeDef",
     "InstanceBlockDeviceMappingTypeDef",
-    "ImageScanningConfigurationOutputTypeDef",
     "ImageScanningConfigurationTypeDef",
     "FastLaunchConfigurationTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListContainerRecipesRequestRequestTypeDef",
     "ListDistributionConfigurationsRequestRequestTypeDef",
     "ListImageBuildVersionsRequestRequestTypeDef",
     "ListImagePipelineImagesRequestRequestTypeDef",
@@ -191,52 +184,46 @@
     "ListWorkflowExecutionsResponseTypeDef",
     "ListWorkflowStepExecutionsResponseTypeDef",
     "LoggingTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
     "ImageScanFindingAggregationTypeDef",
     "OutputResourcesTypeDef",
-    "ComponentConfigurationUnionTypeDef",
     "ListComponentBuildVersionsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "InspectorScoreDetailsTypeDef",
+    "CreateImageRecipeRequestRequestTypeDef",
     "ImageRecipeTypeDef",
-    "InstanceConfigurationOutputTypeDef",
     "InstanceConfigurationTypeDef",
-    "ImagePipelineTypeDef",
     "CreateImagePipelineRequestRequestTypeDef",
     "CreateImageRequestRequestTypeDef",
-    "ImageScanningConfigurationUnionTypeDef",
+    "ImagePipelineTypeDef",
     "UpdateImagePipelineRequestRequestTypeDef",
-    "DistributionOutputTypeDef",
     "DistributionTypeDef",
     "CreateInfrastructureConfigurationRequestRequestTypeDef",
     "InfrastructureConfigurationTypeDef",
     "UpdateInfrastructureConfigurationRequestRequestTypeDef",
     "ListImageScanFindingAggregationsResponseTypeDef",
     "ImageSummaryTypeDef",
-    "CreateImageRecipeRequestRequestTypeDef",
     "ImageScanFindingTypeDef",
     "GetImageRecipeResponseTypeDef",
     "ContainerRecipeTypeDef",
     "CreateContainerRecipeRequestRequestTypeDef",
-    "InstanceConfigurationUnionTypeDef",
     "GetImagePipelineResponseTypeDef",
     "ListImagePipelinesResponseTypeDef",
+    "CreateDistributionConfigurationRequestRequestTypeDef",
     "DistributionConfigurationTypeDef",
-    "DistributionUnionTypeDef",
+    "UpdateDistributionConfigurationRequestRequestTypeDef",
     "GetInfrastructureConfigurationResponseTypeDef",
     "ListImageBuildVersionsResponseTypeDef",
     "ListImagePipelineImagesResponseTypeDef",
     "ListImageScanFindingsResponseTypeDef",
     "GetContainerRecipeResponseTypeDef",
     "GetDistributionConfigurationResponseTypeDef",
     "ImageTypeDef",
-    "CreateDistributionConfigurationRequestRequestTypeDef",
-    "UpdateDistributionConfigurationRequestRequestTypeDef",
     "GetImageResponseTypeDef",
 )
 
 SeverityCountsTypeDef = TypedDict(
     "SeverityCountsTypeDef",
     {
         "all": int,
@@ -251,25 +238,14 @@
     "SystemsManagerAgentTypeDef",
     {
         "uninstallAfterBuild": bool,
     },
     total=False,
 )
 
-LaunchPermissionConfigurationOutputTypeDef = TypedDict(
-    "LaunchPermissionConfigurationOutputTypeDef",
-    {
-        "userIds": List[str],
-        "userGroups": List[str],
-        "organizationArns": List[str],
-        "organizationalUnitArns": List[str],
-    },
-    total=False,
-)
-
 LaunchPermissionConfigurationTypeDef = TypedDict(
     "LaunchPermissionConfigurationTypeDef",
     {
         "userIds": Sequence[str],
         "userGroups": Sequence[str],
         "organizationArns": Sequence[str],
         "organizationalUnitArns": Sequence[str],
@@ -301,22 +277,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-ComponentParameterOutputTypeDef = TypedDict(
-    "ComponentParameterOutputTypeDef",
-    {
-        "name": str,
-        "value": List[str],
-    },
-)
-
 ComponentParameterTypeDef = TypedDict(
     "ComponentParameterTypeDef",
     {
         "name": str,
         "value": Sequence[str],
     },
 )
@@ -590,23 +558,14 @@
         "volumeSize": int,
         "volumeType": EbsVolumeTypeType,
         "throughput": int,
     },
     total=False,
 )
 
-EcrConfigurationOutputTypeDef = TypedDict(
-    "EcrConfigurationOutputTypeDef",
-    {
-        "repositoryName": str,
-        "containerTags": List[str],
-    },
-    total=False,
-)
-
 EcrConfigurationTypeDef = TypedDict(
     "EcrConfigurationTypeDef",
     {
         "repositoryName": str,
         "containerTags": Sequence[str],
     },
     total=False,
@@ -1116,27 +1075,14 @@
     {
         "systemsManagerAgent": SystemsManagerAgentTypeDef,
         "userDataOverride": str,
     },
     total=False,
 )
 
-AmiDistributionConfigurationOutputTypeDef = TypedDict(
-    "AmiDistributionConfigurationOutputTypeDef",
-    {
-        "name": str,
-        "description": str,
-        "targetAccountIds": List[str],
-        "amiTags": Dict[str, str],
-        "kmsKeyId": str,
-        "launchPermission": LaunchPermissionConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 AmiDistributionConfigurationTypeDef = TypedDict(
     "AmiDistributionConfigurationTypeDef",
     {
         "name": str,
         "description": str,
         "targetAccountIds": Sequence[str],
         "amiTags": Mapping[str, str],
@@ -1482,33 +1428,14 @@
         "requestId": str,
         "clientToken": str,
         "infrastructureConfigurationArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredComponentConfigurationOutputTypeDef = TypedDict(
-    "_RequiredComponentConfigurationOutputTypeDef",
-    {
-        "componentArn": str,
-    },
-)
-_OptionalComponentConfigurationOutputTypeDef = TypedDict(
-    "_OptionalComponentConfigurationOutputTypeDef",
-    {
-        "parameters": List[ComponentParameterOutputTypeDef],
-    },
-    total=False,
-)
-
-class ComponentConfigurationOutputTypeDef(
-    _RequiredComponentConfigurationOutputTypeDef, _OptionalComponentConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredComponentConfigurationTypeDef = TypedDict(
     "_RequiredComponentConfigurationTypeDef",
     {
         "componentArn": str,
     },
 )
 _OptionalComponentConfigurationTypeDef = TypedDict(
@@ -1576,35 +1503,14 @@
         "requestId": str,
         "componentVersionList": List[ComponentVersionTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredContainerDistributionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredContainerDistributionConfigurationOutputTypeDef",
-    {
-        "targetRepository": TargetContainerRepositoryTypeDef,
-    },
-)
-_OptionalContainerDistributionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalContainerDistributionConfigurationOutputTypeDef",
-    {
-        "description": str,
-        "containerTags": List[str],
-    },
-    total=False,
-)
-
-class ContainerDistributionConfigurationOutputTypeDef(
-    _RequiredContainerDistributionConfigurationOutputTypeDef,
-    _OptionalContainerDistributionConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredContainerDistributionConfigurationTypeDef = TypedDict(
     "_RequiredContainerDistributionConfigurationTypeDef",
     {
         "targetRepository": TargetContainerRepositoryTypeDef,
     },
 )
 _OptionalContainerDistributionConfigurationTypeDef = TypedDict(
@@ -1662,23 +1568,14 @@
         "ebs": EbsInstanceBlockDeviceSpecificationTypeDef,
         "virtualName": str,
         "noDevice": str,
     },
     total=False,
 )
 
-ImageScanningConfigurationOutputTypeDef = TypedDict(
-    "ImageScanningConfigurationOutputTypeDef",
-    {
-        "imageScanningEnabled": bool,
-        "ecrConfiguration": EcrConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ImageScanningConfigurationTypeDef = TypedDict(
     "ImageScanningConfigurationTypeDef",
     {
         "imageScanningEnabled": bool,
         "ecrConfiguration": EcrConfigurationTypeDef,
     },
     total=False,
@@ -1971,17 +1868,14 @@
     {
         "amis": List[AmiTypeDef],
         "containers": List[ContainerTypeDef],
     },
     total=False,
 )
 
-ComponentConfigurationUnionTypeDef = Union[
-    ComponentConfigurationTypeDef, ComponentConfigurationOutputTypeDef
-]
 ListComponentBuildVersionsResponseTypeDef = TypedDict(
     "ListComponentBuildVersionsResponseTypeDef",
     {
         "requestId": str,
         "componentSummaryList": List[ComponentSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2001,78 +1895,71 @@
     "InspectorScoreDetailsTypeDef",
     {
         "adjustedCvss": CvssScoreDetailsTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImageRecipeRequestRequestTypeDef",
+    {
+        "name": str,
+        "semanticVersion": str,
+        "components": Sequence[ComponentConfigurationTypeDef],
+        "parentImage": str,
+        "clientToken": str,
+    },
+)
+_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImageRecipeRequestRequestTypeDef",
+    {
+        "description": str,
+        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
+        "tags": Mapping[str, str],
+        "workingDirectory": str,
+        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class CreateImageRecipeRequestRequestTypeDef(
+    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
+):
+    pass
+
 ImageRecipeTypeDef = TypedDict(
     "ImageRecipeTypeDef",
     {
         "arn": str,
         "type": ImageTypeType,
         "name": str,
         "description": str,
         "platform": PlatformType,
         "owner": str,
         "version": str,
-        "components": List[ComponentConfigurationOutputTypeDef],
+        "components": List[ComponentConfigurationTypeDef],
         "parentImage": str,
         "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
         "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
     },
     total=False,
 )
 
-InstanceConfigurationOutputTypeDef = TypedDict(
-    "InstanceConfigurationOutputTypeDef",
-    {
-        "image": str,
-        "blockDeviceMappings": List[InstanceBlockDeviceMappingTypeDef],
-    },
-    total=False,
-)
-
 InstanceConfigurationTypeDef = TypedDict(
     "InstanceConfigurationTypeDef",
     {
         "image": str,
         "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
     },
     total=False,
 )
 
-ImagePipelineTypeDef = TypedDict(
-    "ImagePipelineTypeDef",
-    {
-        "arn": str,
-        "name": str,
-        "description": str,
-        "platform": PlatformType,
-        "enhancedImageMetadataEnabled": bool,
-        "imageRecipeArn": str,
-        "containerRecipeArn": str,
-        "infrastructureConfigurationArn": str,
-        "distributionConfigurationArn": str,
-        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
-        "schedule": ScheduleTypeDef,
-        "status": PipelineStatusType,
-        "dateCreated": str,
-        "dateUpdated": str,
-        "dateLastRun": str,
-        "dateNextRun": str,
-        "tags": Dict[str, str],
-        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateImagePipelineRequestRequestTypeDef",
     {
         "name": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2122,17 +2009,39 @@
 )
 
 class CreateImageRequestRequestTypeDef(
     _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
 ):
     pass
 
-ImageScanningConfigurationUnionTypeDef = Union[
-    ImageScanningConfigurationTypeDef, ImageScanningConfigurationOutputTypeDef
-]
+ImagePipelineTypeDef = TypedDict(
+    "ImagePipelineTypeDef",
+    {
+        "arn": str,
+        "name": str,
+        "description": str,
+        "platform": PlatformType,
+        "enhancedImageMetadataEnabled": bool,
+        "imageRecipeArn": str,
+        "containerRecipeArn": str,
+        "infrastructureConfigurationArn": str,
+        "distributionConfigurationArn": str,
+        "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
+        "schedule": ScheduleTypeDef,
+        "status": PipelineStatusType,
+        "dateCreated": str,
+        "dateUpdated": str,
+        "dateLastRun": str,
+        "dateNextRun": str,
+        "tags": Dict[str, str],
+        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateImagePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateImagePipelineRequestRequestTypeDef",
     {
         "imagePipelineArn": str,
         "infrastructureConfigurationArn": str,
         "clientToken": str,
     },
@@ -2155,38 +2064,14 @@
 
 class UpdateImagePipelineRequestRequestTypeDef(
     _RequiredUpdateImagePipelineRequestRequestTypeDef,
     _OptionalUpdateImagePipelineRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDistributionOutputTypeDef = TypedDict(
-    "_RequiredDistributionOutputTypeDef",
-    {
-        "region": str,
-    },
-)
-_OptionalDistributionOutputTypeDef = TypedDict(
-    "_OptionalDistributionOutputTypeDef",
-    {
-        "amiDistributionConfiguration": AmiDistributionConfigurationOutputTypeDef,
-        "containerDistributionConfiguration": ContainerDistributionConfigurationOutputTypeDef,
-        "licenseConfigurationArns": List[str],
-        "launchTemplateConfigurations": List[LaunchTemplateConfigurationTypeDef],
-        "s3ExportConfiguration": S3ExportConfigurationTypeDef,
-        "fastLaunchConfigurations": List[FastLaunchConfigurationTypeDef],
-    },
-    total=False,
-)
-
-class DistributionOutputTypeDef(
-    _RequiredDistributionOutputTypeDef, _OptionalDistributionOutputTypeDef
-):
-    pass
-
 _RequiredDistributionTypeDef = TypedDict(
     "_RequiredDistributionTypeDef",
     {
         "region": str,
     },
 )
 _OptionalDistributionTypeDef = TypedDict(
@@ -2318,41 +2203,14 @@
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
     },
     total=False,
 )
 
-_RequiredCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImageRecipeRequestRequestTypeDef",
-    {
-        "name": str,
-        "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationUnionTypeDef],
-        "parentImage": str,
-        "clientToken": str,
-    },
-)
-_OptionalCreateImageRecipeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImageRecipeRequestRequestTypeDef",
-    {
-        "description": str,
-        "blockDeviceMappings": Sequence[InstanceBlockDeviceMappingTypeDef],
-        "tags": Mapping[str, str],
-        "workingDirectory": str,
-        "additionalInstanceConfiguration": AdditionalInstanceConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class CreateImageRecipeRequestRequestTypeDef(
-    _RequiredCreateImageRecipeRequestRequestTypeDef, _OptionalCreateImageRecipeRequestRequestTypeDef
-):
-    pass
-
 ImageScanFindingTypeDef = TypedDict(
     "ImageScanFindingTypeDef",
     {
         "awsAccountId": str,
         "imageBuildVersionArn": str,
         "imagePipelineArn": str,
         "type": str,
@@ -2385,16 +2243,16 @@
         "arn": str,
         "containerType": Literal["DOCKER"],
         "name": str,
         "description": str,
         "platform": PlatformType,
         "owner": str,
         "version": str,
-        "components": List[ComponentConfigurationOutputTypeDef],
-        "instanceConfiguration": InstanceConfigurationOutputTypeDef,
+        "components": List[ComponentConfigurationTypeDef],
+        "instanceConfiguration": InstanceConfigurationTypeDef,
         "dockerfileTemplateData": str,
         "kmsKeyId": str,
         "encrypted": bool,
         "parentImage": str,
         "dateCreated": str,
         "tags": Dict[str, str],
         "workingDirectory": str,
@@ -2405,15 +2263,15 @@
 
 _RequiredCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerRecipeRequestRequestTypeDef",
     {
         "containerType": Literal["DOCKER"],
         "name": str,
         "semanticVersion": str,
-        "components": Sequence[ComponentConfigurationUnionTypeDef],
+        "components": Sequence[ComponentConfigurationTypeDef],
         "parentImage": str,
         "targetRepository": TargetContainerRepositoryTypeDef,
         "clientToken": str,
     },
 )
 _OptionalCreateContainerRecipeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerRecipeRequestRequestTypeDef",
@@ -2433,17 +2291,14 @@
 
 class CreateContainerRecipeRequestRequestTypeDef(
     _RequiredCreateContainerRecipeRequestRequestTypeDef,
     _OptionalCreateContainerRecipeRequestRequestTypeDef,
 ):
     pass
 
-InstanceConfigurationUnionTypeDef = Union[
-    InstanceConfigurationTypeDef, InstanceConfigurationOutputTypeDef
-]
 GetImagePipelineResponseTypeDef = TypedDict(
     "GetImagePipelineResponseTypeDef",
     {
         "requestId": str,
         "imagePipeline": ImagePipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2455,40 +2310,84 @@
         "requestId": str,
         "imagePipelineList": List[ImagePipelineTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "distributions": Sequence[DistributionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
 _RequiredDistributionConfigurationTypeDef = TypedDict(
     "_RequiredDistributionConfigurationTypeDef",
     {
         "timeoutMinutes": int,
     },
 )
 _OptionalDistributionConfigurationTypeDef = TypedDict(
     "_OptionalDistributionConfigurationTypeDef",
     {
         "arn": str,
         "name": str,
         "description": str,
-        "distributions": List[DistributionOutputTypeDef],
+        "distributions": List[DistributionTypeDef],
         "dateCreated": str,
         "dateUpdated": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class DistributionConfigurationTypeDef(
     _RequiredDistributionConfigurationTypeDef, _OptionalDistributionConfigurationTypeDef
 ):
     pass
 
-DistributionUnionTypeDef = Union[DistributionTypeDef, DistributionOutputTypeDef]
+_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "distributionConfigurationArn": str,
+        "distributions": Sequence[DistributionTypeDef],
+        "clientToken": str,
+    },
+)
+_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
+    {
+        "description": str,
+    },
+    total=False,
+)
+
+class UpdateDistributionConfigurationRequestRequestTypeDef(
+    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
+    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
+):
+    pass
+
 GetInfrastructureConfigurationResponseTypeDef = TypedDict(
     "GetInfrastructureConfigurationResponseTypeDef",
     {
         "requestId": str,
         "infrastructureConfiguration": InfrastructureConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2562,64 +2461,19 @@
         "imageTestsConfiguration": ImageTestsConfigurationTypeDef,
         "dateCreated": str,
         "outputResources": OutputResourcesTypeDef,
         "tags": Dict[str, str],
         "buildType": BuildTypeType,
         "imageSource": ImageSourceType,
         "scanState": ImageScanStateTypeDef,
-        "imageScanningConfiguration": ImageScanningConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "distributions": Sequence[DistributionUnionTypeDef],
-        "clientToken": str,
-    },
-)
-_OptionalCreateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredCreateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalCreateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "distributionConfigurationArn": str,
-        "distributions": Sequence[DistributionUnionTypeDef],
-        "clientToken": str,
-    },
-)
-_OptionalUpdateDistributionConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDistributionConfigurationRequestRequestTypeDef",
-    {
-        "description": str,
+        "imageScanningConfiguration": ImageScanningConfigurationTypeDef,
     },
     total=False,
 )
 
-class UpdateDistributionConfigurationRequestRequestTypeDef(
-    _RequiredUpdateDistributionConfigurationRequestRequestTypeDef,
-    _OptionalUpdateDistributionConfigurationRequestRequestTypeDef,
-):
-    pass
-
 GetImageResponseTypeDef = TypedDict(
     "GetImageResponseTypeDef",
     {
         "requestId": str,
         "image": ImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-imagebuilder-2.5.2.post1/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt` & `types-aiobotocore-imagebuilder-2.5.2.post2/types_aiobotocore_imagebuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

