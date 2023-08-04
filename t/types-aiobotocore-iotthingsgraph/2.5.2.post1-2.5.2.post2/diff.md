# Comparing `tmp/types-aiobotocore-iotthingsgraph-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iotthingsgraph-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotthingsgraph-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotthingsgraph-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1.tar` & `types-aiobotocore-iotthingsgraph-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.613556 types-aiobotocore-iotthingsgraph-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-08-02 14:52:28.605557 types-aiobotocore-iotthingsgraph-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:28.613556 types-aiobotocore-iotthingsgraph-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.605557 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31302 2023-08-02 14:40:59.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31248 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-08-02 14:40:59.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-08-02 14:40:59.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-08-02 14:40:59.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-02 14:40:59.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33751 2023-08-02 14:41:01.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    33704 2023-08-02 14:41:01.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:58.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:28.605557 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19294 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:28.000000 types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.116643 types-aiobotocore-iotthingsgraph-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14891 2023-08-04 13:59:13.116643 types-aiobotocore-iotthingsgraph-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13345 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.116643 types-aiobotocore-iotthingsgraph-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.116643 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2827 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2826 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31302 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31248 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11290 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11288 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13623 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13611 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33751 2023-08-04 13:41:20.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33704 2023-08-04 13:41:19.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:18.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.116643 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14891 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:13.000000 types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/LICENSE` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/setup.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotthingsgraph",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iotthingsgraph"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTThingsGraph 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__init__.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__init__.pyi` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/__main__.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.IoTThingsGraph 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotthingsgraph//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph\nOther"
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

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/client.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/client.pyi` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/literals.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
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
@@ -227,14 +228,15 @@
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
@@ -313,26 +315,28 @@
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

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/literals.pyi` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,15 @@
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
@@ -225,14 +226,15 @@
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
@@ -311,26 +313,28 @@
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

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/paginator.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/paginator.pyi` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/type_defs.py` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph/type_defs.pyi` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotthingsgraph-2.5.2.post1/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt` & `types-aiobotocore-iotthingsgraph-2.5.2.post2/types_aiobotocore_iotthingsgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

