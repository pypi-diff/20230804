# Comparing `tmp/types-aiobotocore-eks-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-eks-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-eks-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-eks-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:50 2023, max compression
```

## Comparing `types-aiobotocore-eks-2.5.2.post1.tar` & `types-aiobotocore-eks-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.561594 types-aiobotocore-eks-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-08-02 14:52:14.557594 types-aiobotocore-eks-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.561594 types-aiobotocore-eks-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.557594 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35204 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-08-02 14:38:04.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52219 2023-08-02 14:38:06.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52146 2023-08-02 14:38:04.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-02 14:38:03.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.557594 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:14.000000 types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.244060 types-aiobotocore-eks-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:30.000000 types-aiobotocore-eks-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-08-04 12:00:50.244060 types-aiobotocore-eks-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-08-04 11:45:30.000000 types-aiobotocore-eks-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:50.244060 types-aiobotocore-eks-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:45:30.000000 types-aiobotocore-eks-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.244060 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-04 11:45:30.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-08-04 11:45:30.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:45:30.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35154 2023-08-04 11:45:31.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35095 2023-08-04 11:45:31.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14213 2023-08-04 11:45:31.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-04 11:45:31.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-04 11:45:31.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-08-04 11:45:31.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:30.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    50618 2023-08-04 11:45:34.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50545 2023-08-04 11:45:33.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:30.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-08-04 11:45:31.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-04 11:45:31.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.244060 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-08-04 12:00:50.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-04 12:00:50.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:50.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:50.000000 types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-eks-2.5.2.post1/LICENSE` & `types-aiobotocore-eks-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post1/setup.py` & `types-aiobotocore-eks-2.5.2.post2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-eks",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_eks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EKS 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__init__.py` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__init__.pyi` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/__main__.py` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EKS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.EKS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS\nOther"
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

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/client.py` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,33 +48,33 @@
     DescribeAddonVersionsResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
-    EncryptionConfigUnionTypeDef,
-    FargateProfileSelectorUnionTypeDef,
+    EncryptionConfigTypeDef,
+    FargateProfileSelectorTypeDef,
     IdentityProviderConfigTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesResponseTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesResponseTypeDef,
-    LoggingUnionTypeDef,
+    LoggingTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     OutpostConfigRequestTypeDef,
     RegisterClusterResponseTypeDef,
-    RemoteAccessConfigUnionTypeDef,
+    RemoteAccessConfigTypeDef,
     TaintTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
@@ -143,15 +143,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#exceptions)
         """
 
     async def associate_encryption_config(
         self,
         *,
         clusterName: str,
-        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef],
+        encryptionConfig: Sequence[EncryptionConfigTypeDef],
         clientRequestToken: str = ...
     ) -> AssociateEncryptionConfigResponseTypeDef:
         """
         Associate encryption configuration to an existing cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#associate_encryption_config)
@@ -211,18 +211,18 @@
         self,
         *,
         name: str,
         roleArn: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef,
         version: str = ...,
         kubernetesNetworkConfig: KubernetesNetworkConfigRequestTypeDef = ...,
-        logging: LoggingUnionTypeDef = ...,
+        logging: LoggingTypeDef = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef] = ...,
+        encryptionConfig: Sequence[EncryptionConfigTypeDef] = ...,
         outpostConfig: OutpostConfigRequestTypeDef = ...
     ) -> CreateClusterResponseTypeDef:
         """
         Creates an Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_cluster)
@@ -231,15 +231,15 @@
     async def create_fargate_profile(
         self,
         *,
         fargateProfileName: str,
         clusterName: str,
         podExecutionRoleArn: str,
         subnets: Sequence[str] = ...,
-        selectors: Sequence[FargateProfileSelectorUnionTypeDef] = ...,
+        selectors: Sequence[FargateProfileSelectorTypeDef] = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFargateProfileResponseTypeDef:
         """
         Creates an Fargate profile for your Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_fargate_profile)
@@ -253,15 +253,15 @@
         nodegroupName: str,
         subnets: Sequence[str],
         nodeRole: str,
         scalingConfig: NodegroupScalingConfigTypeDef = ...,
         diskSize: int = ...,
         instanceTypes: Sequence[str] = ...,
         amiType: AMITypesType = ...,
-        remoteAccess: RemoteAccessConfigUnionTypeDef = ...,
+        remoteAccess: RemoteAccessConfigTypeDef = ...,
         labels: Mapping[str, str] = ...,
         taints: Sequence[TaintTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientRequestToken: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
         capacityType: CapacityTypesType = ...,
@@ -566,15 +566,15 @@
         """
 
     async def update_cluster_config(
         self,
         *,
         name: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef = ...,
-        logging: LoggingUnionTypeDef = ...,
+        logging: LoggingTypeDef = ...,
         clientRequestToken: str = ...
     ) -> UpdateClusterConfigResponseTypeDef:
         """
         Updates an Amazon EKS cluster configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_cluster_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_cluster_config)
```

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/client.pyi` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -48,33 +48,33 @@
     DescribeAddonVersionsResponseTypeDef,
     DescribeClusterResponseTypeDef,
     DescribeFargateProfileResponseTypeDef,
     DescribeIdentityProviderConfigResponseTypeDef,
     DescribeNodegroupResponseTypeDef,
     DescribeUpdateResponseTypeDef,
     DisassociateIdentityProviderConfigResponseTypeDef,
-    EncryptionConfigUnionTypeDef,
-    FargateProfileSelectorUnionTypeDef,
+    EncryptionConfigTypeDef,
+    FargateProfileSelectorTypeDef,
     IdentityProviderConfigTypeDef,
     KubernetesNetworkConfigRequestTypeDef,
     LaunchTemplateSpecificationTypeDef,
     ListAddonsResponseTypeDef,
     ListClustersResponseTypeDef,
     ListFargateProfilesResponseTypeDef,
     ListIdentityProviderConfigsResponseTypeDef,
     ListNodegroupsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUpdatesResponseTypeDef,
-    LoggingUnionTypeDef,
+    LoggingTypeDef,
     NodegroupScalingConfigTypeDef,
     NodegroupUpdateConfigTypeDef,
     OidcIdentityProviderConfigRequestTypeDef,
     OutpostConfigRequestTypeDef,
     RegisterClusterResponseTypeDef,
-    RemoteAccessConfigUnionTypeDef,
+    RemoteAccessConfigTypeDef,
     TaintTypeDef,
     UpdateAddonResponseTypeDef,
     UpdateClusterConfigResponseTypeDef,
     UpdateClusterVersionResponseTypeDef,
     UpdateLabelsPayloadTypeDef,
     UpdateNodegroupConfigResponseTypeDef,
     UpdateNodegroupVersionResponseTypeDef,
@@ -138,15 +138,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#exceptions)
         """
     async def associate_encryption_config(
         self,
         *,
         clusterName: str,
-        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef],
+        encryptionConfig: Sequence[EncryptionConfigTypeDef],
         clientRequestToken: str = ...
     ) -> AssociateEncryptionConfigResponseTypeDef:
         """
         Associate encryption configuration to an existing cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.associate_encryption_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#associate_encryption_config)
@@ -201,18 +201,18 @@
         self,
         *,
         name: str,
         roleArn: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef,
         version: str = ...,
         kubernetesNetworkConfig: KubernetesNetworkConfigRequestTypeDef = ...,
-        logging: LoggingUnionTypeDef = ...,
+        logging: LoggingTypeDef = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...,
-        encryptionConfig: Sequence[EncryptionConfigUnionTypeDef] = ...,
+        encryptionConfig: Sequence[EncryptionConfigTypeDef] = ...,
         outpostConfig: OutpostConfigRequestTypeDef = ...
     ) -> CreateClusterResponseTypeDef:
         """
         Creates an Amazon EKS control plane.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#create_cluster)
@@ -220,15 +220,15 @@
     async def create_fargate_profile(
         self,
         *,
         fargateProfileName: str,
         clusterName: str,
         podExecutionRoleArn: str,
         subnets: Sequence[str] = ...,
-        selectors: Sequence[FargateProfileSelectorUnionTypeDef] = ...,
+        selectors: Sequence[FargateProfileSelectorTypeDef] = ...,
         clientRequestToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFargateProfileResponseTypeDef:
         """
         Creates an Fargate profile for your Amazon EKS cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.create_fargate_profile)
@@ -241,15 +241,15 @@
         nodegroupName: str,
         subnets: Sequence[str],
         nodeRole: str,
         scalingConfig: NodegroupScalingConfigTypeDef = ...,
         diskSize: int = ...,
         instanceTypes: Sequence[str] = ...,
         amiType: AMITypesType = ...,
-        remoteAccess: RemoteAccessConfigUnionTypeDef = ...,
+        remoteAccess: RemoteAccessConfigTypeDef = ...,
         labels: Mapping[str, str] = ...,
         taints: Sequence[TaintTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         clientRequestToken: str = ...,
         launchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         updateConfig: NodegroupUpdateConfigTypeDef = ...,
         capacityType: CapacityTypesType = ...,
@@ -527,15 +527,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_addon)
         """
     async def update_cluster_config(
         self,
         *,
         name: str,
         resourcesVpcConfig: VpcConfigRequestTypeDef = ...,
-        logging: LoggingUnionTypeDef = ...,
+        logging: LoggingTypeDef = ...,
         clientRequestToken: str = ...
     ) -> UpdateClusterConfigResponseTypeDef:
         """
         Updates an Amazon EKS cluster configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client.update_cluster_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_eks/client/#update_cluster_config)
```

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/literals.py` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/literals.pyi` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/paginator.py` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/paginator.pyi` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/type_defs.py` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_eks.type_defs import AddonIssueTypeDef
 
     data: AddonIssueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AddonIssueCodeType,
     AddonStatusType,
     AMITypesType,
     CapacityTypesType,
     ClusterIssueCodeType,
@@ -57,14 +57,15 @@
     "VpcConfigResponseTypeDef",
     "ConnectorConfigRequestTypeDef",
     "ControlPlanePlacementRequestTypeDef",
     "ControlPlanePlacementResponseTypeDef",
     "CreateAddonRequestRequestTypeDef",
     "KubernetesNetworkConfigRequestTypeDef",
     "VpcConfigRequestTypeDef",
+    "FargateProfileSelectorTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "NodegroupScalingConfigTypeDef",
     "NodegroupUpdateConfigTypeDef",
     "RemoteAccessConfigTypeDef",
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
@@ -79,29 +80,25 @@
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
-    "FargateProfileSelectorOutputTypeDef",
-    "FargateProfileSelectorTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
     "ListAddonsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
     "ListNodegroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUpdatesRequestRequestTypeDef",
-    "LogSetupOutputTypeDef",
     "LogSetupTypeDef",
-    "RemoteAccessConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddonRequestRequestTypeDef",
     "UpdateClusterVersionRequestRequestTypeDef",
     "UpdateLabelsPayloadTypeDef",
     "UpdateParamTypeDef",
     "AddonHealthTypeDef",
@@ -115,14 +112,16 @@
     "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
+    "CreateFargateProfileRequestRequestTypeDef",
+    "FargateProfileTypeDef",
     "UpdateNodegroupVersionRequestRequestTypeDef",
     "CreateNodegroupRequestRequestTypeDef",
     "UpdateTaintsPayloadTypeDef",
     "DescribeAddonRequestAddonActiveWaitTypeDef",
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
@@ -136,53 +135,45 @@
     "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
     "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
     "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
-    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
-    "FargateProfileTypeDef",
-    "FargateProfileSelectorUnionTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
-    "LoggingOutputTypeDef",
     "LoggingTypeDef",
-    "RemoteAccessConfigUnionTypeDef",
     "UpdateTypeDef",
     "AddonTypeDef",
     "AddonInfoTypeDef",
-    "UpdateNodegroupConfigRequestRequestTypeDef",
-    "EncryptionConfigUnionTypeDef",
     "CreateFargateProfileResponseTypeDef",
     "DeleteFargateProfileResponseTypeDef",
     "DescribeFargateProfileResponseTypeDef",
-    "CreateFargateProfileRequestRequestTypeDef",
+    "UpdateNodegroupConfigRequestRequestTypeDef",
+    "AssociateEncryptionConfigRequestRequestTypeDef",
     "DescribeIdentityProviderConfigResponseTypeDef",
     "NodegroupTypeDef",
     "ClusterTypeDef",
-    "LoggingUnionTypeDef",
+    "CreateClusterRequestRequestTypeDef",
     "UpdateClusterConfigRequestRequestTypeDef",
     "AssociateEncryptionConfigResponseTypeDef",
     "AssociateIdentityProviderConfigResponseTypeDef",
     "DescribeUpdateResponseTypeDef",
     "DisassociateIdentityProviderConfigResponseTypeDef",
     "UpdateAddonResponseTypeDef",
     "UpdateClusterConfigResponseTypeDef",
     "UpdateClusterVersionResponseTypeDef",
     "UpdateNodegroupConfigResponseTypeDef",
     "UpdateNodegroupVersionResponseTypeDef",
     "CreateAddonResponseTypeDef",
     "DeleteAddonResponseTypeDef",
     "DescribeAddonResponseTypeDef",
     "DescribeAddonVersionsResponseTypeDef",
-    "AssociateEncryptionConfigRequestRequestTypeDef",
-    "CreateClusterRequestRequestTypeDef",
     "CreateNodegroupResponseTypeDef",
     "DeleteNodegroupResponseTypeDef",
     "DescribeNodegroupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DeregisterClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
@@ -387,14 +378,23 @@
         "endpointPublicAccess": bool,
         "endpointPrivateAccess": bool,
         "publicAccessCidrs": Sequence[str],
     },
     total=False,
 )
 
+FargateProfileSelectorTypeDef = TypedDict(
+    "FargateProfileSelectorTypeDef",
+    {
+        "namespace": str,
+        "labels": Mapping[str, str],
+    },
+    total=False,
+)
+
 LaunchTemplateSpecificationTypeDef = TypedDict(
     "LaunchTemplateSpecificationTypeDef",
     {
         "name": str,
         "version": str,
         "id": str,
     },
@@ -608,32 +608,14 @@
         "errorCode": ErrorCodeType,
         "errorMessage": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
-FargateProfileSelectorOutputTypeDef = TypedDict(
-    "FargateProfileSelectorOutputTypeDef",
-    {
-        "namespace": str,
-        "labels": Dict[str, str],
-    },
-    total=False,
-)
-
-FargateProfileSelectorTypeDef = TypedDict(
-    "FargateProfileSelectorTypeDef",
-    {
-        "namespace": str,
-        "labels": Mapping[str, str],
-    },
-    total=False,
-)
-
 OidcIdentityProviderConfigTypeDef = TypedDict(
     "OidcIdentityProviderConfigTypeDef",
     {
         "identityProviderConfigName": str,
         "identityProviderConfigArn": str,
         "clusterName": str,
         "issuerUrl": str,
@@ -794,41 +776,23 @@
 
 class ListUpdatesRequestRequestTypeDef(
     _RequiredListUpdatesRequestRequestTypeDef, _OptionalListUpdatesRequestRequestTypeDef
 ):
     pass
 
 
-LogSetupOutputTypeDef = TypedDict(
-    "LogSetupOutputTypeDef",
-    {
-        "types": List[LogTypeType],
-        "enabled": bool,
-    },
-    total=False,
-)
-
 LogSetupTypeDef = TypedDict(
     "LogSetupTypeDef",
     {
         "types": Sequence[LogTypeType],
         "enabled": bool,
     },
     total=False,
 )
 
-RemoteAccessConfigOutputTypeDef = TypedDict(
-    "RemoteAccessConfigOutputTypeDef",
-    {
-        "ec2SshKey": str,
-        "sourceSecurityGroups": List[str],
-    },
-    total=False,
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1094,14 +1058,57 @@
 
 class OutpostConfigResponseTypeDef(
     _RequiredOutpostConfigResponseTypeDef, _OptionalOutpostConfigResponseTypeDef
 ):
     pass
 
 
+_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFargateProfileRequestRequestTypeDef",
+    {
+        "fargateProfileName": str,
+        "clusterName": str,
+        "podExecutionRoleArn": str,
+    },
+)
+_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFargateProfileRequestRequestTypeDef",
+    {
+        "subnets": Sequence[str],
+        "selectors": Sequence[FargateProfileSelectorTypeDef],
+        "clientRequestToken": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateFargateProfileRequestRequestTypeDef(
+    _RequiredCreateFargateProfileRequestRequestTypeDef,
+    _OptionalCreateFargateProfileRequestRequestTypeDef,
+):
+    pass
+
+
+FargateProfileTypeDef = TypedDict(
+    "FargateProfileTypeDef",
+    {
+        "fargateProfileName": str,
+        "fargateProfileArn": str,
+        "clusterName": str,
+        "createdAt": datetime,
+        "podExecutionRoleArn": str,
+        "subnets": List[str],
+        "selectors": List[FargateProfileSelectorTypeDef],
+        "status": FargateProfileStatusType,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredUpdateNodegroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupVersionRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1523,51 +1530,23 @@
     {
         "identityProviderConfigs": List[IdentityProviderConfigTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EncryptionConfigOutputTypeDef = TypedDict(
-    "EncryptionConfigOutputTypeDef",
-    {
-        "resources": List[str],
-        "provider": ProviderTypeDef,
-    },
-    total=False,
-)
-
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "resources": Sequence[str],
         "provider": ProviderTypeDef,
     },
     total=False,
 )
 
-FargateProfileTypeDef = TypedDict(
-    "FargateProfileTypeDef",
-    {
-        "fargateProfileName": str,
-        "fargateProfileArn": str,
-        "clusterName": str,
-        "createdAt": datetime,
-        "podExecutionRoleArn": str,
-        "subnets": List[str],
-        "selectors": List[FargateProfileSelectorOutputTypeDef],
-        "status": FargateProfileStatusType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-FargateProfileSelectorUnionTypeDef = Union[
-    FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef
-]
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
     },
     total=False,
 )
@@ -1584,31 +1563,22 @@
     "NodegroupHealthTypeDef",
     {
         "issues": List[IssueTypeDef],
     },
     total=False,
 )
 
-LoggingOutputTypeDef = TypedDict(
-    "LoggingOutputTypeDef",
-    {
-        "clusterLogging": List[LogSetupOutputTypeDef],
-    },
-    total=False,
-)
-
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "clusterLogging": Sequence[LogSetupTypeDef],
     },
     total=False,
 )
 
-RemoteAccessConfigUnionTypeDef = Union[RemoteAccessConfigTypeDef, RemoteAccessConfigOutputTypeDef]
 UpdateTypeDef = TypedDict(
     "UpdateTypeDef",
     {
         "id": str,
         "status": UpdateStatusType,
         "type": UpdateTypeType,
         "params": List[UpdateParamTypeDef],
@@ -1648,14 +1618,38 @@
         "publisher": str,
         "owner": str,
         "marketplaceInformation": MarketplaceInformationTypeDef,
     },
     total=False,
 )
 
+CreateFargateProfileResponseTypeDef = TypedDict(
+    "CreateFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFargateProfileResponseTypeDef = TypedDict(
+    "DeleteFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFargateProfileResponseTypeDef = TypedDict(
+    "DescribeFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1675,62 +1669,33 @@
 class UpdateNodegroupConfigRequestRequestTypeDef(
     _RequiredUpdateNodegroupConfigRequestRequestTypeDef,
     _OptionalUpdateNodegroupConfigRequestRequestTypeDef,
 ):
     pass
 
 
-EncryptionConfigUnionTypeDef = Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]
-CreateFargateProfileResponseTypeDef = TypedDict(
-    "CreateFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFargateProfileResponseTypeDef = TypedDict(
-    "DeleteFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFargateProfileResponseTypeDef = TypedDict(
-    "DescribeFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFargateProfileRequestRequestTypeDef",
+_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
     {
-        "fargateProfileName": str,
         "clusterName": str,
-        "podExecutionRoleArn": str,
+        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
     },
 )
-_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFargateProfileRequestRequestTypeDef",
+_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
     {
-        "subnets": Sequence[str],
-        "selectors": Sequence[FargateProfileSelectorUnionTypeDef],
         "clientRequestToken": str,
-        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class CreateFargateProfileRequestRequestTypeDef(
-    _RequiredCreateFargateProfileRequestRequestTypeDef,
-    _OptionalCreateFargateProfileRequestRequestTypeDef,
+class AssociateEncryptionConfigRequestRequestTypeDef(
+    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
+    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
 
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
@@ -1750,15 +1715,15 @@
         "createdAt": datetime,
         "modifiedAt": datetime,
         "status": NodegroupStatusType,
         "capacityType": CapacityTypesType,
         "scalingConfig": NodegroupScalingConfigTypeDef,
         "instanceTypes": List[str],
         "subnets": List[str],
-        "remoteAccess": RemoteAccessConfigOutputTypeDef,
+        "remoteAccess": RemoteAccessConfigTypeDef,
         "amiType": AMITypesType,
         "nodeRole": str,
         "labels": Dict[str, str],
         "taints": List[TaintTypeDef],
         "resources": NodegroupResourcesTypeDef,
         "diskSize": int,
         "health": NodegroupHealthTypeDef,
@@ -1776,31 +1741,59 @@
         "arn": str,
         "createdAt": datetime,
         "version": str,
         "endpoint": str,
         "roleArn": str,
         "resourcesVpcConfig": VpcConfigResponseTypeDef,
         "kubernetesNetworkConfig": KubernetesNetworkConfigResponseTypeDef,
-        "logging": LoggingOutputTypeDef,
+        "logging": LoggingTypeDef,
         "identity": IdentityTypeDef,
         "status": ClusterStatusType,
         "certificateAuthority": CertificateTypeDef,
         "clientRequestToken": str,
         "platformVersion": str,
         "tags": Dict[str, str],
-        "encryptionConfig": List[EncryptionConfigOutputTypeDef],
+        "encryptionConfig": List[EncryptionConfigTypeDef],
         "connectorConfig": ConnectorConfigResponseTypeDef,
         "id": str,
         "health": ClusterHealthTypeDef,
         "outpostConfig": OutpostConfigResponseTypeDef,
     },
     total=False,
 )
 
-LoggingUnionTypeDef = Union[LoggingTypeDef, LoggingOutputTypeDef]
+_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClusterRequestRequestTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "resourcesVpcConfig": VpcConfigRequestTypeDef,
+    },
+)
+_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClusterRequestRequestTypeDef",
+    {
+        "version": str,
+        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
+        "logging": LoggingTypeDef,
+        "clientRequestToken": str,
+        "tags": Mapping[str, str],
+        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
+        "outpostConfig": OutpostConfigRequestTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateClusterRequestRequestTypeDef(
+    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateClusterConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterConfigRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateClusterConfigRequestRequestTypeDef = TypedDict(
@@ -1923,66 +1916,14 @@
     {
         "addons": List[AddonInfoTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
-    {
-        "clusterName": str,
-        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
-    },
-)
-_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-    },
-    total=False,
-)
-
-
-class AssociateEncryptionConfigRequestRequestTypeDef(
-    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
-    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClusterRequestRequestTypeDef",
-    {
-        "name": str,
-        "roleArn": str,
-        "resourcesVpcConfig": VpcConfigRequestTypeDef,
-    },
-)
-_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClusterRequestRequestTypeDef",
-    {
-        "version": str,
-        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
-        "logging": LoggingTypeDef,
-        "clientRequestToken": str,
-        "tags": Mapping[str, str],
-        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
-        "outpostConfig": OutpostConfigRequestTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateClusterRequestRequestTypeDef(
-    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
-):
-    pass
-
-
 CreateNodegroupResponseTypeDef = TypedDict(
     "CreateNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/type_defs.pyi` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_eks.type_defs import AddonIssueTypeDef
 
     data: AddonIssueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AddonIssueCodeType,
     AddonStatusType,
     AMITypesType,
     CapacityTypesType,
     ClusterIssueCodeType,
@@ -56,14 +56,15 @@
     "VpcConfigResponseTypeDef",
     "ConnectorConfigRequestTypeDef",
     "ControlPlanePlacementRequestTypeDef",
     "ControlPlanePlacementResponseTypeDef",
     "CreateAddonRequestRequestTypeDef",
     "KubernetesNetworkConfigRequestTypeDef",
     "VpcConfigRequestTypeDef",
+    "FargateProfileSelectorTypeDef",
     "LaunchTemplateSpecificationTypeDef",
     "NodegroupScalingConfigTypeDef",
     "NodegroupUpdateConfigTypeDef",
     "RemoteAccessConfigTypeDef",
     "TaintTypeDef",
     "DeleteAddonRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
@@ -78,29 +79,25 @@
     "DescribeClusterRequestRequestTypeDef",
     "DescribeFargateProfileRequestRequestTypeDef",
     "IdentityProviderConfigTypeDef",
     "DescribeNodegroupRequestRequestTypeDef",
     "DescribeUpdateRequestRequestTypeDef",
     "ProviderTypeDef",
     "ErrorDetailTypeDef",
-    "FargateProfileSelectorOutputTypeDef",
-    "FargateProfileSelectorTypeDef",
     "OidcIdentityProviderConfigTypeDef",
     "OIDCTypeDef",
     "IssueTypeDef",
     "ListAddonsRequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
     "ListFargateProfilesRequestRequestTypeDef",
     "ListIdentityProviderConfigsRequestRequestTypeDef",
     "ListNodegroupsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListUpdatesRequestRequestTypeDef",
-    "LogSetupOutputTypeDef",
     "LogSetupTypeDef",
-    "RemoteAccessConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAddonRequestRequestTypeDef",
     "UpdateClusterVersionRequestRequestTypeDef",
     "UpdateLabelsPayloadTypeDef",
     "UpdateParamTypeDef",
     "AddonHealthTypeDef",
@@ -114,14 +111,16 @@
     "ListUpdatesResponseTypeDef",
     "AssociateIdentityProviderConfigRequestRequestTypeDef",
     "NodegroupResourcesTypeDef",
     "ClusterHealthTypeDef",
     "RegisterClusterRequestRequestTypeDef",
     "OutpostConfigRequestTypeDef",
     "OutpostConfigResponseTypeDef",
+    "CreateFargateProfileRequestRequestTypeDef",
+    "FargateProfileTypeDef",
     "UpdateNodegroupVersionRequestRequestTypeDef",
     "CreateNodegroupRequestRequestTypeDef",
     "UpdateTaintsPayloadTypeDef",
     "DescribeAddonRequestAddonActiveWaitTypeDef",
     "DescribeAddonRequestAddonDeletedWaitTypeDef",
     "DescribeClusterRequestClusterActiveWaitTypeDef",
     "DescribeClusterRequestClusterDeletedWaitTypeDef",
@@ -135,53 +134,45 @@
     "ListFargateProfilesRequestListFargateProfilesPaginateTypeDef",
     "ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef",
     "ListNodegroupsRequestListNodegroupsPaginateTypeDef",
     "ListUpdatesRequestListUpdatesPaginateTypeDef",
     "DescribeIdentityProviderConfigRequestRequestTypeDef",
     "DisassociateIdentityProviderConfigRequestRequestTypeDef",
     "ListIdentityProviderConfigsResponseTypeDef",
-    "EncryptionConfigOutputTypeDef",
     "EncryptionConfigTypeDef",
-    "FargateProfileTypeDef",
-    "FargateProfileSelectorUnionTypeDef",
     "IdentityProviderConfigResponseTypeDef",
     "IdentityTypeDef",
     "NodegroupHealthTypeDef",
-    "LoggingOutputTypeDef",
     "LoggingTypeDef",
-    "RemoteAccessConfigUnionTypeDef",
     "UpdateTypeDef",
     "AddonTypeDef",
     "AddonInfoTypeDef",
-    "UpdateNodegroupConfigRequestRequestTypeDef",
-    "EncryptionConfigUnionTypeDef",
     "CreateFargateProfileResponseTypeDef",
     "DeleteFargateProfileResponseTypeDef",
     "DescribeFargateProfileResponseTypeDef",
-    "CreateFargateProfileRequestRequestTypeDef",
+    "UpdateNodegroupConfigRequestRequestTypeDef",
+    "AssociateEncryptionConfigRequestRequestTypeDef",
     "DescribeIdentityProviderConfigResponseTypeDef",
     "NodegroupTypeDef",
     "ClusterTypeDef",
-    "LoggingUnionTypeDef",
+    "CreateClusterRequestRequestTypeDef",
     "UpdateClusterConfigRequestRequestTypeDef",
     "AssociateEncryptionConfigResponseTypeDef",
     "AssociateIdentityProviderConfigResponseTypeDef",
     "DescribeUpdateResponseTypeDef",
     "DisassociateIdentityProviderConfigResponseTypeDef",
     "UpdateAddonResponseTypeDef",
     "UpdateClusterConfigResponseTypeDef",
     "UpdateClusterVersionResponseTypeDef",
     "UpdateNodegroupConfigResponseTypeDef",
     "UpdateNodegroupVersionResponseTypeDef",
     "CreateAddonResponseTypeDef",
     "DeleteAddonResponseTypeDef",
     "DescribeAddonResponseTypeDef",
     "DescribeAddonVersionsResponseTypeDef",
-    "AssociateEncryptionConfigRequestRequestTypeDef",
-    "CreateClusterRequestRequestTypeDef",
     "CreateNodegroupResponseTypeDef",
     "DeleteNodegroupResponseTypeDef",
     "DescribeNodegroupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DeregisterClusterResponseTypeDef",
     "DescribeClusterResponseTypeDef",
@@ -382,14 +373,23 @@
         "endpointPublicAccess": bool,
         "endpointPrivateAccess": bool,
         "publicAccessCidrs": Sequence[str],
     },
     total=False,
 )
 
+FargateProfileSelectorTypeDef = TypedDict(
+    "FargateProfileSelectorTypeDef",
+    {
+        "namespace": str,
+        "labels": Mapping[str, str],
+    },
+    total=False,
+)
+
 LaunchTemplateSpecificationTypeDef = TypedDict(
     "LaunchTemplateSpecificationTypeDef",
     {
         "name": str,
         "version": str,
         "id": str,
     },
@@ -599,32 +599,14 @@
         "errorCode": ErrorCodeType,
         "errorMessage": str,
         "resourceIds": List[str],
     },
     total=False,
 )
 
-FargateProfileSelectorOutputTypeDef = TypedDict(
-    "FargateProfileSelectorOutputTypeDef",
-    {
-        "namespace": str,
-        "labels": Dict[str, str],
-    },
-    total=False,
-)
-
-FargateProfileSelectorTypeDef = TypedDict(
-    "FargateProfileSelectorTypeDef",
-    {
-        "namespace": str,
-        "labels": Mapping[str, str],
-    },
-    total=False,
-)
-
 OidcIdentityProviderConfigTypeDef = TypedDict(
     "OidcIdentityProviderConfigTypeDef",
     {
         "identityProviderConfigName": str,
         "identityProviderConfigArn": str,
         "clusterName": str,
         "issuerUrl": str,
@@ -775,41 +757,23 @@
 )
 
 class ListUpdatesRequestRequestTypeDef(
     _RequiredListUpdatesRequestRequestTypeDef, _OptionalListUpdatesRequestRequestTypeDef
 ):
     pass
 
-LogSetupOutputTypeDef = TypedDict(
-    "LogSetupOutputTypeDef",
-    {
-        "types": List[LogTypeType],
-        "enabled": bool,
-    },
-    total=False,
-)
-
 LogSetupTypeDef = TypedDict(
     "LogSetupTypeDef",
     {
         "types": Sequence[LogTypeType],
         "enabled": bool,
     },
     total=False,
 )
 
-RemoteAccessConfigOutputTypeDef = TypedDict(
-    "RemoteAccessConfigOutputTypeDef",
-    {
-        "ec2SshKey": str,
-        "sourceSecurityGroups": List[str],
-    },
-    total=False,
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1063,14 +1027,55 @@
 )
 
 class OutpostConfigResponseTypeDef(
     _RequiredOutpostConfigResponseTypeDef, _OptionalOutpostConfigResponseTypeDef
 ):
     pass
 
+_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFargateProfileRequestRequestTypeDef",
+    {
+        "fargateProfileName": str,
+        "clusterName": str,
+        "podExecutionRoleArn": str,
+    },
+)
+_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFargateProfileRequestRequestTypeDef",
+    {
+        "subnets": Sequence[str],
+        "selectors": Sequence[FargateProfileSelectorTypeDef],
+        "clientRequestToken": str,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateFargateProfileRequestRequestTypeDef(
+    _RequiredCreateFargateProfileRequestRequestTypeDef,
+    _OptionalCreateFargateProfileRequestRequestTypeDef,
+):
+    pass
+
+FargateProfileTypeDef = TypedDict(
+    "FargateProfileTypeDef",
+    {
+        "fargateProfileName": str,
+        "fargateProfileArn": str,
+        "clusterName": str,
+        "createdAt": datetime,
+        "podExecutionRoleArn": str,
+        "subnets": List[str],
+        "selectors": List[FargateProfileSelectorTypeDef],
+        "status": FargateProfileStatusType,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredUpdateNodegroupVersionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupVersionRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1460,51 +1465,23 @@
     {
         "identityProviderConfigs": List[IdentityProviderConfigTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EncryptionConfigOutputTypeDef = TypedDict(
-    "EncryptionConfigOutputTypeDef",
-    {
-        "resources": List[str],
-        "provider": ProviderTypeDef,
-    },
-    total=False,
-)
-
 EncryptionConfigTypeDef = TypedDict(
     "EncryptionConfigTypeDef",
     {
         "resources": Sequence[str],
         "provider": ProviderTypeDef,
     },
     total=False,
 )
 
-FargateProfileTypeDef = TypedDict(
-    "FargateProfileTypeDef",
-    {
-        "fargateProfileName": str,
-        "fargateProfileArn": str,
-        "clusterName": str,
-        "createdAt": datetime,
-        "podExecutionRoleArn": str,
-        "subnets": List[str],
-        "selectors": List[FargateProfileSelectorOutputTypeDef],
-        "status": FargateProfileStatusType,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-FargateProfileSelectorUnionTypeDef = Union[
-    FargateProfileSelectorTypeDef, FargateProfileSelectorOutputTypeDef
-]
 IdentityProviderConfigResponseTypeDef = TypedDict(
     "IdentityProviderConfigResponseTypeDef",
     {
         "oidc": OidcIdentityProviderConfigTypeDef,
     },
     total=False,
 )
@@ -1521,31 +1498,22 @@
     "NodegroupHealthTypeDef",
     {
         "issues": List[IssueTypeDef],
     },
     total=False,
 )
 
-LoggingOutputTypeDef = TypedDict(
-    "LoggingOutputTypeDef",
-    {
-        "clusterLogging": List[LogSetupOutputTypeDef],
-    },
-    total=False,
-)
-
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "clusterLogging": Sequence[LogSetupTypeDef],
     },
     total=False,
 )
 
-RemoteAccessConfigUnionTypeDef = Union[RemoteAccessConfigTypeDef, RemoteAccessConfigOutputTypeDef]
 UpdateTypeDef = TypedDict(
     "UpdateTypeDef",
     {
         "id": str,
         "status": UpdateStatusType,
         "type": UpdateTypeType,
         "params": List[UpdateParamTypeDef],
@@ -1585,14 +1553,38 @@
         "publisher": str,
         "owner": str,
         "marketplaceInformation": MarketplaceInformationTypeDef,
     },
     total=False,
 )
 
+CreateFargateProfileResponseTypeDef = TypedDict(
+    "CreateFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFargateProfileResponseTypeDef = TypedDict(
+    "DeleteFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFargateProfileResponseTypeDef = TypedDict(
+    "DescribeFargateProfileResponseTypeDef",
+    {
+        "fargateProfile": FargateProfileTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateNodegroupConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateNodegroupConfigRequestRequestTypeDef",
     {
         "clusterName": str,
         "nodegroupName": str,
     },
 )
@@ -1610,61 +1602,32 @@
 
 class UpdateNodegroupConfigRequestRequestTypeDef(
     _RequiredUpdateNodegroupConfigRequestRequestTypeDef,
     _OptionalUpdateNodegroupConfigRequestRequestTypeDef,
 ):
     pass
 
-EncryptionConfigUnionTypeDef = Union[EncryptionConfigTypeDef, EncryptionConfigOutputTypeDef]
-CreateFargateProfileResponseTypeDef = TypedDict(
-    "CreateFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteFargateProfileResponseTypeDef = TypedDict(
-    "DeleteFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeFargateProfileResponseTypeDef = TypedDict(
-    "DescribeFargateProfileResponseTypeDef",
-    {
-        "fargateProfile": FargateProfileTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFargateProfileRequestRequestTypeDef",
+_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
     {
-        "fargateProfileName": str,
         "clusterName": str,
-        "podExecutionRoleArn": str,
+        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
     },
 )
-_OptionalCreateFargateProfileRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFargateProfileRequestRequestTypeDef",
+_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
     {
-        "subnets": Sequence[str],
-        "selectors": Sequence[FargateProfileSelectorUnionTypeDef],
         "clientRequestToken": str,
-        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateFargateProfileRequestRequestTypeDef(
-    _RequiredCreateFargateProfileRequestRequestTypeDef,
-    _OptionalCreateFargateProfileRequestRequestTypeDef,
+class AssociateEncryptionConfigRequestRequestTypeDef(
+    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
+    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
 DescribeIdentityProviderConfigResponseTypeDef = TypedDict(
     "DescribeIdentityProviderConfigResponseTypeDef",
     {
         "identityProviderConfig": IdentityProviderConfigResponseTypeDef,
@@ -1683,15 +1646,15 @@
         "createdAt": datetime,
         "modifiedAt": datetime,
         "status": NodegroupStatusType,
         "capacityType": CapacityTypesType,
         "scalingConfig": NodegroupScalingConfigTypeDef,
         "instanceTypes": List[str],
         "subnets": List[str],
-        "remoteAccess": RemoteAccessConfigOutputTypeDef,
+        "remoteAccess": RemoteAccessConfigTypeDef,
         "amiType": AMITypesType,
         "nodeRole": str,
         "labels": Dict[str, str],
         "taints": List[TaintTypeDef],
         "resources": NodegroupResourcesTypeDef,
         "diskSize": int,
         "health": NodegroupHealthTypeDef,
@@ -1709,31 +1672,57 @@
         "arn": str,
         "createdAt": datetime,
         "version": str,
         "endpoint": str,
         "roleArn": str,
         "resourcesVpcConfig": VpcConfigResponseTypeDef,
         "kubernetesNetworkConfig": KubernetesNetworkConfigResponseTypeDef,
-        "logging": LoggingOutputTypeDef,
+        "logging": LoggingTypeDef,
         "identity": IdentityTypeDef,
         "status": ClusterStatusType,
         "certificateAuthority": CertificateTypeDef,
         "clientRequestToken": str,
         "platformVersion": str,
         "tags": Dict[str, str],
-        "encryptionConfig": List[EncryptionConfigOutputTypeDef],
+        "encryptionConfig": List[EncryptionConfigTypeDef],
         "connectorConfig": ConnectorConfigResponseTypeDef,
         "id": str,
         "health": ClusterHealthTypeDef,
         "outpostConfig": OutpostConfigResponseTypeDef,
     },
     total=False,
 )
 
-LoggingUnionTypeDef = Union[LoggingTypeDef, LoggingOutputTypeDef]
+_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClusterRequestRequestTypeDef",
+    {
+        "name": str,
+        "roleArn": str,
+        "resourcesVpcConfig": VpcConfigRequestTypeDef,
+    },
+)
+_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClusterRequestRequestTypeDef",
+    {
+        "version": str,
+        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
+        "logging": LoggingTypeDef,
+        "clientRequestToken": str,
+        "tags": Mapping[str, str],
+        "encryptionConfig": Sequence[EncryptionConfigTypeDef],
+        "outpostConfig": OutpostConfigRequestTypeDef,
+    },
+    total=False,
+)
+
+class CreateClusterRequestRequestTypeDef(
+    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateClusterConfigRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClusterConfigRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalUpdateClusterConfigRequestRequestTypeDef = TypedDict(
@@ -1854,62 +1843,14 @@
     {
         "addons": List[AddonInfoTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateEncryptionConfigRequestRequestTypeDef",
-    {
-        "clusterName": str,
-        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
-    },
-)
-_OptionalAssociateEncryptionConfigRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateEncryptionConfigRequestRequestTypeDef",
-    {
-        "clientRequestToken": str,
-    },
-    total=False,
-)
-
-class AssociateEncryptionConfigRequestRequestTypeDef(
-    _RequiredAssociateEncryptionConfigRequestRequestTypeDef,
-    _OptionalAssociateEncryptionConfigRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateClusterRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClusterRequestRequestTypeDef",
-    {
-        "name": str,
-        "roleArn": str,
-        "resourcesVpcConfig": VpcConfigRequestTypeDef,
-    },
-)
-_OptionalCreateClusterRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClusterRequestRequestTypeDef",
-    {
-        "version": str,
-        "kubernetesNetworkConfig": KubernetesNetworkConfigRequestTypeDef,
-        "logging": LoggingTypeDef,
-        "clientRequestToken": str,
-        "tags": Mapping[str, str],
-        "encryptionConfig": Sequence[EncryptionConfigUnionTypeDef],
-        "outpostConfig": OutpostConfigRequestTypeDef,
-    },
-    total=False,
-)
-
-class CreateClusterRequestRequestTypeDef(
-    _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
-):
-    pass
-
 CreateNodegroupResponseTypeDef = TypedDict(
     "CreateNodegroupResponseTypeDef",
     {
         "nodegroup": NodegroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/waiter.py` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks/waiter.pyi` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-eks-2.5.2.post1/types_aiobotocore_eks.egg-info/SOURCES.txt` & `types-aiobotocore-eks-2.5.2.post2/types_aiobotocore_eks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

