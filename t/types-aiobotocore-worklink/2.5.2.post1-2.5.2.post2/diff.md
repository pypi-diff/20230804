# Comparing `tmp/types-aiobotocore-worklink-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-worklink-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-worklink-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-worklink-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
```

## Comparing `types-aiobotocore-worklink-2.5.2.post1.tar` & `types-aiobotocore-worklink-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.885425 types-aiobotocore-worklink-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-08-02 14:53:10.865425 types-aiobotocore-worklink-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:10.885425 types-aiobotocore-worklink-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.865425 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23834 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23792 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-08-02 14:51:19.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21237 2023-08-02 14:51:19.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21206 2023-08-02 14:51:19.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:18.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.865425 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14778 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:10.000000 types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.256643 types-aiobotocore-worklink-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12293 2023-08-04 13:59:30.256643 types-aiobotocore-worklink-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10771 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.256643 types-aiobotocore-worklink-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.256643 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      450 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      449 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23834 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23792 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8244 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8242 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21237 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21206 2023-08-04 13:56:12.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:11.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.256643 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12293 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      751 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:30.000000 types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-worklink-2.5.2.post1/LICENSE` & `types-aiobotocore-worklink-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post1/setup.py` & `types-aiobotocore-worklink-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-worklink",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_worklink"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WorkLink 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/__main__.py` & `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.WorkLink 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.WorkLink 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_worklink//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/worklink.html#WorkLink\nOther"
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

### Comparing `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/client.py` & `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/client.pyi` & `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/literals.py` & `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,27 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthorizationProviderTypeType",
     "DeviceStatusType",
     "DomainStatusType",
     "FleetStatusType",
     "IdentityProviderTypeType",
     "WorkLinkServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 AuthorizationProviderTypeType = Literal["SAML"]
 DeviceStatusType = Literal["ACTIVE", "SIGNED_OUT"]
 DomainStatusType = Literal[
     "ACTIVE",
     "ASSOCIATING",
     "DISASSOCIATED",
     "DISASSOCIATING",
@@ -59,14 +57,15 @@
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
@@ -162,14 +161,15 @@
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
@@ -248,26 +248,28 @@
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

### Comparing `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/literals.pyi` & `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AuthorizationProviderTypeType",
     "DeviceStatusType",
     "DomainStatusType",
     "FleetStatusType",
     "IdentityProviderTypeType",
     "WorkLinkServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
+
 AuthorizationProviderTypeType = Literal["SAML"]
 DeviceStatusType = Literal["ACTIVE", "SIGNED_OUT"]
 DomainStatusType = Literal[
     "ACTIVE",
     "ASSOCIATING",
     "DISASSOCIATED",
     "DISASSOCIATING",
@@ -57,14 +59,15 @@
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
@@ -160,14 +163,15 @@
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
@@ -246,26 +250,28 @@
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

### Comparing `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/type_defs.py` & `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink/type_defs.pyi` & `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-worklink-2.5.2.post1/types_aiobotocore_worklink.egg-info/SOURCES.txt` & `types-aiobotocore-worklink-2.5.2.post2/types_aiobotocore_worklink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

