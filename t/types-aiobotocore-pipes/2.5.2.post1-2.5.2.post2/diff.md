# Comparing `tmp/types-aiobotocore-pipes-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-pipes-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pipes-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-pipes-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
```

## Comparing `types-aiobotocore-pipes-2.5.2.post1.tar` & `types-aiobotocore-pipes-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:48.325497 types-aiobotocore-pipes-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-08-02 14:52:48.325497 types-aiobotocore-pipes-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:48.325497 types-aiobotocore-pipes-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:48.325497 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43088 2023-08-02 14:45:02.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43046 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:45:01.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:48.325497 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17323 2023-08-02 14:52:48.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:52:48.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:48.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:48.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:48.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:48.000000 types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.696643 types-aiobotocore-pipes-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12890 2023-08-04 13:59:21.696643 types-aiobotocore-pipes-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11369 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.696643 types-aiobotocore-pipes-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2069 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.696643 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      656 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      655 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10880 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10860 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10162 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10160 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2205 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2202 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31941 2023-08-04 13:47:04.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31911 2023-08-04 13:47:04.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:47:03.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.696643 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12890 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      775 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:21.000000 types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pipes-2.5.2.post1/LICENSE` & `types-aiobotocore-pipes-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post1/setup.py` & `types-aiobotocore-pipes-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pipes",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_pipes"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EventBridgePipes 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/__init__.py` & `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/__init__.pyi` & `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/__main__.py` & `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.EventBridgePipes 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes\nOther"
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

### Comparing `types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/client.py` & `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 from .paginator import ListPipesPaginator
 from .type_defs import (
     CreatePipeResponseTypeDef,
     DeletePipeResponseTypeDef,
     DescribePipeResponseTypeDef,
     ListPipesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PipeEnrichmentParametersUnionTypeDef,
-    PipeSourceParametersUnionTypeDef,
-    PipeTargetParametersUnionTypeDef,
+    PipeEnrichmentParametersTypeDef,
+    PipeSourceParametersTypeDef,
+    PipeTargetParametersTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
     UpdatePipeSourceParametersTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -103,18 +103,18 @@
         Name: str,
         RoleArn: str,
         Source: str,
         Target: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: PipeEnrichmentParametersUnionTypeDef = ...,
-        SourceParameters: PipeSourceParametersUnionTypeDef = ...,
+        EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
+        SourceParameters: PipeSourceParametersTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        TargetParameters: PipeTargetParametersUnionTypeDef = ...
+        TargetParameters: PipeTargetParametersTypeDef = ...
     ) -> CreatePipeResponseTypeDef:
         """
         Create a pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.create_pipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes/client/#create_pipe)
         """
@@ -213,18 +213,18 @@
         self,
         *,
         Name: str,
         RoleArn: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: PipeEnrichmentParametersUnionTypeDef = ...,
+        EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
         SourceParameters: UpdatePipeSourceParametersTypeDef = ...,
         Target: str = ...,
-        TargetParameters: PipeTargetParametersUnionTypeDef = ...
+        TargetParameters: PipeTargetParametersTypeDef = ...
     ) -> UpdatePipeResponseTypeDef:
         """
         Update an existing pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.update_pipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes/client/#update_pipe)
         """
```

### Comparing `types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/client.pyi` & `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 from .paginator import ListPipesPaginator
 from .type_defs import (
     CreatePipeResponseTypeDef,
     DeletePipeResponseTypeDef,
     DescribePipeResponseTypeDef,
     ListPipesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PipeEnrichmentParametersUnionTypeDef,
-    PipeSourceParametersUnionTypeDef,
-    PipeTargetParametersUnionTypeDef,
+    PipeEnrichmentParametersTypeDef,
+    PipeSourceParametersTypeDef,
+    PipeTargetParametersTypeDef,
     StartPipeResponseTypeDef,
     StopPipeResponseTypeDef,
     UpdatePipeResponseTypeDef,
     UpdatePipeSourceParametersTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -96,18 +96,18 @@
         Name: str,
         RoleArn: str,
         Source: str,
         Target: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: PipeEnrichmentParametersUnionTypeDef = ...,
-        SourceParameters: PipeSourceParametersUnionTypeDef = ...,
+        EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
+        SourceParameters: PipeSourceParametersTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        TargetParameters: PipeTargetParametersUnionTypeDef = ...
+        TargetParameters: PipeTargetParametersTypeDef = ...
     ) -> CreatePipeResponseTypeDef:
         """
         Create a pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.create_pipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes/client/#create_pipe)
         """
@@ -196,18 +196,18 @@
         self,
         *,
         Name: str,
         RoleArn: str,
         Description: str = ...,
         DesiredState: RequestedPipeStateType = ...,
         Enrichment: str = ...,
-        EnrichmentParameters: PipeEnrichmentParametersUnionTypeDef = ...,
+        EnrichmentParameters: PipeEnrichmentParametersTypeDef = ...,
         SourceParameters: UpdatePipeSourceParametersTypeDef = ...,
         Target: str = ...,
-        TargetParameters: PipeTargetParametersUnionTypeDef = ...
+        TargetParameters: PipeTargetParametersTypeDef = ...
     ) -> UpdatePipeResponseTypeDef:
         """
         Update an existing pipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes.Client.update_pipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pipes/client/#update_pipe)
         """
```

### Comparing `types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/literals.py` & `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
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
@@ -193,14 +194,15 @@
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
@@ -279,26 +281,28 @@
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

### Comparing `types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/literals.pyi` & `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
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
@@ -191,14 +192,15 @@
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
@@ -277,26 +279,28 @@
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

### Comparing `types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/paginator.py` & `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes/paginator.pyi` & `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pipes-2.5.2.post1/types_aiobotocore_pipes.egg-info/SOURCES.txt` & `types-aiobotocore-pipes-2.5.2.post2/types_aiobotocore_pipes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

