# Comparing `tmp/types-aiobotocore-omics-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-omics-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-omics-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-omics-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-omics-2.5.2.post1.tar` & `types-aiobotocore-omics-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.929506 types-aiobotocore-omics-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29782 2023-08-02 14:52:44.925506 types-aiobotocore-omics-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28272 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:44.929506 types-aiobotocore-omics-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.909506 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64693 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    64579 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15764 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22881 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98055 2023-08-02 14:44:17.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97899 2023-08-02 14:44:14.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:12.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-08-02 14:44:13.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:44.925506 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29782 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:44.000000 types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.026643 types-aiobotocore-omics-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18326 2023-08-04 13:59:20.026643 types-aiobotocore-omics-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16816 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.026643 types-aiobotocore-omics-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2058 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.016643 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7574 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7573 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      924 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    64683 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    64569 2023-08-04 13:45:51.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15939 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15937 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22901 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22881 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    97568 2023-08-04 13:45:56.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    97412 2023-08-04 13:45:53.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:50.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15945 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15929 2023-08-04 13:45:52.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.026643 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18326 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      844 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:19.000000 types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-omics-2.5.2.post1/LICENSE` & `types-aiobotocore-omics-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post1/setup.py` & `types-aiobotocore-omics-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-omics",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Omics 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__init__.py` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__init__.pyi` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/__main__.py` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Omics 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Omics 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
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

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/client.py` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
-    StoreOptionsUnionTypeDef,
+    StoreOptionsTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     VariantImportItemSourceTypeDef,
     WorkflowParameterTypeDef,
 )
 from .waiter import (
@@ -284,15 +284,15 @@
         *,
         storeFormat: StoreFormatType,
         reference: ReferenceItemTypeDef = ...,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
         sseConfig: SseConfigTypeDef = ...,
-        storeOptions: StoreOptionsUnionTypeDef = ...
+        storeOptions: StoreOptionsTypeDef = ...
     ) -> CreateAnnotationStoreResponseTypeDef:
         """
         Creates an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_annotation_store)
         """
```

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/client.pyi` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     StartReadSetExportJobResponseTypeDef,
     StartReadSetImportJobResponseTypeDef,
     StartReadSetImportJobSourceItemTypeDef,
     StartReferenceImportJobResponseTypeDef,
     StartReferenceImportJobSourceItemTypeDef,
     StartRunResponseTypeDef,
     StartVariantImportResponseTypeDef,
-    StoreOptionsUnionTypeDef,
+    StoreOptionsTypeDef,
     UpdateAnnotationStoreResponseTypeDef,
     UpdateVariantStoreResponseTypeDef,
     UploadReadSetPartResponseTypeDef,
     VariantImportItemSourceTypeDef,
     WorkflowParameterTypeDef,
 )
 from .waiter import (
@@ -271,15 +271,15 @@
         *,
         storeFormat: StoreFormatType,
         reference: ReferenceItemTypeDef = ...,
         name: str = ...,
         description: str = ...,
         tags: Mapping[str, str] = ...,
         sseConfig: SseConfigTypeDef = ...,
-        storeOptions: StoreOptionsUnionTypeDef = ...
+        storeOptions: StoreOptionsTypeDef = ...
     ) -> CreateAnnotationStoreResponseTypeDef:
         """
         Creates an annotation store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics.Client.create_annotation_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_omics/client/#create_annotation_store)
         """
```

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/literals.py` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AcceleratorsType",
     "AnnotationImportJobCreatedWaiterName",
     "AnnotationStoreCreatedWaiterName",
     "AnnotationStoreDeletedWaiterName",
     "AnnotationTypeType",
+    "CreationTypeType",
     "EncryptionTypeType",
     "FileTypeType",
     "FormatToHeaderKeyType",
     "JobStatusType",
     "ListAnnotationImportJobsPaginatorName",
     "ListAnnotationStoresPaginatorName",
     "ListMultipartReadSetUploadsPaginatorName",
@@ -87,28 +87,28 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AcceleratorsType = Literal["GPU"]
 AnnotationImportJobCreatedWaiterName = Literal["annotation_import_job_created"]
 AnnotationStoreCreatedWaiterName = Literal["annotation_store_created"]
 AnnotationStoreDeletedWaiterName = Literal["annotation_store_deleted"]
 AnnotationTypeType = Literal[
     "CHR_POS",
     "CHR_POS_REF_ALT",
     "CHR_START_END_ONE_BASE",
     "CHR_START_END_REF_ALT_ONE_BASE",
     "CHR_START_END_REF_ALT_ZERO_BASE",
     "CHR_START_END_ZERO_BASE",
     "GENERIC",
 ]
+CreationTypeType = Literal["IMPORT", "UPLOAD"]
 EncryptionTypeType = Literal["KMS"]
 FileTypeType = Literal["BAM", "CRAM", "FASTQ"]
 FormatToHeaderKeyType = Literal["ALT", "CHR", "END", "POS", "REF", "START"]
 JobStatusType = Literal[
     "CANCELLED", "COMPLETED", "COMPLETED_WITH_FAILURES", "FAILED", "IN_PROGRESS", "SUBMITTED"
 ]
 ListAnnotationImportJobsPaginatorName = Literal["list_annotation_import_jobs"]
@@ -195,15 +195,15 @@
 TaskStatusType = Literal[
     "CANCELLED", "COMPLETED", "FAILED", "PENDING", "RUNNING", "STARTING", "STOPPING"
 ]
 VariantImportJobCreatedWaiterName = Literal["variant_import_job_created"]
 VariantStoreCreatedWaiterName = Literal["variant_store_created"]
 VariantStoreDeletedWaiterName = Literal["variant_store_deleted"]
 WorkflowActiveWaiterName = Literal["workflow_active"]
-WorkflowEngineType = Literal["NEXTFLOW", "WDL"]
+WorkflowEngineType = Literal["CWL", "NEXTFLOW", "WDL"]
 WorkflowExportType = Literal["DEFINITION"]
 WorkflowStatusType = Literal["ACTIVE", "CREATING", "DELETED", "FAILED", "INACTIVE", "UPDATING"]
 WorkflowTypeType = Literal["PRIVATE", "READY2RUN"]
 OmicsServiceName = Literal["omics"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -215,14 +215,15 @@
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
@@ -318,14 +319,15 @@
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
@@ -404,26 +406,28 @@
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

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/literals.pyi` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AcceleratorsType",
     "AnnotationImportJobCreatedWaiterName",
     "AnnotationStoreCreatedWaiterName",
     "AnnotationStoreDeletedWaiterName",
     "AnnotationTypeType",
+    "CreationTypeType",
     "EncryptionTypeType",
     "FileTypeType",
     "FormatToHeaderKeyType",
     "JobStatusType",
     "ListAnnotationImportJobsPaginatorName",
     "ListAnnotationStoresPaginatorName",
     "ListMultipartReadSetUploadsPaginatorName",
@@ -86,27 +88,29 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AcceleratorsType = Literal["GPU"]
 AnnotationImportJobCreatedWaiterName = Literal["annotation_import_job_created"]
 AnnotationStoreCreatedWaiterName = Literal["annotation_store_created"]
 AnnotationStoreDeletedWaiterName = Literal["annotation_store_deleted"]
 AnnotationTypeType = Literal[
     "CHR_POS",
     "CHR_POS_REF_ALT",
     "CHR_START_END_ONE_BASE",
     "CHR_START_END_REF_ALT_ONE_BASE",
     "CHR_START_END_REF_ALT_ZERO_BASE",
     "CHR_START_END_ZERO_BASE",
     "GENERIC",
 ]
+CreationTypeType = Literal["IMPORT", "UPLOAD"]
 EncryptionTypeType = Literal["KMS"]
 FileTypeType = Literal["BAM", "CRAM", "FASTQ"]
 FormatToHeaderKeyType = Literal["ALT", "CHR", "END", "POS", "REF", "START"]
 JobStatusType = Literal[
     "CANCELLED", "COMPLETED", "COMPLETED_WITH_FAILURES", "FAILED", "IN_PROGRESS", "SUBMITTED"
 ]
 ListAnnotationImportJobsPaginatorName = Literal["list_annotation_import_jobs"]
@@ -193,15 +197,15 @@
 TaskStatusType = Literal[
     "CANCELLED", "COMPLETED", "FAILED", "PENDING", "RUNNING", "STARTING", "STOPPING"
 ]
 VariantImportJobCreatedWaiterName = Literal["variant_import_job_created"]
 VariantStoreCreatedWaiterName = Literal["variant_store_created"]
 VariantStoreDeletedWaiterName = Literal["variant_store_deleted"]
 WorkflowActiveWaiterName = Literal["workflow_active"]
-WorkflowEngineType = Literal["NEXTFLOW", "WDL"]
+WorkflowEngineType = Literal["CWL", "NEXTFLOW", "WDL"]
 WorkflowExportType = Literal["DEFINITION"]
 WorkflowStatusType = Literal["ACTIVE", "CREATING", "DELETED", "FAILED", "INACTIVE", "UPDATING"]
 WorkflowTypeType = Literal["PRIVATE", "READY2RUN"]
 OmicsServiceName = Literal["omics"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
@@ -213,14 +217,15 @@
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
@@ -316,14 +321,15 @@
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
@@ -402,26 +408,28 @@
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

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/paginator.py` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/paginator.pyi` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/type_defs.py` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
 from .literals import (
     AnnotationTypeType,
+    CreationTypeType,
     FileTypeType,
     FormatToHeaderKeyType,
     JobStatusType,
     ReadSetActivationJobItemStatusType,
     ReadSetActivationJobStatusType,
     ReadSetExportJobItemStatusType,
     ReadSetExportJobStatusType,
@@ -135,15 +136,14 @@
     "ListWorkflowsRequestRequestTypeDef",
     "WorkflowListItemTypeDef",
     "ReadOptionsTypeDef",
     "StartReadSetActivationJobSourceItemTypeDef",
     "StartReferenceImportJobSourceItemTypeDef",
     "StartRunRequestRequestTypeDef",
     "VariantImportItemSourceTypeDef",
-    "TsvStoreOptionsOutputTypeDef",
     "TsvStoreOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnnotationStoreRequestRequestTypeDef",
     "UpdateRunGroupRequestRequestTypeDef",
     "UpdateVariantStoreRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
@@ -247,15 +247,14 @@
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     "ListVariantStoresRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "TsvOptionsTypeDef",
     "StartReadSetActivationJobRequestRequestTypeDef",
     "StartReferenceImportJobRequestRequestTypeDef",
     "StartVariantImportRequestRequestTypeDef",
-    "StoreOptionsOutputTypeDef",
     "StoreOptionsTypeDef",
     "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
     "ListReadSetActivationJobsRequestRequestTypeDef",
     "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
     "ListReadSetExportJobsRequestRequestTypeDef",
     "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
     "ListReadSetImportJobsRequestRequestTypeDef",
@@ -277,19 +276,18 @@
     "ListVariantStoresResponseTypeDef",
     "GetReadSetMetadataResponseTypeDef",
     "GetReferenceMetadataResponseTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
     "StartReadSetImportJobRequestRequestTypeDef",
     "FormatOptionsTypeDef",
+    "CreateAnnotationStoreRequestRequestTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
-    "CreateAnnotationStoreRequestRequestTypeDef",
-    "StoreOptionsUnionTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
 
 AbortMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     {
@@ -1416,24 +1414,14 @@
 VariantImportItemSourceTypeDef = TypedDict(
     "VariantImportItemSourceTypeDef",
     {
         "source": str,
     },
 )
 
-TsvStoreOptionsOutputTypeDef = TypedDict(
-    "TsvStoreOptionsOutputTypeDef",
-    {
-        "annotationType": AnnotationTypeType,
-        "formatToHeader": Dict[FormatToHeaderKeyType, str],
-        "schema": List[Dict[str, SchemaValueTypeType]],
-    },
-    total=False,
-)
-
 TsvStoreOptionsTypeDef = TypedDict(
     "TsvStoreOptionsTypeDef",
     {
         "annotationType": AnnotationTypeType,
         "formatToHeader": Mapping[FormatToHeaderKeyType, str],
         "schema": Sequence[Mapping[str, SchemaValueTypeType]],
     },
@@ -1594,14 +1582,15 @@
         "status": ReadSetStatusType,
         "referenceArn": str,
         "createdAfter": TimestampTypeDef,
         "createdBefore": TimestampTypeDef,
         "sampleId": str,
         "subjectId": str,
         "generatedFrom": str,
+        "creationType": CreationTypeType,
     },
     total=False,
 )
 
 ReadSetUploadPartListFilterTypeDef = TypedDict(
     "ReadSetUploadPartListFilterTypeDef",
     {
@@ -2681,14 +2670,15 @@
         "subjectId": str,
         "sampleId": str,
         "name": str,
         "description": str,
         "referenceArn": str,
         "sequenceInformation": SequenceInformationTypeDef,
         "statusMessage": str,
+        "creationType": CreationTypeType,
     },
     total=False,
 )
 
 
 class ReadSetListItemTypeDef(_RequiredReadSetListItemTypeDef, _OptionalReadSetListItemTypeDef):
     pass
@@ -3110,22 +3100,14 @@
 class StartVariantImportRequestRequestTypeDef(
     _RequiredStartVariantImportRequestRequestTypeDef,
     _OptionalStartVariantImportRequestRequestTypeDef,
 ):
     pass
 
 
-StoreOptionsOutputTypeDef = TypedDict(
-    "StoreOptionsOutputTypeDef",
-    {
-        "tsvStoreOptions": TsvStoreOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 StoreOptionsTypeDef = TypedDict(
     "StoreOptionsTypeDef",
     {
         "tsvStoreOptions": TsvStoreOptionsTypeDef,
     },
     total=False,
 )
@@ -3548,14 +3530,15 @@
         "description": str,
         "fileType": FileTypeType,
         "creationTime": datetime,
         "sequenceInformation": SequenceInformationTypeDef,
         "referenceArn": str,
         "files": ReadSetFilesTypeDef,
         "statusMessage": str,
+        "creationType": CreationTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReferenceMetadataResponseTypeDef = TypedDict(
     "GetReferenceMetadataResponseTypeDef",
     {
@@ -3626,21 +3609,48 @@
     {
         "tsvOptions": TsvOptionsTypeDef,
         "vcfOptions": VcfOptionsTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
+    {
+        "storeFormat": StoreFormatType,
+    },
+)
+_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
+    {
+        "reference": ReferenceItemTypeDef,
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+        "sseConfig": SseConfigTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateAnnotationStoreRequestRequestTypeDef(
+    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
+    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
+):
+    pass
+
+
 CreateAnnotationStoreResponseTypeDef = TypedDict(
     "CreateAnnotationStoreResponseTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "storeFormat": StoreFormatType,
-        "storeOptions": StoreOptionsOutputTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
         "status": StoreStatusType,
         "name": str,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -3653,15 +3663,15 @@
         "storeArn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
-        "storeOptions": StoreOptionsOutputTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
         "storeFormat": StoreFormatType,
         "statusMessage": str,
         "storeSizeBytes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -3671,48 +3681,20 @@
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
-        "storeOptions": StoreOptionsOutputTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
         "storeFormat": StoreFormatType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
-    {
-        "storeFormat": StoreFormatType,
-    },
-)
-_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
-    {
-        "reference": ReferenceItemTypeDef,
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-        "sseConfig": SseConfigTypeDef,
-        "storeOptions": StoreOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateAnnotationStoreRequestRequestTypeDef(
-    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
-    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
-):
-    pass
-
-
-StoreOptionsUnionTypeDef = Union[StoreOptionsTypeDef, StoreOptionsOutputTypeDef]
 GetAnnotationImportResponseTypeDef = TypedDict(
     "GetAnnotationImportResponseTypeDef",
     {
         "id": str,
         "destinationName": str,
         "roleArn": str,
         "status": JobStatusType,
```

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/type_defs.pyi` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
 from .literals import (
     AnnotationTypeType,
+    CreationTypeType,
     FileTypeType,
     FormatToHeaderKeyType,
     JobStatusType,
     ReadSetActivationJobItemStatusType,
     ReadSetActivationJobStatusType,
     ReadSetExportJobItemStatusType,
     ReadSetExportJobStatusType,
@@ -134,15 +135,14 @@
     "ListWorkflowsRequestRequestTypeDef",
     "WorkflowListItemTypeDef",
     "ReadOptionsTypeDef",
     "StartReadSetActivationJobSourceItemTypeDef",
     "StartReferenceImportJobSourceItemTypeDef",
     "StartRunRequestRequestTypeDef",
     "VariantImportItemSourceTypeDef",
-    "TsvStoreOptionsOutputTypeDef",
     "TsvStoreOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnnotationStoreRequestRequestTypeDef",
     "UpdateRunGroupRequestRequestTypeDef",
     "UpdateVariantStoreRequestRequestTypeDef",
     "UpdateWorkflowRequestRequestTypeDef",
@@ -246,15 +246,14 @@
     "ListVariantStoresRequestListVariantStoresPaginateTypeDef",
     "ListVariantStoresRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
     "TsvOptionsTypeDef",
     "StartReadSetActivationJobRequestRequestTypeDef",
     "StartReferenceImportJobRequestRequestTypeDef",
     "StartVariantImportRequestRequestTypeDef",
-    "StoreOptionsOutputTypeDef",
     "StoreOptionsTypeDef",
     "ListReadSetActivationJobsRequestListReadSetActivationJobsPaginateTypeDef",
     "ListReadSetActivationJobsRequestRequestTypeDef",
     "ListReadSetExportJobsRequestListReadSetExportJobsPaginateTypeDef",
     "ListReadSetExportJobsRequestRequestTypeDef",
     "ListReadSetImportJobsRequestListReadSetImportJobsPaginateTypeDef",
     "ListReadSetImportJobsRequestRequestTypeDef",
@@ -276,19 +275,18 @@
     "ListVariantStoresResponseTypeDef",
     "GetReadSetMetadataResponseTypeDef",
     "GetReferenceMetadataResponseTypeDef",
     "ListReadSetsResponseTypeDef",
     "GetReadSetImportJobResponseTypeDef",
     "StartReadSetImportJobRequestRequestTypeDef",
     "FormatOptionsTypeDef",
+    "CreateAnnotationStoreRequestRequestTypeDef",
     "CreateAnnotationStoreResponseTypeDef",
     "GetAnnotationStoreResponseTypeDef",
     "UpdateAnnotationStoreResponseTypeDef",
-    "CreateAnnotationStoreRequestRequestTypeDef",
-    "StoreOptionsUnionTypeDef",
     "GetAnnotationImportResponseTypeDef",
     "StartAnnotationImportRequestRequestTypeDef",
 )
 
 AbortMultipartReadSetUploadRequestRequestTypeDef = TypedDict(
     "AbortMultipartReadSetUploadRequestRequestTypeDef",
     {
@@ -1361,24 +1359,14 @@
 VariantImportItemSourceTypeDef = TypedDict(
     "VariantImportItemSourceTypeDef",
     {
         "source": str,
     },
 )
 
-TsvStoreOptionsOutputTypeDef = TypedDict(
-    "TsvStoreOptionsOutputTypeDef",
-    {
-        "annotationType": AnnotationTypeType,
-        "formatToHeader": Dict[FormatToHeaderKeyType, str],
-        "schema": List[Dict[str, SchemaValueTypeType]],
-    },
-    total=False,
-)
-
 TsvStoreOptionsTypeDef = TypedDict(
     "TsvStoreOptionsTypeDef",
     {
         "annotationType": AnnotationTypeType,
         "formatToHeader": Mapping[FormatToHeaderKeyType, str],
         "schema": Sequence[Mapping[str, SchemaValueTypeType]],
     },
@@ -1531,14 +1519,15 @@
         "status": ReadSetStatusType,
         "referenceArn": str,
         "createdAfter": TimestampTypeDef,
         "createdBefore": TimestampTypeDef,
         "sampleId": str,
         "subjectId": str,
         "generatedFrom": str,
+        "creationType": CreationTypeType,
     },
     total=False,
 )
 
 ReadSetUploadPartListFilterTypeDef = TypedDict(
     "ReadSetUploadPartListFilterTypeDef",
     {
@@ -2574,14 +2563,15 @@
         "subjectId": str,
         "sampleId": str,
         "name": str,
         "description": str,
         "referenceArn": str,
         "sequenceInformation": SequenceInformationTypeDef,
         "statusMessage": str,
+        "creationType": CreationTypeType,
     },
     total=False,
 )
 
 class ReadSetListItemTypeDef(_RequiredReadSetListItemTypeDef, _OptionalReadSetListItemTypeDef):
     pass
 
@@ -2987,22 +2977,14 @@
 
 class StartVariantImportRequestRequestTypeDef(
     _RequiredStartVariantImportRequestRequestTypeDef,
     _OptionalStartVariantImportRequestRequestTypeDef,
 ):
     pass
 
-StoreOptionsOutputTypeDef = TypedDict(
-    "StoreOptionsOutputTypeDef",
-    {
-        "tsvStoreOptions": TsvStoreOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
 StoreOptionsTypeDef = TypedDict(
     "StoreOptionsTypeDef",
     {
         "tsvStoreOptions": TsvStoreOptionsTypeDef,
     },
     total=False,
 )
@@ -3397,14 +3379,15 @@
         "description": str,
         "fileType": FileTypeType,
         "creationTime": datetime,
         "sequenceInformation": SequenceInformationTypeDef,
         "referenceArn": str,
         "files": ReadSetFilesTypeDef,
         "statusMessage": str,
+        "creationType": CreationTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReferenceMetadataResponseTypeDef = TypedDict(
     "GetReferenceMetadataResponseTypeDef",
     {
@@ -3473,21 +3456,46 @@
     {
         "tsvOptions": TsvOptionsTypeDef,
         "vcfOptions": VcfOptionsTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
+    {
+        "storeFormat": StoreFormatType,
+    },
+)
+_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
+    {
+        "reference": ReferenceItemTypeDef,
+        "name": str,
+        "description": str,
+        "tags": Mapping[str, str],
+        "sseConfig": SseConfigTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
+    },
+    total=False,
+)
+
+class CreateAnnotationStoreRequestRequestTypeDef(
+    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
+    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
+):
+    pass
+
 CreateAnnotationStoreResponseTypeDef = TypedDict(
     "CreateAnnotationStoreResponseTypeDef",
     {
         "id": str,
         "reference": ReferenceItemTypeDef,
         "storeFormat": StoreFormatType,
-        "storeOptions": StoreOptionsOutputTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
         "status": StoreStatusType,
         "name": str,
         "creationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -3500,15 +3508,15 @@
         "storeArn": str,
         "name": str,
         "description": str,
         "sseConfig": SseConfigTypeDef,
         "creationTime": datetime,
         "updateTime": datetime,
         "tags": Dict[str, str],
-        "storeOptions": StoreOptionsOutputTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
         "storeFormat": StoreFormatType,
         "statusMessage": str,
         "storeSizeBytes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -3518,46 +3526,20 @@
         "id": str,
         "reference": ReferenceItemTypeDef,
         "status": StoreStatusType,
         "name": str,
         "description": str,
         "creationTime": datetime,
         "updateTime": datetime,
-        "storeOptions": StoreOptionsOutputTypeDef,
+        "storeOptions": StoreOptionsTypeDef,
         "storeFormat": StoreFormatType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAnnotationStoreRequestRequestTypeDef",
-    {
-        "storeFormat": StoreFormatType,
-    },
-)
-_OptionalCreateAnnotationStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAnnotationStoreRequestRequestTypeDef",
-    {
-        "reference": ReferenceItemTypeDef,
-        "name": str,
-        "description": str,
-        "tags": Mapping[str, str],
-        "sseConfig": SseConfigTypeDef,
-        "storeOptions": StoreOptionsTypeDef,
-    },
-    total=False,
-)
-
-class CreateAnnotationStoreRequestRequestTypeDef(
-    _RequiredCreateAnnotationStoreRequestRequestTypeDef,
-    _OptionalCreateAnnotationStoreRequestRequestTypeDef,
-):
-    pass
-
-StoreOptionsUnionTypeDef = Union[StoreOptionsTypeDef, StoreOptionsOutputTypeDef]
 GetAnnotationImportResponseTypeDef = TypedDict(
     "GetAnnotationImportResponseTypeDef",
     {
         "id": str,
         "destinationName": str,
         "roleArn": str,
         "status": JobStatusType,
```

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/waiter.py` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics/waiter.pyi` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-omics-2.5.2.post1/types_aiobotocore_omics.egg-info/SOURCES.txt` & `types-aiobotocore-omics-2.5.2.post2/types_aiobotocore_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

