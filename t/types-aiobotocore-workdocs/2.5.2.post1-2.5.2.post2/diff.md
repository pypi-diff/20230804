# Comparing `tmp/types-aiobotocore-workdocs-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-workdocs-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workdocs-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-workdocs-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
```

## Comparing `types-aiobotocore-workdocs-2.5.2.post1.tar` & `types-aiobotocore-workdocs-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.521426 types-aiobotocore-workdocs-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20047 2023-08-02 14:53:10.521426 types-aiobotocore-workdocs-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18525 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:10.521426 types-aiobotocore-workdocs-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.517426 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40851 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40788 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-08-02 14:51:17.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-08-02 14:51:14.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14406 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    50590 2023-08-02 14:51:18.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    50499 2023-08-02 14:51:17.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:13.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.521426 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20047 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:10.000000 types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.166643 types-aiobotocore-workdocs-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14505 2023-08-04 13:59:30.166643 types-aiobotocore-workdocs-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12983 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.166643 types-aiobotocore-workdocs-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.156643 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2765 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2764 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40851 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40788 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13900 2023-08-04 13:56:06.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13898 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14406 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14393 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    50590 2023-08-04 13:56:10.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    50499 2023-08-04 13:56:06.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:05.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.166643 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14505 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:30.000000 types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/LICENSE` & `types-aiobotocore-workdocs-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/setup.py` & `types-aiobotocore-workdocs-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workdocs",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_workdocs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WorkDocs 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__init__.py` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__init__.pyi` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/__main__.py` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkDocs 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.WorkDocs 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workdocs//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#WorkDocs\nOther"
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

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/client.py` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/client.pyi` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/literals.py` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,14 +212,15 @@
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
@@ -315,14 +316,15 @@
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
@@ -401,26 +403,28 @@
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

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/literals.pyi` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,15 @@
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
@@ -313,14 +314,15 @@
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
@@ -399,26 +401,28 @@
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

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/paginator.py` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/paginator.pyi` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/type_defs.py` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs/type_defs.pyi` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workdocs-2.5.2.post1/types_aiobotocore_workdocs.egg-info/SOURCES.txt` & `types-aiobotocore-workdocs-2.5.2.post2/types_aiobotocore_workdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

