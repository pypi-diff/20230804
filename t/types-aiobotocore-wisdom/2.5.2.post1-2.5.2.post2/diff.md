# Comparing `tmp/types-aiobotocore-wisdom-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-wisdom-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wisdom-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-wisdom-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
```

## Comparing `types-aiobotocore-wisdom-2.5.2.post1.tar` & `types-aiobotocore-wisdom-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.481426 types-aiobotocore-wisdom-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-08-02 14:53:10.481426 types-aiobotocore-wisdom-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16488 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:10.481426 types-aiobotocore-wisdom-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.481426 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26949 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26902 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-08-02 14:51:12.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-08-02 14:51:12.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-08-02 14:51:12.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36521 2023-08-02 14:51:12.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36458 2023-08-02 14:51:12.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:11.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.481426 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18016 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:53:10.000000 types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.076643 types-aiobotocore-wisdom-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13871 2023-08-04 13:59:30.066643 types-aiobotocore-wisdom-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12343 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.076643 types-aiobotocore-wisdom-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.066643 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1949 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1948 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      956 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26939 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26892 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9967 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9965 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8962 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8953 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    36192 2023-08-04 13:56:03.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    36131 2023-08-04 13:56:03.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:02.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.066643 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13871 2023-08-04 13:59:29.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      794 2023-08-04 13:59:30.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:29.000000 types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/LICENSE` & `types-aiobotocore-wisdom-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/setup.py` & `types-aiobotocore-wisdom-2.5.2.post2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wisdom",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_wisdom"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConnectWisdomService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__init__.py` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__init__.pyi` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/__main__.py` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ConnectWisdomService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService\nOther"
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

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/client.py` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     QueryAssistantResponseTypeDef,
     RenderingConfigurationTypeDef,
     SearchContentResponseTypeDef,
     SearchExpressionTypeDef,
     SearchSessionsResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SourceConfigurationUnionTypeDef,
+    SourceConfigurationTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -181,15 +181,15 @@
         *,
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        sourceConfiguration: SourceConfigurationUnionTypeDef = ...,
+        sourceConfiguration: SourceConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_knowledge_base)
```

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/client.pyi` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     NotifyRecommendationsReceivedResponseTypeDef,
     QueryAssistantResponseTypeDef,
     RenderingConfigurationTypeDef,
     SearchContentResponseTypeDef,
     SearchExpressionTypeDef,
     SearchSessionsResponseTypeDef,
     ServerSideEncryptionConfigurationTypeDef,
-    SourceConfigurationUnionTypeDef,
+    SourceConfigurationTypeDef,
     StartContentUploadResponseTypeDef,
     UpdateContentResponseTypeDef,
     UpdateKnowledgeBaseTemplateUriResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -171,15 +171,15 @@
         *,
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        sourceConfiguration: SourceConfigurationUnionTypeDef = ...,
+        sourceConfiguration: SourceConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_knowledge_base)
```

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/literals.py` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/literals.py`

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

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/literals.pyi` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
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
@@ -201,14 +202,15 @@
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
@@ -287,26 +289,28 @@
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

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/paginator.py` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/paginator.pyi` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/type_defs.py` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for wisdom service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_wisdom.type_defs import AppIntegrationsConfigurationOutputTypeDef
+    from types_aiobotocore_wisdom.type_defs import AppIntegrationsConfigurationTypeDef
 
-    data: AppIntegrationsConfigurationOutputTypeDef = ...
+    data: AppIntegrationsConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AssistantStatusType,
     ContentStatusType,
     KnowledgeBaseStatusType,
     KnowledgeBaseTypeType,
     RecommendationSourceTypeType,
@@ -31,27 +31,26 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AppIntegrationsConfigurationOutputTypeDef",
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
+    "AssistantIntegrationConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "ContentDataTypeDef",
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "CreateSessionRequestRequestTypeDef",
-    "SessionDataTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
     "DeleteKnowledgeBaseRequestRequestTypeDef",
     "HighlightTypeDef",
     "FilterTypeDef",
     "GetAssistantAssociationRequestRequestTypeDef",
@@ -69,96 +68,74 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
     "QueryAssistantRequestRequestTypeDef",
     "QueryRecommendationTriggerDataTypeDef",
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
     "SessionSummaryTypeDef",
+    "SessionIntegrationConfigurationTypeDef",
     "StartContentUploadRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContentRequestRequestTypeDef",
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
-    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "CreateAssistantAssociationRequestRequestTypeDef",
     "AssistantAssociationOutputDataTypeDef",
     "AssistantDataTypeDef",
     "AssistantSummaryTypeDef",
     "CreateAssistantRequestRequestTypeDef",
     "CreateContentResponseTypeDef",
     "GetContentResponseTypeDef",
     "GetContentSummaryResponseTypeDef",
     "ListContentsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SearchContentResponseTypeDef",
     "StartContentUploadResponseTypeDef",
     "UpdateContentResponseTypeDef",
-    "CreateSessionResponseTypeDef",
-    "GetSessionResponseTypeDef",
     "DocumentTextTypeDef",
     "SearchExpressionTypeDef",
     "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListContentsRequestListContentsPaginateTypeDef",
     "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "NotifyRecommendationsReceivedResponseTypeDef",
     "RecommendationTriggerDataTypeDef",
     "SearchSessionsResponseTypeDef",
+    "SessionDataTypeDef",
+    "CreateKnowledgeBaseRequestRequestTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
-    "CreateKnowledgeBaseRequestRequestTypeDef",
-    "SourceConfigurationUnionTypeDef",
     "AssistantAssociationDataTypeDef",
     "AssistantAssociationSummaryTypeDef",
     "CreateAssistantResponseTypeDef",
     "GetAssistantResponseTypeDef",
     "ListAssistantsResponseTypeDef",
     "DocumentTypeDef",
     "SearchContentRequestRequestTypeDef",
     "SearchContentRequestSearchContentPaginateTypeDef",
     "SearchSessionsRequestRequestTypeDef",
     "SearchSessionsRequestSearchSessionsPaginateTypeDef",
     "RecommendationTriggerTypeDef",
+    "CreateSessionResponseTypeDef",
+    "GetSessionResponseTypeDef",
     "CreateKnowledgeBaseResponseTypeDef",
     "GetKnowledgeBaseResponseTypeDef",
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     "ListKnowledgeBasesResponseTypeDef",
     "CreateAssistantAssociationResponseTypeDef",
     "GetAssistantAssociationResponseTypeDef",
     "ListAssistantAssociationsResponseTypeDef",
     "RecommendationDataTypeDef",
     "ResultDataTypeDef",
     "GetRecommendationsResponseTypeDef",
     "QueryAssistantResponseTypeDef",
 )
 
-_RequiredAppIntegrationsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAppIntegrationsConfigurationOutputTypeDef",
-    {
-        "appIntegrationArn": str,
-    },
-)
-_OptionalAppIntegrationsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAppIntegrationsConfigurationOutputTypeDef",
-    {
-        "objectFields": List[str],
-    },
-    total=False,
-)
-
-
-class AppIntegrationsConfigurationOutputTypeDef(
-    _RequiredAppIntegrationsConfigurationOutputTypeDef,
-    _OptionalAppIntegrationsConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredAppIntegrationsConfigurationTypeDef = TypedDict(
     "_RequiredAppIntegrationsConfigurationTypeDef",
     {
         "appIntegrationArn": str,
     },
 )
 _OptionalAppIntegrationsConfigurationTypeDef = TypedDict(
@@ -189,14 +166,22 @@
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
     },
     total=False,
 )
 
+AssistantIntegrationConfigurationTypeDef = TypedDict(
+    "AssistantIntegrationConfigurationTypeDef",
+    {
+        "topicIntegrationArn": str,
+    },
+    total=False,
+)
+
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
@@ -337,36 +322,14 @@
 
 class CreateSessionRequestRequestTypeDef(
     _RequiredCreateSessionRequestRequestTypeDef, _OptionalCreateSessionRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredSessionDataTypeDef = TypedDict(
-    "_RequiredSessionDataTypeDef",
-    {
-        "name": str,
-        "sessionArn": str,
-        "sessionId": str,
-    },
-)
-_OptionalSessionDataTypeDef = TypedDict(
-    "_OptionalSessionDataTypeDef",
-    {
-        "description": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class SessionDataTypeDef(_RequiredSessionDataTypeDef, _OptionalSessionDataTypeDef):
-    pass
-
-
 DeleteAssistantAssociationRequestRequestTypeDef = TypedDict(
     "DeleteAssistantAssociationRequestRequestTypeDef",
     {
         "assistantAssociationId": str,
         "assistantId": str,
     },
 )
@@ -623,14 +586,22 @@
         "assistantArn": str,
         "assistantId": str,
         "sessionArn": str,
         "sessionId": str,
     },
 )
 
+SessionIntegrationConfigurationTypeDef = TypedDict(
+    "SessionIntegrationConfigurationTypeDef",
+    {
+        "topicIntegrationArn": str,
+    },
+    total=False,
+)
+
 StartContentUploadRequestRequestTypeDef = TypedDict(
     "StartContentUploadRequestRequestTypeDef",
     {
         "contentType": str,
         "knowledgeBaseId": str,
     },
 )
@@ -682,22 +653,14 @@
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "templateUri": str,
     },
 )
 
-SourceConfigurationOutputTypeDef = TypedDict(
-    "SourceConfigurationOutputTypeDef",
-    {
-        "appIntegrations": AppIntegrationsConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "appIntegrations": AppIntegrationsConfigurationTypeDef,
     },
     total=False,
 )
@@ -745,14 +708,15 @@
         "type": Literal["AGENT"],
     },
 )
 _OptionalAssistantDataTypeDef = TypedDict(
     "_OptionalAssistantDataTypeDef",
     {
         "description": str,
+        "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
@@ -770,14 +734,15 @@
         "type": Literal["AGENT"],
     },
 )
 _OptionalAssistantSummaryTypeDef = TypedDict(
     "_OptionalAssistantSummaryTypeDef",
     {
         "description": str,
+        "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
@@ -875,30 +840,14 @@
     "UpdateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateSessionResponseTypeDef = TypedDict(
-    "CreateSessionResponseTypeDef",
-    {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DocumentTextTypeDef = TypedDict(
     "DocumentTextTypeDef",
     {
         "highlights": List[HighlightTypeDef],
         "text": str,
     },
     total=False,
@@ -1016,104 +965,124 @@
     {
         "nextToken": str,
         "sessionSummaries": List[SessionSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredKnowledgeBaseDataTypeDef = TypedDict(
-    "_RequiredKnowledgeBaseDataTypeDef",
+_RequiredSessionDataTypeDef = TypedDict(
+    "_RequiredSessionDataTypeDef",
+    {
+        "name": str,
+        "sessionArn": str,
+        "sessionId": str,
+    },
+)
+_OptionalSessionDataTypeDef = TypedDict(
+    "_OptionalSessionDataTypeDef",
+    {
+        "description": str,
+        "integrationConfiguration": SessionIntegrationConfigurationTypeDef,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class SessionDataTypeDef(_RequiredSessionDataTypeDef, _OptionalSessionDataTypeDef):
+    pass
+
+
+_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
     {
-        "knowledgeBaseArn": str,
-        "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
-        "status": KnowledgeBaseStatusType,
     },
 )
-_OptionalKnowledgeBaseDataTypeDef = TypedDict(
-    "_OptionalKnowledgeBaseDataTypeDef",
+_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
     {
+        "clientToken": str,
         "description": str,
-        "lastContentModificationTime": datetime,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationOutputTypeDef,
-        "tags": Dict[str, str],
+        "sourceConfiguration": SourceConfigurationTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class KnowledgeBaseDataTypeDef(
-    _RequiredKnowledgeBaseDataTypeDef, _OptionalKnowledgeBaseDataTypeDef
+class CreateKnowledgeBaseRequestRequestTypeDef(
+    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
+    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredKnowledgeBaseSummaryTypeDef = TypedDict(
-    "_RequiredKnowledgeBaseSummaryTypeDef",
+_RequiredKnowledgeBaseDataTypeDef = TypedDict(
+    "_RequiredKnowledgeBaseDataTypeDef",
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
         "status": KnowledgeBaseStatusType,
     },
 )
-_OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
-    "_OptionalKnowledgeBaseSummaryTypeDef",
+_OptionalKnowledgeBaseDataTypeDef = TypedDict(
+    "_OptionalKnowledgeBaseDataTypeDef",
     {
         "description": str,
+        "lastContentModificationTime": datetime,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationOutputTypeDef,
+        "sourceConfiguration": SourceConfigurationTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class KnowledgeBaseSummaryTypeDef(
-    _RequiredKnowledgeBaseSummaryTypeDef, _OptionalKnowledgeBaseSummaryTypeDef
+class KnowledgeBaseDataTypeDef(
+    _RequiredKnowledgeBaseDataTypeDef, _OptionalKnowledgeBaseDataTypeDef
 ):
     pass
 
 
-_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
+_RequiredKnowledgeBaseSummaryTypeDef = TypedDict(
+    "_RequiredKnowledgeBaseSummaryTypeDef",
     {
+        "knowledgeBaseArn": str,
+        "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
+        "status": KnowledgeBaseStatusType,
     },
 )
-_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
+_OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
+    "_OptionalKnowledgeBaseSummaryTypeDef",
     {
-        "clientToken": str,
         "description": str,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "sourceConfiguration": SourceConfigurationTypeDef,
-        "tags": Mapping[str, str],
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class CreateKnowledgeBaseRequestRequestTypeDef(
-    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
-    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
+class KnowledgeBaseSummaryTypeDef(
+    _RequiredKnowledgeBaseSummaryTypeDef, _OptionalKnowledgeBaseSummaryTypeDef
 ):
     pass
 
 
-SourceConfigurationUnionTypeDef = Union[
-    SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
-]
 _RequiredAssistantAssociationDataTypeDef = TypedDict(
     "_RequiredAssistantAssociationDataTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
@@ -1306,14 +1275,30 @@
         "id": str,
         "recommendationIds": List[str],
         "source": RecommendationSourceTypeType,
         "type": Literal["QUERY"],
     },
 )
 
+CreateSessionResponseTypeDef = TypedDict(
+    "CreateSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateKnowledgeBaseResponseTypeDef = TypedDict(
     "CreateKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom/type_defs.pyi` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for wisdom service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_wisdom.type_defs import AppIntegrationsConfigurationOutputTypeDef
+    from types_aiobotocore_wisdom.type_defs import AppIntegrationsConfigurationTypeDef
 
-    data: AppIntegrationsConfigurationOutputTypeDef = ...
+    data: AppIntegrationsConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AssistantStatusType,
     ContentStatusType,
     KnowledgeBaseStatusType,
     KnowledgeBaseTypeType,
     RecommendationSourceTypeType,
@@ -30,27 +30,26 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AppIntegrationsConfigurationOutputTypeDef",
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
+    "AssistantIntegrationConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
     "ContentDataTypeDef",
     "ContentReferenceTypeDef",
     "ContentSummaryTypeDef",
     "ResponseMetadataTypeDef",
     "CreateContentRequestRequestTypeDef",
     "RenderingConfigurationTypeDef",
     "CreateSessionRequestRequestTypeDef",
-    "SessionDataTypeDef",
     "DeleteAssistantAssociationRequestRequestTypeDef",
     "DeleteAssistantRequestRequestTypeDef",
     "DeleteContentRequestRequestTypeDef",
     "DeleteKnowledgeBaseRequestRequestTypeDef",
     "HighlightTypeDef",
     "FilterTypeDef",
     "GetAssistantAssociationRequestRequestTypeDef",
@@ -68,94 +67,74 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "NotifyRecommendationsReceivedErrorTypeDef",
     "NotifyRecommendationsReceivedRequestRequestTypeDef",
     "QueryAssistantRequestRequestTypeDef",
     "QueryRecommendationTriggerDataTypeDef",
     "RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef",
     "SessionSummaryTypeDef",
+    "SessionIntegrationConfigurationTypeDef",
     "StartContentUploadRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateContentRequestRequestTypeDef",
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
-    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "CreateAssistantAssociationRequestRequestTypeDef",
     "AssistantAssociationOutputDataTypeDef",
     "AssistantDataTypeDef",
     "AssistantSummaryTypeDef",
     "CreateAssistantRequestRequestTypeDef",
     "CreateContentResponseTypeDef",
     "GetContentResponseTypeDef",
     "GetContentSummaryResponseTypeDef",
     "ListContentsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "SearchContentResponseTypeDef",
     "StartContentUploadResponseTypeDef",
     "UpdateContentResponseTypeDef",
-    "CreateSessionResponseTypeDef",
-    "GetSessionResponseTypeDef",
     "DocumentTextTypeDef",
     "SearchExpressionTypeDef",
     "ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef",
     "ListAssistantsRequestListAssistantsPaginateTypeDef",
     "ListContentsRequestListContentsPaginateTypeDef",
     "ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef",
     "QueryAssistantRequestQueryAssistantPaginateTypeDef",
     "NotifyRecommendationsReceivedResponseTypeDef",
     "RecommendationTriggerDataTypeDef",
     "SearchSessionsResponseTypeDef",
+    "SessionDataTypeDef",
+    "CreateKnowledgeBaseRequestRequestTypeDef",
     "KnowledgeBaseDataTypeDef",
     "KnowledgeBaseSummaryTypeDef",
-    "CreateKnowledgeBaseRequestRequestTypeDef",
-    "SourceConfigurationUnionTypeDef",
     "AssistantAssociationDataTypeDef",
     "AssistantAssociationSummaryTypeDef",
     "CreateAssistantResponseTypeDef",
     "GetAssistantResponseTypeDef",
     "ListAssistantsResponseTypeDef",
     "DocumentTypeDef",
     "SearchContentRequestRequestTypeDef",
     "SearchContentRequestSearchContentPaginateTypeDef",
     "SearchSessionsRequestRequestTypeDef",
     "SearchSessionsRequestSearchSessionsPaginateTypeDef",
     "RecommendationTriggerTypeDef",
+    "CreateSessionResponseTypeDef",
+    "GetSessionResponseTypeDef",
     "CreateKnowledgeBaseResponseTypeDef",
     "GetKnowledgeBaseResponseTypeDef",
     "UpdateKnowledgeBaseTemplateUriResponseTypeDef",
     "ListKnowledgeBasesResponseTypeDef",
     "CreateAssistantAssociationResponseTypeDef",
     "GetAssistantAssociationResponseTypeDef",
     "ListAssistantAssociationsResponseTypeDef",
     "RecommendationDataTypeDef",
     "ResultDataTypeDef",
     "GetRecommendationsResponseTypeDef",
     "QueryAssistantResponseTypeDef",
 )
 
-_RequiredAppIntegrationsConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAppIntegrationsConfigurationOutputTypeDef",
-    {
-        "appIntegrationArn": str,
-    },
-)
-_OptionalAppIntegrationsConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAppIntegrationsConfigurationOutputTypeDef",
-    {
-        "objectFields": List[str],
-    },
-    total=False,
-)
-
-class AppIntegrationsConfigurationOutputTypeDef(
-    _RequiredAppIntegrationsConfigurationOutputTypeDef,
-    _OptionalAppIntegrationsConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredAppIntegrationsConfigurationTypeDef = TypedDict(
     "_RequiredAppIntegrationsConfigurationTypeDef",
     {
         "appIntegrationArn": str,
     },
 )
 _OptionalAppIntegrationsConfigurationTypeDef = TypedDict(
@@ -184,14 +163,22 @@
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
     },
     total=False,
 )
 
+AssistantIntegrationConfigurationTypeDef = TypedDict(
+    "AssistantIntegrationConfigurationTypeDef",
+    {
+        "topicIntegrationArn": str,
+    },
+    total=False,
+)
+
 ServerSideEncryptionConfigurationTypeDef = TypedDict(
     "ServerSideEncryptionConfigurationTypeDef",
     {
         "kmsKeyId": str,
     },
     total=False,
 )
@@ -324,34 +311,14 @@
 )
 
 class CreateSessionRequestRequestTypeDef(
     _RequiredCreateSessionRequestRequestTypeDef, _OptionalCreateSessionRequestRequestTypeDef
 ):
     pass
 
-_RequiredSessionDataTypeDef = TypedDict(
-    "_RequiredSessionDataTypeDef",
-    {
-        "name": str,
-        "sessionArn": str,
-        "sessionId": str,
-    },
-)
-_OptionalSessionDataTypeDef = TypedDict(
-    "_OptionalSessionDataTypeDef",
-    {
-        "description": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-class SessionDataTypeDef(_RequiredSessionDataTypeDef, _OptionalSessionDataTypeDef):
-    pass
-
 DeleteAssistantAssociationRequestRequestTypeDef = TypedDict(
     "DeleteAssistantAssociationRequestRequestTypeDef",
     {
         "assistantAssociationId": str,
         "assistantId": str,
     },
 )
@@ -600,14 +567,22 @@
         "assistantArn": str,
         "assistantId": str,
         "sessionArn": str,
         "sessionId": str,
     },
 )
 
+SessionIntegrationConfigurationTypeDef = TypedDict(
+    "SessionIntegrationConfigurationTypeDef",
+    {
+        "topicIntegrationArn": str,
+    },
+    total=False,
+)
+
 StartContentUploadRequestRequestTypeDef = TypedDict(
     "StartContentUploadRequestRequestTypeDef",
     {
         "contentType": str,
         "knowledgeBaseId": str,
     },
 )
@@ -657,22 +632,14 @@
     "UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef",
     {
         "knowledgeBaseId": str,
         "templateUri": str,
     },
 )
 
-SourceConfigurationOutputTypeDef = TypedDict(
-    "SourceConfigurationOutputTypeDef",
-    {
-        "appIntegrations": AppIntegrationsConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "appIntegrations": AppIntegrationsConfigurationTypeDef,
     },
     total=False,
 )
@@ -718,14 +685,15 @@
         "type": Literal["AGENT"],
     },
 )
 _OptionalAssistantDataTypeDef = TypedDict(
     "_OptionalAssistantDataTypeDef",
     {
         "description": str,
+        "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class AssistantDataTypeDef(_RequiredAssistantDataTypeDef, _OptionalAssistantDataTypeDef):
@@ -741,14 +709,15 @@
         "type": Literal["AGENT"],
     },
 )
 _OptionalAssistantSummaryTypeDef = TypedDict(
     "_OptionalAssistantSummaryTypeDef",
     {
         "description": str,
+        "integrationConfiguration": AssistantIntegrationConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class AssistantSummaryTypeDef(_RequiredAssistantSummaryTypeDef, _OptionalAssistantSummaryTypeDef):
@@ -842,30 +811,14 @@
     "UpdateContentResponseTypeDef",
     {
         "content": ContentDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateSessionResponseTypeDef = TypedDict(
-    "CreateSessionResponseTypeDef",
-    {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "session": SessionDataTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DocumentTextTypeDef = TypedDict(
     "DocumentTextTypeDef",
     {
         "highlights": List[HighlightTypeDef],
         "text": str,
     },
     total=False,
@@ -977,98 +930,116 @@
     {
         "nextToken": str,
         "sessionSummaries": List[SessionSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredKnowledgeBaseDataTypeDef = TypedDict(
-    "_RequiredKnowledgeBaseDataTypeDef",
+_RequiredSessionDataTypeDef = TypedDict(
+    "_RequiredSessionDataTypeDef",
+    {
+        "name": str,
+        "sessionArn": str,
+        "sessionId": str,
+    },
+)
+_OptionalSessionDataTypeDef = TypedDict(
+    "_OptionalSessionDataTypeDef",
+    {
+        "description": str,
+        "integrationConfiguration": SessionIntegrationConfigurationTypeDef,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+class SessionDataTypeDef(_RequiredSessionDataTypeDef, _OptionalSessionDataTypeDef):
+    pass
+
+_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
     {
-        "knowledgeBaseArn": str,
-        "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
-        "status": KnowledgeBaseStatusType,
     },
 )
-_OptionalKnowledgeBaseDataTypeDef = TypedDict(
-    "_OptionalKnowledgeBaseDataTypeDef",
+_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
     {
+        "clientToken": str,
         "description": str,
-        "lastContentModificationTime": datetime,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationOutputTypeDef,
-        "tags": Dict[str, str],
+        "sourceConfiguration": SourceConfigurationTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class KnowledgeBaseDataTypeDef(
-    _RequiredKnowledgeBaseDataTypeDef, _OptionalKnowledgeBaseDataTypeDef
+class CreateKnowledgeBaseRequestRequestTypeDef(
+    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
+    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
 ):
     pass
 
-_RequiredKnowledgeBaseSummaryTypeDef = TypedDict(
-    "_RequiredKnowledgeBaseSummaryTypeDef",
+_RequiredKnowledgeBaseDataTypeDef = TypedDict(
+    "_RequiredKnowledgeBaseDataTypeDef",
     {
         "knowledgeBaseArn": str,
         "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
         "status": KnowledgeBaseStatusType,
     },
 )
-_OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
-    "_OptionalKnowledgeBaseSummaryTypeDef",
+_OptionalKnowledgeBaseDataTypeDef = TypedDict(
+    "_OptionalKnowledgeBaseDataTypeDef",
     {
         "description": str,
+        "lastContentModificationTime": datetime,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
-        "sourceConfiguration": SourceConfigurationOutputTypeDef,
+        "sourceConfiguration": SourceConfigurationTypeDef,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-class KnowledgeBaseSummaryTypeDef(
-    _RequiredKnowledgeBaseSummaryTypeDef, _OptionalKnowledgeBaseSummaryTypeDef
+class KnowledgeBaseDataTypeDef(
+    _RequiredKnowledgeBaseDataTypeDef, _OptionalKnowledgeBaseDataTypeDef
 ):
     pass
 
-_RequiredCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKnowledgeBaseRequestRequestTypeDef",
+_RequiredKnowledgeBaseSummaryTypeDef = TypedDict(
+    "_RequiredKnowledgeBaseSummaryTypeDef",
     {
+        "knowledgeBaseArn": str,
+        "knowledgeBaseId": str,
         "knowledgeBaseType": KnowledgeBaseTypeType,
         "name": str,
+        "status": KnowledgeBaseStatusType,
     },
 )
-_OptionalCreateKnowledgeBaseRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKnowledgeBaseRequestRequestTypeDef",
+_OptionalKnowledgeBaseSummaryTypeDef = TypedDict(
+    "_OptionalKnowledgeBaseSummaryTypeDef",
     {
-        "clientToken": str,
         "description": str,
         "renderingConfiguration": RenderingConfigurationTypeDef,
         "serverSideEncryptionConfiguration": ServerSideEncryptionConfigurationTypeDef,
         "sourceConfiguration": SourceConfigurationTypeDef,
-        "tags": Mapping[str, str],
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateKnowledgeBaseRequestRequestTypeDef(
-    _RequiredCreateKnowledgeBaseRequestRequestTypeDef,
-    _OptionalCreateKnowledgeBaseRequestRequestTypeDef,
+class KnowledgeBaseSummaryTypeDef(
+    _RequiredKnowledgeBaseSummaryTypeDef, _OptionalKnowledgeBaseSummaryTypeDef
 ):
     pass
 
-SourceConfigurationUnionTypeDef = Union[
-    SourceConfigurationTypeDef, SourceConfigurationOutputTypeDef
-]
 _RequiredAssistantAssociationDataTypeDef = TypedDict(
     "_RequiredAssistantAssociationDataTypeDef",
     {
         "assistantArn": str,
         "assistantAssociationArn": str,
         "assistantAssociationId": str,
         "assistantId": str,
@@ -1247,14 +1218,30 @@
         "id": str,
         "recommendationIds": List[str],
         "source": RecommendationSourceTypeType,
         "type": Literal["QUERY"],
     },
 )
 
+CreateSessionResponseTypeDef = TypedDict(
+    "CreateSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "session": SessionDataTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateKnowledgeBaseResponseTypeDef = TypedDict(
     "CreateKnowledgeBaseResponseTypeDef",
     {
         "knowledgeBase": KnowledgeBaseDataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-wisdom-2.5.2.post1/types_aiobotocore_wisdom.egg-info/SOURCES.txt` & `types-aiobotocore-wisdom-2.5.2.post2/types_aiobotocore_wisdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

