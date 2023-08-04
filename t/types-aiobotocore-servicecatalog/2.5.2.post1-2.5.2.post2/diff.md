# Comparing `tmp/types-aiobotocore-servicecatalog-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-servicecatalog-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-servicecatalog-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-servicecatalog-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
```

## Comparing `types-aiobotocore-servicecatalog-2.5.2.post1.tar` & `types-aiobotocore-servicecatalog-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.709458 types-aiobotocore-servicecatalog-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-08-02 14:53:00.709458 types-aiobotocore-servicecatalog-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26549 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:00.709458 types-aiobotocore-servicecatalog-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:49:31.000000 types-aiobotocore-servicecatalog-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.705458 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79727 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    79612 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22687 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   102707 2023-08-02 14:49:34.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   102562 2023-08-02 14:49:33.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:32.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:00.709458 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28095 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:53:00.000000 types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.376643 types-aiobotocore-servicecatalog-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:18.000000 types-aiobotocore-servicecatalog-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16195 2023-08-04 13:59:26.356643 types-aiobotocore-servicecatalog-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14649 2023-08-04 13:53:18.000000 types-aiobotocore-servicecatalog-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.376643 types-aiobotocore-servicecatalog-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:53:17.000000 types-aiobotocore-servicecatalog-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.356643 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4639 2023-08-04 13:53:18.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4638 2023-08-04 13:53:18.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:53:18.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    79727 2023-08-04 13:53:18.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    79612 2023-08-04 13:53:18.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14884 2023-08-04 13:53:19.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14882 2023-08-04 13:53:19.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22687 2023-08-04 13:53:19.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22668 2023-08-04 13:53:18.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:18.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   102707 2023-08-04 13:53:21.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   102562 2023-08-04 13:53:20.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:18.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.356643 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16195 2023-08-04 13:59:26.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:26.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:26.000000 types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/LICENSE` & `types-aiobotocore-servicecatalog-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/setup.py` & `types-aiobotocore-servicecatalog-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-servicecatalog",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_servicecatalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ServiceCatalog 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__init__.py` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__init__.pyi` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/__main__.py` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ServiceCatalog 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_servicecatalog//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog\nOther"
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

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/client.py` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/client.pyi` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/literals.py` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
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
@@ -277,14 +278,15 @@
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
@@ -363,26 +365,28 @@
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

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/literals.pyi` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,15 @@
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
@@ -275,14 +276,15 @@
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
@@ -361,26 +363,28 @@
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

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/paginator.py` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/paginator.pyi` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/type_defs.py` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog/type_defs.pyi` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-servicecatalog-2.5.2.post1/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt` & `types-aiobotocore-servicecatalog-2.5.2.post2/types_aiobotocore_servicecatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

