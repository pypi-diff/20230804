# Comparing `tmp/types-aiobotocore-swf-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-swf-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-swf-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-swf-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
```

## Comparing `types-aiobotocore-swf-2.5.2.post1.tar` & `types-aiobotocore-swf-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.649440 types-aiobotocore-swf-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-08-02 14:53:06.645440 types-aiobotocore-swf-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20310 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.649440 types-aiobotocore-swf-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.637440 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32985 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32932 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16003 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-08-02 14:50:30.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    83962 2023-08-02 14:50:31.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    83805 2023-08-02 14:50:31.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:29.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.645440 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21812 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:06.000000 types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.476643 types-aiobotocore-swf-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13798 2023-08-04 13:59:28.476643 types-aiobotocore-swf-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12296 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.476643 types-aiobotocore-swf-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.476643 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2081 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2080 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    32985 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    32932 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16118 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16116 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10148 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10139 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    83962 2023-08-04 13:54:54.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    83805 2023-08-04 13:54:53.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:52.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.476643 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13798 2023-08-04 13:59:28.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:28.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:28.000000 types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-swf-2.5.2.post1/LICENSE` & `types-aiobotocore-swf-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2.post1/setup.py` & `types-aiobotocore-swf-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-swf",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_swf"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SWF 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__init__.py` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__init__.pyi` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/__main__.py` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SWF 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SWF 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_swf//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF\nOther"
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

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/client.py` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/client.pyi` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/literals.py` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ActivityTaskTimeoutTypeType",
     "CancelTimerFailedCauseType",
     "CancelWorkflowExecutionFailedCauseType",
     "ChildPolicyType",
     "CloseStatusType",
     "CompleteWorkflowExecutionFailedCauseType",
@@ -56,15 +55,14 @@
     "SWFServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActivityTaskTimeoutTypeType = Literal[
     "HEARTBEAT", "SCHEDULE_TO_CLOSE", "SCHEDULE_TO_START", "START_TO_CLOSE"
 ]
 CancelTimerFailedCauseType = Literal["OPERATION_NOT_PERMITTED", "TIMER_ID_UNKNOWN"]
 CancelWorkflowExecutionFailedCauseType = Literal["OPERATION_NOT_PERMITTED", "UNHANDLED_DECISION"]
 ChildPolicyType = Literal["ABANDON", "REQUEST_CANCEL", "TERMINATE"]
 CloseStatusType = Literal[
@@ -233,14 +231,15 @@
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
@@ -336,14 +335,15 @@
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
@@ -422,26 +422,28 @@
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
@@ -611,14 +613,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/literals.pyi` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ActivityTaskTimeoutTypeType",
     "CancelTimerFailedCauseType",
     "CancelWorkflowExecutionFailedCauseType",
     "ChildPolicyType",
     "CloseStatusType",
     "CompleteWorkflowExecutionFailedCauseType",
@@ -55,14 +56,15 @@
     "SWFServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ActivityTaskTimeoutTypeType = Literal[
     "HEARTBEAT", "SCHEDULE_TO_CLOSE", "SCHEDULE_TO_START", "START_TO_CLOSE"
 ]
 CancelTimerFailedCauseType = Literal["OPERATION_NOT_PERMITTED", "TIMER_ID_UNKNOWN"]
 CancelWorkflowExecutionFailedCauseType = Literal["OPERATION_NOT_PERMITTED", "UNHANDLED_DECISION"]
 ChildPolicyType = Literal["ABANDON", "REQUEST_CANCEL", "TERMINATE"]
 CloseStatusType = Literal[
@@ -231,14 +233,15 @@
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
@@ -334,14 +337,15 @@
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
@@ -420,26 +424,28 @@
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
@@ -609,14 +615,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/paginator.py` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/paginator.pyi` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/type_defs.py` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf/type_defs.pyi` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-swf-2.5.2.post1/types_aiobotocore_swf.egg-info/SOURCES.txt` & `types-aiobotocore-swf-2.5.2.post2/types_aiobotocore_swf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

