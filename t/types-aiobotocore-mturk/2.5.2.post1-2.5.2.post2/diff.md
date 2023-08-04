# Comparing `tmp/types-aiobotocore-mturk-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mturk-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mturk-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-mturk-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-mturk-2.5.2.post1.tar` & `types-aiobotocore-mturk-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.929513 types-aiobotocore-mturk-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18798 2023-08-02 14:52:42.921513 types-aiobotocore-mturk-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17288 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:42.929513 types-aiobotocore-mturk-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:43:49.000000 types-aiobotocore-mturk-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.921513 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35409 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35352 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39546 2023-08-02 14:43:51.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39487 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:50.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:42.921513 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18798 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:42.000000 types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.166643 types-aiobotocore-mturk-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14240 2023-08-04 13:59:19.166643 types-aiobotocore-mturk-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12730 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.166643 types-aiobotocore-mturk-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2058 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.166643 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2567 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2566 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      924 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35369 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35312 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10690 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10688 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11742 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11731 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37592 2023-08-04 13:45:21.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37537 2023-08-04 13:45:20.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.166643 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14240 2023-08-04 13:59:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      775 2023-08-04 13:59:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:19.000000 types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mturk-2.5.2.post1/LICENSE` & `types-aiobotocore-mturk-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.5.2.post1/setup.py` & `types-aiobotocore-mturk-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mturk",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mturk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MTurk 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__init__.py` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__init__.pyi` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/__main__.py` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MTurk 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MTurk 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk\nOther"
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

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/client.py` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     ListQualificationTypesResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersResponseTypeDef,
-    QualificationRequirementUnionTypeDef,
-    ReviewPolicyUnionTypeDef,
+    QualificationRequirementTypeDef,
+    ReviewPolicyTypeDef,
     TimestampTypeDef,
     UpdateQualificationTypeResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -182,18 +182,18 @@
         Title: str,
         Description: str,
         MaxAssignments: int = ...,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...,
+        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITResponseTypeDef:
         """
         The `CreateHIT` operation creates a new Human Intelligence Task (HIT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit)
@@ -205,15 +205,15 @@
         *,
         AssignmentDurationInSeconds: int,
         Reward: str,
         Title: str,
         Description: str,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...
+        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...
     ) -> CreateHITTypeResponseTypeDef:
         """
         The `CreateHITType` operation creates a new HIT type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#create_hit_type)
         """
@@ -223,16 +223,16 @@
         *,
         HITTypeId: str,
         LifetimeInSeconds: int,
         MaxAssignments: int = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITWithHITTypeResponseTypeDef:
         """
         The `CreateHITWithHITType` operation creates a new Human Intelligence Task (HIT)
         using an existing HITTypeID generated by the `CreateHITType` operation.
```

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/client.pyi` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     ListQualificationTypesResponseTypeDef,
     ListReviewableHITsResponseTypeDef,
     ListReviewPolicyResultsForHITResponseTypeDef,
     ListWorkerBlocksResponseTypeDef,
     ListWorkersWithQualificationTypeResponseTypeDef,
     NotificationSpecificationTypeDef,
     NotifyWorkersResponseTypeDef,
-    QualificationRequirementUnionTypeDef,
-    ReviewPolicyUnionTypeDef,
+    QualificationRequirementTypeDef,
+    ReviewPolicyTypeDef,
     TimestampTypeDef,
     UpdateQualificationTypeResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -171,18 +171,18 @@
         Title: str,
         Description: str,
         MaxAssignments: int = ...,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...,
+        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITResponseTypeDef:
         """
         The `CreateHIT` operation creates a new Human Intelligence Task (HIT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit)
@@ -193,15 +193,15 @@
         *,
         AssignmentDurationInSeconds: int,
         Reward: str,
         Title: str,
         Description: str,
         AutoApprovalDelayInSeconds: int = ...,
         Keywords: str = ...,
-        QualificationRequirements: Sequence[QualificationRequirementUnionTypeDef] = ...
+        QualificationRequirements: Sequence[QualificationRequirementTypeDef] = ...
     ) -> CreateHITTypeResponseTypeDef:
         """
         The `CreateHITType` operation creates a new HIT type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client.create_hit_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mturk/client/#create_hit_type)
         """
@@ -210,16 +210,16 @@
         *,
         HITTypeId: str,
         LifetimeInSeconds: int,
         MaxAssignments: int = ...,
         Question: str = ...,
         RequesterAnnotation: str = ...,
         UniqueRequestToken: str = ...,
-        AssignmentReviewPolicy: ReviewPolicyUnionTypeDef = ...,
-        HITReviewPolicy: ReviewPolicyUnionTypeDef = ...,
+        AssignmentReviewPolicy: ReviewPolicyTypeDef = ...,
+        HITReviewPolicy: ReviewPolicyTypeDef = ...,
         HITLayoutId: str = ...,
         HITLayoutParameters: Sequence[HITLayoutParameterTypeDef] = ...
     ) -> CreateHITWithHITTypeResponseTypeDef:
         """
         The `CreateHITWithHITType` operation creates a new Human Intelligence Task (HIT)
         using an existing HITTypeID generated by the `CreateHITType` operation.
```

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/literals.py` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,15 @@
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
@@ -213,14 +214,15 @@
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
@@ -299,26 +301,28 @@
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

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/literals.pyi` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,15 @@
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
@@ -211,14 +212,15 @@
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
@@ -297,26 +299,28 @@
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

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/paginator.py` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/paginator.pyi` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/type_defs.py` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,14 @@
     "ListWorkerBlocksRequestRequestTypeDef",
     "WorkerBlockTypeDef",
     "ListWorkersWithQualificationTypeRequestRequestTypeDef",
     "LocaleTypeDef",
     "NotificationSpecificationTypeDef",
     "NotifyWorkersFailureStatusTypeDef",
     "NotifyWorkersRequestRequestTypeDef",
-    "ParameterMapEntryOutputTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
     "TimestampTypeDef",
@@ -102,42 +101,37 @@
     "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
     "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
     "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
     "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
     "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListQualificationRequestsResponseTypeDef",
     "ListWorkerBlocksResponseTypeDef",
-    "QualificationRequirementOutputTypeDef",
     "QualificationRequirementTypeDef",
     "QualificationTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
-    "PolicyParameterOutputTypeDef",
     "PolicyParameterTypeDef",
     "ReviewReportTypeDef",
     "UpdateExpirationForHITRequestRequestTypeDef",
+    "CreateHITTypeRequestRequestTypeDef",
     "HITTypeDef",
-    "QualificationRequirementUnionTypeDef",
     "GetQualificationScoreResponseTypeDef",
     "ListWorkersWithQualificationTypeResponseTypeDef",
-    "ReviewPolicyOutputTypeDef",
     "ReviewPolicyTypeDef",
     "CreateHITResponseTypeDef",
     "CreateHITWithHITTypeResponseTypeDef",
     "GetAssignmentResponseTypeDef",
     "GetHITResponseTypeDef",
     "ListHITsForQualificationTypeResponseTypeDef",
     "ListHITsResponseTypeDef",
     "ListReviewableHITsResponseTypeDef",
-    "CreateHITTypeRequestRequestTypeDef",
-    "ListReviewPolicyResultsForHITResponseTypeDef",
     "CreateHITRequestRequestTypeDef",
     "CreateHITWithHITTypeRequestRequestTypeDef",
-    "ReviewPolicyUnionTypeDef",
+    "ListReviewPolicyResultsForHITResponseTypeDef",
 )
 
 _RequiredAcceptQualificationRequestRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptQualificationRequestRequestRequestTypeDef",
     {
         "QualificationRequestId": str,
     },
@@ -678,23 +672,14 @@
     {
         "Subject": str,
         "MessageText": str,
         "WorkerIds": Sequence[str],
     },
 )
 
-ParameterMapEntryOutputTypeDef = TypedDict(
-    "ParameterMapEntryOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-    },
-    total=False,
-)
-
 ParameterMapEntryTypeDef = TypedDict(
     "ParameterMapEntryTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -1074,39 +1059,14 @@
         "NextToken": str,
         "NumResults": int,
         "WorkerBlocks": List[WorkerBlockTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredQualificationRequirementOutputTypeDef = TypedDict(
-    "_RequiredQualificationRequirementOutputTypeDef",
-    {
-        "QualificationTypeId": str,
-        "Comparator": ComparatorType,
-    },
-)
-_OptionalQualificationRequirementOutputTypeDef = TypedDict(
-    "_OptionalQualificationRequirementOutputTypeDef",
-    {
-        "IntegerValues": List[int],
-        "LocaleValues": List[LocaleTypeDef],
-        "RequiredToPreview": bool,
-        "ActionsGuarded": HITAccessActionsType,
-    },
-    total=False,
-)
-
-
-class QualificationRequirementOutputTypeDef(
-    _RequiredQualificationRequirementOutputTypeDef, _OptionalQualificationRequirementOutputTypeDef
-):
-    pass
-
-
 _RequiredQualificationRequirementTypeDef = TypedDict(
     "_RequiredQualificationRequirementTypeDef",
     {
         "QualificationTypeId": str,
         "Comparator": ComparatorType,
     },
 )
@@ -1176,24 +1136,14 @@
     "NotifyWorkersResponseTypeDef",
     {
         "NotifyWorkersFailureStatuses": List[NotifyWorkersFailureStatusTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PolicyParameterOutputTypeDef = TypedDict(
-    "PolicyParameterOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-        "MapEntries": List[ParameterMapEntryOutputTypeDef],
-    },
-    total=False,
-)
-
 PolicyParameterTypeDef = TypedDict(
     "PolicyParameterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MapEntries": Sequence[ParameterMapEntryTypeDef],
     },
@@ -1213,14 +1163,40 @@
     "UpdateExpirationForHITRequestRequestTypeDef",
     {
         "HITId": str,
         "ExpireAt": TimestampTypeDef,
     },
 )
 
+_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHITTypeRequestRequestTypeDef",
+    {
+        "AssignmentDurationInSeconds": int,
+        "Reward": str,
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHITTypeRequestRequestTypeDef",
+    {
+        "AutoApprovalDelayInSeconds": int,
+        "Keywords": str,
+        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateHITTypeRequestRequestTypeDef(
+    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
+):
+    pass
+
+
 HITTypeDef = TypedDict(
     "HITTypeDef",
     {
         "HITId": str,
         "HITTypeId": str,
         "HITGroupId": str,
         "HITLayoutId": str,
@@ -1232,26 +1208,23 @@
         "HITStatus": HITStatusType,
         "MaxAssignments": int,
         "Reward": str,
         "AutoApprovalDelayInSeconds": int,
         "Expiration": datetime,
         "AssignmentDurationInSeconds": int,
         "RequesterAnnotation": str,
-        "QualificationRequirements": List[QualificationRequirementOutputTypeDef],
+        "QualificationRequirements": List[QualificationRequirementTypeDef],
         "HITReviewStatus": HITReviewStatusType,
         "NumberOfAssignmentsPending": int,
         "NumberOfAssignmentsAvailable": int,
         "NumberOfAssignmentsCompleted": int,
     },
     total=False,
 )
 
-QualificationRequirementUnionTypeDef = Union[
-    QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef
-]
 GetQualificationScoreResponseTypeDef = TypedDict(
     "GetQualificationScoreResponseTypeDef",
     {
         "Qualification": QualificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1262,35 +1235,14 @@
         "NextToken": str,
         "NumResults": int,
         "Qualifications": List[QualificationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredReviewPolicyOutputTypeDef = TypedDict(
-    "_RequiredReviewPolicyOutputTypeDef",
-    {
-        "PolicyName": str,
-    },
-)
-_OptionalReviewPolicyOutputTypeDef = TypedDict(
-    "_OptionalReviewPolicyOutputTypeDef",
-    {
-        "Parameters": List[PolicyParameterOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class ReviewPolicyOutputTypeDef(
-    _RequiredReviewPolicyOutputTypeDef, _OptionalReviewPolicyOutputTypeDef
-):
-    pass
-
-
 _RequiredReviewPolicyTypeDef = TypedDict(
     "_RequiredReviewPolicyTypeDef",
     {
         "PolicyName": str,
     },
 )
 _OptionalReviewPolicyTypeDef = TypedDict(
@@ -1365,53 +1317,14 @@
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHITTypeRequestRequestTypeDef",
-    {
-        "AssignmentDurationInSeconds": int,
-        "Reward": str,
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHITTypeRequestRequestTypeDef",
-    {
-        "AutoApprovalDelayInSeconds": int,
-        "Keywords": str,
-        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateHITTypeRequestRequestTypeDef(
-    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
-):
-    pass
-
-
-ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
-    "ListReviewPolicyResultsForHITResponseTypeDef",
-    {
-        "HITId": str,
-        "AssignmentReviewPolicy": ReviewPolicyOutputTypeDef,
-        "HITReviewPolicy": ReviewPolicyOutputTypeDef,
-        "AssignmentReviewReport": ReviewReportTypeDef,
-        "HITReviewReport": ReviewReportTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateHITRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITRequestRequestTypeDef",
     {
         "LifetimeInSeconds": int,
         "AssignmentDurationInSeconds": int,
         "Reward": str,
         "Title": str,
@@ -1422,15 +1335,15 @@
     "_OptionalCreateHITRequestRequestTypeDef",
     {
         "MaxAssignments": int,
         "AutoApprovalDelayInSeconds": int,
         "Keywords": str,
         "Question": str,
         "RequesterAnnotation": str,
-        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
+        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
         "UniqueRequestToken": str,
         "AssignmentReviewPolicy": ReviewPolicyTypeDef,
         "HITReviewPolicy": ReviewPolicyTypeDef,
         "HITLayoutId": str,
         "HITLayoutParameters": Sequence[HITLayoutParameterTypeDef],
     },
     total=False,
@@ -1469,8 +1382,19 @@
 class CreateHITWithHITTypeRequestRequestTypeDef(
     _RequiredCreateHITWithHITTypeRequestRequestTypeDef,
     _OptionalCreateHITWithHITTypeRequestRequestTypeDef,
 ):
     pass
 
 
-ReviewPolicyUnionTypeDef = Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef]
+ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
+    "ListReviewPolicyResultsForHITResponseTypeDef",
+    {
+        "HITId": str,
+        "AssignmentReviewPolicy": ReviewPolicyTypeDef,
+        "HITReviewPolicy": ReviewPolicyTypeDef,
+        "AssignmentReviewReport": ReviewReportTypeDef,
+        "HITReviewReport": ReviewReportTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk/type_defs.pyi` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -70,15 +70,14 @@
     "ListWorkerBlocksRequestRequestTypeDef",
     "WorkerBlockTypeDef",
     "ListWorkersWithQualificationTypeRequestRequestTypeDef",
     "LocaleTypeDef",
     "NotificationSpecificationTypeDef",
     "NotifyWorkersFailureStatusTypeDef",
     "NotifyWorkersRequestRequestTypeDef",
-    "ParameterMapEntryOutputTypeDef",
     "ParameterMapEntryTypeDef",
     "RejectAssignmentRequestRequestTypeDef",
     "RejectQualificationRequestRequestRequestTypeDef",
     "ReviewActionDetailTypeDef",
     "ReviewResultDetailTypeDef",
     "SendBonusRequestRequestTypeDef",
     "TimestampTypeDef",
@@ -101,42 +100,37 @@
     "ListQualificationRequestsRequestListQualificationRequestsPaginateTypeDef",
     "ListQualificationTypesRequestListQualificationTypesPaginateTypeDef",
     "ListReviewableHITsRequestListReviewableHITsPaginateTypeDef",
     "ListWorkerBlocksRequestListWorkerBlocksPaginateTypeDef",
     "ListWorkersWithQualificationTypeRequestListWorkersWithQualificationTypePaginateTypeDef",
     "ListQualificationRequestsResponseTypeDef",
     "ListWorkerBlocksResponseTypeDef",
-    "QualificationRequirementOutputTypeDef",
     "QualificationRequirementTypeDef",
     "QualificationTypeDef",
     "SendTestEventNotificationRequestRequestTypeDef",
     "UpdateNotificationSettingsRequestRequestTypeDef",
     "NotifyWorkersResponseTypeDef",
-    "PolicyParameterOutputTypeDef",
     "PolicyParameterTypeDef",
     "ReviewReportTypeDef",
     "UpdateExpirationForHITRequestRequestTypeDef",
+    "CreateHITTypeRequestRequestTypeDef",
     "HITTypeDef",
-    "QualificationRequirementUnionTypeDef",
     "GetQualificationScoreResponseTypeDef",
     "ListWorkersWithQualificationTypeResponseTypeDef",
-    "ReviewPolicyOutputTypeDef",
     "ReviewPolicyTypeDef",
     "CreateHITResponseTypeDef",
     "CreateHITWithHITTypeResponseTypeDef",
     "GetAssignmentResponseTypeDef",
     "GetHITResponseTypeDef",
     "ListHITsForQualificationTypeResponseTypeDef",
     "ListHITsResponseTypeDef",
     "ListReviewableHITsResponseTypeDef",
-    "CreateHITTypeRequestRequestTypeDef",
-    "ListReviewPolicyResultsForHITResponseTypeDef",
     "CreateHITRequestRequestTypeDef",
     "CreateHITWithHITTypeRequestRequestTypeDef",
-    "ReviewPolicyUnionTypeDef",
+    "ListReviewPolicyResultsForHITResponseTypeDef",
 )
 
 _RequiredAcceptQualificationRequestRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptQualificationRequestRequestRequestTypeDef",
     {
         "QualificationRequestId": str,
     },
@@ -651,23 +645,14 @@
     {
         "Subject": str,
         "MessageText": str,
         "WorkerIds": Sequence[str],
     },
 )
 
-ParameterMapEntryOutputTypeDef = TypedDict(
-    "ParameterMapEntryOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-    },
-    total=False,
-)
-
 ParameterMapEntryTypeDef = TypedDict(
     "ParameterMapEntryTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -1031,37 +1016,14 @@
         "NextToken": str,
         "NumResults": int,
         "WorkerBlocks": List[WorkerBlockTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredQualificationRequirementOutputTypeDef = TypedDict(
-    "_RequiredQualificationRequirementOutputTypeDef",
-    {
-        "QualificationTypeId": str,
-        "Comparator": ComparatorType,
-    },
-)
-_OptionalQualificationRequirementOutputTypeDef = TypedDict(
-    "_OptionalQualificationRequirementOutputTypeDef",
-    {
-        "IntegerValues": List[int],
-        "LocaleValues": List[LocaleTypeDef],
-        "RequiredToPreview": bool,
-        "ActionsGuarded": HITAccessActionsType,
-    },
-    total=False,
-)
-
-class QualificationRequirementOutputTypeDef(
-    _RequiredQualificationRequirementOutputTypeDef, _OptionalQualificationRequirementOutputTypeDef
-):
-    pass
-
 _RequiredQualificationRequirementTypeDef = TypedDict(
     "_RequiredQualificationRequirementTypeDef",
     {
         "QualificationTypeId": str,
         "Comparator": ComparatorType,
     },
 )
@@ -1127,24 +1089,14 @@
     "NotifyWorkersResponseTypeDef",
     {
         "NotifyWorkersFailureStatuses": List[NotifyWorkersFailureStatusTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PolicyParameterOutputTypeDef = TypedDict(
-    "PolicyParameterOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-        "MapEntries": List[ParameterMapEntryOutputTypeDef],
-    },
-    total=False,
-)
-
 PolicyParameterTypeDef = TypedDict(
     "PolicyParameterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MapEntries": Sequence[ParameterMapEntryTypeDef],
     },
@@ -1164,14 +1116,38 @@
     "UpdateExpirationForHITRequestRequestTypeDef",
     {
         "HITId": str,
         "ExpireAt": TimestampTypeDef,
     },
 )
 
+_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateHITTypeRequestRequestTypeDef",
+    {
+        "AssignmentDurationInSeconds": int,
+        "Reward": str,
+        "Title": str,
+        "Description": str,
+    },
+)
+_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateHITTypeRequestRequestTypeDef",
+    {
+        "AutoApprovalDelayInSeconds": int,
+        "Keywords": str,
+        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
+    },
+    total=False,
+)
+
+class CreateHITTypeRequestRequestTypeDef(
+    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
+):
+    pass
+
 HITTypeDef = TypedDict(
     "HITTypeDef",
     {
         "HITId": str,
         "HITTypeId": str,
         "HITGroupId": str,
         "HITLayoutId": str,
@@ -1183,26 +1159,23 @@
         "HITStatus": HITStatusType,
         "MaxAssignments": int,
         "Reward": str,
         "AutoApprovalDelayInSeconds": int,
         "Expiration": datetime,
         "AssignmentDurationInSeconds": int,
         "RequesterAnnotation": str,
-        "QualificationRequirements": List[QualificationRequirementOutputTypeDef],
+        "QualificationRequirements": List[QualificationRequirementTypeDef],
         "HITReviewStatus": HITReviewStatusType,
         "NumberOfAssignmentsPending": int,
         "NumberOfAssignmentsAvailable": int,
         "NumberOfAssignmentsCompleted": int,
     },
     total=False,
 )
 
-QualificationRequirementUnionTypeDef = Union[
-    QualificationRequirementTypeDef, QualificationRequirementOutputTypeDef
-]
 GetQualificationScoreResponseTypeDef = TypedDict(
     "GetQualificationScoreResponseTypeDef",
     {
         "Qualification": QualificationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1213,33 +1186,14 @@
         "NextToken": str,
         "NumResults": int,
         "Qualifications": List[QualificationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredReviewPolicyOutputTypeDef = TypedDict(
-    "_RequiredReviewPolicyOutputTypeDef",
-    {
-        "PolicyName": str,
-    },
-)
-_OptionalReviewPolicyOutputTypeDef = TypedDict(
-    "_OptionalReviewPolicyOutputTypeDef",
-    {
-        "Parameters": List[PolicyParameterOutputTypeDef],
-    },
-    total=False,
-)
-
-class ReviewPolicyOutputTypeDef(
-    _RequiredReviewPolicyOutputTypeDef, _OptionalReviewPolicyOutputTypeDef
-):
-    pass
-
 _RequiredReviewPolicyTypeDef = TypedDict(
     "_RequiredReviewPolicyTypeDef",
     {
         "PolicyName": str,
     },
 )
 _OptionalReviewPolicyTypeDef = TypedDict(
@@ -1312,51 +1266,14 @@
         "NextToken": str,
         "NumResults": int,
         "HITs": List[HITTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateHITTypeRequestRequestTypeDef",
-    {
-        "AssignmentDurationInSeconds": int,
-        "Reward": str,
-        "Title": str,
-        "Description": str,
-    },
-)
-_OptionalCreateHITTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateHITTypeRequestRequestTypeDef",
-    {
-        "AutoApprovalDelayInSeconds": int,
-        "Keywords": str,
-        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateHITTypeRequestRequestTypeDef(
-    _RequiredCreateHITTypeRequestRequestTypeDef, _OptionalCreateHITTypeRequestRequestTypeDef
-):
-    pass
-
-ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
-    "ListReviewPolicyResultsForHITResponseTypeDef",
-    {
-        "HITId": str,
-        "AssignmentReviewPolicy": ReviewPolicyOutputTypeDef,
-        "HITReviewPolicy": ReviewPolicyOutputTypeDef,
-        "AssignmentReviewReport": ReviewReportTypeDef,
-        "HITReviewReport": ReviewReportTypeDef,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateHITRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHITRequestRequestTypeDef",
     {
         "LifetimeInSeconds": int,
         "AssignmentDurationInSeconds": int,
         "Reward": str,
         "Title": str,
@@ -1367,15 +1284,15 @@
     "_OptionalCreateHITRequestRequestTypeDef",
     {
         "MaxAssignments": int,
         "AutoApprovalDelayInSeconds": int,
         "Keywords": str,
         "Question": str,
         "RequesterAnnotation": str,
-        "QualificationRequirements": Sequence[QualificationRequirementUnionTypeDef],
+        "QualificationRequirements": Sequence[QualificationRequirementTypeDef],
         "UniqueRequestToken": str,
         "AssignmentReviewPolicy": ReviewPolicyTypeDef,
         "HITReviewPolicy": ReviewPolicyTypeDef,
         "HITLayoutId": str,
         "HITLayoutParameters": Sequence[HITLayoutParameterTypeDef],
     },
     total=False,
@@ -1410,8 +1327,19 @@
 
 class CreateHITWithHITTypeRequestRequestTypeDef(
     _RequiredCreateHITWithHITTypeRequestRequestTypeDef,
     _OptionalCreateHITWithHITTypeRequestRequestTypeDef,
 ):
     pass
 
-ReviewPolicyUnionTypeDef = Union[ReviewPolicyTypeDef, ReviewPolicyOutputTypeDef]
+ListReviewPolicyResultsForHITResponseTypeDef = TypedDict(
+    "ListReviewPolicyResultsForHITResponseTypeDef",
+    {
+        "HITId": str,
+        "AssignmentReviewPolicy": ReviewPolicyTypeDef,
+        "HITReviewPolicy": ReviewPolicyTypeDef,
+        "AssignmentReviewReport": ReviewReportTypeDef,
+        "HITReviewReport": ReviewReportTypeDef,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-mturk-2.5.2.post1/types_aiobotocore_mturk.egg-info/SOURCES.txt` & `types-aiobotocore-mturk-2.5.2.post2/types_aiobotocore_mturk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

