# Comparing `tmp/types-aiobotocore-dataexchange-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-dataexchange-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dataexchange-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-dataexchange-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:44 2023, max compression
```

## Comparing `types-aiobotocore-dataexchange-2.5.2.post1.tar` & `types-aiobotocore-dataexchange-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.425608 types-aiobotocore-dataexchange-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-08-02 14:52:09.425608 types-aiobotocore-dataexchange-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:09.425608 types-aiobotocore-dataexchange-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:36:05.000000 types-aiobotocore-dataexchange-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.425608 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23279 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23236 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46582 2023-08-02 14:36:07.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46513 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:06.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.425608 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18623 2023-08-02 14:52:09.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:09.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:09.000000 types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.351836 types-aiobotocore-dataexchange-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-08-04 12:00:44.351836 types-aiobotocore-dataexchange-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:44.351836 types-aiobotocore-dataexchange-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.343836 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23279 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23236 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-08-04 11:43:26.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10427 2023-08-04 11:43:26.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45176 2023-08-04 11:43:27.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45109 2023-08-04 11:43:26.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:25.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.351836 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-08-04 12:00:44.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:00:44.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:44.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:44.000000 types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/LICENSE` & `types-aiobotocore-dataexchange-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/setup.py` & `types-aiobotocore-dataexchange-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dataexchange",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_dataexchange"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DataExchange 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/__init__.py` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/__init__.pyi` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/__main__.py` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DataExchange 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.DataExchange 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dataexchange//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange\nOther"
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

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/client.py` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/client.pyi` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/literals.py` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/literals.pyi` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/paginator.py` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/paginator.pyi` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/type_defs.py` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     "AutoExportRevisionDestinationEntryTypeDef",
     "ExportServerSideEncryptionTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "OriginDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "CreateRevisionRequestRequestTypeDef",
-    "LFTagOutputTypeDef",
     "LFTagTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
     "DeleteEventActionRequestRequestTypeDef",
     "DeleteRevisionRequestRequestTypeDef",
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
     "RevisionPublishedTypeDef",
@@ -102,58 +101,55 @@
     "GetDataSetResponseTypeDef",
     "GetRevisionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RevokeRevisionResponseTypeDef",
     "SendApiAssetResponseTypeDef",
     "UpdateDataSetResponseTypeDef",
     "UpdateRevisionResponseTypeDef",
-    "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
-    "DatabaseLFTagPolicyTypeDef",
-    "TableLFTagPolicyAndPermissionsOutputTypeDef",
-    "TableLFTagPolicyTypeDef",
     "DatabaseLFTagPolicyAndPermissionsTypeDef",
+    "DatabaseLFTagPolicyTypeDef",
     "TableLFTagPolicyAndPermissionsTypeDef",
+    "TableLFTagPolicyTypeDef",
     "DetailsTypeDef",
     "EventTypeDef",
     "ExportRevisionsToS3RequestDetailsTypeDef",
     "ExportRevisionsToS3ResponseDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
-    "S3DataAccessAssetSourceEntryOutputTypeDef",
     "S3DataAccessAssetSourceEntryTypeDef",
     "S3DataAccessAssetTypeDef",
     "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListEventActionsRequestListEventActionsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     "ListDataSetRevisionsResponseTypeDef",
     "ActionTypeDef",
     "ListDataSetsResponseTypeDef",
+    "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     "LFResourceDetailsTypeDef",
-    "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "JobErrorTypeDef",
-    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
+    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     "CreateEventActionRequestRequestTypeDef",
     "CreateEventActionResponseTypeDef",
     "EventActionEntryTypeDef",
     "GetEventActionResponseTypeDef",
     "UpdateEventActionRequestRequestTypeDef",
     "UpdateEventActionResponseTypeDef",
     "LFTagPolicyDetailsTypeDef",
-    "ResponseDetailsTypeDef",
     "RequestDetailsTypeDef",
+    "ResponseDetailsTypeDef",
     "ListEventActionsResponseTypeDef",
     "LakeFormationDataPermissionDetailsTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "JobEntryTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "LakeFormationDataPermissionAssetTypeDef",
     "ListJobsResponseTypeDef",
     "AssetDetailsTypeDef",
     "AssetEntryTypeDef",
     "GetAssetResponseTypeDef",
     "UpdateAssetResponseTypeDef",
     "ListRevisionAssetsResponseTypeDef",
@@ -328,22 +324,14 @@
 
 class CreateRevisionRequestRequestTypeDef(
     _RequiredCreateRevisionRequestRequestTypeDef, _OptionalCreateRevisionRequestRequestTypeDef
 ):
     pass
 
 
-LFTagOutputTypeDef = TypedDict(
-    "LFTagOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": List[str],
-    },
-)
-
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -1094,57 +1082,41 @@
         "RevocationComment": str,
         "Revoked": bool,
         "RevokedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatabaseLFTagPolicyAndPermissionsOutputTypeDef = TypedDict(
-    "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
+DatabaseLFTagPolicyAndPermissionsTypeDef = TypedDict(
+    "DatabaseLFTagPolicyAndPermissionsTypeDef",
     {
-        "Expression": List[LFTagOutputTypeDef],
-        "Permissions": List[Literal["DESCRIBE"]],
+        "Expression": Sequence[LFTagTypeDef],
+        "Permissions": Sequence[Literal["DESCRIBE"]],
     },
 )
 
 DatabaseLFTagPolicyTypeDef = TypedDict(
     "DatabaseLFTagPolicyTypeDef",
     {
-        "Expression": List[LFTagOutputTypeDef],
+        "Expression": List[LFTagTypeDef],
     },
 )
 
-TableLFTagPolicyAndPermissionsOutputTypeDef = TypedDict(
-    "TableLFTagPolicyAndPermissionsOutputTypeDef",
+TableLFTagPolicyAndPermissionsTypeDef = TypedDict(
+    "TableLFTagPolicyAndPermissionsTypeDef",
     {
-        "Expression": List[LFTagOutputTypeDef],
-        "Permissions": List[TableTagPolicyLFPermissionType],
+        "Expression": Sequence[LFTagTypeDef],
+        "Permissions": Sequence[TableTagPolicyLFPermissionType],
     },
 )
 
 TableLFTagPolicyTypeDef = TypedDict(
     "TableLFTagPolicyTypeDef",
     {
-        "Expression": List[LFTagOutputTypeDef],
-    },
-)
-
-DatabaseLFTagPolicyAndPermissionsTypeDef = TypedDict(
-    "DatabaseLFTagPolicyAndPermissionsTypeDef",
-    {
-        "Expression": Sequence[LFTagTypeDef],
-        "Permissions": Sequence[Literal["DESCRIBE"]],
-    },
-)
-
-TableLFTagPolicyAndPermissionsTypeDef = TypedDict(
-    "TableLFTagPolicyAndPermissionsTypeDef",
-    {
-        "Expression": Sequence[LFTagTypeDef],
-        "Permissions": Sequence[TableTagPolicyLFPermissionType],
+        "Expression": List[LFTagTypeDef],
     },
 )
 
 DetailsTypeDef = TypedDict(
     "DetailsTypeDef",
     {
         "ImportAssetFromSignedUrlJobErrorDetails": ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
@@ -1222,38 +1194,14 @@
     {
         "AssetSources": List[RedshiftDataShareAssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-_RequiredS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
-    "_RequiredS3DataAccessAssetSourceEntryOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
-    "_OptionalS3DataAccessAssetSourceEntryOutputTypeDef",
-    {
-        "KeyPrefixes": List[str],
-        "Keys": List[str],
-        "KmsKeysToGrant": List[KmsKeyToGrantTypeDef],
-    },
-    total=False,
-)
-
-
-class S3DataAccessAssetSourceEntryOutputTypeDef(
-    _RequiredS3DataAccessAssetSourceEntryOutputTypeDef,
-    _OptionalS3DataAccessAssetSourceEntryOutputTypeDef,
-):
-    pass
-
-
 _RequiredS3DataAccessAssetSourceEntryTypeDef = TypedDict(
     "_RequiredS3DataAccessAssetSourceEntryTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalS3DataAccessAssetSourceEntryTypeDef = TypedDict(
@@ -1393,75 +1341,75 @@
     {
         "DataSets": List[DataSetEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
-    "_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
+_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
+    "_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     {
         "CatalogId": str,
         "RoleArn": str,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
-_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
-    "_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
+_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
+    "_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     {
-        "Database": DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
-        "Table": TableLFTagPolicyAndPermissionsOutputTypeDef,
+        "Database": DatabaseLFTagPolicyAndPermissionsTypeDef,
+        "Table": TableLFTagPolicyAndPermissionsTypeDef,
     },
     total=False,
 )
 
 
-class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(
-    _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
-    _OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
+class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(
+    _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
+    _OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
 ):
     pass
 
 
-LFResourceDetailsTypeDef = TypedDict(
-    "LFResourceDetailsTypeDef",
-    {
-        "Database": DatabaseLFTagPolicyTypeDef,
-        "Table": TableLFTagPolicyTypeDef,
-    },
-    total=False,
-)
-
-_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
-    "_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
+_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
+    "_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     {
         "CatalogId": str,
         "RoleArn": str,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
-_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
-    "_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
+_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
+    "_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     {
         "Database": DatabaseLFTagPolicyAndPermissionsTypeDef,
         "Table": TableLFTagPolicyAndPermissionsTypeDef,
     },
     total=False,
 )
 
 
-class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(
-    _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
-    _OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
+class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(
+    _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
+    _OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
 ):
     pass
 
 
+LFResourceDetailsTypeDef = TypedDict(
+    "LFResourceDetailsTypeDef",
+    {
+        "Database": DatabaseLFTagPolicyTypeDef,
+        "Table": TableLFTagPolicyTypeDef,
+    },
+    total=False,
+)
+
 _RequiredJobErrorTypeDef = TypedDict(
     "_RequiredJobErrorTypeDef",
     {
         "Code": CodeType,
         "Message": str,
     },
 )
@@ -1478,25 +1426,25 @@
 )
 
 
 class JobErrorTypeDef(_RequiredJobErrorTypeDef, _OptionalJobErrorTypeDef):
     pass
 
 
-CreateS3DataAccessFromS3BucketResponseDetailsTypeDef = TypedDict(
-    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
+CreateS3DataAccessFromS3BucketRequestDetailsTypeDef = TypedDict(
+    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
     {
-        "AssetSource": S3DataAccessAssetSourceEntryOutputTypeDef,
+        "AssetSource": S3DataAccessAssetSourceEntryTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-CreateS3DataAccessFromS3BucketRequestDetailsTypeDef = TypedDict(
-    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
+CreateS3DataAccessFromS3BucketResponseDetailsTypeDef = TypedDict(
+    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     {
         "AssetSource": S3DataAccessAssetSourceEntryTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
@@ -1585,34 +1533,14 @@
     {
         "CatalogId": str,
         "ResourceType": LFResourceTypeType,
         "ResourceDetails": LFResourceDetailsTypeDef,
     },
 )
 
-ResponseDetailsTypeDef = TypedDict(
-    "ResponseDetailsTypeDef",
-    {
-        "ExportAssetToSignedUrl": ExportAssetToSignedUrlResponseDetailsTypeDef,
-        "ExportAssetsToS3": ExportAssetsToS3ResponseDetailsTypeDef,
-        "ExportRevisionsToS3": ExportRevisionsToS3ResponseDetailsTypeDef,
-        "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlResponseDetailsTypeDef,
-        "ImportAssetsFromS3": ImportAssetsFromS3ResponseDetailsTypeDef,
-        "ImportAssetsFromRedshiftDataShares": (
-            ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef
-        ),
-        "ImportAssetFromApiGatewayApi": ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
-        "CreateS3DataAccessFromS3Bucket": CreateS3DataAccessFromS3BucketResponseDetailsTypeDef,
-        "ImportAssetsFromLakeFormationTagPolicy": (
-            ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef
-        ),
-    },
-    total=False,
-)
-
 RequestDetailsTypeDef = TypedDict(
     "RequestDetailsTypeDef",
     {
         "ExportAssetToSignedUrl": ExportAssetToSignedUrlRequestDetailsTypeDef,
         "ExportAssetsToS3": ExportAssetsToS3RequestDetailsTypeDef,
         "ExportRevisionsToS3": ExportRevisionsToS3RequestDetailsTypeDef,
         "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlRequestDetailsTypeDef,
@@ -1625,14 +1553,34 @@
         "ImportAssetsFromLakeFormationTagPolicy": (
             ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef
         ),
     },
     total=False,
 )
 
+ResponseDetailsTypeDef = TypedDict(
+    "ResponseDetailsTypeDef",
+    {
+        "ExportAssetToSignedUrl": ExportAssetToSignedUrlResponseDetailsTypeDef,
+        "ExportAssetsToS3": ExportAssetsToS3ResponseDetailsTypeDef,
+        "ExportRevisionsToS3": ExportRevisionsToS3ResponseDetailsTypeDef,
+        "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlResponseDetailsTypeDef,
+        "ImportAssetsFromS3": ImportAssetsFromS3ResponseDetailsTypeDef,
+        "ImportAssetsFromRedshiftDataShares": (
+            ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef
+        ),
+        "ImportAssetFromApiGatewayApi": ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
+        "CreateS3DataAccessFromS3Bucket": CreateS3DataAccessFromS3BucketResponseDetailsTypeDef,
+        "ImportAssetsFromLakeFormationTagPolicy": (
+            ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef
+        ),
+    },
+    total=False,
+)
+
 ListEventActionsResponseTypeDef = TypedDict(
     "ListEventActionsResponseTypeDef",
     {
         "EventActions": List[EventActionEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1642,14 +1590,22 @@
     "LakeFormationDataPermissionDetailsTypeDef",
     {
         "LFTagPolicy": LFTagPolicyDetailsTypeDef,
     },
     total=False,
 )
 
+CreateJobRequestRequestTypeDef = TypedDict(
+    "CreateJobRequestRequestTypeDef",
+    {
+        "Details": RequestDetailsTypeDef,
+        "Type": TypeType,
+    },
+)
+
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
@@ -1697,22 +1653,14 @@
 )
 
 
 class JobEntryTypeDef(_RequiredJobEntryTypeDef, _OptionalJobEntryTypeDef):
     pass
 
 
-CreateJobRequestRequestTypeDef = TypedDict(
-    "CreateJobRequestRequestTypeDef",
-    {
-        "Details": RequestDetailsTypeDef,
-        "Type": TypeType,
-    },
-)
-
 _RequiredLakeFormationDataPermissionAssetTypeDef = TypedDict(
     "_RequiredLakeFormationDataPermissionAssetTypeDef",
     {
         "LakeFormationDataPermissionDetails": LakeFormationDataPermissionDetailsTypeDef,
         "LakeFormationDataPermissionType": Literal["LFTagPolicy"],
         "Permissions": List[LFPermissionType],
     },
```

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange/type_defs.pyi` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "AutoExportRevisionDestinationEntryTypeDef",
     "ExportServerSideEncryptionTypeDef",
     "CancelJobRequestRequestTypeDef",
     "CreateDataSetRequestRequestTypeDef",
     "OriginDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "CreateRevisionRequestRequestTypeDef",
-    "LFTagOutputTypeDef",
     "LFTagTypeDef",
     "DeleteAssetRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
     "DeleteEventActionRequestRequestTypeDef",
     "DeleteRevisionRequestRequestTypeDef",
     "ImportAssetFromSignedUrlJobErrorDetailsTypeDef",
     "RevisionPublishedTypeDef",
@@ -101,58 +100,55 @@
     "GetDataSetResponseTypeDef",
     "GetRevisionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "RevokeRevisionResponseTypeDef",
     "SendApiAssetResponseTypeDef",
     "UpdateDataSetResponseTypeDef",
     "UpdateRevisionResponseTypeDef",
-    "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
-    "DatabaseLFTagPolicyTypeDef",
-    "TableLFTagPolicyAndPermissionsOutputTypeDef",
-    "TableLFTagPolicyTypeDef",
     "DatabaseLFTagPolicyAndPermissionsTypeDef",
+    "DatabaseLFTagPolicyTypeDef",
     "TableLFTagPolicyAndPermissionsTypeDef",
+    "TableLFTagPolicyTypeDef",
     "DetailsTypeDef",
     "EventTypeDef",
     "ExportRevisionsToS3RequestDetailsTypeDef",
     "ExportRevisionsToS3ResponseDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef",
     "ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef",
-    "S3DataAccessAssetSourceEntryOutputTypeDef",
     "S3DataAccessAssetSourceEntryTypeDef",
     "S3DataAccessAssetTypeDef",
     "ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef",
     "ListDataSetsRequestListDataSetsPaginateTypeDef",
     "ListEventActionsRequestListEventActionsPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef",
     "ListDataSetRevisionsResponseTypeDef",
     "ActionTypeDef",
     "ListDataSetsResponseTypeDef",
+    "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     "LFResourceDetailsTypeDef",
-    "ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     "JobErrorTypeDef",
-    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
+    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     "CreateEventActionRequestRequestTypeDef",
     "CreateEventActionResponseTypeDef",
     "EventActionEntryTypeDef",
     "GetEventActionResponseTypeDef",
     "UpdateEventActionRequestRequestTypeDef",
     "UpdateEventActionResponseTypeDef",
     "LFTagPolicyDetailsTypeDef",
-    "ResponseDetailsTypeDef",
     "RequestDetailsTypeDef",
+    "ResponseDetailsTypeDef",
     "ListEventActionsResponseTypeDef",
     "LakeFormationDataPermissionDetailsTypeDef",
+    "CreateJobRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "JobEntryTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "LakeFormationDataPermissionAssetTypeDef",
     "ListJobsResponseTypeDef",
     "AssetDetailsTypeDef",
     "AssetEntryTypeDef",
     "GetAssetResponseTypeDef",
     "UpdateAssetResponseTypeDef",
     "ListRevisionAssetsResponseTypeDef",
@@ -317,22 +313,14 @@
 )
 
 class CreateRevisionRequestRequestTypeDef(
     _RequiredCreateRevisionRequestRequestTypeDef, _OptionalCreateRevisionRequestRequestTypeDef
 ):
     pass
 
-LFTagOutputTypeDef = TypedDict(
-    "LFTagOutputTypeDef",
-    {
-        "TagKey": str,
-        "TagValues": List[str],
-    },
-)
-
 LFTagTypeDef = TypedDict(
     "LFTagTypeDef",
     {
         "TagKey": str,
         "TagValues": Sequence[str],
     },
 )
@@ -1053,57 +1041,41 @@
         "RevocationComment": str,
         "Revoked": bool,
         "RevokedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatabaseLFTagPolicyAndPermissionsOutputTypeDef = TypedDict(
-    "DatabaseLFTagPolicyAndPermissionsOutputTypeDef",
+DatabaseLFTagPolicyAndPermissionsTypeDef = TypedDict(
+    "DatabaseLFTagPolicyAndPermissionsTypeDef",
     {
-        "Expression": List[LFTagOutputTypeDef],
-        "Permissions": List[Literal["DESCRIBE"]],
+        "Expression": Sequence[LFTagTypeDef],
+        "Permissions": Sequence[Literal["DESCRIBE"]],
     },
 )
 
 DatabaseLFTagPolicyTypeDef = TypedDict(
     "DatabaseLFTagPolicyTypeDef",
     {
-        "Expression": List[LFTagOutputTypeDef],
+        "Expression": List[LFTagTypeDef],
     },
 )
 
-TableLFTagPolicyAndPermissionsOutputTypeDef = TypedDict(
-    "TableLFTagPolicyAndPermissionsOutputTypeDef",
+TableLFTagPolicyAndPermissionsTypeDef = TypedDict(
+    "TableLFTagPolicyAndPermissionsTypeDef",
     {
-        "Expression": List[LFTagOutputTypeDef],
-        "Permissions": List[TableTagPolicyLFPermissionType],
+        "Expression": Sequence[LFTagTypeDef],
+        "Permissions": Sequence[TableTagPolicyLFPermissionType],
     },
 )
 
 TableLFTagPolicyTypeDef = TypedDict(
     "TableLFTagPolicyTypeDef",
     {
-        "Expression": List[LFTagOutputTypeDef],
-    },
-)
-
-DatabaseLFTagPolicyAndPermissionsTypeDef = TypedDict(
-    "DatabaseLFTagPolicyAndPermissionsTypeDef",
-    {
-        "Expression": Sequence[LFTagTypeDef],
-        "Permissions": Sequence[Literal["DESCRIBE"]],
-    },
-)
-
-TableLFTagPolicyAndPermissionsTypeDef = TypedDict(
-    "TableLFTagPolicyAndPermissionsTypeDef",
-    {
-        "Expression": Sequence[LFTagTypeDef],
-        "Permissions": Sequence[TableTagPolicyLFPermissionType],
+        "Expression": List[LFTagTypeDef],
     },
 )
 
 DetailsTypeDef = TypedDict(
     "DetailsTypeDef",
     {
         "ImportAssetFromSignedUrlJobErrorDetails": ImportAssetFromSignedUrlJobErrorDetailsTypeDef,
@@ -1177,36 +1149,14 @@
     {
         "AssetSources": List[RedshiftDataShareAssetSourceEntryTypeDef],
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-_RequiredS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
-    "_RequiredS3DataAccessAssetSourceEntryOutputTypeDef",
-    {
-        "Bucket": str,
-    },
-)
-_OptionalS3DataAccessAssetSourceEntryOutputTypeDef = TypedDict(
-    "_OptionalS3DataAccessAssetSourceEntryOutputTypeDef",
-    {
-        "KeyPrefixes": List[str],
-        "Keys": List[str],
-        "KmsKeysToGrant": List[KmsKeyToGrantTypeDef],
-    },
-    total=False,
-)
-
-class S3DataAccessAssetSourceEntryOutputTypeDef(
-    _RequiredS3DataAccessAssetSourceEntryOutputTypeDef,
-    _OptionalS3DataAccessAssetSourceEntryOutputTypeDef,
-):
-    pass
-
 _RequiredS3DataAccessAssetSourceEntryTypeDef = TypedDict(
     "_RequiredS3DataAccessAssetSourceEntryTypeDef",
     {
         "Bucket": str,
     },
 )
 _OptionalS3DataAccessAssetSourceEntryTypeDef = TypedDict(
@@ -1338,71 +1288,71 @@
     {
         "DataSets": List[DataSetEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
-    "_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
+_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
+    "_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     {
         "CatalogId": str,
         "RoleArn": str,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
-_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
-    "_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
+_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
+    "_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
     {
-        "Database": DatabaseLFTagPolicyAndPermissionsOutputTypeDef,
-        "Table": TableLFTagPolicyAndPermissionsOutputTypeDef,
+        "Database": DatabaseLFTagPolicyAndPermissionsTypeDef,
+        "Table": TableLFTagPolicyAndPermissionsTypeDef,
     },
     total=False,
 )
 
-class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(
-    _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
-    _OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
+class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(
+    _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
+    _OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
 ):
     pass
 
-LFResourceDetailsTypeDef = TypedDict(
-    "LFResourceDetailsTypeDef",
-    {
-        "Database": DatabaseLFTagPolicyTypeDef,
-        "Table": TableLFTagPolicyTypeDef,
-    },
-    total=False,
-)
-
-_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
-    "_RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
+_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
+    "_RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     {
         "CatalogId": str,
         "RoleArn": str,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
-_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef = TypedDict(
-    "_OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef",
+_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef = TypedDict(
+    "_OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef",
     {
         "Database": DatabaseLFTagPolicyAndPermissionsTypeDef,
         "Table": TableLFTagPolicyAndPermissionsTypeDef,
     },
     total=False,
 )
 
-class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(
-    _RequiredImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
-    _OptionalImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef,
+class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(
+    _RequiredImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
+    _OptionalImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef,
 ):
     pass
 
+LFResourceDetailsTypeDef = TypedDict(
+    "LFResourceDetailsTypeDef",
+    {
+        "Database": DatabaseLFTagPolicyTypeDef,
+        "Table": TableLFTagPolicyTypeDef,
+    },
+    total=False,
+)
+
 _RequiredJobErrorTypeDef = TypedDict(
     "_RequiredJobErrorTypeDef",
     {
         "Code": CodeType,
         "Message": str,
     },
 )
@@ -1417,25 +1367,25 @@
     },
     total=False,
 )
 
 class JobErrorTypeDef(_RequiredJobErrorTypeDef, _OptionalJobErrorTypeDef):
     pass
 
-CreateS3DataAccessFromS3BucketResponseDetailsTypeDef = TypedDict(
-    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
+CreateS3DataAccessFromS3BucketRequestDetailsTypeDef = TypedDict(
+    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
     {
-        "AssetSource": S3DataAccessAssetSourceEntryOutputTypeDef,
+        "AssetSource": S3DataAccessAssetSourceEntryTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
-CreateS3DataAccessFromS3BucketRequestDetailsTypeDef = TypedDict(
-    "CreateS3DataAccessFromS3BucketRequestDetailsTypeDef",
+CreateS3DataAccessFromS3BucketResponseDetailsTypeDef = TypedDict(
+    "CreateS3DataAccessFromS3BucketResponseDetailsTypeDef",
     {
         "AssetSource": S3DataAccessAssetSourceEntryTypeDef,
         "DataSetId": str,
         "RevisionId": str,
     },
 )
 
@@ -1522,34 +1472,14 @@
     {
         "CatalogId": str,
         "ResourceType": LFResourceTypeType,
         "ResourceDetails": LFResourceDetailsTypeDef,
     },
 )
 
-ResponseDetailsTypeDef = TypedDict(
-    "ResponseDetailsTypeDef",
-    {
-        "ExportAssetToSignedUrl": ExportAssetToSignedUrlResponseDetailsTypeDef,
-        "ExportAssetsToS3": ExportAssetsToS3ResponseDetailsTypeDef,
-        "ExportRevisionsToS3": ExportRevisionsToS3ResponseDetailsTypeDef,
-        "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlResponseDetailsTypeDef,
-        "ImportAssetsFromS3": ImportAssetsFromS3ResponseDetailsTypeDef,
-        "ImportAssetsFromRedshiftDataShares": (
-            ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef
-        ),
-        "ImportAssetFromApiGatewayApi": ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
-        "CreateS3DataAccessFromS3Bucket": CreateS3DataAccessFromS3BucketResponseDetailsTypeDef,
-        "ImportAssetsFromLakeFormationTagPolicy": (
-            ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef
-        ),
-    },
-    total=False,
-)
-
 RequestDetailsTypeDef = TypedDict(
     "RequestDetailsTypeDef",
     {
         "ExportAssetToSignedUrl": ExportAssetToSignedUrlRequestDetailsTypeDef,
         "ExportAssetsToS3": ExportAssetsToS3RequestDetailsTypeDef,
         "ExportRevisionsToS3": ExportRevisionsToS3RequestDetailsTypeDef,
         "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlRequestDetailsTypeDef,
@@ -1562,14 +1492,34 @@
         "ImportAssetsFromLakeFormationTagPolicy": (
             ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef
         ),
     },
     total=False,
 )
 
+ResponseDetailsTypeDef = TypedDict(
+    "ResponseDetailsTypeDef",
+    {
+        "ExportAssetToSignedUrl": ExportAssetToSignedUrlResponseDetailsTypeDef,
+        "ExportAssetsToS3": ExportAssetsToS3ResponseDetailsTypeDef,
+        "ExportRevisionsToS3": ExportRevisionsToS3ResponseDetailsTypeDef,
+        "ImportAssetFromSignedUrl": ImportAssetFromSignedUrlResponseDetailsTypeDef,
+        "ImportAssetsFromS3": ImportAssetsFromS3ResponseDetailsTypeDef,
+        "ImportAssetsFromRedshiftDataShares": (
+            ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef
+        ),
+        "ImportAssetFromApiGatewayApi": ImportAssetFromApiGatewayApiResponseDetailsTypeDef,
+        "CreateS3DataAccessFromS3Bucket": CreateS3DataAccessFromS3BucketResponseDetailsTypeDef,
+        "ImportAssetsFromLakeFormationTagPolicy": (
+            ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef
+        ),
+    },
+    total=False,
+)
+
 ListEventActionsResponseTypeDef = TypedDict(
     "ListEventActionsResponseTypeDef",
     {
         "EventActions": List[EventActionEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1579,14 +1529,22 @@
     "LakeFormationDataPermissionDetailsTypeDef",
     {
         "LFTagPolicy": LFTagPolicyDetailsTypeDef,
     },
     total=False,
 )
 
+CreateJobRequestRequestTypeDef = TypedDict(
+    "CreateJobRequestRequestTypeDef",
+    {
+        "Details": RequestDetailsTypeDef,
+        "Type": TypeType,
+    },
+)
+
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Details": ResponseDetailsTypeDef,
         "Errors": List[JobErrorTypeDef],
@@ -1632,22 +1590,14 @@
     },
     total=False,
 )
 
 class JobEntryTypeDef(_RequiredJobEntryTypeDef, _OptionalJobEntryTypeDef):
     pass
 
-CreateJobRequestRequestTypeDef = TypedDict(
-    "CreateJobRequestRequestTypeDef",
-    {
-        "Details": RequestDetailsTypeDef,
-        "Type": TypeType,
-    },
-)
-
 _RequiredLakeFormationDataPermissionAssetTypeDef = TypedDict(
     "_RequiredLakeFormationDataPermissionAssetTypeDef",
     {
         "LakeFormationDataPermissionDetails": LakeFormationDataPermissionDetailsTypeDef,
         "LakeFormationDataPermissionType": Literal["LFTagPolicy"],
         "Permissions": List[LFPermissionType],
     },
```

### Comparing `types-aiobotocore-dataexchange-2.5.2.post1/types_aiobotocore_dataexchange.egg-info/SOURCES.txt` & `types-aiobotocore-dataexchange-2.5.2.post2/types_aiobotocore_dataexchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

