# Comparing `tmp/types-aiobotocore-signer-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-signer-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-signer-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-signer-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
```

## Comparing `types-aiobotocore-signer-2.5.2.post1.tar` & `types-aiobotocore-signer-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.729455 types-aiobotocore-signer-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-08-02 14:53:01.725455 types-aiobotocore-signer-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14934 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:01.729455 types-aiobotocore-signer-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.721455 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18592 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9078 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-08-02 14:49:47.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21613 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-02 14:49:46.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.725455 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:53:01.000000 types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.746643 types-aiobotocore-signer-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13944 2023-08-04 13:59:26.746643 types-aiobotocore-signer-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12430 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.746643 types-aiobotocore-signer-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.746643 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1347 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1346 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18592 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18560 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9173 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9171 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4874 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4869 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21630 2023-08-04 13:53:44.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    21613 2023-08-04 13:53:44.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1564 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1563 2023-08-04 13:53:43.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.746643 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13944 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      865 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:26.000000 types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-signer-2.5.2.post1/LICENSE` & `types-aiobotocore-signer-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/README.md` & `types-aiobotocore-signer-2.5.2.post2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-signer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,113 +293,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_signer.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `signer` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/literals/).
+
 ```python
-from types_aiobotocore_signer.literals import (
-    CategoryType,
-    EncryptionAlgorithmType,
-    HashAlgorithmType,
-    ImageFormatType,
-    ListSigningJobsPaginatorName,
-    ListSigningPlatformsPaginatorName,
-    ListSigningProfilesPaginatorName,
-    SigningProfileStatusType,
-    SigningStatusType,
-    SuccessfulSigningJobWaiterName,
-    ValidityTypeType,
-    signerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_signer.literals import CategoryType
 
 
 def check_value(value: CategoryType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_signer.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `signer` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer/type_defs/).
+
 ```python
-from types_aiobotocore_signer.type_defs import (
-    AddProfilePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    BlobTypeDef,
-    CancelSigningProfileRequestRequestTypeDef,
-    DescribeSigningJobRequestRequestTypeDef,
-    WaiterConfigTypeDef,
-    SigningJobRevocationRecordTypeDef,
-    SigningMaterialTypeDef,
-    S3DestinationTypeDef,
-    EncryptionAlgorithmOptionsTypeDef,
-    TimestampTypeDef,
-    GetSigningPlatformRequestRequestTypeDef,
-    SigningImageFormatTypeDef,
-    GetSigningProfileRequestRequestTypeDef,
-    SignatureValidityPeriodTypeDef,
-    SigningProfileRevocationRecordTypeDef,
-    HashAlgorithmOptionsTypeDef,
-    ListProfilePermissionsRequestRequestTypeDef,
-    PermissionTypeDef,
-    PaginatorConfigTypeDef,
-    ListSigningPlatformsRequestRequestTypeDef,
-    ListSigningProfilesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RemoveProfilePermissionRequestRequestTypeDef,
-    RevokeSignatureRequestRequestTypeDef,
-    S3SignedObjectTypeDef,
-    S3SourceTypeDef,
-    SigningConfigurationOverridesTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AddProfilePermissionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetRevocationStatusResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutSigningProfileResponseTypeDef,
-    RemoveProfilePermissionResponseTypeDef,
-    SignPayloadResponseTypeDef,
-    StartSigningJobResponseTypeDef,
-    SignPayloadRequestRequestTypeDef,
-    DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
-    DestinationTypeDef,
-    GetRevocationStatusRequestRequestTypeDef,
-    ListSigningJobsRequestRequestTypeDef,
-    RevokeSigningProfileRequestRequestTypeDef,
-    SigningProfileTypeDef,
-    SigningConfigurationTypeDef,
-    ListProfilePermissionsResponseTypeDef,
-    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
-    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
-    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
-    SignedObjectTypeDef,
-    SourceTypeDef,
-    SigningPlatformOverridesTypeDef,
-    ListSigningProfilesResponseTypeDef,
-    GetSigningPlatformResponseTypeDef,
-    SigningPlatformTypeDef,
-    SigningJobTypeDef,
-    StartSigningJobRequestRequestTypeDef,
-    DescribeSigningJobResponseTypeDef,
-    GetSigningProfileResponseTypeDef,
-    PutSigningProfileRequestRequestTypeDef,
-    ListSigningPlatformsResponseTypeDef,
-    ListSigningJobsResponseTypeDef,
-)
+from types_aiobotocore_signer.type_defs import AddProfilePermissionRequestRequestTypeDef
 
 
 def get_value() -> AddProfilePermissionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-signer-2.5.2.post1/setup.py` & `types-aiobotocore-signer-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-signer",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_signer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.signer 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__init__.py` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__init__.pyi` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/__main__.py` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.signer 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.signer 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_signer//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer\nOther"
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

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/client.py` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/client.pyi` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/literals.py` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
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
@@ -166,14 +167,15 @@
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
@@ -252,26 +254,28 @@
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

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/literals.pyi` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
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
@@ -164,14 +165,15 @@
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
@@ -250,26 +252,28 @@
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

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/paginator.py` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/paginator.pyi` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/type_defs.py` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/type_defs.pyi` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/waiter.py` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer/waiter.pyi` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-signer-2.5.2.post1/types_aiobotocore_signer.egg-info/SOURCES.txt` & `types-aiobotocore-signer-2.5.2.post2/types_aiobotocore_signer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

