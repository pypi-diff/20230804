# Comparing `tmp/types-aiobotocore-inspector-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-inspector-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-inspector-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-inspector-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
```

## Comparing `types-aiobotocore-inspector-2.5.2.post1.tar` & `types-aiobotocore-inspector-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.201569 types-aiobotocore-inspector-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19200 2023-08-02 14:52:24.201569 types-aiobotocore-inspector-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17674 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.201569 types-aiobotocore-inspector-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.197569 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34033 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33978 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-08-02 14:40:14.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40508 2023-08-02 14:40:14.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40443 2023-08-02 14:40:14.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:13.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.201569 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19200 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:24.000000 types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.206642 types-aiobotocore-inspector-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14272 2023-08-04 13:59:11.206642 types-aiobotocore-inspector-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12746 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.206642 types-aiobotocore-inspector-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.206642 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2443 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2442 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34033 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33978 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11003 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11001 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11783 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11772 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40508 2023-08-04 13:40:20.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40443 2023-08-04 13:40:19.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:18.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.206642 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14272 2023-08-04 13:59:11.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:11.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:11.000000 types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-inspector-2.5.2.post1/LICENSE` & `types-aiobotocore-inspector-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2.post1/setup.py` & `types-aiobotocore-inspector-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-inspector",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_inspector"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Inspector 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__init__.py` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__init__.pyi` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/__main__.py` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Inspector 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Inspector 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#Inspector\nOther"
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

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/client.py` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/client.pyi` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/literals.py` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,15 @@
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
@@ -220,14 +221,15 @@
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
@@ -306,26 +308,28 @@
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

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/literals.pyi` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
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
@@ -218,14 +219,15 @@
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
@@ -304,26 +306,28 @@
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

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/paginator.py` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/paginator.pyi` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/type_defs.py` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector/type_defs.pyi` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector-2.5.2.post1/types_aiobotocore_inspector.egg-info/SOURCES.txt` & `types-aiobotocore-inspector-2.5.2.post2/types_aiobotocore_inspector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

