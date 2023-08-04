# Comparing `tmp/types-aiobotocore-redshift-serverless-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-redshift-serverless-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-serverless-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-serverless-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
```

## Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1.tar` & `types-aiobotocore-redshift-serverless-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.337483 types-aiobotocore-redshift-serverless-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18678 2023-08-02 14:52:52.329483 types-aiobotocore-redshift-serverless-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17113 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.337483 types-aiobotocore-redshift-serverless-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.329483 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35080 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9609 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9813 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33772 2023-08-02 14:47:45.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33741 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:44.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.329483 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18678 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.000000 types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-redshift-serverless-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14519 2023-08-04 13:59:22.906643 types-aiobotocore-redshift-serverless-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12954 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.906643 types-aiobotocore-redshift-serverless-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2008 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2007 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      989 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35136 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35080 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9706 2023-08-04 13:50:31.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9704 2023-08-04 13:50:31.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9813 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9804 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33772 2023-08-04 13:50:32.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33741 2023-08-04 13:50:31.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:30.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14519 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1041 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.000000 types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/LICENSE` & `types-aiobotocore-redshift-serverless-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/setup.py` & `types-aiobotocore-redshift-serverless-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift-serverless",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_redshift_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.RedshiftServerless 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__init__.py` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__init__.pyi` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/__main__.py` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.RedshiftServerless 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_serverless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless\nOther"
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

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/client.py` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/client.pyi` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/literals.py` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
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
@@ -171,14 +172,15 @@
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
@@ -257,26 +259,28 @@
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

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/literals.pyi` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
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
@@ -169,14 +170,15 @@
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
@@ -255,26 +257,28 @@
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

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/paginator.py` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/paginator.pyi` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/type_defs.py` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless/type_defs.pyi` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-serverless-2.5.2.post1/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-serverless-2.5.2.post2/types_aiobotocore_redshift_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

