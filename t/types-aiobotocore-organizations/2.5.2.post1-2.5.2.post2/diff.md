# Comparing `tmp/types-aiobotocore-organizations-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-organizations-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-organizations-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-organizations-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-organizations-2.5.2.post1.tar` & `types-aiobotocore-organizations-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.669504 types-aiobotocore-organizations-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22300 2023-08-02 14:52:45.665504 types-aiobotocore-organizations-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20758 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:45.669504 types-aiobotocore-organizations-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.665504 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49679 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49599 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12261 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20503 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20485 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44300 2023-08-02 14:44:30.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44245 2023-08-02 14:44:30.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:29.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.665504 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22300 2023-08-02 14:52:45.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:45.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:45.000000 types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-organizations-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15860 2023-08-04 13:59:20.276643 types-aiobotocore-organizations-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14318 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.276643 types-aiobotocore-organizations-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2114 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4303 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4302 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      967 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    49679 2023-08-04 13:46:14.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    49599 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12356 2023-08-04 13:46:14.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12354 2023-08-04 13:46:14.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20503 2023-08-04 13:46:14.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20485 2023-08-04 13:46:14.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    44300 2023-08-04 13:46:17.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    44245 2023-08-04 13:46:16.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:13.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.276643 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15860 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      927 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:20.000000 types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-organizations-2.5.2.post1/LICENSE` & `types-aiobotocore-organizations-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post1/setup.py` & `types-aiobotocore-organizations-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-organizations",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_organizations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Organizations 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/__init__.py` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/__init__.pyi` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/__main__.py` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.Organizations 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_organizations//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations\nOther"
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

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/client.py` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/client.pyi` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/literals.py` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
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
@@ -237,14 +238,15 @@
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
@@ -323,26 +325,28 @@
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

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/literals.pyi` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
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
@@ -235,14 +236,15 @@
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
@@ -321,26 +323,28 @@
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

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/paginator.py` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/paginator.pyi` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/type_defs.py` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations/type_defs.pyi` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-organizations-2.5.2.post1/types_aiobotocore_organizations.egg-info/SOURCES.txt` & `types-aiobotocore-organizations-2.5.2.post2/types_aiobotocore_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

