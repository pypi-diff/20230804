# Comparing `tmp/types-aiobotocore-m2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-m2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-m2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-m2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
```

## Comparing `types-aiobotocore-m2-2.5.2.post1.tar` & `types-aiobotocore-m2-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.973533 types-aiobotocore-m2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-08-02 14:52:35.969533 types-aiobotocore-m2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:35.973533 types-aiobotocore-m2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.961533 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42321 2023-08-02 14:42:39.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42253 2023-08-02 14:42:39.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:36.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.969533 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:52:35.000000 types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.246643 types-aiobotocore-m2-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14159 2023-08-04 13:59:16.246643 types-aiobotocore-m2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12641 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.256643 types-aiobotocore-m2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2033 2023-08-04 13:43:32.000000 types-aiobotocore-m2-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.246643 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2529 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2528 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      952 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29883 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29832 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10455 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10453 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11866 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11855 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    42562 2023-08-04 13:43:34.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    42494 2023-08-04 13:43:34.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:33.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.246643 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14159 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      718 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       21 2023-08-04 13:59:16.000000 types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-m2-2.5.2.post1/LICENSE` & `types-aiobotocore-m2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post1/setup.py` & `types-aiobotocore-m2-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-m2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_m2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MainframeModernization 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__init__.py` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__init__.pyi` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/__main__.py` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.MainframeModernization 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization\nOther"
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

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/client.py` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     GetApplicationResponseTypeDef,
     GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     GetDataSetDetailsResponseTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     GetDeploymentResponseTypeDef,
     GetEnvironmentResponseTypeDef,
+    GetSignedBluinsightsUrlResponseTypeDef,
     HighAvailabilityConfigTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     ListDataSetsResponseTypeDef,
@@ -314,14 +315,22 @@
         """
         Describes a specific runtime environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#get_environment)
         """
 
+    async def get_signed_bluinsights_url(self) -> GetSignedBluinsightsUrlResponseTypeDef:
+        """
+        Gets a single sign-on URL that can be used to connect to AWS Blu Insights.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_signed_bluinsights_url)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#get_signed_bluinsights_url)
+        """
+
     async def list_application_versions(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListApplicationVersionsResponseTypeDef:
         """
         Returns a list of the application versions for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_application_versions)
```

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/client.pyi` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     GetApplicationResponseTypeDef,
     GetApplicationVersionResponseTypeDef,
     GetBatchJobExecutionResponseTypeDef,
     GetDataSetDetailsResponseTypeDef,
     GetDataSetImportTaskResponseTypeDef,
     GetDeploymentResponseTypeDef,
     GetEnvironmentResponseTypeDef,
+    GetSignedBluinsightsUrlResponseTypeDef,
     HighAvailabilityConfigTypeDef,
     ListApplicationsResponseTypeDef,
     ListApplicationVersionsResponseTypeDef,
     ListBatchJobDefinitionsResponseTypeDef,
     ListBatchJobExecutionsResponseTypeDef,
     ListDataSetImportHistoryResponseTypeDef,
     ListDataSetsResponseTypeDef,
@@ -291,14 +292,21 @@
     async def get_environment(self, *, environmentId: str) -> GetEnvironmentResponseTypeDef:
         """
         Describes a specific runtime environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#get_environment)
         """
+    async def get_signed_bluinsights_url(self) -> GetSignedBluinsightsUrlResponseTypeDef:
+        """
+        Gets a single sign-on URL that can be used to connect to AWS Blu Insights.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.get_signed_bluinsights_url)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_m2/client/#get_signed_bluinsights_url)
+        """
     async def list_application_versions(
         self, *, applicationId: str, maxResults: int = ..., nextToken: str = ...
     ) -> ListApplicationVersionsResponseTypeDef:
         """
         Returns a list of the application versions for a specific application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#MainframeModernization.Client.list_application_versions)
```

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/literals.py` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/literals.py`

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

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/literals.pyi` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
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
@@ -199,14 +200,15 @@
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
@@ -285,26 +287,28 @@
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

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/paginator.py` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/paginator.pyi` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/type_defs.py` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     "UpdateApplicationRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "CreateDataSetImportTaskResponseTypeDef",
     "CreateDeploymentResponseTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "GetApplicationVersionResponseTypeDef",
     "GetDeploymentResponseTypeDef",
+    "GetSignedBluinsightsUrlResponseTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartBatchJobResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "DataSetImportTaskTypeDef",
@@ -1017,14 +1018,22 @@
         "environmentId": str,
         "status": DeploymentLifecycleType,
         "statusReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetSignedBluinsightsUrlResponseTypeDef = TypedDict(
+    "GetSignedBluinsightsUrlResponseTypeDef",
+    {
+        "signedBiUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "applicationVersions": List[ApplicationVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2/type_defs.pyi` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     "UpdateApplicationRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "CreateDataSetImportTaskResponseTypeDef",
     "CreateDeploymentResponseTypeDef",
     "CreateEnvironmentResponseTypeDef",
     "GetApplicationVersionResponseTypeDef",
     "GetDeploymentResponseTypeDef",
+    "GetSignedBluinsightsUrlResponseTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartBatchJobResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "DataSetImportTaskTypeDef",
@@ -974,14 +975,22 @@
         "environmentId": str,
         "status": DeploymentLifecycleType,
         "statusReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetSignedBluinsightsUrlResponseTypeDef = TypedDict(
+    "GetSignedBluinsightsUrlResponseTypeDef",
+    {
+        "signedBiUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListApplicationVersionsResponseTypeDef = TypedDict(
     "ListApplicationVersionsResponseTypeDef",
     {
         "applicationVersions": List[ApplicationVersionSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-m2-2.5.2.post1/types_aiobotocore_m2.egg-info/SOURCES.txt` & `types-aiobotocore-m2-2.5.2.post2/types_aiobotocore_m2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

