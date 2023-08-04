# Comparing `tmp/types-aiobotocore-route53-recovery-readiness-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-route53-recovery-readiness-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-recovery-readiness-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-recovery-readiness-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1.tar` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.845475 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-08-02 14:52:54.841475 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:54.845475 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.837475 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30713 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30662 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-08-02 14:48:08.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-08-02 14:48:08.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    30186 2023-08-02 14:48:08.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30149 2023-08-02 14:48:08.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.841475 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19429 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.876643 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15606 2023-08-04 13:59:23.876643 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14014 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.876643 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2206 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.876643 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2973 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2972 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1015 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    30666 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    30615 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9384 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9382 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13790 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13778 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29773 2023-08-04 13:51:12.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29736 2023-08-04 13:51:11.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:10.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.876643 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15606 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1174 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       45 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/LICENSE` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/setup.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53-recovery-readiness",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_route53_recovery_readiness"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/__init__.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/__init__.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/__main__.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.Route53RecoveryReadiness 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness\nOther"
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

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/client.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     ListCellsResponseTypeDef,
     ListCrossAccountAuthorizationsResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListRulesResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
-    ResourceUnionTypeDef,
+    ResourceTypeDef,
     UpdateCellResponseTypeDef,
     UpdateReadinessCheckResponseTypeDef,
     UpdateRecoveryGroupResponseTypeDef,
     UpdateResourceSetResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -163,15 +163,15 @@
         """
 
     async def create_resource_set(
         self,
         *,
         ResourceSetName: str,
         ResourceSetType: str,
-        Resources: Sequence[ResourceUnionTypeDef],
+        Resources: Sequence[ResourceTypeDef],
         Tags: Mapping[str, str] = ...
     ) -> CreateResourceSetResponseTypeDef:
         """
         Creates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_resource_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#create_resource_set)
@@ -451,19 +451,15 @@
         Updates a recovery group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_recovery_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#update_recovery_group)
         """
 
     async def update_resource_set(
-        self,
-        *,
-        ResourceSetName: str,
-        ResourceSetType: str,
-        Resources: Sequence[ResourceUnionTypeDef]
+        self, *, ResourceSetName: str, ResourceSetType: str, Resources: Sequence[ResourceTypeDef]
     ) -> UpdateResourceSetResponseTypeDef:
         """
         Updates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_resource_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#update_resource_set)
         """
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/client.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     ListCellsResponseTypeDef,
     ListCrossAccountAuthorizationsResponseTypeDef,
     ListReadinessChecksResponseTypeDef,
     ListRecoveryGroupsResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListRulesResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
-    ResourceUnionTypeDef,
+    ResourceTypeDef,
     UpdateCellResponseTypeDef,
     UpdateReadinessCheckResponseTypeDef,
     UpdateRecoveryGroupResponseTypeDef,
     UpdateResourceSetResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -152,15 +152,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#create_recovery_group)
         """
     async def create_resource_set(
         self,
         *,
         ResourceSetName: str,
         ResourceSetType: str,
-        Resources: Sequence[ResourceUnionTypeDef],
+        Resources: Sequence[ResourceTypeDef],
         Tags: Mapping[str, str] = ...
     ) -> CreateResourceSetResponseTypeDef:
         """
         Creates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_resource_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#create_resource_set)
@@ -412,19 +412,15 @@
         """
         Updates a recovery group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_recovery_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#update_recovery_group)
         """
     async def update_resource_set(
-        self,
-        *,
-        ResourceSetName: str,
-        ResourceSetType: str,
-        Resources: Sequence[ResourceUnionTypeDef]
+        self, *, ResourceSetName: str, ResourceSetType: str, Resources: Sequence[ResourceTypeDef]
     ) -> UpdateResourceSetResponseTypeDef:
         """
         Updates a resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_resource_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_readiness/client/#update_resource_set)
         """
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/literals.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
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
@@ -164,14 +165,15 @@
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
@@ -250,26 +252,28 @@
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

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/literals.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
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
@@ -162,14 +163,15 @@
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
@@ -248,26 +250,28 @@
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

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/paginator.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/paginator.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/type_defs.py` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_route53_recovery_readiness.type_defs import CellOutputTypeDef
 
     data: CellOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import ReadinessType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -97,24 +97,22 @@
     "GetReadinessCheckStatusResponseTypeDef",
     "ListReadinessChecksResponseTypeDef",
     "ListRecoveryGroupsResponseTypeDef",
     "ListRulesResponseTypeDef",
     "TargetResourceTypeDef",
     "GetReadinessCheckResourceStatusResponseTypeDef",
     "DNSTargetResourceTypeDef",
-    "ResourceOutputTypeDef",
     "ResourceTypeDef",
+    "CreateResourceSetRequestRequestTypeDef",
     "CreateResourceSetResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "ResourceSetOutputTypeDef",
+    "UpdateResourceSetRequestRequestTypeDef",
     "UpdateResourceSetResponseTypeDef",
-    "ResourceUnionTypeDef",
     "ListResourceSetsResponseTypeDef",
-    "CreateResourceSetRequestRequestTypeDef",
-    "UpdateResourceSetRequestRequestTypeDef",
 )
 
 _RequiredCellOutputTypeDef = TypedDict(
     "_RequiredCellOutputTypeDef",
     {
         "CellArn": str,
         "CellName": str,
@@ -1015,67 +1013,79 @@
         "RecordSetId": str,
         "RecordType": str,
         "TargetResource": TargetResourceTypeDef,
     },
     total=False,
 )
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
     {
         "ComponentId": str,
         "DnsTargetResource": DNSTargetResourceTypeDef,
-        "ReadinessScopes": List[str],
+        "ReadinessScopes": Sequence[str],
         "ResourceArn": str,
     },
     total=False,
 )
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
+_RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateResourceSetRequestRequestTypeDef",
     {
-        "ComponentId": str,
-        "DnsTargetResource": DNSTargetResourceTypeDef,
-        "ReadinessScopes": Sequence[str],
-        "ResourceArn": str,
+        "ResourceSetName": str,
+        "ResourceSetType": str,
+        "Resources": Sequence[ResourceTypeDef],
+    },
+)
+_OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateResourceSetRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
+class CreateResourceSetRequestRequestTypeDef(
+    _RequiredCreateResourceSetRequestRequestTypeDef, _OptionalCreateResourceSetRequestRequestTypeDef
+):
+    pass
+
+
 CreateResourceSetResponseTypeDef = TypedDict(
     "CreateResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceOutputTypeDef],
+        "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceOutputTypeDef],
+        "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResourceSetOutputTypeDef = TypedDict(
     "_RequiredResourceSetOutputTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceOutputTypeDef],
+        "Resources": List[ResourceTypeDef],
     },
 )
 _OptionalResourceSetOutputTypeDef = TypedDict(
     "_OptionalResourceSetOutputTypeDef",
     {
         "Tags": Dict[str, str],
     },
@@ -1085,60 +1095,36 @@
 
 class ResourceSetOutputTypeDef(
     _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
 ):
     pass
 
 
+UpdateResourceSetRequestRequestTypeDef = TypedDict(
+    "UpdateResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSetName": str,
+        "ResourceSetType": str,
+        "Resources": Sequence[ResourceTypeDef],
+    },
+)
+
 UpdateResourceSetResponseTypeDef = TypedDict(
     "UpdateResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceOutputTypeDef],
+        "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "NextToken": str,
         "ResourceSets": List[ResourceSetOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSetName": str,
-        "ResourceSetType": str,
-        "Resources": Sequence[ResourceUnionTypeDef],
-    },
-)
-_OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateResourceSetRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateResourceSetRequestRequestTypeDef(
-    _RequiredCreateResourceSetRequestRequestTypeDef, _OptionalCreateResourceSetRequestRequestTypeDef
-):
-    pass
-
-
-UpdateResourceSetRequestRequestTypeDef = TypedDict(
-    "UpdateResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSetName": str,
-        "ResourceSetType": str,
-        "Resources": Sequence[ResourceUnionTypeDef],
-    },
-)
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness/type_defs.pyi` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_route53_recovery_readiness.type_defs import CellOutputTypeDef
 
     data: CellOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import ReadinessType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -96,24 +96,22 @@
     "GetReadinessCheckStatusResponseTypeDef",
     "ListReadinessChecksResponseTypeDef",
     "ListRecoveryGroupsResponseTypeDef",
     "ListRulesResponseTypeDef",
     "TargetResourceTypeDef",
     "GetReadinessCheckResourceStatusResponseTypeDef",
     "DNSTargetResourceTypeDef",
-    "ResourceOutputTypeDef",
     "ResourceTypeDef",
+    "CreateResourceSetRequestRequestTypeDef",
     "CreateResourceSetResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "ResourceSetOutputTypeDef",
+    "UpdateResourceSetRequestRequestTypeDef",
     "UpdateResourceSetResponseTypeDef",
-    "ResourceUnionTypeDef",
     "ListResourceSetsResponseTypeDef",
-    "CreateResourceSetRequestRequestTypeDef",
-    "UpdateResourceSetRequestRequestTypeDef",
 )
 
 _RequiredCellOutputTypeDef = TypedDict(
     "_RequiredCellOutputTypeDef",
     {
         "CellArn": str,
         "CellName": str,
@@ -982,67 +980,77 @@
         "RecordSetId": str,
         "RecordType": str,
         "TargetResource": TargetResourceTypeDef,
     },
     total=False,
 )
 
-ResourceOutputTypeDef = TypedDict(
-    "ResourceOutputTypeDef",
+ResourceTypeDef = TypedDict(
+    "ResourceTypeDef",
     {
         "ComponentId": str,
         "DnsTargetResource": DNSTargetResourceTypeDef,
-        "ReadinessScopes": List[str],
+        "ReadinessScopes": Sequence[str],
         "ResourceArn": str,
     },
     total=False,
 )
 
-ResourceTypeDef = TypedDict(
-    "ResourceTypeDef",
+_RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateResourceSetRequestRequestTypeDef",
     {
-        "ComponentId": str,
-        "DnsTargetResource": DNSTargetResourceTypeDef,
-        "ReadinessScopes": Sequence[str],
-        "ResourceArn": str,
+        "ResourceSetName": str,
+        "ResourceSetType": str,
+        "Resources": Sequence[ResourceTypeDef],
+    },
+)
+_OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateResourceSetRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+class CreateResourceSetRequestRequestTypeDef(
+    _RequiredCreateResourceSetRequestRequestTypeDef, _OptionalCreateResourceSetRequestRequestTypeDef
+):
+    pass
+
 CreateResourceSetResponseTypeDef = TypedDict(
     "CreateResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceOutputTypeDef],
+        "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceOutputTypeDef],
+        "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResourceSetOutputTypeDef = TypedDict(
     "_RequiredResourceSetOutputTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceOutputTypeDef],
+        "Resources": List[ResourceTypeDef],
     },
 )
 _OptionalResourceSetOutputTypeDef = TypedDict(
     "_OptionalResourceSetOutputTypeDef",
     {
         "Tags": Dict[str, str],
     },
@@ -1050,58 +1058,36 @@
 )
 
 class ResourceSetOutputTypeDef(
     _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
 ):
     pass
 
+UpdateResourceSetRequestRequestTypeDef = TypedDict(
+    "UpdateResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSetName": str,
+        "ResourceSetType": str,
+        "Resources": Sequence[ResourceTypeDef],
+    },
+)
+
 UpdateResourceSetResponseTypeDef = TypedDict(
     "UpdateResourceSetResponseTypeDef",
     {
         "ResourceSetArn": str,
         "ResourceSetName": str,
         "ResourceSetType": str,
-        "Resources": List[ResourceOutputTypeDef],
+        "Resources": List[ResourceTypeDef],
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResourceUnionTypeDef = Union[ResourceTypeDef, ResourceOutputTypeDef]
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "NextToken": str,
         "ResourceSets": List[ResourceSetOutputTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSetName": str,
-        "ResourceSetType": str,
-        "Resources": Sequence[ResourceUnionTypeDef],
-    },
-)
-_OptionalCreateResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateResourceSetRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateResourceSetRequestRequestTypeDef(
-    _RequiredCreateResourceSetRequestRequestTypeDef, _OptionalCreateResourceSetRequestRequestTypeDef
-):
-    pass
-
-UpdateResourceSetRequestRequestTypeDef = TypedDict(
-    "UpdateResourceSetRequestRequestTypeDef",
-    {
-        "ResourceSetName": str,
-        "ResourceSetType": str,
-        "Resources": Sequence[ResourceUnionTypeDef],
-    },
-)
```

### Comparing `types-aiobotocore-route53-recovery-readiness-2.5.2.post1/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt` & `types-aiobotocore-route53-recovery-readiness-2.5.2.post2/types_aiobotocore_route53_recovery_readiness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

