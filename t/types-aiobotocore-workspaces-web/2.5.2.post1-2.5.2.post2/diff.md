# Comparing `tmp/types-aiobotocore-workspaces-web-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-workspaces-web-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workspaces-web-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-workspaces-web-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
```

## Comparing `types-aiobotocore-workspaces-web-2.5.2.post1.tar` & `types-aiobotocore-workspaces-web-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.377424 types-aiobotocore-workspaces-web-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-08-02 14:53:11.377424 types-aiobotocore-workspaces-web-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:11.377424 types-aiobotocore-workspaces-web-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:51:24.000000 types-aiobotocore-workspaces-web-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.377424 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40343 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40277 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8340 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41342 2023-08-02 14:51:26.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41291 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:25.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.377424 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:53:11.000000 types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.426643 types-aiobotocore-workspaces-web-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12606 2023-08-04 13:59:30.426643 types-aiobotocore-workspaces-web-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11061 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.426643 types-aiobotocore-workspaces-web-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2120 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.426643 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      493 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      492 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40343 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40277 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8437 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8435 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    41342 2023-08-04 13:56:29.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    41291 2023-08-04 13:56:29.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:24.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.426643 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12606 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      853 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:30.000000 types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workspaces-web-2.5.2.post1/LICENSE` & `types-aiobotocore-workspaces-web-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-web-2.5.2.post1/setup.py` & `types-aiobotocore-workspaces-web-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workspaces-web",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_workspaces_web"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WorkSpacesWeb 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/client.py` & `types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/client.pyi` & `types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/literals.py` & `types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
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
@@ -156,14 +157,15 @@
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
@@ -242,26 +244,28 @@
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

### Comparing `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/literals.pyi` & `types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
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
@@ -154,14 +155,15 @@
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
@@ -240,26 +242,28 @@
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

### Comparing `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/type_defs.py` & `types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web/type_defs.pyi` & `types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workspaces-web-2.5.2.post1/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt` & `types-aiobotocore-workspaces-web-2.5.2.post2/types_aiobotocore_workspaces_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

