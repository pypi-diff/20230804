# Comparing `tmp/types-aiobotocore-neptune-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-neptune-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-neptune-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-neptune-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-neptune-2.5.2.post1.tar` & `types-aiobotocore-neptune-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.237512 types-aiobotocore-neptune-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-08-02 14:52:43.237512 types-aiobotocore-neptune-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24609 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.237512 types-aiobotocore-neptune-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.233512 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70608 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    70512 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-08-02 14:43:56.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-08-02 14:43:56.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22183 2023-08-02 14:43:56.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22165 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    84484 2023-08-02 14:43:57.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    84407 2023-08-02 14:43:57.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:55.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-02 14:43:56.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-02 14:43:56.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.237512 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:43.000000 types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.306643 types-aiobotocore-neptune-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16653 2023-08-04 13:59:19.306643 types-aiobotocore-neptune-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15135 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.306643 types-aiobotocore-neptune-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2072 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.306643 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5033 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5032 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      943 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    70608 2023-08-04 13:45:27.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    70512 2023-08-04 13:45:26.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11377 2023-08-04 13:45:28.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11375 2023-08-04 13:45:28.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22183 2023-08-04 13:45:28.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22165 2023-08-04 13:45:27.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    84484 2023-08-04 13:45:30.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    84407 2023-08-04 13:45:29.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:25.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2901 2023-08-04 13:45:28.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2899 2023-08-04 13:45:28.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.306643 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16653 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      886 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 13:59:19.000000 types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-neptune-2.5.2.post1/LICENSE` & `types-aiobotocore-neptune-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/setup.py` & `types-aiobotocore-neptune-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-neptune",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_neptune"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Neptune 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__init__.py` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__init__.pyi` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/__main__.py` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Neptune 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Neptune 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptune//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#Neptune\nOther"
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

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/client.py` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/client.pyi` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/literals.py` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/literals.py`

 * *Files 0% similar despite different names*

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
@@ -476,14 +480,15 @@
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

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/literals.pyi` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,15 @@
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
@@ -189,14 +190,15 @@
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
@@ -275,26 +277,28 @@
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
@@ -474,14 +478,15 @@
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

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/paginator.py` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/paginator.pyi` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/type_defs.py` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/type_defs.pyi` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/waiter.py` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune/waiter.pyi` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptune-2.5.2.post1/types_aiobotocore_neptune.egg-info/SOURCES.txt` & `types-aiobotocore-neptune-2.5.2.post2/types_aiobotocore_neptune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

