# Comparing `tmp/types-aiobotocore-kinesisanalyticsv2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kinesisanalyticsv2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisanalyticsv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisanalyticsv2-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
```

## Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1.tar` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.513548 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-08-02 14:52:31.513548 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20055 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:31.513548 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.509548 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29367 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29325 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-08-02 14:41:36.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-08-02 14:41:35.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    69867 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69764 2023-08-02 14:41:36.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:33.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.513548 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.326643 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13781 2023-08-04 13:59:14.316643 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12219 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.326643 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2149 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.316643 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1010 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1009 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      987 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29367 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    29325 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10103 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10101 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3422 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3418 2023-08-04 13:42:09.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    69136 2023-08-04 13:42:11.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    69035 2023-08-04 13:42:10.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:08.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.316643 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13781 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1022 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       37 2023-08-04 13:59:14.000000 types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/LICENSE` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/setup.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisanalyticsv2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kinesisanalyticsv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__init__.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__init__.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/__main__.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.KinesisAnalyticsV2 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2\nOther"
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

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/client.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/client.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/literals.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     "FLINK-1_13",
     "FLINK-1_15",
     "FLINK-1_6",
     "FLINK-1_8",
     "SQL-1_0",
     "ZEPPELIN-FLINK-1_0",
     "ZEPPELIN-FLINK-2_0",
+    "ZEPPELIN-FLINK-3_0",
 ]
 SnapshotStatusType = Literal["CREATING", "DELETING", "FAILED", "READY"]
 UrlTypeType = Literal["FLINK_DASHBOARD_URL", "ZEPPELIN_UI_URL"]
 KinesisAnalyticsV2ServiceName = Literal["kinesisanalyticsv2"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -93,14 +94,15 @@
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
@@ -196,14 +198,15 @@
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
@@ -282,26 +285,28 @@
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

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/literals.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     "FLINK-1_13",
     "FLINK-1_15",
     "FLINK-1_6",
     "FLINK-1_8",
     "SQL-1_0",
     "ZEPPELIN-FLINK-1_0",
     "ZEPPELIN-FLINK-2_0",
+    "ZEPPELIN-FLINK-3_0",
 ]
 SnapshotStatusType = Literal["CREATING", "DELETING", "FAILED", "READY"]
 UrlTypeType = Literal["FLINK_DASHBOARD_URL", "ZEPPELIN_UI_URL"]
 KinesisAnalyticsV2ServiceName = Literal["kinesisanalyticsv2"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -91,14 +92,15 @@
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
@@ -194,14 +196,15 @@
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
@@ -280,26 +283,28 @@
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

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/paginator.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/paginator.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/type_defs.py` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     "SnapshotDetailsTypeDef",
     "DescribeApplicationVersionRequestRequestTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "PropertyGroupTypeDef",
-    "PropertyGroupOutputTypeDef",
     "MonitoringConfigurationDescriptionTypeDef",
     "ParallelismConfigurationDescriptionTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParallelismConfigurationTypeDef",
     "MonitoringConfigurationUpdateTypeDef",
     "ParallelismConfigurationUpdateTypeDef",
     "FlinkRunConfigurationTypeDef",
@@ -160,16 +159,16 @@
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     "DeployAsApplicationConfigurationTypeDef",
     "DeployAsApplicationConfigurationUpdateTypeDef",
     "DescribeApplicationSnapshotResponseTypeDef",
     "ListApplicationSnapshotsResponseTypeDef",
     "SqlRunConfigurationTypeDef",
     "EnvironmentPropertiesTypeDef",
-    "EnvironmentPropertyUpdatesTypeDef",
     "EnvironmentPropertyDescriptionsTypeDef",
+    "EnvironmentPropertyUpdatesTypeDef",
     "FlinkApplicationConfigurationDescriptionTypeDef",
     "FlinkApplicationConfigurationTypeDef",
     "FlinkApplicationConfigurationUpdateTypeDef",
     "RunConfigurationDescriptionTypeDef",
     "RunConfigurationUpdateTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
@@ -191,27 +190,26 @@
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputResponseTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "InputSchemaUpdateTypeDef",
-    "SourceSchemaOutputTypeDef",
     "SourceSchemaTypeDef",
     "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
-    "ReferenceDataSourceDescriptionTypeDef",
     "InputTypeDef",
+    "ReferenceDataSourceDescriptionTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
     "AddApplicationInputResponseTypeDef",
+    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceResponseTypeDef",
     "SqlApplicationConfigurationDescriptionTypeDef",
-    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "SqlApplicationConfigurationTypeDef",
     "SqlApplicationConfigurationUpdateTypeDef",
     "ApplicationConfigurationDescriptionTypeDef",
     "ApplicationConfigurationTypeDef",
     "ApplicationConfigurationUpdateTypeDef",
     "ApplicationDetailTypeDef",
@@ -819,22 +817,14 @@
     "PropertyGroupTypeDef",
     {
         "PropertyGroupId": str,
         "PropertyMap": Mapping[str, str],
     },
 )
 
-PropertyGroupOutputTypeDef = TypedDict(
-    "PropertyGroupOutputTypeDef",
-    {
-        "PropertyGroupId": str,
-        "PropertyMap": Dict[str, str],
-    },
-)
-
 MonitoringConfigurationDescriptionTypeDef = TypedDict(
     "MonitoringConfigurationDescriptionTypeDef",
     {
         "ConfigurationType": ConfigurationTypeType,
         "MetricsLevel": MetricsLevelType,
         "LogLevel": LogLevelType,
     },
@@ -1680,27 +1670,27 @@
 EnvironmentPropertiesTypeDef = TypedDict(
     "EnvironmentPropertiesTypeDef",
     {
         "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
 )
 
-EnvironmentPropertyUpdatesTypeDef = TypedDict(
-    "EnvironmentPropertyUpdatesTypeDef",
+EnvironmentPropertyDescriptionsTypeDef = TypedDict(
+    "EnvironmentPropertyDescriptionsTypeDef",
     {
-        "PropertyGroups": Sequence[PropertyGroupTypeDef],
+        "PropertyGroupDescriptions": List[PropertyGroupTypeDef],
     },
+    total=False,
 )
 
-EnvironmentPropertyDescriptionsTypeDef = TypedDict(
-    "EnvironmentPropertyDescriptionsTypeDef",
+EnvironmentPropertyUpdatesTypeDef = TypedDict(
+    "EnvironmentPropertyUpdatesTypeDef",
     {
-        "PropertyGroupDescriptions": List[PropertyGroupOutputTypeDef],
+        "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
-    total=False,
 )
 
 FlinkApplicationConfigurationDescriptionTypeDef = TypedDict(
     "FlinkApplicationConfigurationDescriptionTypeDef",
     {
         "CheckpointConfigurationDescription": CheckpointConfigurationDescriptionTypeDef,
         "MonitoringConfigurationDescription": MonitoringConfigurationDescriptionTypeDef,
@@ -2090,36 +2080,14 @@
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
     },
     total=False,
 )
 
-_RequiredSourceSchemaOutputTypeDef = TypedDict(
-    "_RequiredSourceSchemaOutputTypeDef",
-    {
-        "RecordFormat": RecordFormatTypeDef,
-        "RecordColumns": List[RecordColumnTypeDef],
-    },
-)
-_OptionalSourceSchemaOutputTypeDef = TypedDict(
-    "_OptionalSourceSchemaOutputTypeDef",
-    {
-        "RecordEncoding": str,
-    },
-    total=False,
-)
-
-
-class SourceSchemaOutputTypeDef(
-    _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
-):
-    pass
-
-
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
 )
@@ -2159,15 +2127,15 @@
 class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
     pass
 
 
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
-        "InputSchema": SourceSchemaOutputTypeDef,
+        "InputSchema": SourceSchemaTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2176,64 +2144,64 @@
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
-        "InputSchema": SourceSchemaOutputTypeDef,
+        "InputSchema": SourceSchemaTypeDef,
         "InputParallelism": InputParallelismTypeDef,
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_RequiredReferenceDataSourceDescriptionTypeDef",
+_RequiredInputTypeDef = TypedDict(
+    "_RequiredInputTypeDef",
     {
-        "ReferenceId": str,
-        "TableName": str,
-        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
+        "NamePrefix": str,
+        "InputSchema": SourceSchemaTypeDef,
     },
 )
-_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_OptionalReferenceDataSourceDescriptionTypeDef",
+_OptionalInputTypeDef = TypedDict(
+    "_OptionalInputTypeDef",
     {
-        "ReferenceSchema": SourceSchemaOutputTypeDef,
+        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
+        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
+        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
+        "InputParallelism": InputParallelismTypeDef,
     },
     total=False,
 )
 
 
-class ReferenceDataSourceDescriptionTypeDef(
-    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
-):
+class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
 
-_RequiredInputTypeDef = TypedDict(
-    "_RequiredInputTypeDef",
+_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_RequiredReferenceDataSourceDescriptionTypeDef",
     {
-        "NamePrefix": str,
-        "InputSchema": SourceSchemaTypeDef,
+        "ReferenceId": str,
+        "TableName": str,
+        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
     },
 )
-_OptionalInputTypeDef = TypedDict(
-    "_OptionalInputTypeDef",
+_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_OptionalReferenceDataSourceDescriptionTypeDef",
     {
-        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
-        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
-        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
-        "InputParallelism": InputParallelismTypeDef,
+        "ReferenceSchema": SourceSchemaTypeDef,
     },
     total=False,
 )
 
 
-class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
+class ReferenceDataSourceDescriptionTypeDef(
+    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
+):
     pass
 
 
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
@@ -2284,14 +2252,23 @@
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputDescriptions": List[InputDescriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AddApplicationInputRequestRequestTypeDef = TypedDict(
+    "AddApplicationInputRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CurrentApplicationVersionId": int,
+        "Input": InputTypeDef,
+    },
+)
+
 AddApplicationReferenceDataSourceResponseTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2304,23 +2281,14 @@
         "InputDescriptions": List[InputDescriptionTypeDef],
         "OutputDescriptions": List[OutputDescriptionTypeDef],
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
     },
     total=False,
 )
 
-AddApplicationInputRequestRequestTypeDef = TypedDict(
-    "AddApplicationInputRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CurrentApplicationVersionId": int,
-        "Input": InputTypeDef,
-    },
-)
-
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     "DescribeApplicationSnapshotRequestRequestTypeDef",
     "SnapshotDetailsTypeDef",
     "DescribeApplicationVersionRequestRequestTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "PropertyGroupTypeDef",
-    "PropertyGroupOutputTypeDef",
     "MonitoringConfigurationDescriptionTypeDef",
     "ParallelismConfigurationDescriptionTypeDef",
     "MonitoringConfigurationTypeDef",
     "ParallelismConfigurationTypeDef",
     "MonitoringConfigurationUpdateTypeDef",
     "ParallelismConfigurationUpdateTypeDef",
     "FlinkRunConfigurationTypeDef",
@@ -159,16 +158,16 @@
     "DeployAsApplicationConfigurationDescriptionTypeDef",
     "DeployAsApplicationConfigurationTypeDef",
     "DeployAsApplicationConfigurationUpdateTypeDef",
     "DescribeApplicationSnapshotResponseTypeDef",
     "ListApplicationSnapshotsResponseTypeDef",
     "SqlRunConfigurationTypeDef",
     "EnvironmentPropertiesTypeDef",
-    "EnvironmentPropertyUpdatesTypeDef",
     "EnvironmentPropertyDescriptionsTypeDef",
+    "EnvironmentPropertyUpdatesTypeDef",
     "FlinkApplicationConfigurationDescriptionTypeDef",
     "FlinkApplicationConfigurationTypeDef",
     "FlinkApplicationConfigurationUpdateTypeDef",
     "RunConfigurationDescriptionTypeDef",
     "RunConfigurationUpdateTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
@@ -190,27 +189,26 @@
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputResponseTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "InputSchemaUpdateTypeDef",
-    "SourceSchemaOutputTypeDef",
     "SourceSchemaTypeDef",
     "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
-    "ReferenceDataSourceDescriptionTypeDef",
     "InputTypeDef",
+    "ReferenceDataSourceDescriptionTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
     "AddApplicationInputResponseTypeDef",
+    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceResponseTypeDef",
     "SqlApplicationConfigurationDescriptionTypeDef",
-    "AddApplicationInputRequestRequestTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "SqlApplicationConfigurationTypeDef",
     "SqlApplicationConfigurationUpdateTypeDef",
     "ApplicationConfigurationDescriptionTypeDef",
     "ApplicationConfigurationTypeDef",
     "ApplicationConfigurationUpdateTypeDef",
     "ApplicationDetailTypeDef",
@@ -786,22 +784,14 @@
     "PropertyGroupTypeDef",
     {
         "PropertyGroupId": str,
         "PropertyMap": Mapping[str, str],
     },
 )
 
-PropertyGroupOutputTypeDef = TypedDict(
-    "PropertyGroupOutputTypeDef",
-    {
-        "PropertyGroupId": str,
-        "PropertyMap": Dict[str, str],
-    },
-)
-
 MonitoringConfigurationDescriptionTypeDef = TypedDict(
     "MonitoringConfigurationDescriptionTypeDef",
     {
         "ConfigurationType": ConfigurationTypeType,
         "MetricsLevel": MetricsLevelType,
         "LogLevel": LogLevelType,
     },
@@ -1615,27 +1605,27 @@
 EnvironmentPropertiesTypeDef = TypedDict(
     "EnvironmentPropertiesTypeDef",
     {
         "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
 )
 
-EnvironmentPropertyUpdatesTypeDef = TypedDict(
-    "EnvironmentPropertyUpdatesTypeDef",
+EnvironmentPropertyDescriptionsTypeDef = TypedDict(
+    "EnvironmentPropertyDescriptionsTypeDef",
     {
-        "PropertyGroups": Sequence[PropertyGroupTypeDef],
+        "PropertyGroupDescriptions": List[PropertyGroupTypeDef],
     },
+    total=False,
 )
 
-EnvironmentPropertyDescriptionsTypeDef = TypedDict(
-    "EnvironmentPropertyDescriptionsTypeDef",
+EnvironmentPropertyUpdatesTypeDef = TypedDict(
+    "EnvironmentPropertyUpdatesTypeDef",
     {
-        "PropertyGroupDescriptions": List[PropertyGroupOutputTypeDef],
+        "PropertyGroups": Sequence[PropertyGroupTypeDef],
     },
-    total=False,
 )
 
 FlinkApplicationConfigurationDescriptionTypeDef = TypedDict(
     "FlinkApplicationConfigurationDescriptionTypeDef",
     {
         "CheckpointConfigurationDescription": CheckpointConfigurationDescriptionTypeDef,
         "MonitoringConfigurationDescription": MonitoringConfigurationDescriptionTypeDef,
@@ -2007,34 +1997,14 @@
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
     },
     total=False,
 )
 
-_RequiredSourceSchemaOutputTypeDef = TypedDict(
-    "_RequiredSourceSchemaOutputTypeDef",
-    {
-        "RecordFormat": RecordFormatTypeDef,
-        "RecordColumns": List[RecordColumnTypeDef],
-    },
-)
-_OptionalSourceSchemaOutputTypeDef = TypedDict(
-    "_OptionalSourceSchemaOutputTypeDef",
-    {
-        "RecordEncoding": str,
-    },
-    total=False,
-)
-
-class SourceSchemaOutputTypeDef(
-    _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
-):
-    pass
-
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
 )
@@ -2070,15 +2040,15 @@
 
 class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
     pass
 
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
-        "InputSchema": SourceSchemaOutputTypeDef,
+        "InputSchema": SourceSchemaTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -2087,42 +2057,21 @@
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
-        "InputSchema": SourceSchemaOutputTypeDef,
+        "InputSchema": SourceSchemaTypeDef,
         "InputParallelism": InputParallelismTypeDef,
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_RequiredReferenceDataSourceDescriptionTypeDef",
-    {
-        "ReferenceId": str,
-        "TableName": str,
-        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
-    },
-)
-_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_OptionalReferenceDataSourceDescriptionTypeDef",
-    {
-        "ReferenceSchema": SourceSchemaOutputTypeDef,
-    },
-    total=False,
-)
-
-class ReferenceDataSourceDescriptionTypeDef(
-    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
-):
-    pass
-
 _RequiredInputTypeDef = TypedDict(
     "_RequiredInputTypeDef",
     {
         "NamePrefix": str,
         "InputSchema": SourceSchemaTypeDef,
     },
 )
@@ -2136,14 +2085,35 @@
     },
     total=False,
 )
 
 class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
+_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_RequiredReferenceDataSourceDescriptionTypeDef",
+    {
+        "ReferenceId": str,
+        "TableName": str,
+        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
+    },
+)
+_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_OptionalReferenceDataSourceDescriptionTypeDef",
+    {
+        "ReferenceSchema": SourceSchemaTypeDef,
+    },
+    total=False,
+)
+
+class ReferenceDataSourceDescriptionTypeDef(
+    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
+):
+    pass
+
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
         "ReferenceSchema": SourceSchemaTypeDef,
     },
 )
@@ -2187,14 +2157,23 @@
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "InputDescriptions": List[InputDescriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AddApplicationInputRequestRequestTypeDef = TypedDict(
+    "AddApplicationInputRequestRequestTypeDef",
+    {
+        "ApplicationName": str,
+        "CurrentApplicationVersionId": int,
+        "Input": InputTypeDef,
+    },
+)
+
 AddApplicationReferenceDataSourceResponseTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceResponseTypeDef",
     {
         "ApplicationARN": str,
         "ApplicationVersionId": int,
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2207,23 +2186,14 @@
         "InputDescriptions": List[InputDescriptionTypeDef],
         "OutputDescriptions": List[OutputDescriptionTypeDef],
         "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
     },
     total=False,
 )
 
-AddApplicationInputRequestRequestTypeDef = TypedDict(
-    "AddApplicationInputRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CurrentApplicationVersionId": int,
-        "Input": InputTypeDef,
-    },
-)
-
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.5.2.post1/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisanalyticsv2-2.5.2.post2/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

