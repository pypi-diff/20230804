# Comparing `tmp/types-aiobotocore-sns-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sns-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sns-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:03 2023, max compression
+gzip compressed data, was "types-aiobotocore-sns-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-sns-2.5.2.post1.tar` & `types-aiobotocore-sns-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.221451 types-aiobotocore-sns-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:55.000000 types-aiobotocore-sns-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-08-02 14:53:03.221451 types-aiobotocore-sns-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19885 2023-08-02 14:49:55.000000 types-aiobotocore-sns-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:03.221451 types-aiobotocore-sns-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:49:55.000000 types-aiobotocore-sns-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.221451 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-02 14:49:55.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-02 14:49:55.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:49:55.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35353 2023-08-02 14:49:55.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35294 2023-08-02 14:49:55.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-08-02 14:49:56.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-08-02 14:49:56.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10074 2023-08-02 14:49:56.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-08-02 14:49:56.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:55.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37388 2023-08-02 14:49:56.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    37313 2023-08-02 14:49:56.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34610 2023-08-02 14:49:56.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34563 2023-08-02 14:49:56.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:55.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:03.221451 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21387 2023-08-02 14:53:03.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-02 14:53:03.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:03.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:03.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:03.000000 types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.356643 types-aiobotocore-sns-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16539 2023-08-04 13:59:27.336643 types-aiobotocore-sns-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15037 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.356643 types-aiobotocore-sns-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.336643 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2599 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2597 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35353 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35294 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9976 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9974 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10074 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10064 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37388 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/service_resource.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37313 2023-08-04 13:53:59.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/service_resource.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34610 2023-08-04 13:54:00.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34563 2023-08-04 13:54:00.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:55.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.336643 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16539 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      822 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:27.000000 types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sns-2.5.2.post1/LICENSE` & `types-aiobotocore-sns-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/setup.py` & `types-aiobotocore-sns-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sns",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sns"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SNS 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/__init__.py` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/__init__.pyi` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/__main__.py` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SNS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SNS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sns//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS\nOther"
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

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/client.py` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/client.pyi` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/literals.py` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
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
@@ -181,14 +182,15 @@
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
@@ -267,26 +269,28 @@
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
@@ -457,14 +461,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/literals.pyi` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/literals.pyi`

 * *Files 2% similar despite different names*

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
@@ -455,14 +459,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/paginator.py` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/paginator.pyi` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/service_resource.py` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/service_resource.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/service_resource.pyi` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/type_defs.py` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns/type_defs.pyi` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sns-2.5.2.post1/types_aiobotocore_sns.egg-info/SOURCES.txt` & `types-aiobotocore-sns-2.5.2.post2/types_aiobotocore_sns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

