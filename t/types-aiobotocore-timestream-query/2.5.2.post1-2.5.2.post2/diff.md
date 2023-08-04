# Comparing `tmp/types-aiobotocore-timestream-query-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-timestream-query-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-timestream-query-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-timestream-query-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
```

## Comparing `types-aiobotocore-timestream-query-2.5.2.post1.tar` & `types-aiobotocore-timestream-query-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.965439 types-aiobotocore-timestream-query-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-08-02 14:53:06.965439 types-aiobotocore-timestream-query-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.965439 types-aiobotocore-timestream-query-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.965439 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14514 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21902 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.965439 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.636643 types-aiobotocore-timestream-query-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13750 2023-08-04 13:59:28.636643 types-aiobotocore-timestream-query-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12197 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.636643 types-aiobotocore-timestream-query-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2134 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.636643 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1117 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1116 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      977 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14504 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14479 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8978 2023-08-04 13:55:04.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8976 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4436 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4431 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19511 2023-08-04 13:55:04.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19480 2023-08-04 13:55:04.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:03.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.636643 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13750 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      984 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:28.000000 types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/LICENSE` & `types-aiobotocore-timestream-query-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/setup.py` & `types-aiobotocore-timestream-query-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-timestream-query",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.TimestreamQuery 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__init__.py` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__init__.pyi` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__main__.py` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.TimestreamQuery 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\nOther"
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

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/client.py` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ListScheduledQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    TargetConfigurationUnionTypeDef,
+    TargetConfigurationTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -116,15 +116,15 @@
         *,
         Name: str,
         QueryString: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
-        TargetConfiguration: TargetConfigurationUnionTypeDef = ...,
+        TargetConfiguration: TargetConfigurationTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
```

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/client.pyi` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ListScheduledQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    TargetConfigurationUnionTypeDef,
+    TargetConfigurationTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -108,15 +108,15 @@
         *,
         Name: str,
         QueryString: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
-        TargetConfiguration: TargetConfigurationUnionTypeDef = ...,
+        TargetConfiguration: TargetConfigurationTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
```

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/literals.py` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
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
@@ -179,14 +180,15 @@
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
@@ -265,26 +267,28 @@
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

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/literals.pyi` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
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
@@ -177,14 +178,15 @@
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
@@ -263,26 +265,28 @@
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

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/paginator.py` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/paginator.pyi` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/type_defs.py` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelQueryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
     "RowTypeDef",
@@ -73,32 +72,27 @@
     "DescribeEndpointsResponseTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
     "ExecuteScheduledQueryRequestRequestTypeDef",
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "QueryRequestQueryPaginateTypeDef",
-    "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
-    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
-    "TimestreamConfigurationOutputTypeDef",
     "TimestreamConfigurationTypeDef",
     "ScheduledQueryTypeDef",
-    "TargetConfigurationOutputTypeDef",
     "TargetConfigurationTypeDef",
     "ListScheduledQueriesResponseTypeDef",
-    "ScheduledQueryDescriptionTypeDef",
     "CreateScheduledQueryRequestRequestTypeDef",
-    "TargetConfigurationUnionTypeDef",
+    "ScheduledQueryDescriptionTypeDef",
     "DescribeScheduledQueryResponseTypeDef",
 )
 
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
@@ -126,19 +120,17 @@
     "_OptionalColumnInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class ColumnInfoTypeDef(_RequiredColumnInfoTypeDef, _OptionalColumnInfoTypeDef):
     pass
 
-
 ScheduleConfigurationTypeDef = TypedDict(
     "ScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
@@ -206,19 +198,17 @@
     {
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
     },
     total=False,
 )
 
-
 class S3ConfigurationTypeDef(_RequiredS3ConfigurationTypeDef, _OptionalS3ConfigurationTypeDef):
     pass
 
-
 S3ReportLocationTypeDef = TypedDict(
     "S3ReportLocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
@@ -267,22 +257,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredMultiMeasureAttributeMappingTypeDef = TypedDict(
     "_RequiredMultiMeasureAttributeMappingTypeDef",
     {
         "SourceColumn": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
 )
@@ -290,21 +278,19 @@
     "_OptionalMultiMeasureAttributeMappingTypeDef",
     {
         "TargetMultiMeasureAttributeName": str,
     },
     total=False,
 )
 
-
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
-
 SnsConfigurationTypeDef = TypedDict(
     "SnsConfigurationTypeDef",
     {
         "TopicArn": str,
     },
 )
 
@@ -326,21 +312,19 @@
     "_OptionalPrepareQueryRequestRequestTypeDef",
     {
         "ValidateOnly": bool,
     },
     total=False,
 )
 
-
 class PrepareQueryRequestRequestTypeDef(
     _RequiredPrepareQueryRequestRequestTypeDef, _OptionalPrepareQueryRequestRequestTypeDef
 ):
     pass
 
-
 SelectColumnTypeDef = TypedDict(
     "SelectColumnTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
         "DatabaseName": str,
         "TableName": str,
@@ -361,21 +345,19 @@
         "ClientToken": str,
         "NextToken": str,
         "MaxRows": int,
     },
     total=False,
 )
 
-
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
-
 QueryStatusTypeDef = TypedDict(
     "QueryStatusTypeDef",
     {
         "ProgressPercentage": float,
         "CumulativeBytesScanned": int,
         "CumulativeBytesMetered": int,
     },
@@ -504,22 +486,20 @@
     "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class ExecuteScheduledQueryRequestRequestTypeDef(
     _RequiredExecuteScheduledQueryRequestRequestTypeDef,
     _OptionalExecuteScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
-
 ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -534,22 +514,20 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 _RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
     "_RequiredQueryRequestQueryPaginateTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
@@ -557,45 +535,19 @@
     {
         "ClientToken": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class QueryRequestQueryPaginateTypeDef(
     _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
 ):
     pass
 
-
-_RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
-    "_RequiredMixedMeasureMappingOutputTypeDef",
-    {
-        "MeasureValueType": MeasureValueTypeType,
-    },
-)
-_OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
-    "_OptionalMixedMeasureMappingOutputTypeDef",
-    {
-        "MeasureName": str,
-        "SourceColumn": str,
-        "TargetMeasureName": str,
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
-    },
-    total=False,
-)
-
-
-class MixedMeasureMappingOutputTypeDef(
-    _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
-):
-    pass
-
-
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -605,63 +557,38 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
-
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
-
-_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureMappingsOutputTypeDef",
-    {
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
-    },
-)
-_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureMappingsOutputTypeDef",
-    {
-        "TargetMultiMeasureName": str,
-    },
-    total=False,
-)
-
-
-class MultiMeasureMappingsOutputTypeDef(
-    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
-):
-    pass
-
-
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
-
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
-
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "SnsConfiguration": SnsConfigurationTypeDef,
     },
 )
 
@@ -704,40 +631,14 @@
         "ExecutionStats": ExecutionStatsTypeDef,
         "ErrorReportLocation": ErrorReportLocationTypeDef,
         "FailureReason": str,
     },
     total=False,
 )
 
-_RequiredTimestreamConfigurationOutputTypeDef = TypedDict(
-    "_RequiredTimestreamConfigurationOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "TimeColumn": str,
-        "DimensionMappings": List[DimensionMappingTypeDef],
-    },
-)
-_OptionalTimestreamConfigurationOutputTypeDef = TypedDict(
-    "_OptionalTimestreamConfigurationOutputTypeDef",
-    {
-        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
-        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
-        "MeasureNameColumn": str,
-    },
-    total=False,
-)
-
-
-class TimestreamConfigurationOutputTypeDef(
-    _RequiredTimestreamConfigurationOutputTypeDef, _OptionalTimestreamConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredTimestreamConfigurationTypeDef = TypedDict(
     "_RequiredTimestreamConfigurationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
@@ -749,21 +650,19 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
-
 class TimestreamConfigurationTypeDef(
     _RequiredTimestreamConfigurationTypeDef, _OptionalTimestreamConfigurationTypeDef
 ):
     pass
 
-
 _RequiredScheduledQueryTypeDef = TypedDict(
     "_RequiredScheduledQueryTypeDef",
     {
         "Arn": str,
         "Name": str,
         "State": ScheduledQueryStateType,
     },
@@ -777,26 +676,17 @@
         "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
         "TargetDestination": TargetDestinationTypeDef,
         "LastRunStatus": ScheduledQueryRunStatusType,
     },
     total=False,
 )
 
-
 class ScheduledQueryTypeDef(_RequiredScheduledQueryTypeDef, _OptionalScheduledQueryTypeDef):
     pass
 
-
-TargetConfigurationOutputTypeDef = TypedDict(
-    "TargetConfigurationOutputTypeDef",
-    {
-        "TimestreamConfiguration": TimestreamConfigurationOutputTypeDef,
-    },
-)
-
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "TimestreamConfiguration": TimestreamConfigurationTypeDef,
     },
 )
 
@@ -805,81 +695,74 @@
     {
         "ScheduledQueries": List[ScheduledQueryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
-    "_RequiredScheduledQueryDescriptionTypeDef",
+_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
     {
-        "Arn": str,
         "Name": str,
         "QueryString": str,
-        "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
     },
 )
-_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
-    "_OptionalScheduledQueryDescriptionTypeDef",
+_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
     {
-        "CreationTime": datetime,
-        "PreviousInvocationTime": datetime,
-        "NextInvocationTime": datetime,
-        "TargetConfiguration": TargetConfigurationOutputTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
+        "TargetConfiguration": TargetConfigurationTypeDef,
+        "ClientToken": str,
+        "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
-        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
-        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-
-class ScheduledQueryDescriptionTypeDef(
-    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
+class CreateScheduledQueryRequestRequestTypeDef(
+    _RequiredCreateScheduledQueryRequestRequestTypeDef,
+    _OptionalCreateScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
+_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
+    "_RequiredScheduledQueryDescriptionTypeDef",
     {
+        "Arn": str,
         "Name": str,
         "QueryString": str,
+        "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
     },
 )
-_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
+_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
+    "_OptionalScheduledQueryDescriptionTypeDef",
     {
+        "CreationTime": datetime,
+        "PreviousInvocationTime": datetime,
+        "NextInvocationTime": datetime,
         "TargetConfiguration": TargetConfigurationTypeDef,
-        "ClientToken": str,
-        "Tags": Sequence[TagTypeDef],
+        "ScheduledQueryExecutionRoleArn": str,
         "KmsKeyId": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
+        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
+        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-
-class CreateScheduledQueryRequestRequestTypeDef(
-    _RequiredCreateScheduledQueryRequestRequestTypeDef,
-    _OptionalCreateScheduledQueryRequestRequestTypeDef,
+class ScheduledQueryDescriptionTypeDef(
+    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
 ):
     pass
 
-
-TargetConfigurationUnionTypeDef = Union[
-    TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
-]
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/type_defs.pyi` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelQueryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
     "RowTypeDef",
@@ -72,32 +73,27 @@
     "DescribeEndpointsResponseTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
     "ExecuteScheduledQueryRequestRequestTypeDef",
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "QueryRequestQueryPaginateTypeDef",
-    "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
-    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
-    "TimestreamConfigurationOutputTypeDef",
     "TimestreamConfigurationTypeDef",
     "ScheduledQueryTypeDef",
-    "TargetConfigurationOutputTypeDef",
     "TargetConfigurationTypeDef",
     "ListScheduledQueriesResponseTypeDef",
-    "ScheduledQueryDescriptionTypeDef",
     "CreateScheduledQueryRequestRequestTypeDef",
-    "TargetConfigurationUnionTypeDef",
+    "ScheduledQueryDescriptionTypeDef",
     "DescribeScheduledQueryResponseTypeDef",
 )
 
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
@@ -125,17 +121,19 @@
     "_OptionalColumnInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class ColumnInfoTypeDef(_RequiredColumnInfoTypeDef, _OptionalColumnInfoTypeDef):
     pass
 
+
 ScheduleConfigurationTypeDef = TypedDict(
     "ScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
@@ -203,17 +201,19 @@
     {
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
     },
     total=False,
 )
 
+
 class S3ConfigurationTypeDef(_RequiredS3ConfigurationTypeDef, _OptionalS3ConfigurationTypeDef):
     pass
 
+
 S3ReportLocationTypeDef = TypedDict(
     "S3ReportLocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
@@ -262,20 +262,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredMultiMeasureAttributeMappingTypeDef = TypedDict(
     "_RequiredMultiMeasureAttributeMappingTypeDef",
     {
         "SourceColumn": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
 )
@@ -283,19 +285,21 @@
     "_OptionalMultiMeasureAttributeMappingTypeDef",
     {
         "TargetMultiMeasureAttributeName": str,
     },
     total=False,
 )
 
+
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
+
 SnsConfigurationTypeDef = TypedDict(
     "SnsConfigurationTypeDef",
     {
         "TopicArn": str,
     },
 )
 
@@ -317,19 +321,21 @@
     "_OptionalPrepareQueryRequestRequestTypeDef",
     {
         "ValidateOnly": bool,
     },
     total=False,
 )
 
+
 class PrepareQueryRequestRequestTypeDef(
     _RequiredPrepareQueryRequestRequestTypeDef, _OptionalPrepareQueryRequestRequestTypeDef
 ):
     pass
 
+
 SelectColumnTypeDef = TypedDict(
     "SelectColumnTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
         "DatabaseName": str,
         "TableName": str,
@@ -350,19 +356,21 @@
         "ClientToken": str,
         "NextToken": str,
         "MaxRows": int,
     },
     total=False,
 )
 
+
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
+
 QueryStatusTypeDef = TypedDict(
     "QueryStatusTypeDef",
     {
         "ProgressPercentage": float,
         "CumulativeBytesScanned": int,
         "CumulativeBytesMetered": int,
     },
@@ -491,20 +499,22 @@
     "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class ExecuteScheduledQueryRequestRequestTypeDef(
     _RequiredExecuteScheduledQueryRequestRequestTypeDef,
     _OptionalExecuteScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
+
 ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -519,20 +529,22 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+
 _RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
     "_RequiredQueryRequestQueryPaginateTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
@@ -540,40 +552,20 @@
     {
         "ClientToken": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class QueryRequestQueryPaginateTypeDef(
     _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
 ):
     pass
 
-_RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
-    "_RequiredMixedMeasureMappingOutputTypeDef",
-    {
-        "MeasureValueType": MeasureValueTypeType,
-    },
-)
-_OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
-    "_OptionalMixedMeasureMappingOutputTypeDef",
-    {
-        "MeasureName": str,
-        "SourceColumn": str,
-        "TargetMeasureName": str,
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
-    },
-    total=False,
-)
-
-class MixedMeasureMappingOutputTypeDef(
-    _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
-):
-    pass
 
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
@@ -584,37 +576,20 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
+
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
-_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureMappingsOutputTypeDef",
-    {
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
-    },
-)
-_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureMappingsOutputTypeDef",
-    {
-        "TargetMultiMeasureName": str,
-    },
-    total=False,
-)
-
-class MultiMeasureMappingsOutputTypeDef(
-    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
-):
-    pass
 
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
@@ -622,19 +597,21 @@
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
+
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
+
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "SnsConfiguration": SnsConfigurationTypeDef,
     },
 )
 
@@ -677,38 +654,14 @@
         "ExecutionStats": ExecutionStatsTypeDef,
         "ErrorReportLocation": ErrorReportLocationTypeDef,
         "FailureReason": str,
     },
     total=False,
 )
 
-_RequiredTimestreamConfigurationOutputTypeDef = TypedDict(
-    "_RequiredTimestreamConfigurationOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "TableName": str,
-        "TimeColumn": str,
-        "DimensionMappings": List[DimensionMappingTypeDef],
-    },
-)
-_OptionalTimestreamConfigurationOutputTypeDef = TypedDict(
-    "_OptionalTimestreamConfigurationOutputTypeDef",
-    {
-        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
-        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
-        "MeasureNameColumn": str,
-    },
-    total=False,
-)
-
-class TimestreamConfigurationOutputTypeDef(
-    _RequiredTimestreamConfigurationOutputTypeDef, _OptionalTimestreamConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredTimestreamConfigurationTypeDef = TypedDict(
     "_RequiredTimestreamConfigurationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
@@ -720,19 +673,21 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
+
 class TimestreamConfigurationTypeDef(
     _RequiredTimestreamConfigurationTypeDef, _OptionalTimestreamConfigurationTypeDef
 ):
     pass
 
+
 _RequiredScheduledQueryTypeDef = TypedDict(
     "_RequiredScheduledQueryTypeDef",
     {
         "Arn": str,
         "Name": str,
         "State": ScheduledQueryStateType,
     },
@@ -746,23 +701,18 @@
         "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
         "TargetDestination": TargetDestinationTypeDef,
         "LastRunStatus": ScheduledQueryRunStatusType,
     },
     total=False,
 )
 
+
 class ScheduledQueryTypeDef(_RequiredScheduledQueryTypeDef, _OptionalScheduledQueryTypeDef):
     pass
 
-TargetConfigurationOutputTypeDef = TypedDict(
-    "TargetConfigurationOutputTypeDef",
-    {
-        "TimestreamConfiguration": TimestreamConfigurationOutputTypeDef,
-    },
-)
 
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "TimestreamConfiguration": TimestreamConfigurationTypeDef,
     },
 )
@@ -772,77 +722,78 @@
     {
         "ScheduledQueries": List[ScheduledQueryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
-    "_RequiredScheduledQueryDescriptionTypeDef",
+_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
     {
-        "Arn": str,
         "Name": str,
         "QueryString": str,
-        "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
     },
 )
-_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
-    "_OptionalScheduledQueryDescriptionTypeDef",
+_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
     {
-        "CreationTime": datetime,
-        "PreviousInvocationTime": datetime,
-        "NextInvocationTime": datetime,
-        "TargetConfiguration": TargetConfigurationOutputTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
+        "TargetConfiguration": TargetConfigurationTypeDef,
+        "ClientToken": str,
+        "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
-        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
-        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-class ScheduledQueryDescriptionTypeDef(
-    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
+
+class CreateScheduledQueryRequestRequestTypeDef(
+    _RequiredCreateScheduledQueryRequestRequestTypeDef,
+    _OptionalCreateScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
+
+_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
+    "_RequiredScheduledQueryDescriptionTypeDef",
     {
+        "Arn": str,
         "Name": str,
         "QueryString": str,
+        "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
     },
 )
-_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
+_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
+    "_OptionalScheduledQueryDescriptionTypeDef",
     {
+        "CreationTime": datetime,
+        "PreviousInvocationTime": datetime,
+        "NextInvocationTime": datetime,
         "TargetConfiguration": TargetConfigurationTypeDef,
-        "ClientToken": str,
-        "Tags": Sequence[TagTypeDef],
+        "ScheduledQueryExecutionRoleArn": str,
         "KmsKeyId": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
+        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
+        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-class CreateScheduledQueryRequestRequestTypeDef(
-    _RequiredCreateScheduledQueryRequestRequestTypeDef,
-    _OptionalCreateScheduledQueryRequestRequestTypeDef,
+
+class ScheduledQueryDescriptionTypeDef(
+    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
 ):
     pass
 
-TargetConfigurationUnionTypeDef = Union[
-    TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
-]
+
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/SOURCES.txt` & `types-aiobotocore-timestream-query-2.5.2.post2/types_aiobotocore_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

