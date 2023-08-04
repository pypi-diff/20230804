# Comparing `tmp/types-aiobotocore-mediaconnect-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mediaconnect-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediaconnect-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediaconnect-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
```

## Comparing `types-aiobotocore-mediaconnect-2.5.2.post1.tar` & `types-aiobotocore-mediaconnect-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.289527 types-aiobotocore-mediaconnect-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:51.000000 types-aiobotocore-mediaconnect-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-08-02 14:52:38.281527 types-aiobotocore-mediaconnect-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20954 2023-08-02 14:42:51.000000 types-aiobotocore-mediaconnect-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:38.289527 types-aiobotocore-mediaconnect-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:42:51.000000 types-aiobotocore-mediaconnect-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.273527 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-02 14:42:51.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 14:42:51.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:42:51.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42802 2023-08-02 14:42:52.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42733 2023-08-02 14:42:52.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11819 2023-08-02 14:42:52.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11817 2023-08-02 14:42:52.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-08-02 14:42:52.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-02 14:42:52.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:51.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64964 2023-08-02 14:42:56.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-08-02 14:42:55.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:51.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-02 14:42:52.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-02 14:42:52.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.281527 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.326643 types-aiobotocore-mediaconnect-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14917 2023-08-04 13:59:17.326643 types-aiobotocore-mediaconnect-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13379 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.326643 types-aiobotocore-mediaconnect-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.326643 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2311 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2310 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    42802 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    42733 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11974 2023-08-04 13:43:59.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11972 2023-08-04 13:43:59.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8625 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8616 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    64964 2023-08-04 13:44:01.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    64873 2023-08-04 13:44:01.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3403 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3400 2023-08-04 13:43:58.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.326643 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14917 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      991 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/LICENSE` & `types-aiobotocore-mediaconnect-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/setup.py` & `types-aiobotocore-mediaconnect-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediaconnect",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mediaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MediaConnect 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/__init__.py` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/__init__.pyi` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/__main__.py` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaConnect 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MediaConnect 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect\nOther"
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

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/client.py` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/client.pyi` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/literals.py` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,15 @@
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
@@ -254,14 +255,15 @@
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
@@ -340,26 +342,28 @@
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
@@ -510,20 +514,23 @@
     "list_gateway_instances",
     "list_gateways",
     "list_offerings",
     "list_reservations",
 ]
 WaiterName = Literal["flow_active", "flow_deleted", "flow_standby"]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "sa-east-1",
     "us-east-1",
```

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/literals.pyi` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,15 @@
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
@@ -252,14 +253,15 @@
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
@@ -338,26 +340,28 @@
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
@@ -508,20 +512,23 @@
     "list_gateway_instances",
     "list_gateways",
     "list_offerings",
     "list_reservations",
 ]
 WaiterName = Literal["flow_active", "flow_deleted", "flow_standby"]
 RegionName = Literal[
+    "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
+    "ap-northeast-3",
     "ap-south-1",
     "ap-southeast-1",
     "ap-southeast-2",
+    "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
     "sa-east-1",
     "us-east-1",
```

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/paginator.py` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/paginator.pyi` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/type_defs.py` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/type_defs.pyi` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/waiter.py` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect/waiter.pyi` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.5.2.post1/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt` & `types-aiobotocore-mediaconnect-2.5.2.post2/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

