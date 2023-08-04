# Comparing `tmp/types-aiobotocore-greengrassv2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-greengrassv2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-greengrassv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-greengrassv2-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:58 2023, max compression
```

## Comparing `types-aiobotocore-greengrassv2-2.5.2.post1.tar` & `types-aiobotocore-greengrassv2-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.689576 types-aiobotocore-greengrassv2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19779 2023-08-02 14:52:21.685576 types-aiobotocore-greengrassv2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18241 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:21.689576 types-aiobotocore-greengrassv2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.677576 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27468 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27423 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39124 2023-08-02 14:39:45.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39091 2023-08-02 14:39:45.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:44.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.685576 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19779 2023-08-02 14:52:21.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:21.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:21.000000 types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.512366 types-aiobotocore-greengrassv2-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:47:14.000000 types-aiobotocore-greengrassv2-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-08-04 12:00:58.512366 types-aiobotocore-greengrassv2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12791 2023-08-04 11:47:14.000000 types-aiobotocore-greengrassv2-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:58.512366 types-aiobotocore-greengrassv2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:47:14.000000 types-aiobotocore-greengrassv2-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.508366 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-04 11:47:15.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-08-04 11:47:14.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:47:15.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27438 2023-08-04 11:47:16.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27393 2023-08-04 11:47:15.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-08-04 11:47:16.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-08-04 11:47:16.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-08-04 11:47:16.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-08-04 11:47:16.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:47:15.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37212 2023-08-04 11:47:17.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-08-04 11:47:16.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:47:14.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:58.512366 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-08-04 12:00:58.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:00:58.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:58.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:58.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:58.000000 types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/LICENSE` & `types-aiobotocore-greengrassv2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/setup.py` & `types-aiobotocore-greengrassv2-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-greengrassv2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_greengrassv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.GreengrassV2 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/__init__.py` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/__init__.pyi` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/__main__.py` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GreengrassV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.GreengrassV2 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2\nOther"
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

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/client.py` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,20 +40,20 @@
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     BlobTypeDef,
     CancelDeploymentResponseTypeDef,
     ComponentCandidateTypeDef,
-    ComponentDeploymentSpecificationUnionTypeDef,
-    ComponentPlatformUnionTypeDef,
+    ComponentDeploymentSpecificationTypeDef,
+    ComponentPlatformTypeDef,
     ConnectivityInfoTypeDef,
     CreateComponentVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
-    DeploymentIoTJobConfigurationUnionTypeDef,
+    DeploymentIoTJobConfigurationTypeDef,
     DeploymentPoliciesTypeDef,
     DescribeComponentResponseTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComponentResponseTypeDef,
     GetComponentVersionArtifactResponseTypeDef,
@@ -197,16 +197,16 @@
         """
 
     async def create_deployment(
         self,
         *,
         targetArn: str,
         deploymentName: str = ...,
-        components: Mapping[str, ComponentDeploymentSpecificationUnionTypeDef] = ...,
-        iotJobConfiguration: DeploymentIoTJobConfigurationUnionTypeDef = ...,
+        components: Mapping[str, ComponentDeploymentSpecificationTypeDef] = ...,
+        iotJobConfiguration: DeploymentIoTJobConfigurationTypeDef = ...,
         deploymentPolicies: DeploymentPoliciesTypeDef = ...,
         parentTargetArn: str = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates a continuous deployment for a target, which is a Greengrass core device
@@ -427,15 +427,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_tags_for_resource)
         """
 
     async def resolve_component_candidates(
         self,
         *,
-        platform: ComponentPlatformUnionTypeDef = ...,
+        platform: ComponentPlatformTypeDef = ...,
         componentCandidates: Sequence[ComponentCandidateTypeDef] = ...
     ) -> ResolveComponentCandidatesResponseTypeDef:
         """
         Retrieves a list of components that meet the component, version, and platform
         requirements of a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.resolve_component_candidates)
```

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/client.pyi` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,20 +40,20 @@
     AssociateClientDeviceWithCoreDeviceEntryTypeDef,
     AssociateServiceRoleToAccountResponseTypeDef,
     BatchAssociateClientDeviceWithCoreDeviceResponseTypeDef,
     BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef,
     BlobTypeDef,
     CancelDeploymentResponseTypeDef,
     ComponentCandidateTypeDef,
-    ComponentDeploymentSpecificationUnionTypeDef,
-    ComponentPlatformUnionTypeDef,
+    ComponentDeploymentSpecificationTypeDef,
+    ComponentPlatformTypeDef,
     ConnectivityInfoTypeDef,
     CreateComponentVersionResponseTypeDef,
     CreateDeploymentResponseTypeDef,
-    DeploymentIoTJobConfigurationUnionTypeDef,
+    DeploymentIoTJobConfigurationTypeDef,
     DeploymentPoliciesTypeDef,
     DescribeComponentResponseTypeDef,
     DisassociateClientDeviceFromCoreDeviceEntryTypeDef,
     DisassociateServiceRoleFromAccountResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetComponentResponseTypeDef,
     GetComponentVersionArtifactResponseTypeDef,
@@ -185,16 +185,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#create_component_version)
         """
     async def create_deployment(
         self,
         *,
         targetArn: str,
         deploymentName: str = ...,
-        components: Mapping[str, ComponentDeploymentSpecificationUnionTypeDef] = ...,
-        iotJobConfiguration: DeploymentIoTJobConfigurationUnionTypeDef = ...,
+        components: Mapping[str, ComponentDeploymentSpecificationTypeDef] = ...,
+        iotJobConfiguration: DeploymentIoTJobConfigurationTypeDef = ...,
         deploymentPolicies: DeploymentPoliciesTypeDef = ...,
         parentTargetArn: str = ...,
         tags: Mapping[str, str] = ...,
         clientToken: str = ...
     ) -> CreateDeploymentResponseTypeDef:
         """
         Creates a continuous deployment for a target, which is a Greengrass core device
@@ -394,15 +394,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_greengrassv2/client/#list_tags_for_resource)
         """
     async def resolve_component_candidates(
         self,
         *,
-        platform: ComponentPlatformUnionTypeDef = ...,
+        platform: ComponentPlatformTypeDef = ...,
         componentCandidates: Sequence[ComponentCandidateTypeDef] = ...
     ) -> ResolveComponentCandidatesResponseTypeDef:
         """
         Retrieves a list of components that meet the component, version, and platform
         requirements of a deployment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Client.resolve_component_candidates)
```

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/literals.py` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/literals.pyi` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/paginator.py` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/paginator.pyi` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/type_defs.py` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,18 +56,16 @@
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
     "BlobTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
-    "ComponentConfigurationUpdateOutputTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
-    "ComponentPlatformOutputTypeDef",
     "ComponentPlatformTypeDef",
     "SystemResourceLimitsTypeDef",
     "ComponentVersionListItemTypeDef",
     "ConnectivityInfoTypeDef",
     "CoreDeviceTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteCoreDeviceRequestRequestTypeDef",
@@ -116,51 +114,45 @@
     "UpdateConnectivityInfoResponseTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
-    "ComponentPlatformUnionTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
     "ComponentRunWithTypeDef",
     "ListComponentVersionsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ListCoreDevicesResponseTypeDef",
     "DeploymentPoliciesTypeDef",
     "ListDeploymentsResponseTypeDef",
     "EffectiveDeploymentTypeDef",
     "ListInstalledComponentsResponseTypeDef",
-    "IoTJobAbortConfigOutputTypeDef",
     "IoTJobAbortConfigTypeDef",
     "IoTJobExponentialRolloutRateTypeDef",
     "LambdaContainerParamsTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
     "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
     "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ResolveComponentCandidatesResponseTypeDef",
     "ComponentTypeDef",
-    "ComponentDeploymentSpecificationOutputTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
     "ListComponentsResponseTypeDef",
-    "ComponentDeploymentSpecificationUnionTypeDef",
-    "DeploymentIoTJobConfigurationOutputTypeDef",
     "DeploymentIoTJobConfigurationTypeDef",
     "LambdaExecutionParametersTypeDef",
-    "GetDeploymentResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "DeploymentIoTJobConfigurationUnionTypeDef",
+    "GetDeploymentResponseTypeDef",
     "LambdaFunctionRecipeSourceTypeDef",
     "CreateComponentVersionRequestRequestTypeDef",
 )
 
 AssociateClientDeviceWithCoreDeviceEntryTypeDef = TypedDict(
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     {
@@ -248,23 +240,14 @@
         "componentName": str,
         "componentVersion": str,
         "versionRequirements": Mapping[str, str],
     },
     total=False,
 )
 
-ComponentConfigurationUpdateOutputTypeDef = TypedDict(
-    "ComponentConfigurationUpdateOutputTypeDef",
-    {
-        "merge": str,
-        "reset": List[str],
-    },
-    total=False,
-)
-
 ComponentConfigurationUpdateTypeDef = TypedDict(
     "ComponentConfigurationUpdateTypeDef",
     {
         "merge": str,
         "reset": Sequence[str],
     },
     total=False,
@@ -275,23 +258,14 @@
     {
         "versionRequirement": str,
         "dependencyType": ComponentDependencyTypeType,
     },
     total=False,
 )
 
-ComponentPlatformOutputTypeDef = TypedDict(
-    "ComponentPlatformOutputTypeDef",
-    {
-        "name": str,
-        "attributes": Dict[str, str],
-    },
-    total=False,
-)
-
 ComponentPlatformTypeDef = TypedDict(
     "ComponentPlatformTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
     total=False,
@@ -908,36 +882,35 @@
     "ComponentLatestVersionTypeDef",
     {
         "arn": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "description": str,
         "publisher": str,
-        "platforms": List[ComponentPlatformOutputTypeDef],
+        "platforms": List[ComponentPlatformTypeDef],
     },
     total=False,
 )
 
 DescribeComponentResponseTypeDef = TypedDict(
     "DescribeComponentResponseTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "publisher": str,
         "description": str,
         "status": CloudComponentStatusTypeDef,
-        "platforms": List[ComponentPlatformOutputTypeDef],
+        "platforms": List[ComponentPlatformTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ComponentPlatformUnionTypeDef = Union[ComponentPlatformTypeDef, ComponentPlatformOutputTypeDef]
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": ComponentPlatformTypeDef,
         "componentCandidates": Sequence[ComponentCandidateTypeDef],
     },
     total=False,
@@ -1042,21 +1015,14 @@
     {
         "installedComponents": List[InstalledComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IoTJobAbortConfigOutputTypeDef = TypedDict(
-    "IoTJobAbortConfigOutputTypeDef",
-    {
-        "criteriaList": List[IoTJobAbortCriteriaTypeDef],
-    },
-)
-
 IoTJobAbortConfigTypeDef = TypedDict(
     "IoTJobAbortConfigTypeDef",
     {
         "criteriaList": Sequence[IoTJobAbortCriteriaTypeDef],
     },
 )
 
@@ -1213,24 +1179,14 @@
         "arn": str,
         "componentName": str,
         "latestVersion": ComponentLatestVersionTypeDef,
     },
     total=False,
 )
 
-ComponentDeploymentSpecificationOutputTypeDef = TypedDict(
-    "ComponentDeploymentSpecificationOutputTypeDef",
-    {
-        "componentVersion": str,
-        "configurationUpdate": ComponentConfigurationUpdateOutputTypeDef,
-        "runWith": ComponentRunWithTypeDef,
-    },
-    total=False,
-)
-
 ComponentDeploymentSpecificationTypeDef = TypedDict(
     "ComponentDeploymentSpecificationTypeDef",
     {
         "componentVersion": str,
         "configurationUpdate": ComponentConfigurationUpdateTypeDef,
         "runWith": ComponentRunWithTypeDef,
     },
@@ -1269,27 +1225,14 @@
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ComponentDeploymentSpecificationUnionTypeDef = Union[
-    ComponentDeploymentSpecificationTypeDef, ComponentDeploymentSpecificationOutputTypeDef
-]
-DeploymentIoTJobConfigurationOutputTypeDef = TypedDict(
-    "DeploymentIoTJobConfigurationOutputTypeDef",
-    {
-        "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
-        "abortConfig": IoTJobAbortConfigOutputTypeDef,
-        "timeoutConfig": IoTJobTimeoutConfigTypeDef,
-    },
-    total=False,
-)
-
 DeploymentIoTJobConfigurationTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationTypeDef",
     {
         "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
         "abortConfig": IoTJobAbortConfigTypeDef,
         "timeoutConfig": IoTJobTimeoutConfigTypeDef,
     },
@@ -1310,46 +1253,25 @@
         "execArgs": Sequence[str],
         "environmentVariables": Mapping[str, str],
         "linuxProcessParams": LambdaLinuxProcessParamsTypeDef,
     },
     total=False,
 )
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "targetArn": str,
-        "revisionId": str,
-        "deploymentId": str,
-        "deploymentName": str,
-        "deploymentStatus": DeploymentStatusType,
-        "iotJobId": str,
-        "iotJobArn": str,
-        "components": Dict[str, ComponentDeploymentSpecificationOutputTypeDef],
-        "deploymentPolicies": DeploymentPoliciesTypeDef,
-        "iotJobConfiguration": DeploymentIoTJobConfigurationOutputTypeDef,
-        "creationTimestamp": datetime,
-        "isLatestForTarget": bool,
-        "parentTargetArn": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "targetArn": str,
     },
 )
 _OptionalCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDeploymentRequestRequestTypeDef",
     {
         "deploymentName": str,
-        "components": Mapping[str, ComponentDeploymentSpecificationUnionTypeDef],
+        "components": Mapping[str, ComponentDeploymentSpecificationTypeDef],
         "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
         "deploymentPolicies": DeploymentPoliciesTypeDef,
         "parentTargetArn": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
@@ -1358,17 +1280,35 @@
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
 
-DeploymentIoTJobConfigurationUnionTypeDef = Union[
-    DeploymentIoTJobConfigurationTypeDef, DeploymentIoTJobConfigurationOutputTypeDef
-]
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "targetArn": str,
+        "revisionId": str,
+        "deploymentId": str,
+        "deploymentName": str,
+        "deploymentStatus": DeploymentStatusType,
+        "iotJobId": str,
+        "iotJobArn": str,
+        "components": Dict[str, ComponentDeploymentSpecificationTypeDef],
+        "deploymentPolicies": DeploymentPoliciesTypeDef,
+        "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
+        "creationTimestamp": datetime,
+        "isLatestForTarget": bool,
+        "parentTargetArn": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredLambdaFunctionRecipeSourceTypeDef = TypedDict(
     "_RequiredLambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
     },
 )
 _OptionalLambdaFunctionRecipeSourceTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2/type_defs.pyi` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -55,18 +55,16 @@
     "AssociatedClientDeviceTypeDef",
     "DisassociateClientDeviceFromCoreDeviceEntryTypeDef",
     "DisassociateClientDeviceFromCoreDeviceErrorEntryTypeDef",
     "BlobTypeDef",
     "CancelDeploymentRequestRequestTypeDef",
     "CloudComponentStatusTypeDef",
     "ComponentCandidateTypeDef",
-    "ComponentConfigurationUpdateOutputTypeDef",
     "ComponentConfigurationUpdateTypeDef",
     "ComponentDependencyRequirementTypeDef",
-    "ComponentPlatformOutputTypeDef",
     "ComponentPlatformTypeDef",
     "SystemResourceLimitsTypeDef",
     "ComponentVersionListItemTypeDef",
     "ConnectivityInfoTypeDef",
     "CoreDeviceTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteCoreDeviceRequestRequestTypeDef",
@@ -115,51 +113,45 @@
     "UpdateConnectivityInfoResponseTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceRequestRequestTypeDef",
     "BatchDisassociateClientDeviceFromCoreDeviceResponseTypeDef",
     "CreateComponentVersionResponseTypeDef",
     "ComponentLatestVersionTypeDef",
     "DescribeComponentResponseTypeDef",
-    "ComponentPlatformUnionTypeDef",
     "ResolveComponentCandidatesRequestRequestTypeDef",
     "ComponentRunWithTypeDef",
     "ListComponentVersionsResponseTypeDef",
     "GetConnectivityInfoResponseTypeDef",
     "UpdateConnectivityInfoRequestRequestTypeDef",
     "ListCoreDevicesResponseTypeDef",
     "DeploymentPoliciesTypeDef",
     "ListDeploymentsResponseTypeDef",
     "EffectiveDeploymentTypeDef",
     "ListInstalledComponentsResponseTypeDef",
-    "IoTJobAbortConfigOutputTypeDef",
     "IoTJobAbortConfigTypeDef",
     "IoTJobExponentialRolloutRateTypeDef",
     "LambdaContainerParamsTypeDef",
     "ListClientDevicesAssociatedWithCoreDeviceRequestListClientDevicesAssociatedWithCoreDevicePaginateTypeDef",
     "ListComponentVersionsRequestListComponentVersionsPaginateTypeDef",
     "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListCoreDevicesRequestListCoreDevicesPaginateTypeDef",
     "ListDeploymentsRequestListDeploymentsPaginateTypeDef",
     "ListEffectiveDeploymentsRequestListEffectiveDeploymentsPaginateTypeDef",
     "ListInstalledComponentsRequestListInstalledComponentsPaginateTypeDef",
     "ResolveComponentCandidatesResponseTypeDef",
     "ComponentTypeDef",
-    "ComponentDeploymentSpecificationOutputTypeDef",
     "ComponentDeploymentSpecificationTypeDef",
     "ListEffectiveDeploymentsResponseTypeDef",
     "IoTJobExecutionsRolloutConfigTypeDef",
     "LambdaLinuxProcessParamsTypeDef",
     "ListComponentsResponseTypeDef",
-    "ComponentDeploymentSpecificationUnionTypeDef",
-    "DeploymentIoTJobConfigurationOutputTypeDef",
     "DeploymentIoTJobConfigurationTypeDef",
     "LambdaExecutionParametersTypeDef",
-    "GetDeploymentResponseTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "DeploymentIoTJobConfigurationUnionTypeDef",
+    "GetDeploymentResponseTypeDef",
     "LambdaFunctionRecipeSourceTypeDef",
     "CreateComponentVersionRequestRequestTypeDef",
 )
 
 AssociateClientDeviceWithCoreDeviceEntryTypeDef = TypedDict(
     "AssociateClientDeviceWithCoreDeviceEntryTypeDef",
     {
@@ -247,23 +239,14 @@
         "componentName": str,
         "componentVersion": str,
         "versionRequirements": Mapping[str, str],
     },
     total=False,
 )
 
-ComponentConfigurationUpdateOutputTypeDef = TypedDict(
-    "ComponentConfigurationUpdateOutputTypeDef",
-    {
-        "merge": str,
-        "reset": List[str],
-    },
-    total=False,
-)
-
 ComponentConfigurationUpdateTypeDef = TypedDict(
     "ComponentConfigurationUpdateTypeDef",
     {
         "merge": str,
         "reset": Sequence[str],
     },
     total=False,
@@ -274,23 +257,14 @@
     {
         "versionRequirement": str,
         "dependencyType": ComponentDependencyTypeType,
     },
     total=False,
 )
 
-ComponentPlatformOutputTypeDef = TypedDict(
-    "ComponentPlatformOutputTypeDef",
-    {
-        "name": str,
-        "attributes": Dict[str, str],
-    },
-    total=False,
-)
-
 ComponentPlatformTypeDef = TypedDict(
     "ComponentPlatformTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
     total=False,
@@ -889,36 +863,35 @@
     "ComponentLatestVersionTypeDef",
     {
         "arn": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "description": str,
         "publisher": str,
-        "platforms": List[ComponentPlatformOutputTypeDef],
+        "platforms": List[ComponentPlatformTypeDef],
     },
     total=False,
 )
 
 DescribeComponentResponseTypeDef = TypedDict(
     "DescribeComponentResponseTypeDef",
     {
         "arn": str,
         "componentName": str,
         "componentVersion": str,
         "creationTimestamp": datetime,
         "publisher": str,
         "description": str,
         "status": CloudComponentStatusTypeDef,
-        "platforms": List[ComponentPlatformOutputTypeDef],
+        "platforms": List[ComponentPlatformTypeDef],
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ComponentPlatformUnionTypeDef = Union[ComponentPlatformTypeDef, ComponentPlatformOutputTypeDef]
 ResolveComponentCandidatesRequestRequestTypeDef = TypedDict(
     "ResolveComponentCandidatesRequestRequestTypeDef",
     {
         "platform": ComponentPlatformTypeDef,
         "componentCandidates": Sequence[ComponentCandidateTypeDef],
     },
     total=False,
@@ -1021,21 +994,14 @@
     {
         "installedComponents": List[InstalledComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IoTJobAbortConfigOutputTypeDef = TypedDict(
-    "IoTJobAbortConfigOutputTypeDef",
-    {
-        "criteriaList": List[IoTJobAbortCriteriaTypeDef],
-    },
-)
-
 IoTJobAbortConfigTypeDef = TypedDict(
     "IoTJobAbortConfigTypeDef",
     {
         "criteriaList": Sequence[IoTJobAbortCriteriaTypeDef],
     },
 )
 
@@ -1184,24 +1150,14 @@
         "arn": str,
         "componentName": str,
         "latestVersion": ComponentLatestVersionTypeDef,
     },
     total=False,
 )
 
-ComponentDeploymentSpecificationOutputTypeDef = TypedDict(
-    "ComponentDeploymentSpecificationOutputTypeDef",
-    {
-        "componentVersion": str,
-        "configurationUpdate": ComponentConfigurationUpdateOutputTypeDef,
-        "runWith": ComponentRunWithTypeDef,
-    },
-    total=False,
-)
-
 ComponentDeploymentSpecificationTypeDef = TypedDict(
     "ComponentDeploymentSpecificationTypeDef",
     {
         "componentVersion": str,
         "configurationUpdate": ComponentConfigurationUpdateTypeDef,
         "runWith": ComponentRunWithTypeDef,
     },
@@ -1240,27 +1196,14 @@
     {
         "components": List[ComponentTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ComponentDeploymentSpecificationUnionTypeDef = Union[
-    ComponentDeploymentSpecificationTypeDef, ComponentDeploymentSpecificationOutputTypeDef
-]
-DeploymentIoTJobConfigurationOutputTypeDef = TypedDict(
-    "DeploymentIoTJobConfigurationOutputTypeDef",
-    {
-        "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
-        "abortConfig": IoTJobAbortConfigOutputTypeDef,
-        "timeoutConfig": IoTJobTimeoutConfigTypeDef,
-    },
-    total=False,
-)
-
 DeploymentIoTJobConfigurationTypeDef = TypedDict(
     "DeploymentIoTJobConfigurationTypeDef",
     {
         "jobExecutionsRolloutConfig": IoTJobExecutionsRolloutConfigTypeDef,
         "abortConfig": IoTJobAbortConfigTypeDef,
         "timeoutConfig": IoTJobTimeoutConfigTypeDef,
     },
@@ -1281,63 +1224,60 @@
         "execArgs": Sequence[str],
         "environmentVariables": Mapping[str, str],
         "linuxProcessParams": LambdaLinuxProcessParamsTypeDef,
     },
     total=False,
 )
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "targetArn": str,
-        "revisionId": str,
-        "deploymentId": str,
-        "deploymentName": str,
-        "deploymentStatus": DeploymentStatusType,
-        "iotJobId": str,
-        "iotJobArn": str,
-        "components": Dict[str, ComponentDeploymentSpecificationOutputTypeDef],
-        "deploymentPolicies": DeploymentPoliciesTypeDef,
-        "iotJobConfiguration": DeploymentIoTJobConfigurationOutputTypeDef,
-        "creationTimestamp": datetime,
-        "isLatestForTarget": bool,
-        "parentTargetArn": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "targetArn": str,
     },
 )
 _OptionalCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDeploymentRequestRequestTypeDef",
     {
         "deploymentName": str,
-        "components": Mapping[str, ComponentDeploymentSpecificationUnionTypeDef],
+        "components": Mapping[str, ComponentDeploymentSpecificationTypeDef],
         "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
         "deploymentPolicies": DeploymentPoliciesTypeDef,
         "parentTargetArn": str,
         "tags": Mapping[str, str],
         "clientToken": str,
     },
     total=False,
 )
 
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-DeploymentIoTJobConfigurationUnionTypeDef = Union[
-    DeploymentIoTJobConfigurationTypeDef, DeploymentIoTJobConfigurationOutputTypeDef
-]
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "targetArn": str,
+        "revisionId": str,
+        "deploymentId": str,
+        "deploymentName": str,
+        "deploymentStatus": DeploymentStatusType,
+        "iotJobId": str,
+        "iotJobArn": str,
+        "components": Dict[str, ComponentDeploymentSpecificationTypeDef],
+        "deploymentPolicies": DeploymentPoliciesTypeDef,
+        "iotJobConfiguration": DeploymentIoTJobConfigurationTypeDef,
+        "creationTimestamp": datetime,
+        "isLatestForTarget": bool,
+        "parentTargetArn": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredLambdaFunctionRecipeSourceTypeDef = TypedDict(
     "_RequiredLambdaFunctionRecipeSourceTypeDef",
     {
         "lambdaArn": str,
     },
 )
 _OptionalLambdaFunctionRecipeSourceTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-greengrassv2-2.5.2.post1/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt` & `types-aiobotocore-greengrassv2-2.5.2.post2/types_aiobotocore_greengrassv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

