# Comparing `tmp/types-aiobotocore-textract-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-textract-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-textract-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-textract-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
```

## Comparing `types-aiobotocore-textract-2.5.2.post1.tar` & `types-aiobotocore-textract-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.865439 types-aiobotocore-textract-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-08-02 14:53:06.861439 types-aiobotocore-textract-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.865439 types-aiobotocore-textract-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.861439 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14089 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23383 2023-08-02 14:50:34.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:33.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.861439 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:06.000000 types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.626643 types-aiobotocore-textract-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12235 2023-08-04 13:59:28.626643 types-aiobotocore-textract-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10713 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.626643 types-aiobotocore-textract-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.626643 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      450 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      449 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14110 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14089 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9142 2023-08-04 13:55:02.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9140 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22984 2023-08-04 13:55:02.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22957 2023-08-04 13:55:02.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:01.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.626643 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12235 2023-08-04 13:59:28.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      751 2023-08-04 13:59:28.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:28.000000 types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-textract-2.5.2.post1/LICENSE` & `types-aiobotocore-textract-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.5.2.post1/setup.py` & `types-aiobotocore-textract-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-textract",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_textract"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Textract 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/__main__.py` & `types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Textract 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Textract 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract\nOther"
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

### Comparing `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/client.py` & `types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/client.pyi` & `types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/literals.py` & `types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
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
@@ -195,14 +196,15 @@
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
@@ -281,26 +283,28 @@
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

### Comparing `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/literals.pyi` & `types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/literals.pyi`

 * *Files 1% similar despite different names*

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

### Comparing `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/type_defs.py` & `types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 __all__ = (
     "DocumentMetadataTypeDef",
     "HumanLoopActivationOutputTypeDef",
     "ResponseMetadataTypeDef",
     "NormalizedValueTypeDef",
     "BlobTypeDef",
-    "QueryOutputTypeDef",
+    "QueryTypeDef",
     "RelationshipTypeDef",
     "BoundingBoxTypeDef",
     "DetectedSignatureTypeDef",
     "SplitDocumentTypeDef",
     "UndetectedSignatureTypeDef",
     "S3ObjectTypeDef",
     "ExpenseCurrencyTypeDef",
@@ -60,41 +60,40 @@
     "GetExpenseAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryRequestRequestTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "NotificationChannelTypeDef",
     "OutputConfigTypeDef",
     "PredictionTypeDef",
-    "QueryTypeDef",
     "StartDocumentAnalysisResponseTypeDef",
     "StartDocumentTextDetectionResponseTypeDef",
     "StartExpenseAnalysisResponseTypeDef",
     "StartLendingAnalysisResponseTypeDef",
     "AnalyzeIDDetectionsTypeDef",
+    "QueriesConfigTypeDef",
     "DocumentGroupTypeDef",
     "DocumentLocationTypeDef",
     "DocumentTypeDef",
     "GeometryTypeDef",
     "HumanLoopConfigTypeDef",
     "PageClassificationTypeDef",
-    "QueriesConfigTypeDef",
     "IdentityDocumentFieldTypeDef",
     "LendingSummaryTypeDef",
+    "StartDocumentAnalysisRequestRequestTypeDef",
     "StartDocumentTextDetectionRequestRequestTypeDef",
     "StartExpenseAnalysisRequestRequestTypeDef",
     "StartLendingAnalysisRequestRequestTypeDef",
     "AnalyzeExpenseRequestRequestTypeDef",
     "AnalyzeIDRequestRequestTypeDef",
     "DetectDocumentTextRequestRequestTypeDef",
     "BlockTypeDef",
     "ExpenseDetectionTypeDef",
     "LendingDetectionTypeDef",
     "SignatureDetectionTypeDef",
     "AnalyzeDocumentRequestRequestTypeDef",
-    "StartDocumentAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryResponseTypeDef",
     "AnalyzeDocumentResponseTypeDef",
     "DetectDocumentTextResponseTypeDef",
     "GetDocumentAnalysisResponseTypeDef",
     "GetDocumentTextDetectionResponseTypeDef",
     "IdentityDocumentTypeDef",
     "ExpenseFieldTypeDef",
@@ -146,31 +145,31 @@
         "Value": str,
         "ValueType": Literal["DATE"],
     },
     total=False,
 )
 
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-_RequiredQueryOutputTypeDef = TypedDict(
-    "_RequiredQueryOutputTypeDef",
+_RequiredQueryTypeDef = TypedDict(
+    "_RequiredQueryTypeDef",
     {
         "Text": str,
     },
 )
-_OptionalQueryOutputTypeDef = TypedDict(
-    "_OptionalQueryOutputTypeDef",
+_OptionalQueryTypeDef = TypedDict(
+    "_OptionalQueryTypeDef",
     {
         "Alias": str,
-        "Pages": List[str],
+        "Pages": Sequence[str],
     },
     total=False,
 )
 
 
-class QueryOutputTypeDef(_RequiredQueryOutputTypeDef, _OptionalQueryOutputTypeDef):
+class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
     pass
 
 
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "Type": RelationshipTypeType,
@@ -409,34 +408,14 @@
     {
         "Value": str,
         "Confidence": float,
     },
     total=False,
 )
 
-_RequiredQueryTypeDef = TypedDict(
-    "_RequiredQueryTypeDef",
-    {
-        "Text": str,
-    },
-)
-_OptionalQueryTypeDef = TypedDict(
-    "_OptionalQueryTypeDef",
-    {
-        "Alias": str,
-        "Pages": Sequence[str],
-    },
-    total=False,
-)
-
-
-class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
-    pass
-
-
 StartDocumentAnalysisResponseTypeDef = TypedDict(
     "StartDocumentAnalysisResponseTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -483,14 +462,21 @@
 
 class AnalyzeIDDetectionsTypeDef(
     _RequiredAnalyzeIDDetectionsTypeDef, _OptionalAnalyzeIDDetectionsTypeDef
 ):
     pass
 
 
+QueriesConfigTypeDef = TypedDict(
+    "QueriesConfigTypeDef",
+    {
+        "Queries": Sequence[QueryTypeDef],
+    },
+)
+
 DocumentGroupTypeDef = TypedDict(
     "DocumentGroupTypeDef",
     {
         "Type": str,
         "SplitDocuments": List[SplitDocumentTypeDef],
         "DetectedSignatures": List[DetectedSignatureTypeDef],
         "UndetectedSignatures": List[UndetectedSignatureTypeDef],
@@ -548,21 +534,14 @@
     "PageClassificationTypeDef",
     {
         "PageType": List[PredictionTypeDef],
         "PageNumber": List[PredictionTypeDef],
     },
 )
 
-QueriesConfigTypeDef = TypedDict(
-    "QueriesConfigTypeDef",
-    {
-        "Queries": Sequence[QueryTypeDef],
-    },
-)
-
 IdentityDocumentFieldTypeDef = TypedDict(
     "IdentityDocumentFieldTypeDef",
     {
         "Type": AnalyzeIDDetectionsTypeDef,
         "ValueDetection": AnalyzeIDDetectionsTypeDef,
     },
     total=False,
@@ -573,14 +552,42 @@
     {
         "DocumentGroups": List[DocumentGroupTypeDef],
         "UndetectedDocumentTypes": List[str],
     },
     total=False,
 )
 
+_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "DocumentLocation": DocumentLocationTypeDef,
+        "FeatureTypes": Sequence[FeatureTypeType],
+    },
+)
+_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "JobTag": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "OutputConfig": OutputConfigTypeDef,
+        "KMSKeyId": str,
+        "QueriesConfig": QueriesConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class StartDocumentAnalysisRequestRequestTypeDef(
+    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
+    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentTextDetectionRequestRequestTypeDef",
     {
         "DocumentLocation": DocumentLocationTypeDef,
     },
 )
 _OptionalStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
@@ -689,15 +696,15 @@
         "ColumnSpan": int,
         "Geometry": GeometryTypeDef,
         "Id": str,
         "Relationships": List[RelationshipTypeDef],
         "EntityTypes": List[EntityTypeType],
         "SelectionStatus": SelectionStatusType,
         "Page": int,
-        "Query": QueryOutputTypeDef,
+        "Query": QueryTypeDef,
     },
     total=False,
 )
 
 ExpenseDetectionTypeDef = TypedDict(
     "ExpenseDetectionTypeDef",
     {
@@ -747,42 +754,14 @@
 
 class AnalyzeDocumentRequestRequestTypeDef(
     _RequiredAnalyzeDocumentRequestRequestTypeDef, _OptionalAnalyzeDocumentRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "DocumentLocation": DocumentLocationTypeDef,
-        "FeatureTypes": Sequence[FeatureTypeType],
-    },
-)
-_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "JobTag": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "OutputConfig": OutputConfigTypeDef,
-        "KMSKeyId": str,
-        "QueriesConfig": QueriesConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class StartDocumentAnalysisRequestRequestTypeDef(
-    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
-    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
-):
-    pass
-
-
 GetLendingAnalysisSummaryResponseTypeDef = TypedDict(
     "GetLendingAnalysisSummaryResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "Summary": LendingSummaryTypeDef,
         "Warnings": List[WarningTypeDef],
```

### Comparing `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract/type_defs.pyi` & `types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 __all__ = (
     "DocumentMetadataTypeDef",
     "HumanLoopActivationOutputTypeDef",
     "ResponseMetadataTypeDef",
     "NormalizedValueTypeDef",
     "BlobTypeDef",
-    "QueryOutputTypeDef",
+    "QueryTypeDef",
     "RelationshipTypeDef",
     "BoundingBoxTypeDef",
     "DetectedSignatureTypeDef",
     "SplitDocumentTypeDef",
     "UndetectedSignatureTypeDef",
     "S3ObjectTypeDef",
     "ExpenseCurrencyTypeDef",
@@ -59,41 +59,40 @@
     "GetExpenseAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryRequestRequestTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "NotificationChannelTypeDef",
     "OutputConfigTypeDef",
     "PredictionTypeDef",
-    "QueryTypeDef",
     "StartDocumentAnalysisResponseTypeDef",
     "StartDocumentTextDetectionResponseTypeDef",
     "StartExpenseAnalysisResponseTypeDef",
     "StartLendingAnalysisResponseTypeDef",
     "AnalyzeIDDetectionsTypeDef",
+    "QueriesConfigTypeDef",
     "DocumentGroupTypeDef",
     "DocumentLocationTypeDef",
     "DocumentTypeDef",
     "GeometryTypeDef",
     "HumanLoopConfigTypeDef",
     "PageClassificationTypeDef",
-    "QueriesConfigTypeDef",
     "IdentityDocumentFieldTypeDef",
     "LendingSummaryTypeDef",
+    "StartDocumentAnalysisRequestRequestTypeDef",
     "StartDocumentTextDetectionRequestRequestTypeDef",
     "StartExpenseAnalysisRequestRequestTypeDef",
     "StartLendingAnalysisRequestRequestTypeDef",
     "AnalyzeExpenseRequestRequestTypeDef",
     "AnalyzeIDRequestRequestTypeDef",
     "DetectDocumentTextRequestRequestTypeDef",
     "BlockTypeDef",
     "ExpenseDetectionTypeDef",
     "LendingDetectionTypeDef",
     "SignatureDetectionTypeDef",
     "AnalyzeDocumentRequestRequestTypeDef",
-    "StartDocumentAnalysisRequestRequestTypeDef",
     "GetLendingAnalysisSummaryResponseTypeDef",
     "AnalyzeDocumentResponseTypeDef",
     "DetectDocumentTextResponseTypeDef",
     "GetDocumentAnalysisResponseTypeDef",
     "GetDocumentTextDetectionResponseTypeDef",
     "IdentityDocumentTypeDef",
     "ExpenseFieldTypeDef",
@@ -145,30 +144,30 @@
         "Value": str,
         "ValueType": Literal["DATE"],
     },
     total=False,
 )
 
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-_RequiredQueryOutputTypeDef = TypedDict(
-    "_RequiredQueryOutputTypeDef",
+_RequiredQueryTypeDef = TypedDict(
+    "_RequiredQueryTypeDef",
     {
         "Text": str,
     },
 )
-_OptionalQueryOutputTypeDef = TypedDict(
-    "_OptionalQueryOutputTypeDef",
+_OptionalQueryTypeDef = TypedDict(
+    "_OptionalQueryTypeDef",
     {
         "Alias": str,
-        "Pages": List[str],
+        "Pages": Sequence[str],
     },
     total=False,
 )
 
-class QueryOutputTypeDef(_RequiredQueryOutputTypeDef, _OptionalQueryOutputTypeDef):
+class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
     pass
 
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "Type": RelationshipTypeType,
         "Ids": List[str],
@@ -396,32 +395,14 @@
     {
         "Value": str,
         "Confidence": float,
     },
     total=False,
 )
 
-_RequiredQueryTypeDef = TypedDict(
-    "_RequiredQueryTypeDef",
-    {
-        "Text": str,
-    },
-)
-_OptionalQueryTypeDef = TypedDict(
-    "_OptionalQueryTypeDef",
-    {
-        "Alias": str,
-        "Pages": Sequence[str],
-    },
-    total=False,
-)
-
-class QueryTypeDef(_RequiredQueryTypeDef, _OptionalQueryTypeDef):
-    pass
-
 StartDocumentAnalysisResponseTypeDef = TypedDict(
     "StartDocumentAnalysisResponseTypeDef",
     {
         "JobId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -466,14 +447,21 @@
 )
 
 class AnalyzeIDDetectionsTypeDef(
     _RequiredAnalyzeIDDetectionsTypeDef, _OptionalAnalyzeIDDetectionsTypeDef
 ):
     pass
 
+QueriesConfigTypeDef = TypedDict(
+    "QueriesConfigTypeDef",
+    {
+        "Queries": Sequence[QueryTypeDef],
+    },
+)
+
 DocumentGroupTypeDef = TypedDict(
     "DocumentGroupTypeDef",
     {
         "Type": str,
         "SplitDocuments": List[SplitDocumentTypeDef],
         "DetectedSignatures": List[DetectedSignatureTypeDef],
         "UndetectedSignatures": List[UndetectedSignatureTypeDef],
@@ -529,21 +517,14 @@
     "PageClassificationTypeDef",
     {
         "PageType": List[PredictionTypeDef],
         "PageNumber": List[PredictionTypeDef],
     },
 )
 
-QueriesConfigTypeDef = TypedDict(
-    "QueriesConfigTypeDef",
-    {
-        "Queries": Sequence[QueryTypeDef],
-    },
-)
-
 IdentityDocumentFieldTypeDef = TypedDict(
     "IdentityDocumentFieldTypeDef",
     {
         "Type": AnalyzeIDDetectionsTypeDef,
         "ValueDetection": AnalyzeIDDetectionsTypeDef,
     },
     total=False,
@@ -554,14 +535,40 @@
     {
         "DocumentGroups": List[DocumentGroupTypeDef],
         "UndetectedDocumentTypes": List[str],
     },
     total=False,
 )
 
+_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "DocumentLocation": DocumentLocationTypeDef,
+        "FeatureTypes": Sequence[FeatureTypeType],
+    },
+)
+_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
+    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "JobTag": str,
+        "NotificationChannel": NotificationChannelTypeDef,
+        "OutputConfig": OutputConfigTypeDef,
+        "KMSKeyId": str,
+        "QueriesConfig": QueriesConfigTypeDef,
+    },
+    total=False,
+)
+
+class StartDocumentAnalysisRequestRequestTypeDef(
+    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
+    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
+):
+    pass
+
 _RequiredStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentTextDetectionRequestRequestTypeDef",
     {
         "DocumentLocation": DocumentLocationTypeDef,
     },
 )
 _OptionalStartDocumentTextDetectionRequestRequestTypeDef = TypedDict(
@@ -664,15 +671,15 @@
         "ColumnSpan": int,
         "Geometry": GeometryTypeDef,
         "Id": str,
         "Relationships": List[RelationshipTypeDef],
         "EntityTypes": List[EntityTypeType],
         "SelectionStatus": SelectionStatusType,
         "Page": int,
-        "Query": QueryOutputTypeDef,
+        "Query": QueryTypeDef,
     },
     total=False,
 )
 
 ExpenseDetectionTypeDef = TypedDict(
     "ExpenseDetectionTypeDef",
     {
@@ -720,40 +727,14 @@
 )
 
 class AnalyzeDocumentRequestRequestTypeDef(
     _RequiredAnalyzeDocumentRequestRequestTypeDef, _OptionalAnalyzeDocumentRequestRequestTypeDef
 ):
     pass
 
-_RequiredStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_RequiredStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "DocumentLocation": DocumentLocationTypeDef,
-        "FeatureTypes": Sequence[FeatureTypeType],
-    },
-)
-_OptionalStartDocumentAnalysisRequestRequestTypeDef = TypedDict(
-    "_OptionalStartDocumentAnalysisRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "JobTag": str,
-        "NotificationChannel": NotificationChannelTypeDef,
-        "OutputConfig": OutputConfigTypeDef,
-        "KMSKeyId": str,
-        "QueriesConfig": QueriesConfigTypeDef,
-    },
-    total=False,
-)
-
-class StartDocumentAnalysisRequestRequestTypeDef(
-    _RequiredStartDocumentAnalysisRequestRequestTypeDef,
-    _OptionalStartDocumentAnalysisRequestRequestTypeDef,
-):
-    pass
-
 GetLendingAnalysisSummaryResponseTypeDef = TypedDict(
     "GetLendingAnalysisSummaryResponseTypeDef",
     {
         "DocumentMetadata": DocumentMetadataTypeDef,
         "JobStatus": JobStatusType,
         "Summary": LendingSummaryTypeDef,
         "Warnings": List[WarningTypeDef],
```

### Comparing `types-aiobotocore-textract-2.5.2.post1/types_aiobotocore_textract.egg-info/SOURCES.txt` & `types-aiobotocore-textract-2.5.2.post2/types_aiobotocore_textract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

