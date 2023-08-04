# Comparing `tmp/types-aiobotocore-memorydb-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-memorydb-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-memorydb-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-memorydb-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
```

## Comparing `types-aiobotocore-memorydb-2.5.2.post1.tar` & `types-aiobotocore-memorydb-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.533521 types-aiobotocore-memorydb-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20058 2023-08-02 14:52:40.533521 types-aiobotocore-memorydb-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18536 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:40.533521 types-aiobotocore-memorydb-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.529521 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38428 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    38369 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-08-02 14:43:33.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10218 2023-08-02 14:43:33.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15801 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15787 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41416 2023-08-02 14:43:33.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41381 2023-08-02 14:43:33.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:32.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.533521 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20058 2023-08-02 14:52:40.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:40.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:40.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:40.000000 types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.386643 types-aiobotocore-memorydb-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14729 2023-08-04 13:59:18.386643 types-aiobotocore-memorydb-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13207 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.386643 types-aiobotocore-memorydb-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.386643 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3143 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3142 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    38428 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    38369 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10315 2023-08-04 13:44:51.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10313 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15801 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15787 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    41416 2023-08-04 13:44:52.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    41381 2023-08-04 13:44:51.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:50.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.386643 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14729 2023-08-04 13:59:18.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:18.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:18.000000 types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/LICENSE` & `types-aiobotocore-memorydb-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/setup.py` & `types-aiobotocore-memorydb-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-memorydb",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_memorydb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MemoryDB 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/__init__.py` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/__init__.pyi` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/__main__.py` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MemoryDB 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MemoryDB 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB\nOther"
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

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/client.py` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/client.pyi` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/literals.py` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/literals.py`

 * *Files 0% similar despite different names*

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
```

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/literals.pyi` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/literals.pyi`

 * *Files 0% similar despite different names*

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

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/paginator.py` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/paginator.pyi` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/type_defs.py` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb/type_defs.pyi` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.5.2.post1/types_aiobotocore_memorydb.egg-info/SOURCES.txt` & `types-aiobotocore-memorydb-2.5.2.post2/types_aiobotocore_memorydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

