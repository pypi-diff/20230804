# Comparing `tmp/types-aiobotocore-networkmanager-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-networkmanager-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-networkmanager-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-networkmanager-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-networkmanager-2.5.2.post1.tar` & `types-aiobotocore-networkmanager-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.349511 types-aiobotocore-networkmanager-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-08-02 14:52:43.345512 types-aiobotocore-networkmanager-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27209 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.349511 types-aiobotocore-networkmanager-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.341512 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73474 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    73359 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-08-02 14:44:04.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14631 2023-08-02 14:44:04.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28537 2023-08-02 14:44:04.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28513 2023-08-02 14:44:04.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    95682 2023-08-02 14:44:06.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    95565 2023-08-02 14:44:05.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.345512 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.466643 types-aiobotocore-networkmanager-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16689 2023-08-04 13:59:19.466643 types-aiobotocore-networkmanager-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15143 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.466643 types-aiobotocore-networkmanager-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.466643 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5443 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5442 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    73474 2023-08-04 13:45:37.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    73359 2023-08-04 13:45:37.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14728 2023-08-04 13:45:39.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14726 2023-08-04 13:45:39.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28537 2023-08-04 13:45:37.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28513 2023-08-04 13:45:37.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    95682 2023-08-04 13:45:41.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    95565 2023-08-04 13:45:40.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:36.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.466643 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16689 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:19.000000 types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/LICENSE` & `types-aiobotocore-networkmanager-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/setup.py` & `types-aiobotocore-networkmanager-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-networkmanager",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_networkmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.NetworkManager 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__init__.py` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__init__.pyi` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__main__.py` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.NetworkManager 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager\nOther"
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

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/client.py` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/client.pyi` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/literals.py` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,15 @@
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
@@ -289,14 +290,15 @@
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
@@ -375,26 +377,28 @@
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

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/literals.pyi` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -184,14 +184,15 @@
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
@@ -287,14 +288,15 @@
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
@@ -373,26 +375,28 @@
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

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/paginator.py` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/paginator.pyi` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/type_defs.py` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/type_defs.pyi` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/SOURCES.txt` & `types-aiobotocore-networkmanager-2.5.2.post2/types_aiobotocore_networkmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

