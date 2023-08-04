# Comparing `tmp/types-aiobotocore-wellarchitected-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-wellarchitected-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wellarchitected-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-wellarchitected-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
```

## Comparing `types-aiobotocore-wellarchitected-2.5.2.post1.tar` & `types-aiobotocore-wellarchitected-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.329427 types-aiobotocore-wellarchitected-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-08-02 14:53:10.329427 types-aiobotocore-wellarchitected-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:10.329427 types-aiobotocore-wellarchitected-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.329427 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40473 2023-08-02 14:51:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40409 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-08-02 14:51:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11030 2023-08-02 14:51:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53538 2023-08-02 14:51:11.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53481 2023-08-02 14:51:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:09.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:10.329427 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18307 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:53:10.000000 types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.106643 types-aiobotocore-wellarchitected-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12626 2023-08-04 13:59:30.106643 types-aiobotocore-wellarchitected-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11076 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.106643 types-aiobotocore-wellarchitected-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2128 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.106643 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      506 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      505 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      975 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40458 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40394 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11127 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11125 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    53047 2023-08-04 13:56:01.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    52990 2023-08-04 13:56:00.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:59.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.106643 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12626 2023-08-04 13:59:30.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      870 2023-08-04 13:59:30.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:30.000000 types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2.post1/LICENSE` & `types-aiobotocore-wellarchitected-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wellarchitected-2.5.2.post1/setup.py` & `types-aiobotocore-wellarchitected-2.5.2.post2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wellarchitected",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_wellarchitected"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WellArchitected 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/__main__.py` & `types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.WellArchitected 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected\nOther"
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

### Comparing `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/client.py` & `types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     ProfileQuestionUpdateTypeDef,
     UpdateAnswerOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     UpdateProfileOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
-    WorkloadDiscoveryConfigUnionTypeDef,
+    WorkloadDiscoveryConfigTypeDef,
 )
 
 __all__ = ("WellArchitectedClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -233,15 +233,15 @@
         PillarPriorities: Sequence[str] = ...,
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
-        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
         Applications: Sequence[str] = ...,
         ProfileArns: Sequence[str] = ...
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
@@ -815,15 +815,15 @@
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IsReviewOwnerUpdateAcknowledged: bool = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         ImprovementStatus: WorkloadImprovementStatusType = ...,
-        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
         Applications: Sequence[str] = ...
     ) -> UpdateWorkloadOutputTypeDef:
         """
         Update an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_workload)
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/client.pyi` & `types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     ProfileQuestionUpdateTypeDef,
     UpdateAnswerOutputTypeDef,
     UpdateLensReviewOutputTypeDef,
     UpdateProfileOutputTypeDef,
     UpdateShareInvitationOutputTypeDef,
     UpdateWorkloadOutputTypeDef,
     UpdateWorkloadShareOutputTypeDef,
-    WorkloadDiscoveryConfigUnionTypeDef,
+    WorkloadDiscoveryConfigTypeDef,
 )
 
 __all__ = ("WellArchitectedClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -220,15 +220,15 @@
         PillarPriorities: Sequence[str] = ...,
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         Tags: Mapping[str, str] = ...,
-        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
         Applications: Sequence[str] = ...,
         ProfileArns: Sequence[str] = ...
     ) -> CreateWorkloadOutputTypeDef:
         """
         Create a new workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.create_workload)
@@ -756,15 +756,15 @@
         ArchitecturalDesign: str = ...,
         ReviewOwner: str = ...,
         IsReviewOwnerUpdateAcknowledged: bool = ...,
         IndustryType: str = ...,
         Industry: str = ...,
         Notes: str = ...,
         ImprovementStatus: WorkloadImprovementStatusType = ...,
-        DiscoveryConfig: WorkloadDiscoveryConfigUnionTypeDef = ...,
+        DiscoveryConfig: WorkloadDiscoveryConfigTypeDef = ...,
         Applications: Sequence[str] = ...
     ) -> UpdateWorkloadOutputTypeDef:
         """
         Update an existing workload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#WellArchitected.Client.update_workload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wellarchitected/client/#update_workload)
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/literals.py` & `types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
@@ -52,15 +51,14 @@
     "WorkloadImprovementStatusType",
     "WellArchitectedServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AdditionalResourceTypeType = Literal["HELPFUL_RESOURCE", "IMPROVEMENT_PLAN"]
 AnswerReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 CheckFailureReasonType = Literal[
     "ACCESS_DENIED", "ASSUME_ROLE_ERROR", "PREMIUM_SUPPORT_REQUIRED", "UNKNOWN_ERROR"
 ]
@@ -109,14 +107,15 @@
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
@@ -212,14 +211,15 @@
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
@@ -298,26 +298,28 @@
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

### Comparing `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/literals.pyi` & `types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/literals.py`

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
     "AdditionalResourceTypeType",
     "AnswerReasonType",
     "CheckFailureReasonType",
     "CheckProviderType",
     "CheckStatusType",
     "ChoiceReasonType",
@@ -51,14 +52,15 @@
     "WorkloadImprovementStatusType",
     "WellArchitectedServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AdditionalResourceTypeType = Literal["HELPFUL_RESOURCE", "IMPROVEMENT_PLAN"]
 AnswerReasonType = Literal[
     "ARCHITECTURE_CONSTRAINTS", "BUSINESS_PRIORITIES", "NONE", "OTHER", "OUT_OF_SCOPE"
 ]
 CheckFailureReasonType = Literal[
     "ACCESS_DENIED", "ASSUME_ROLE_ERROR", "PREMIUM_SUPPORT_REQUIRED", "UNKNOWN_ERROR"
 ]
@@ -107,14 +109,15 @@
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
@@ -210,14 +213,15 @@
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
@@ -296,26 +300,28 @@
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

### Comparing `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/type_defs.py` & `types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_wellarchitected.type_defs import ChoiceContentTypeDef
 
     data: ChoiceContentTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
@@ -131,15 +131,14 @@
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
     "UpgradeProfileVersionInputRequestTypeDef",
-    "WorkloadDiscoveryConfigOutputTypeDef",
     "AdditionalResourcesTypeDef",
     "QuestionMetricTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
     "CreateLensShareOutputTypeDef",
     "CreateLensVersionOutputTypeDef",
     "CreateMilestoneOutputTypeDef",
@@ -157,54 +156,53 @@
     "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
     "LensReviewSummaryTypeDef",
     "WorkloadSummaryTypeDef",
+    "WorkloadTypeDef",
     "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
     "ListProfileNotificationsOutputTypeDef",
     "ListProfileSharesOutputTypeDef",
     "ListProfilesOutputTypeDef",
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
     "PillarDifferenceTypeDef",
     "ProfileQuestionTypeDef",
     "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
-    "WorkloadDiscoveryConfigUnionTypeDef",
-    "WorkloadTypeDef",
     "ChoiceTypeDef",
     "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
     "ListLensReviewsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
+    "GetWorkloadOutputTypeDef",
+    "MilestoneTypeDef",
+    "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "VersionDifferencesTypeDef",
     "ProfileTypeDef",
     "ProfileTemplateTypeDef",
-    "GetWorkloadOutputTypeDef",
-    "MilestoneTypeDef",
-    "UpdateWorkloadOutputTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
     "LensMetricTypeDef",
     "ListMilestonesOutputTypeDef",
+    "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
     "GetProfileOutputTypeDef",
     "UpdateProfileOutputTypeDef",
     "GetProfileTemplateOutputTypeDef",
-    "GetMilestoneOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
     "ConsolidatedReportMetricTypeDef",
     "GetConsolidatedReportOutputTypeDef",
 )
 
@@ -1318,23 +1316,14 @@
 class UpgradeProfileVersionInputRequestTypeDef(
     _RequiredUpgradeProfileVersionInputRequestTypeDef,
     _OptionalUpgradeProfileVersionInputRequestTypeDef,
 ):
     pass
 
 
-WorkloadDiscoveryConfigOutputTypeDef = TypedDict(
-    "WorkloadDiscoveryConfigOutputTypeDef",
-    {
-        "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
-        "WorkloadResourceDefinition": List[DefinitionTypeType],
-    },
-    total=False,
-)
-
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
@@ -1668,14 +1657,48 @@
         "ImprovementStatus": WorkloadImprovementStatusType,
         "Profiles": List[WorkloadProfileTypeDef],
         "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "WorkloadName": str,
+        "Description": str,
+        "Environment": WorkloadEnvironmentType,
+        "UpdatedAt": datetime,
+        "AccountIds": List[str],
+        "AwsRegions": List[str],
+        "NonAwsRegions": List[str],
+        "ArchitecturalDesign": str,
+        "ReviewOwner": str,
+        "ReviewRestrictionDate": datetime,
+        "IsReviewOwnerUpdateAcknowledged": bool,
+        "IndustryType": str,
+        "Industry": str,
+        "Notes": str,
+        "ImprovementStatus": WorkloadImprovementStatusType,
+        "RiskCounts": Dict[RiskType, int],
+        "PillarPriorities": List[str],
+        "Lenses": List[str],
+        "Owner": str,
+        "ShareInvitationId": str,
+        "Tags": Dict[str, str],
+        "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
+        "Applications": List[str],
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
+    },
+    total=False,
+)
+
 LensReviewTypeDef = TypedDict(
     "LensReviewTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "LensVersion": str,
         "LensName": str,
@@ -1815,51 +1838,14 @@
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WorkloadDiscoveryConfigUnionTypeDef = Union[
-    WorkloadDiscoveryConfigTypeDef, WorkloadDiscoveryConfigOutputTypeDef
-]
-WorkloadTypeDef = TypedDict(
-    "WorkloadTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "WorkloadName": str,
-        "Description": str,
-        "Environment": WorkloadEnvironmentType,
-        "UpdatedAt": datetime,
-        "AccountIds": List[str],
-        "AwsRegions": List[str],
-        "NonAwsRegions": List[str],
-        "ArchitecturalDesign": str,
-        "ReviewOwner": str,
-        "ReviewRestrictionDate": datetime,
-        "IsReviewOwnerUpdateAcknowledged": bool,
-        "IndustryType": str,
-        "Industry": str,
-        "Notes": str,
-        "ImprovementStatus": WorkloadImprovementStatusType,
-        "RiskCounts": Dict[RiskType, int],
-        "PillarPriorities": List[str],
-        "Lenses": List[str],
-        "Owner": str,
-        "ShareInvitationId": str,
-        "Tags": Dict[str, str],
-        "DiscoveryConfig": WorkloadDiscoveryConfigOutputTypeDef,
-        "Applications": List[str],
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
 ChoiceTypeDef = TypedDict(
     "ChoiceTypeDef",
     {
         "ChoiceId": str,
         "Title": str,
         "Description": str,
         "HelpfulResource": ChoiceContentTypeDef,
@@ -1919,14 +1905,41 @@
         "MilestoneName": str,
         "RecordedAt": datetime,
         "WorkloadSummary": WorkloadSummaryTypeDef,
     },
     total=False,
 )
 
+GetWorkloadOutputTypeDef = TypedDict(
+    "GetWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MilestoneTypeDef = TypedDict(
+    "MilestoneTypeDef",
+    {
+        "MilestoneNumber": int,
+        "MilestoneName": str,
+        "RecordedAt": datetime,
+        "Workload": WorkloadTypeDef,
+    },
+    total=False,
+)
+
+UpdateWorkloadOutputTypeDef = TypedDict(
+    "UpdateWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetLensReviewOutputTypeDef = TypedDict(
     "GetLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReview": LensReviewTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1983,41 +1996,14 @@
         "TemplateQuestions": List[ProfileTemplateQuestionTypeDef],
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
-GetWorkloadOutputTypeDef = TypedDict(
-    "GetWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MilestoneTypeDef = TypedDict(
-    "MilestoneTypeDef",
-    {
-        "MilestoneNumber": int,
-        "MilestoneName": str,
-        "RecordedAt": datetime,
-        "Workload": WorkloadTypeDef,
-    },
-    total=False,
-)
-
-UpdateWorkloadOutputTypeDef = TypedDict(
-    "UpdateWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Choices": List[ChoiceTypeDef],
@@ -2068,14 +2054,23 @@
         "WorkloadId": str,
         "MilestoneSummaries": List[MilestoneSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetMilestoneOutputTypeDef = TypedDict(
+    "GetMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "Milestone": MilestoneTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetLensVersionDifferenceOutputTypeDef = TypedDict(
     "GetLensVersionDifferenceOutputTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "BaseLensVersion": str,
         "TargetLensVersion": str,
@@ -2105,23 +2100,14 @@
     "GetProfileTemplateOutputTypeDef",
     {
         "ProfileTemplate": ProfileTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMilestoneOutputTypeDef = TypedDict(
-    "GetMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "Milestone": MilestoneTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected/type_defs.pyi` & `types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_wellarchitected.type_defs import ChoiceContentTypeDef
 
     data: ChoiceContentTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AdditionalResourceTypeType,
     AnswerReasonType,
     CheckFailureReasonType,
     CheckStatusType,
     ChoiceReasonType,
@@ -130,15 +130,14 @@
     "UpdateGlobalSettingsInputRequestTypeDef",
     "UpdateLensReviewInputRequestTypeDef",
     "UpdateShareInvitationInputRequestTypeDef",
     "UpdateWorkloadShareInputRequestTypeDef",
     "WorkloadShareTypeDef",
     "UpgradeLensReviewInputRequestTypeDef",
     "UpgradeProfileVersionInputRequestTypeDef",
-    "WorkloadDiscoveryConfigOutputTypeDef",
     "AdditionalResourcesTypeDef",
     "QuestionMetricTypeDef",
     "ImprovementSummaryTypeDef",
     "UpdateAnswerInputRequestTypeDef",
     "CreateLensShareOutputTypeDef",
     "CreateLensVersionOutputTypeDef",
     "CreateMilestoneOutputTypeDef",
@@ -156,54 +155,53 @@
     "UpdateProfileInputRequestTypeDef",
     "CreateWorkloadInputRequestTypeDef",
     "UpdateWorkloadInputRequestTypeDef",
     "GetLensOutputTypeDef",
     "GetLensReviewReportOutputTypeDef",
     "LensReviewSummaryTypeDef",
     "WorkloadSummaryTypeDef",
+    "WorkloadTypeDef",
     "LensReviewTypeDef",
     "ListLensSharesOutputTypeDef",
     "ListLensesOutputTypeDef",
     "NotificationSummaryTypeDef",
     "ListProfileNotificationsOutputTypeDef",
     "ListProfileSharesOutputTypeDef",
     "ListProfilesOutputTypeDef",
     "ListShareInvitationsOutputTypeDef",
     "ListWorkloadSharesOutputTypeDef",
     "PillarDifferenceTypeDef",
     "ProfileQuestionTypeDef",
     "ProfileTemplateQuestionTypeDef",
     "UpdateShareInvitationOutputTypeDef",
     "UpdateWorkloadShareOutputTypeDef",
-    "WorkloadDiscoveryConfigUnionTypeDef",
-    "WorkloadTypeDef",
     "ChoiceTypeDef",
     "PillarMetricTypeDef",
     "ListLensReviewImprovementsOutputTypeDef",
     "ListLensReviewsOutputTypeDef",
     "ListWorkloadsOutputTypeDef",
     "MilestoneSummaryTypeDef",
+    "GetWorkloadOutputTypeDef",
+    "MilestoneTypeDef",
+    "UpdateWorkloadOutputTypeDef",
     "GetLensReviewOutputTypeDef",
     "UpdateLensReviewOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "VersionDifferencesTypeDef",
     "ProfileTypeDef",
     "ProfileTemplateTypeDef",
-    "GetWorkloadOutputTypeDef",
-    "MilestoneTypeDef",
-    "UpdateWorkloadOutputTypeDef",
     "AnswerSummaryTypeDef",
     "AnswerTypeDef",
     "LensMetricTypeDef",
     "ListMilestonesOutputTypeDef",
+    "GetMilestoneOutputTypeDef",
     "GetLensVersionDifferenceOutputTypeDef",
     "GetProfileOutputTypeDef",
     "UpdateProfileOutputTypeDef",
     "GetProfileTemplateOutputTypeDef",
-    "GetMilestoneOutputTypeDef",
     "ListAnswersOutputTypeDef",
     "GetAnswerOutputTypeDef",
     "UpdateAnswerOutputTypeDef",
     "ConsolidatedReportMetricTypeDef",
     "GetConsolidatedReportOutputTypeDef",
 )
 
@@ -1271,23 +1269,14 @@
 
 class UpgradeProfileVersionInputRequestTypeDef(
     _RequiredUpgradeProfileVersionInputRequestTypeDef,
     _OptionalUpgradeProfileVersionInputRequestTypeDef,
 ):
     pass
 
-WorkloadDiscoveryConfigOutputTypeDef = TypedDict(
-    "WorkloadDiscoveryConfigOutputTypeDef",
-    {
-        "TrustedAdvisorIntegrationStatus": TrustedAdvisorIntegrationStatusType,
-        "WorkloadResourceDefinition": List[DefinitionTypeType],
-    },
-    total=False,
-)
-
 AdditionalResourcesTypeDef = TypedDict(
     "AdditionalResourcesTypeDef",
     {
         "Type": AdditionalResourceTypeType,
         "Content": List[ChoiceContentTypeDef],
     },
     total=False,
@@ -1611,14 +1600,48 @@
         "ImprovementStatus": WorkloadImprovementStatusType,
         "Profiles": List[WorkloadProfileTypeDef],
         "PrioritizedRiskCounts": Dict[RiskType, int],
     },
     total=False,
 )
 
+WorkloadTypeDef = TypedDict(
+    "WorkloadTypeDef",
+    {
+        "WorkloadId": str,
+        "WorkloadArn": str,
+        "WorkloadName": str,
+        "Description": str,
+        "Environment": WorkloadEnvironmentType,
+        "UpdatedAt": datetime,
+        "AccountIds": List[str],
+        "AwsRegions": List[str],
+        "NonAwsRegions": List[str],
+        "ArchitecturalDesign": str,
+        "ReviewOwner": str,
+        "ReviewRestrictionDate": datetime,
+        "IsReviewOwnerUpdateAcknowledged": bool,
+        "IndustryType": str,
+        "Industry": str,
+        "Notes": str,
+        "ImprovementStatus": WorkloadImprovementStatusType,
+        "RiskCounts": Dict[RiskType, int],
+        "PillarPriorities": List[str],
+        "Lenses": List[str],
+        "Owner": str,
+        "ShareInvitationId": str,
+        "Tags": Dict[str, str],
+        "DiscoveryConfig": WorkloadDiscoveryConfigTypeDef,
+        "Applications": List[str],
+        "Profiles": List[WorkloadProfileTypeDef],
+        "PrioritizedRiskCounts": Dict[RiskType, int],
+    },
+    total=False,
+)
+
 LensReviewTypeDef = TypedDict(
     "LensReviewTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "LensVersion": str,
         "LensName": str,
@@ -1758,51 +1781,14 @@
     {
         "WorkloadId": str,
         "WorkloadShare": WorkloadShareTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-WorkloadDiscoveryConfigUnionTypeDef = Union[
-    WorkloadDiscoveryConfigTypeDef, WorkloadDiscoveryConfigOutputTypeDef
-]
-WorkloadTypeDef = TypedDict(
-    "WorkloadTypeDef",
-    {
-        "WorkloadId": str,
-        "WorkloadArn": str,
-        "WorkloadName": str,
-        "Description": str,
-        "Environment": WorkloadEnvironmentType,
-        "UpdatedAt": datetime,
-        "AccountIds": List[str],
-        "AwsRegions": List[str],
-        "NonAwsRegions": List[str],
-        "ArchitecturalDesign": str,
-        "ReviewOwner": str,
-        "ReviewRestrictionDate": datetime,
-        "IsReviewOwnerUpdateAcknowledged": bool,
-        "IndustryType": str,
-        "Industry": str,
-        "Notes": str,
-        "ImprovementStatus": WorkloadImprovementStatusType,
-        "RiskCounts": Dict[RiskType, int],
-        "PillarPriorities": List[str],
-        "Lenses": List[str],
-        "Owner": str,
-        "ShareInvitationId": str,
-        "Tags": Dict[str, str],
-        "DiscoveryConfig": WorkloadDiscoveryConfigOutputTypeDef,
-        "Applications": List[str],
-        "Profiles": List[WorkloadProfileTypeDef],
-        "PrioritizedRiskCounts": Dict[RiskType, int],
-    },
-    total=False,
-)
-
 ChoiceTypeDef = TypedDict(
     "ChoiceTypeDef",
     {
         "ChoiceId": str,
         "Title": str,
         "Description": str,
         "HelpfulResource": ChoiceContentTypeDef,
@@ -1862,14 +1848,41 @@
         "MilestoneName": str,
         "RecordedAt": datetime,
         "WorkloadSummary": WorkloadSummaryTypeDef,
     },
     total=False,
 )
 
+GetWorkloadOutputTypeDef = TypedDict(
+    "GetWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MilestoneTypeDef = TypedDict(
+    "MilestoneTypeDef",
+    {
+        "MilestoneNumber": int,
+        "MilestoneName": str,
+        "RecordedAt": datetime,
+        "Workload": WorkloadTypeDef,
+    },
+    total=False,
+)
+
+UpdateWorkloadOutputTypeDef = TypedDict(
+    "UpdateWorkloadOutputTypeDef",
+    {
+        "Workload": WorkloadTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetLensReviewOutputTypeDef = TypedDict(
     "GetLensReviewOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensReview": LensReviewTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1926,41 +1939,14 @@
         "TemplateQuestions": List[ProfileTemplateQuestionTypeDef],
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
     },
     total=False,
 )
 
-GetWorkloadOutputTypeDef = TypedDict(
-    "GetWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-MilestoneTypeDef = TypedDict(
-    "MilestoneTypeDef",
-    {
-        "MilestoneNumber": int,
-        "MilestoneName": str,
-        "RecordedAt": datetime,
-        "Workload": WorkloadTypeDef,
-    },
-    total=False,
-)
-
-UpdateWorkloadOutputTypeDef = TypedDict(
-    "UpdateWorkloadOutputTypeDef",
-    {
-        "Workload": WorkloadTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 AnswerSummaryTypeDef = TypedDict(
     "AnswerSummaryTypeDef",
     {
         "QuestionId": str,
         "PillarId": str,
         "QuestionTitle": str,
         "Choices": List[ChoiceTypeDef],
@@ -2011,14 +1997,23 @@
         "WorkloadId": str,
         "MilestoneSummaries": List[MilestoneSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetMilestoneOutputTypeDef = TypedDict(
+    "GetMilestoneOutputTypeDef",
+    {
+        "WorkloadId": str,
+        "Milestone": MilestoneTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetLensVersionDifferenceOutputTypeDef = TypedDict(
     "GetLensVersionDifferenceOutputTypeDef",
     {
         "LensAlias": str,
         "LensArn": str,
         "BaseLensVersion": str,
         "TargetLensVersion": str,
@@ -2048,23 +2043,14 @@
     "GetProfileTemplateOutputTypeDef",
     {
         "ProfileTemplate": ProfileTemplateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMilestoneOutputTypeDef = TypedDict(
-    "GetMilestoneOutputTypeDef",
-    {
-        "WorkloadId": str,
-        "Milestone": MilestoneTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListAnswersOutputTypeDef = TypedDict(
     "ListAnswersOutputTypeDef",
     {
         "WorkloadId": str,
         "MilestoneNumber": int,
         "LensAlias": str,
         "LensArn": str,
```

### Comparing `types-aiobotocore-wellarchitected-2.5.2.post1/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt` & `types-aiobotocore-wellarchitected-2.5.2.post2/types_aiobotocore_wellarchitected.egg-info/SOURCES.txt`

 * *Files identical despite different names*

