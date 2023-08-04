# Comparing `tmp/types-aiobotocore-tnb-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-tnb-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-tnb-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-tnb-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
```

## Comparing `types-aiobotocore-tnb-2.5.2.post1.tar` & `types-aiobotocore-tnb-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.945435 types-aiobotocore-tnb-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-08-02 14:53:07.945435 types-aiobotocore-tnb-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:07.945435 types-aiobotocore-tnb-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.945435 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26984 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26937 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-08-02 14:50:37.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34594 2023-08-02 14:50:37.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34563 2023-08-02 14:50:37.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:36.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.945435 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:07.000000 types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.316643 types-aiobotocore-tnb-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13618 2023-08-04 13:59:29.316643 types-aiobotocore-tnb-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12100 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.316643 types-aiobotocore-tnb-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2036 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.316643 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1775 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1774 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      948 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26984 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26937 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10005 2023-08-04 13:55:08.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10003 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6826 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6819 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34594 2023-08-04 13:55:08.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    34563 2023-08-04 13:55:08.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:07.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.316643 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13618 2023-08-04 13:59:29.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:29.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:29.000000 types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-tnb-2.5.2.post1/LICENSE` & `types-aiobotocore-tnb-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2.post1/setup.py` & `types-aiobotocore-tnb-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-tnb",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_tnb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.TelcoNetworkBuilder 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__init__.py` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__init__.pyi` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/__main__.py` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.TelcoNetworkBuilder 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_tnb//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#TelcoNetworkBuilder\nOther"
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

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/client.py` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/client.pyi` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/literals.py` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
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
@@ -193,14 +194,15 @@
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
@@ -279,26 +281,28 @@
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

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/literals.pyi` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
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
@@ -191,14 +192,15 @@
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
@@ -277,26 +279,28 @@
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

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/paginator.py` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/paginator.pyi` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/type_defs.py` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb/type_defs.pyi` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-tnb-2.5.2.post1/types_aiobotocore_tnb.egg-info/SOURCES.txt` & `types-aiobotocore-tnb-2.5.2.post2/types_aiobotocore_tnb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

