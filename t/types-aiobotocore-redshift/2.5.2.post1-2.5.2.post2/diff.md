# Comparing `tmp/types-aiobotocore-redshift-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-redshift-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
```

## Comparing `types-aiobotocore-redshift-2.5.2.post1.tar` & `types-aiobotocore-redshift-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.237483 types-aiobotocore-redshift-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37716 2023-08-02 14:52:52.237483 types-aiobotocore-redshift-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36194 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.237483 types-aiobotocore-redshift-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.237483 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   119965 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   119796 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17276 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17274 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    45116 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    45081 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   134049 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   133930 2023-08-02 14:47:38.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:36.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-08-02 14:47:37.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.237483 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37716 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.766643 types-aiobotocore-redshift-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20300 2023-08-04 13:59:22.766643 types-aiobotocore-redshift-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18778 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.766643 types-aiobotocore-redshift-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.766643 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10002 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10001 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   119965 2023-08-04 13:50:20.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   119796 2023-08-04 13:50:20.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17391 2023-08-04 13:50:21.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    17389 2023-08-04 13:50:21.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    45116 2023-08-04 13:50:20.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    45081 2023-08-04 13:50:20.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   134049 2023-08-04 13:50:24.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   133930 2023-08-04 13:50:23.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:19.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5583 2023-08-04 13:50:21.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5579 2023-08-04 13:50:21.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.766643 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20300 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      907 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-2.5.2.post1/LICENSE` & `types-aiobotocore-redshift-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/setup.py` & `types-aiobotocore-redshift-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Redshift 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__init__.py` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__init__.pyi` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/__main__.py` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Redshift 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Redshift 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\nOther"
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

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/client.py` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/client.pyi` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/literals.py` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
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
@@ -290,14 +291,15 @@
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
@@ -376,26 +378,28 @@
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
@@ -594,14 +598,15 @@
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

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/literals.pyi` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
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
@@ -288,14 +289,15 @@
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
@@ -374,26 +376,28 @@
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
@@ -592,14 +596,15 @@
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

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/paginator.py` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/paginator.pyi` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/type_defs.py` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/type_defs.pyi` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/waiter.py` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift/waiter.pyi` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-2.5.2.post1/types_aiobotocore_redshift.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-2.5.2.post2/types_aiobotocore_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

