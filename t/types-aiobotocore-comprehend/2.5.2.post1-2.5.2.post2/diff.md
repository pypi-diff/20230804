# Comparing `tmp/types-aiobotocore-comprehend-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-comprehend-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-comprehend-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-comprehend-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:39 2023, max compression
```

## Comparing `types-aiobotocore-comprehend-2.5.2.post1.tar` & `types-aiobotocore-comprehend-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.049618 types-aiobotocore-comprehend-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-08-02 14:52:05.049618 types-aiobotocore-comprehend-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27223 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:05.049618 types-aiobotocore-comprehend-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:35:25.000000 types-aiobotocore-comprehend-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.037618 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70451 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    70348 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-08-02 14:35:27.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   105243 2023-08-02 14:35:29.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   105154 2023-08-02 14:35:28.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:26.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:05.049618 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:04.000000 types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.447647 types-aiobotocore-comprehend-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14899 2023-08-04 12:00:39.439647 types-aiobotocore-comprehend-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13369 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:39.447647 types-aiobotocore-comprehend-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.435647 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70286 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70183 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-08-04 11:42:45.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14744 2023-08-04 11:42:45.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14161 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98449 2023-08-04 11:42:48.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98372 2023-08-04 11:42:46.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:44.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.439647 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14899 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:39.000000 types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/LICENSE` & `types-aiobotocore-comprehend-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/setup.py` & `types-aiobotocore-comprehend-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-comprehend",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_comprehend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Comprehend 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__init__.py` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__init__.pyi` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/__main__.py` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Comprehend 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Comprehend 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend\nOther"
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

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/client.py` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     ClassifyDocumentResponseTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDocumentClassifierResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEntityRecognizerResponseTypeDef,
     CreateFlywheelResponseTypeDef,
-    DataSecurityConfigUnionTypeDef,
+    DataSecurityConfigTypeDef,
     DatasetFilterTypeDef,
     DatasetInputDataConfigTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     DescribeDocumentClassifierResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     DescribeEndpointResponseTypeDef,
@@ -79,27 +79,27 @@
     DetectKeyPhrasesResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
     DetectSentimentResponseTypeDef,
     DetectSyntaxResponseTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     DocumentClassificationJobFilterTypeDef,
     DocumentClassifierFilterTypeDef,
-    DocumentClassifierInputDataConfigUnionTypeDef,
+    DocumentClassifierInputDataConfigTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
-    DocumentReaderConfigUnionTypeDef,
+    DocumentReaderConfigTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
     EntityRecognizerFilterTypeDef,
-    EntityRecognizerInputDataConfigUnionTypeDef,
+    EntityRecognizerInputDataConfigTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     ImportModelResponseTypeDef,
-    InputDataConfigUnionTypeDef,
+    InputDataConfigTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
     ListDatasetsResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     ListDocumentClassifiersResponseTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     ListEndpointsResponseTypeDef,
@@ -114,15 +114,15 @@
     ListSentimentDetectionJobsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     OutputDataConfigTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     PutResourcePolicyResponseTypeDef,
-    RedactionConfigUnionTypeDef,
+    RedactionConfigTypeDef,
     SentimentDetectionJobFilterTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
@@ -135,20 +135,20 @@
     StopEventsDetectionJobResponseTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
     TagTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
-    TaskConfigUnionTypeDef,
+    TaskConfigTypeDef,
     TopicsDetectionJobFilterTypeDef,
     UpdateDataSecurityConfigTypeDef,
     UpdateEndpointResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
-    VpcConfigUnionTypeDef,
+    VpcConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -275,15 +275,15 @@
 
     async def classify_document(
         self,
         *,
         EndpointArn: str,
         Text: str = ...,
         Bytes: BlobTypeDef = ...,
-        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
+        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
     ) -> ClassifyDocumentResponseTypeDef:
         """
         Creates a new document classification request to analyze a single document in
         real-time, using a previously created and trained custom model and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.classify_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#classify_document)
@@ -329,22 +329,22 @@
         """
 
     async def create_document_classifier(
         self,
         *,
         DocumentClassifierName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: DocumentClassifierInputDataConfigUnionTypeDef,
+        InputDataConfig: DocumentClassifierInputDataConfigTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OutputDataConfig: DocumentClassifierOutputDataConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Mode: DocumentClassifierModeType = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateDocumentClassifierResponseTypeDef:
         """
         Creates a new document classifier that you can use to categorize documents.
 
@@ -374,21 +374,21 @@
         """
 
     async def create_entity_recognizer(
         self,
         *,
         RecognizerName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: EntityRecognizerInputDataConfigUnionTypeDef,
+        InputDataConfig: EntityRecognizerInputDataConfigTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateEntityRecognizerResponseTypeDef:
         """
         Creates an entity recognizer using submitted files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_entity_recognizer)
@@ -398,17 +398,17 @@
     async def create_flywheel(
         self,
         *,
         FlywheelName: str,
         DataAccessRoleArn: str,
         DataLakeS3Uri: str,
         ActiveModelArn: str = ...,
-        TaskConfig: TaskConfigUnionTypeDef = ...,
+        TaskConfig: TaskConfigTypeDef = ...,
         ModelType: ModelTypeType = ...,
-        DataSecurityConfig: DataSecurityConfigUnionTypeDef = ...,
+        DataSecurityConfig: DataSecurityConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFlywheelResponseTypeDef:
         """
         A flywheel is an Amazon Web Services resource that orchestrates the ongoing
         training of a model for custom classification or custom entity recognition.
 
@@ -626,15 +626,15 @@
     async def detect_entities(
         self,
         *,
         Text: str = ...,
         LanguageCode: LanguageCodeType = ...,
         EndpointArn: str = ...,
         Bytes: BlobTypeDef = ...,
-        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
+        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
     ) -> DetectEntitiesResponseTypeDef:
         """
         Detects named entities in input text when you use the pre-trained model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_entities)
         """
@@ -970,78 +970,78 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#put_resource_policy)
         """
 
     async def start_document_classification_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         DocumentClassifierArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartDocumentClassificationJobResponseTypeDef:
         """
         Starts an asynchronous document classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_document_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_document_classification_job)
         """
 
     async def start_dominant_language_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartDominantLanguageDetectionJobResponseTypeDef:
         """
         Starts an asynchronous dominant language detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_dominant_language_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_dominant_language_detection_job)
         """
 
     async def start_entities_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         EntityRecognizerArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_entities_detection_job)
         """
 
     async def start_events_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         TargetEventTypes: Sequence[str],
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
@@ -1063,103 +1063,103 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_flywheel_iteration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_flywheel_iteration)
         """
 
     async def start_key_phrases_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartKeyPhrasesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous key phrase detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_key_phrases_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_key_phrases_detection_job)
         """
 
     async def start_pii_entities_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         Mode: PiiEntitiesDetectionModeType,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
-        RedactionConfig: RedactionConfigUnionTypeDef = ...,
+        RedactionConfig: RedactionConfigTypeDef = ...,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartPiiEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous PII entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_pii_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_pii_entities_detection_job)
         """
 
     async def start_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous sentiment detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_sentiment_detection_job)
         """
 
     async def start_targeted_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTargetedSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous targeted sentiment detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_targeted_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_targeted_sentiment_detection_job)
         """
 
     async def start_topics_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         NumberOfTopics: int = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTopicsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous topic detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_topics_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_topics_detection_job)
```

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/client.pyi` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     ClassifyDocumentResponseTypeDef,
     ContainsPiiEntitiesResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDocumentClassifierResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEntityRecognizerResponseTypeDef,
     CreateFlywheelResponseTypeDef,
-    DataSecurityConfigUnionTypeDef,
+    DataSecurityConfigTypeDef,
     DatasetFilterTypeDef,
     DatasetInputDataConfigTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDocumentClassificationJobResponseTypeDef,
     DescribeDocumentClassifierResponseTypeDef,
     DescribeDominantLanguageDetectionJobResponseTypeDef,
     DescribeEndpointResponseTypeDef,
@@ -79,27 +79,27 @@
     DetectKeyPhrasesResponseTypeDef,
     DetectPiiEntitiesResponseTypeDef,
     DetectSentimentResponseTypeDef,
     DetectSyntaxResponseTypeDef,
     DetectTargetedSentimentResponseTypeDef,
     DocumentClassificationJobFilterTypeDef,
     DocumentClassifierFilterTypeDef,
-    DocumentClassifierInputDataConfigUnionTypeDef,
+    DocumentClassifierInputDataConfigTypeDef,
     DocumentClassifierOutputDataConfigTypeDef,
-    DocumentReaderConfigUnionTypeDef,
+    DocumentReaderConfigTypeDef,
     DominantLanguageDetectionJobFilterTypeDef,
     EndpointFilterTypeDef,
     EntitiesDetectionJobFilterTypeDef,
     EntityRecognizerFilterTypeDef,
-    EntityRecognizerInputDataConfigUnionTypeDef,
+    EntityRecognizerInputDataConfigTypeDef,
     EventsDetectionJobFilterTypeDef,
     FlywheelFilterTypeDef,
     FlywheelIterationFilterTypeDef,
     ImportModelResponseTypeDef,
-    InputDataConfigUnionTypeDef,
+    InputDataConfigTypeDef,
     KeyPhrasesDetectionJobFilterTypeDef,
     ListDatasetsResponseTypeDef,
     ListDocumentClassificationJobsResponseTypeDef,
     ListDocumentClassifiersResponseTypeDef,
     ListDocumentClassifierSummariesResponseTypeDef,
     ListDominantLanguageDetectionJobsResponseTypeDef,
     ListEndpointsResponseTypeDef,
@@ -114,15 +114,15 @@
     ListSentimentDetectionJobsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetedSentimentDetectionJobsResponseTypeDef,
     ListTopicsDetectionJobsResponseTypeDef,
     OutputDataConfigTypeDef,
     PiiEntitiesDetectionJobFilterTypeDef,
     PutResourcePolicyResponseTypeDef,
-    RedactionConfigUnionTypeDef,
+    RedactionConfigTypeDef,
     SentimentDetectionJobFilterTypeDef,
     StartDocumentClassificationJobResponseTypeDef,
     StartDominantLanguageDetectionJobResponseTypeDef,
     StartEntitiesDetectionJobResponseTypeDef,
     StartEventsDetectionJobResponseTypeDef,
     StartFlywheelIterationResponseTypeDef,
     StartKeyPhrasesDetectionJobResponseTypeDef,
@@ -135,20 +135,20 @@
     StopEventsDetectionJobResponseTypeDef,
     StopKeyPhrasesDetectionJobResponseTypeDef,
     StopPiiEntitiesDetectionJobResponseTypeDef,
     StopSentimentDetectionJobResponseTypeDef,
     StopTargetedSentimentDetectionJobResponseTypeDef,
     TagTypeDef,
     TargetedSentimentDetectionJobFilterTypeDef,
-    TaskConfigUnionTypeDef,
+    TaskConfigTypeDef,
     TopicsDetectionJobFilterTypeDef,
     UpdateDataSecurityConfigTypeDef,
     UpdateEndpointResponseTypeDef,
     UpdateFlywheelResponseTypeDef,
-    VpcConfigUnionTypeDef,
+    VpcConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -263,15 +263,15 @@
         """
     async def classify_document(
         self,
         *,
         EndpointArn: str,
         Text: str = ...,
         Bytes: BlobTypeDef = ...,
-        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
+        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
     ) -> ClassifyDocumentResponseTypeDef:
         """
         Creates a new document classification request to analyze a single document in
         real-time, using a previously created and trained custom model and an endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.classify_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#classify_document)
@@ -313,22 +313,22 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_dataset)
         """
     async def create_document_classifier(
         self,
         *,
         DocumentClassifierName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: DocumentClassifierInputDataConfigUnionTypeDef,
+        InputDataConfig: DocumentClassifierInputDataConfigTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OutputDataConfig: DocumentClassifierOutputDataConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Mode: DocumentClassifierModeType = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateDocumentClassifierResponseTypeDef:
         """
         Creates a new document classifier that you can use to categorize documents.
 
@@ -356,21 +356,21 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_endpoint)
         """
     async def create_entity_recognizer(
         self,
         *,
         RecognizerName: str,
         DataAccessRoleArn: str,
-        InputDataConfig: EntityRecognizerInputDataConfigUnionTypeDef,
+        InputDataConfig: EntityRecognizerInputDataConfigTypeDef,
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         ModelKmsKeyId: str = ...,
         ModelPolicy: str = ...
     ) -> CreateEntityRecognizerResponseTypeDef:
         """
         Creates an entity recognizer using submitted files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_entity_recognizer)
@@ -379,17 +379,17 @@
     async def create_flywheel(
         self,
         *,
         FlywheelName: str,
         DataAccessRoleArn: str,
         DataLakeS3Uri: str,
         ActiveModelArn: str = ...,
-        TaskConfig: TaskConfigUnionTypeDef = ...,
+        TaskConfig: TaskConfigTypeDef = ...,
         ModelType: ModelTypeType = ...,
-        DataSecurityConfig: DataSecurityConfigUnionTypeDef = ...,
+        DataSecurityConfig: DataSecurityConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateFlywheelResponseTypeDef:
         """
         A flywheel is an Amazon Web Services resource that orchestrates the ongoing
         training of a model for custom classification or custom entity recognition.
 
@@ -584,15 +584,15 @@
     async def detect_entities(
         self,
         *,
         Text: str = ...,
         LanguageCode: LanguageCodeType = ...,
         EndpointArn: str = ...,
         Bytes: BlobTypeDef = ...,
-        DocumentReaderConfig: DocumentReaderConfigUnionTypeDef = ...
+        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
     ) -> DetectEntitiesResponseTypeDef:
         """
         Detects named entities in input text when you use the pre-trained model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_entities)
         """
@@ -901,75 +901,75 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.put_resource_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#put_resource_policy)
         """
     async def start_document_classification_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         DocumentClassifierArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartDocumentClassificationJobResponseTypeDef:
         """
         Starts an asynchronous document classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_document_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_document_classification_job)
         """
     async def start_dominant_language_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartDominantLanguageDetectionJobResponseTypeDef:
         """
         Starts an asynchronous dominant language detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_dominant_language_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_dominant_language_detection_job)
         """
     async def start_entities_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         EntityRecognizerArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FlywheelArn: str = ...
     ) -> StartEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_entities_detection_job)
         """
     async def start_events_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         TargetEventTypes: Sequence[str],
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
@@ -989,99 +989,99 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_flywheel_iteration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_flywheel_iteration)
         """
     async def start_key_phrases_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartKeyPhrasesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous key phrase detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_key_phrases_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_key_phrases_detection_job)
         """
     async def start_pii_entities_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         Mode: PiiEntitiesDetectionModeType,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
-        RedactionConfig: RedactionConfigUnionTypeDef = ...,
+        RedactionConfig: RedactionConfigTypeDef = ...,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartPiiEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous PII entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_pii_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_pii_entities_detection_job)
         """
     async def start_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous sentiment detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_sentiment_detection_job)
         """
     async def start_targeted_sentiment_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTargetedSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous targeted sentiment detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_targeted_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_targeted_sentiment_detection_job)
         """
     async def start_topics_detection_job(
         self,
         *,
-        InputDataConfig: InputDataConfigUnionTypeDef,
+        InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         NumberOfTopics: int = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
-        VpcConfig: VpcConfigUnionTypeDef = ...,
+        VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> StartTopicsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous topic detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_topics_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_topics_detection_job)
```

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/literals.py` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/literals.pyi` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/paginator.py` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/paginator.pyi` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/type_defs.py` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for comprehend service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_comprehend.type_defs import AugmentedManifestsListItemOutputTypeDef
+    from types_aiobotocore_comprehend.type_defs import AugmentedManifestsListItemTypeDef
 
-    data: AugmentedManifestsListItemOutputTypeDef = ...
+    data: AugmentedManifestsListItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -59,15 +59,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AugmentedManifestsListItemOutputTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
@@ -88,15 +87,14 @@
     "ErrorsListItemTypeDef",
     "WarningsListItemTypeDef",
     "ContainsPiiEntitiesRequestRequestTypeDef",
     "EntityLabelTypeDef",
     "TagTypeDef",
     "DocumentClassifierOutputDataConfigTypeDef",
     "VpcConfigTypeDef",
-    "VpcConfigOutputTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
     "TimestampTypeDef",
     "DatasetPropertiesTypeDef",
@@ -125,19 +123,17 @@
     "DetectDominantLanguageRequestRequestTypeDef",
     "DetectKeyPhrasesRequestRequestTypeDef",
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
-    "DocumentClassificationConfigOutputTypeDef",
     "DocumentClassificationConfigTypeDef",
     "OutputDataConfigTypeDef",
     "DocumentClassifierDocumentsTypeDef",
-    "DocumentReaderConfigOutputTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
     "EntityTypesListItemTypeDef",
     "EntityRecognizerAnnotationsTypeDef",
     "EntityRecognizerDocumentsTypeDef",
     "EntityRecognizerEntityListTypeDef",
     "EntityRecognizerEvaluationMetricsTypeDef",
@@ -149,17 +145,16 @@
     "PointTypeDef",
     "PaginatorConfigTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
-    "RedactionConfigOutputTypeDef",
-    "PutResourcePolicyRequestRequestTypeDef",
     "RedactionConfigTypeDef",
+    "PutResourcePolicyRequestRequestTypeDef",
     "StartFlywheelIterationRequestRequestTypeDef",
     "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     "StopEntitiesDetectionJobRequestRequestTypeDef",
     "StopEventsDetectionJobRequestRequestTypeDef",
     "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StopSentimentDetectionJobRequestRequestTypeDef",
@@ -209,16 +204,14 @@
     "ContainsPiiEntitiesResponseTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "ImportModelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DataSecurityConfigTypeDef",
     "UpdateDataSecurityConfigTypeDef",
-    "DataSecurityConfigOutputTypeDef",
-    "VpcConfigUnionTypeDef",
     "DatasetEntityRecognizerInputDataConfigTypeDef",
     "DatasetFilterTypeDef",
     "DocumentClassificationJobFilterTypeDef",
     "DocumentClassifierFilterTypeDef",
     "DominantLanguageDetectionJobFilterTypeDef",
     "EndpointFilterTypeDef",
     "EntitiesDetectionJobFilterTypeDef",
@@ -233,46 +226,48 @@
     "TopicsDetectionJobFilterTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
     "DocumentClassifierInputDataConfigTypeDef",
-    "DocumentClassifierInputDataConfigOutputTypeDef",
-    "DocumentReaderConfigUnionTypeDef",
-    "InputDataConfigOutputTypeDef",
     "ListDocumentClassifierSummariesResponseTypeDef",
     "DocumentMetadataTypeDef",
-    "EntityRecognitionConfigOutputTypeDef",
     "EntityRecognitionConfigTypeDef",
-    "EntityRecognizerInputDataConfigOutputTypeDef",
     "EntityRecognizerInputDataConfigTypeDef",
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     "ListEntityRecognizerSummariesResponseTypeDef",
     "FlywheelIterationPropertiesTypeDef",
     "ListFlywheelsResponseTypeDef",
     "GeometryTypeDef",
     "SyntaxTokenTypeDef",
-    "RedactionConfigUnionTypeDef",
     "BatchDetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentResponseTypeDef",
     "TargetedSentimentMentionTypeDef",
     "EntityTypeDef",
+    "DocumentClassificationJobPropertiesTypeDef",
+    "DominantLanguageDetectionJobPropertiesTypeDef",
+    "EntitiesDetectionJobPropertiesTypeDef",
+    "EventsDetectionJobPropertiesTypeDef",
+    "KeyPhrasesDetectionJobPropertiesTypeDef",
+    "PiiEntitiesDetectionJobPropertiesTypeDef",
+    "SentimentDetectionJobPropertiesTypeDef",
     "StartDocumentClassificationJobRequestRequestTypeDef",
     "StartDominantLanguageDetectionJobRequestRequestTypeDef",
     "StartEntitiesDetectionJobRequestRequestTypeDef",
     "StartEventsDetectionJobRequestRequestTypeDef",
     "StartKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StartPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StartSentimentDetectionJobRequestRequestTypeDef",
     "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StartTopicsDetectionJobRequestRequestTypeDef",
+    "TargetedSentimentDetectionJobPropertiesTypeDef",
+    "TopicsDetectionJobPropertiesTypeDef",
     "UpdateFlywheelRequestRequestTypeDef",
-    "DataSecurityConfigUnionTypeDef",
     "DatasetInputDataConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
     "ListDocumentClassificationJobsRequestRequestTypeDef",
     "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
     "ListDocumentClassifiersRequestRequestTypeDef",
     "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
@@ -292,42 +287,26 @@
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     "ListSentimentDetectionJobsRequestRequestTypeDef",
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     "CreateDocumentClassifierRequestRequestTypeDef",
-    "DocumentClassifierInputDataConfigUnionTypeDef",
     "DocumentClassifierPropertiesTypeDef",
-    "DocumentClassificationJobPropertiesTypeDef",
-    "DominantLanguageDetectionJobPropertiesTypeDef",
-    "EntitiesDetectionJobPropertiesTypeDef",
-    "EventsDetectionJobPropertiesTypeDef",
-    "InputDataConfigUnionTypeDef",
-    "KeyPhrasesDetectionJobPropertiesTypeDef",
-    "PiiEntitiesDetectionJobPropertiesTypeDef",
-    "SentimentDetectionJobPropertiesTypeDef",
-    "TargetedSentimentDetectionJobPropertiesTypeDef",
-    "TopicsDetectionJobPropertiesTypeDef",
     "ClassifyDocumentResponseTypeDef",
-    "TaskConfigOutputTypeDef",
     "TaskConfigTypeDef",
     "CreateEntityRecognizerRequestRequestTypeDef",
-    "EntityRecognizerInputDataConfigUnionTypeDef",
     "EntityRecognizerMetadataTypeDef",
     "DescribeFlywheelIterationResponseTypeDef",
     "ListFlywheelIterationHistoryResponseTypeDef",
     "BlockTypeDef",
     "BatchDetectSyntaxItemResultTypeDef",
     "DetectSyntaxResponseTypeDef",
     "TargetedSentimentEntityTypeDef",
     "BatchDetectEntitiesItemResultTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "DescribeDocumentClassifierResponseTypeDef",
-    "ListDocumentClassifiersResponseTypeDef",
     "DescribeDocumentClassificationJobResponseTypeDef",
     "ListDocumentClassificationJobsResponseTypeDef",
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     "DescribeEntitiesDetectionJobResponseTypeDef",
     "ListEntitiesDetectionJobsResponseTypeDef",
     "DescribeEventsDetectionJobResponseTypeDef",
@@ -338,56 +317,32 @@
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     "DescribeSentimentDetectionJobResponseTypeDef",
     "ListSentimentDetectionJobsResponseTypeDef",
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     "DescribeTopicsDetectionJobResponseTypeDef",
     "ListTopicsDetectionJobsResponseTypeDef",
-    "FlywheelPropertiesTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "DescribeDocumentClassifierResponseTypeDef",
+    "ListDocumentClassifiersResponseTypeDef",
     "CreateFlywheelRequestRequestTypeDef",
-    "TaskConfigUnionTypeDef",
+    "FlywheelPropertiesTypeDef",
     "EntityRecognizerPropertiesTypeDef",
     "DetectEntitiesResponseTypeDef",
     "BatchDetectSyntaxResponseTypeDef",
     "BatchDetectTargetedSentimentItemResultTypeDef",
     "DetectTargetedSentimentResponseTypeDef",
     "BatchDetectEntitiesResponseTypeDef",
     "DescribeFlywheelResponseTypeDef",
     "UpdateFlywheelResponseTypeDef",
     "DescribeEntityRecognizerResponseTypeDef",
     "ListEntityRecognizersResponseTypeDef",
     "BatchDetectTargetedSentimentResponseTypeDef",
 )
 
-_RequiredAugmentedManifestsListItemOutputTypeDef = TypedDict(
-    "_RequiredAugmentedManifestsListItemOutputTypeDef",
-    {
-        "S3Uri": str,
-        "AttributeNames": List[str],
-    },
-)
-_OptionalAugmentedManifestsListItemOutputTypeDef = TypedDict(
-    "_OptionalAugmentedManifestsListItemOutputTypeDef",
-    {
-        "Split": SplitType,
-        "AnnotationDataS3Uri": str,
-        "SourceDocumentsS3Uri": str,
-        "DocumentType": AugmentedManifestsDocumentTypeFormatType,
-    },
-    total=False,
-)
-
-
-class AugmentedManifestsListItemOutputTypeDef(
-    _RequiredAugmentedManifestsListItemOutputTypeDef,
-    _OptionalAugmentedManifestsListItemOutputTypeDef,
-):
-    pass
-
-
 _RequiredAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredAugmentedManifestsListItemTypeDef",
     {
         "S3Uri": str,
         "AttributeNames": Sequence[str],
     },
 )
@@ -675,22 +630,14 @@
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
 
-VpcConfigOutputTypeDef = TypedDict(
-    "VpcConfigOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "Subnets": List[str],
-    },
-)
-
 _RequiredDatasetAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredDatasetAugmentedManifestsListItemTypeDef",
     {
         "AttributeNames": Sequence[str],
         "S3Uri": str,
     },
 )
@@ -1024,36 +971,14 @@
     "DetectTargetedSentimentRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
     },
 )
 
-_RequiredDocumentClassificationConfigOutputTypeDef = TypedDict(
-    "_RequiredDocumentClassificationConfigOutputTypeDef",
-    {
-        "Mode": DocumentClassifierModeType,
-    },
-)
-_OptionalDocumentClassificationConfigOutputTypeDef = TypedDict(
-    "_OptionalDocumentClassificationConfigOutputTypeDef",
-    {
-        "Labels": List[str],
-    },
-    total=False,
-)
-
-
-class DocumentClassificationConfigOutputTypeDef(
-    _RequiredDocumentClassificationConfigOutputTypeDef,
-    _OptionalDocumentClassificationConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredDocumentClassificationConfigTypeDef = TypedDict(
     "_RequiredDocumentClassificationConfigTypeDef",
     {
         "Mode": DocumentClassifierModeType,
     },
 )
 _OptionalDocumentClassificationConfigTypeDef = TypedDict(
@@ -1107,36 +1032,14 @@
 
 class DocumentClassifierDocumentsTypeDef(
     _RequiredDocumentClassifierDocumentsTypeDef, _OptionalDocumentClassifierDocumentsTypeDef
 ):
     pass
 
 
-_RequiredDocumentReaderConfigOutputTypeDef = TypedDict(
-    "_RequiredDocumentReaderConfigOutputTypeDef",
-    {
-        "DocumentReadAction": DocumentReadActionType,
-    },
-)
-_OptionalDocumentReaderConfigOutputTypeDef = TypedDict(
-    "_OptionalDocumentReaderConfigOutputTypeDef",
-    {
-        "DocumentReadMode": DocumentReadModeType,
-        "FeatureTypes": List[DocumentReadFeatureTypesType],
-    },
-    total=False,
-)
-
-
-class DocumentReaderConfigOutputTypeDef(
-    _RequiredDocumentReaderConfigOutputTypeDef, _OptionalDocumentReaderConfigOutputTypeDef
-):
-    pass
-
-
 DocumentClassifierSummaryTypeDef = TypedDict(
     "DocumentClassifierSummaryTypeDef",
     {
         "DocumentClassifierName": str,
         "NumberOfVersions": int,
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
@@ -1348,16 +1251,16 @@
 
 class PiiOutputDataConfigTypeDef(
     _RequiredPiiOutputDataConfigTypeDef, _OptionalPiiOutputDataConfigTypeDef
 ):
     pass
 
 
-RedactionConfigOutputTypeDef = TypedDict(
-    "RedactionConfigOutputTypeDef",
+RedactionConfigTypeDef = TypedDict(
+    "RedactionConfigTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
     total=False,
 )
@@ -1380,24 +1283,14 @@
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
 
-RedactionConfigTypeDef = TypedDict(
-    "RedactionConfigTypeDef",
-    {
-        "PiiEntityTypes": Sequence[PiiEntityTypeType],
-        "MaskMode": PiiEntitiesDetectionMaskModeType,
-        "MaskCharacter": str,
-    },
-    total=False,
-)
-
 _RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
     "_RequiredStartFlywheelIterationRequestRequestTypeDef",
     {
         "FlywheelArn": str,
     },
 )
 _OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
@@ -1984,26 +1877,14 @@
         "ModelKmsKeyId": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
-DataSecurityConfigOutputTypeDef = TypedDict(
-    "DataSecurityConfigOutputTypeDef",
-    {
-        "ModelKmsKeyId": str,
-        "VolumeKmsKeyId": str,
-        "DataLakeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetEntityRecognizerInputDataConfigTypeDef",
     {
         "Documents": DatasetEntityRecognizerDocumentsTypeDef,
     },
 )
 _OptionalDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2238,54 +2119,14 @@
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
         "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-DocumentClassifierInputDataConfigOutputTypeDef = TypedDict(
-    "DocumentClassifierInputDataConfigOutputTypeDef",
-    {
-        "DataFormat": DocumentClassifierDataFormatType,
-        "S3Uri": str,
-        "TestS3Uri": str,
-        "LabelDelimiter": str,
-        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
-        "DocumentType": DocumentClassifierDocumentTypeFormatType,
-        "Documents": DocumentClassifierDocumentsTypeDef,
-        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-DocumentReaderConfigUnionTypeDef = Union[
-    DocumentReaderConfigTypeDef, DocumentReaderConfigOutputTypeDef
-]
-_RequiredInputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredInputDataConfigOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalInputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalInputDataConfigOutputTypeDef",
-    {
-        "InputFormat": InputFormatType,
-        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class InputDataConfigOutputTypeDef(
-    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
-):
-    pass
-
-
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2296,54 +2137,21 @@
     {
         "Pages": int,
         "ExtractedCharacters": List[ExtractedCharactersListItemTypeDef],
     },
     total=False,
 )
 
-EntityRecognitionConfigOutputTypeDef = TypedDict(
-    "EntityRecognitionConfigOutputTypeDef",
-    {
-        "EntityTypes": List[EntityTypesListItemTypeDef],
-    },
-)
-
 EntityRecognitionConfigTypeDef = TypedDict(
     "EntityRecognitionConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 
-_RequiredEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredEntityRecognizerInputDataConfigOutputTypeDef",
-    {
-        "EntityTypes": List[EntityTypesListItemTypeDef],
-    },
-)
-_OptionalEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalEntityRecognizerInputDataConfigOutputTypeDef",
-    {
-        "DataFormat": EntityRecognizerDataFormatType,
-        "Documents": EntityRecognizerDocumentsTypeDef,
-        "Annotations": EntityRecognizerAnnotationsTypeDef,
-        "EntityList": EntityRecognizerEntityListTypeDef,
-        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class EntityRecognizerInputDataConfigOutputTypeDef(
-    _RequiredEntityRecognizerInputDataConfigOutputTypeDef,
-    _OptionalEntityRecognizerInputDataConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredEntityRecognizerInputDataConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 _OptionalEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2428,15 +2236,14 @@
         "BeginOffset": int,
         "EndOffset": int,
         "PartOfSpeech": PartOfSpeechTagTypeDef,
     },
     total=False,
 )
 
-RedactionConfigUnionTypeDef = Union[RedactionConfigTypeDef, RedactionConfigOutputTypeDef]
 BatchDetectDominantLanguageResponseTypeDef = TypedDict(
     "BatchDetectDominantLanguageResponseTypeDef",
     {
         "ResultList": List[BatchDetectDominantLanguageItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2483,14 +2290,155 @@
         "BeginOffset": int,
         "EndOffset": int,
         "BlockReferences": List[BlockReferenceTypeDef],
     },
     total=False,
 )
 
+DocumentClassificationJobPropertiesTypeDef = TypedDict(
+    "DocumentClassificationJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "DocumentClassifierArn": str,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
+    "DominantLanguageDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
+EntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "EntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "EntityRecognizerArn": str,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+EventsDetectionJobPropertiesTypeDef = TypedDict(
+    "EventsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "TargetEventTypes": List[str],
+    },
+    total=False,
+)
+
+KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
+    "KeyPhrasesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
+PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "PiiEntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": PiiOutputDataConfigTypeDef,
+        "RedactionConfig": RedactionConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "Mode": PiiEntitiesDetectionModeType,
+    },
+    total=False,
+)
+
+SentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "SentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStartDocumentClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentClassificationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2745,14 +2693,54 @@
 class StartTopicsDetectionJobRequestRequestTypeDef(
     _RequiredStartTopicsDetectionJobRequestRequestTypeDef,
     _OptionalStartTopicsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
 
+TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "TargetedSentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
+TopicsDetectionJobPropertiesTypeDef = TypedDict(
+    "TopicsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "NumberOfTopics": int,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlywheelRequestRequestTypeDef",
     {
         "FlywheelArn": str,
     },
 )
 _OptionalUpdateFlywheelRequestRequestTypeDef = TypedDict(
@@ -2768,15 +2756,14 @@
 
 class UpdateFlywheelRequestRequestTypeDef(
     _RequiredUpdateFlywheelRequestRequestTypeDef, _OptionalUpdateFlywheelRequestRequestTypeDef
 ):
     pass
 
 
-DataSecurityConfigUnionTypeDef = Union[DataSecurityConfigTypeDef, DataSecurityConfigOutputTypeDef]
 DatasetInputDataConfigTypeDef = TypedDict(
     "DatasetInputDataConfigTypeDef",
     {
         "AugmentedManifests": Sequence[DatasetAugmentedManifestsListItemTypeDef],
         "DataFormat": DatasetDataFormatType,
         "DocumentClassifierInputDataConfig": DatasetDocumentClassifierInputDataConfigTypeDef,
         "EntityRecognizerInputDataConfig": DatasetEntityRecognizerInputDataConfigTypeDef,
@@ -3070,258 +3057,53 @@
 class CreateDocumentClassifierRequestRequestTypeDef(
     _RequiredCreateDocumentClassifierRequestRequestTypeDef,
     _OptionalCreateDocumentClassifierRequestRequestTypeDef,
 ):
     pass
 
 
-DocumentClassifierInputDataConfigUnionTypeDef = Union[
-    DocumentClassifierInputDataConfigTypeDef, DocumentClassifierInputDataConfigOutputTypeDef
-]
 DocumentClassifierPropertiesTypeDef = TypedDict(
     "DocumentClassifierPropertiesTypeDef",
     {
         "DocumentClassifierArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": DocumentClassifierInputDataConfigOutputTypeDef,
+        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
         "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
         "ClassifierMetadata": ClassifierMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
-DocumentClassificationJobPropertiesTypeDef = TypedDict(
-    "DocumentClassificationJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "DocumentClassifierArn": str,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
-    "DominantLanguageDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-EntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "EntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "EntityRecognizerArn": str,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-EventsDetectionJobPropertiesTypeDef = TypedDict(
-    "EventsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "TargetEventTypes": List[str],
-    },
-    total=False,
-)
-
-InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
-KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
-    "KeyPhrasesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "PiiEntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": PiiOutputDataConfigTypeDef,
-        "RedactionConfig": RedactionConfigOutputTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "Mode": PiiEntitiesDetectionModeType,
-    },
-    total=False,
-)
-
-SentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "SentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "TargetedSentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-TopicsDetectionJobPropertiesTypeDef = TypedDict(
-    "TopicsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "NumberOfTopics": int,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ClassifyDocumentResponseTypeDef = TypedDict(
     "ClassifyDocumentResponseTypeDef",
     {
         "Classes": List[DocumentClassTypeDef],
         "Labels": List[DocumentLabelTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
         "Warnings": List[WarningsListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTaskConfigOutputTypeDef = TypedDict(
-    "_RequiredTaskConfigOutputTypeDef",
-    {
-        "LanguageCode": LanguageCodeType,
-    },
-)
-_OptionalTaskConfigOutputTypeDef = TypedDict(
-    "_OptionalTaskConfigOutputTypeDef",
-    {
-        "DocumentClassificationConfig": DocumentClassificationConfigOutputTypeDef,
-        "EntityRecognitionConfig": EntityRecognitionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class TaskConfigOutputTypeDef(_RequiredTaskConfigOutputTypeDef, _OptionalTaskConfigOutputTypeDef):
-    pass
-
-
 _RequiredTaskConfigTypeDef = TypedDict(
     "_RequiredTaskConfigTypeDef",
     {
         "LanguageCode": LanguageCodeType,
     },
 )
 _OptionalTaskConfigTypeDef = TypedDict(
@@ -3365,17 +3147,14 @@
 class CreateEntityRecognizerRequestRequestTypeDef(
     _RequiredCreateEntityRecognizerRequestRequestTypeDef,
     _OptionalCreateEntityRecognizerRequestRequestTypeDef,
 ):
     pass
 
 
-EntityRecognizerInputDataConfigUnionTypeDef = Union[
-    EntityRecognizerInputDataConfigTypeDef, EntityRecognizerInputDataConfigOutputTypeDef
-]
 EntityRecognizerMetadataTypeDef = TypedDict(
     "EntityRecognizerMetadataTypeDef",
     {
         "NumberOfTrainedDocuments": int,
         "NumberOfTestDocuments": int,
         "EvaluationMetrics": EntityRecognizerEvaluationMetricsTypeDef,
         "EntityTypes": List[EntityRecognizerMetadataEntityTypesListItemTypeDef],
@@ -3444,57 +3223,14 @@
     {
         "Index": int,
         "Entities": List[EntityTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "FlywheelArn": str,
-        "DatasetName": str,
-        "InputDataConfig": DatasetInputDataConfigTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "Description": str,
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-
-DescribeDocumentClassifierResponseTypeDef = TypedDict(
-    "DescribeDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDocumentClassifiersResponseTypeDef = TypedDict(
-    "ListDocumentClassifiersResponseTypeDef",
-    {
-        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeDocumentClassificationJobResponseTypeDef = TypedDict(
     "DescribeDocumentClassificationJobResponseTypeDef",
     {
         "DocumentClassificationJobProperties": DocumentClassificationJobPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3644,33 +3380,57 @@
     {
         "TopicsDetectionJobPropertiesList": List[TopicsDetectionJobPropertiesTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FlywheelPropertiesTypeDef = TypedDict(
-    "FlywheelPropertiesTypeDef",
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "DataAccessRoleArn": str,
-        "TaskConfig": TaskConfigOutputTypeDef,
-        "DataLakeS3Uri": str,
-        "DataSecurityConfig": DataSecurityConfigOutputTypeDef,
-        "Status": FlywheelStatusType,
-        "ModelType": ModelTypeType,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LatestFlywheelIteration": str,
+        "DatasetName": str,
+        "InputDataConfig": DatasetInputDataConfigTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "Description": str,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+
+DescribeDocumentClassifierResponseTypeDef = TypedDict(
+    "DescribeDocumentClassifierResponseTypeDef",
+    {
+        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDocumentClassifiersResponseTypeDef = TypedDict(
+    "ListDocumentClassifiersResponseTypeDef",
+    {
+        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlywheelRequestRequestTypeDef",
     {
         "FlywheelName": str,
         "DataAccessRoleArn": str,
         "DataLakeS3Uri": str,
     },
@@ -3691,31 +3451,49 @@
 
 class CreateFlywheelRequestRequestTypeDef(
     _RequiredCreateFlywheelRequestRequestTypeDef, _OptionalCreateFlywheelRequestRequestTypeDef
 ):
     pass
 
 
-TaskConfigUnionTypeDef = Union[TaskConfigTypeDef, TaskConfigOutputTypeDef]
+FlywheelPropertiesTypeDef = TypedDict(
+    "FlywheelPropertiesTypeDef",
+    {
+        "FlywheelArn": str,
+        "ActiveModelArn": str,
+        "DataAccessRoleArn": str,
+        "TaskConfig": TaskConfigTypeDef,
+        "DataLakeS3Uri": str,
+        "DataSecurityConfig": DataSecurityConfigTypeDef,
+        "Status": FlywheelStatusType,
+        "ModelType": ModelTypeType,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LatestFlywheelIteration": str,
+    },
+    total=False,
+)
+
 EntityRecognizerPropertiesTypeDef = TypedDict(
     "EntityRecognizerPropertiesTypeDef",
     {
         "EntityRecognizerArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": EntityRecognizerInputDataConfigOutputTypeDef,
+        "InputDataConfig": EntityRecognizerInputDataConfigTypeDef,
         "RecognizerMetadata": EntityRecognizerMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
         "OutputDataConfig": EntityRecognizerOutputDataConfigTypeDef,
     },
     total=False,
```

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend/type_defs.pyi` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for comprehend service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_comprehend.type_defs import AugmentedManifestsListItemOutputTypeDef
+    from types_aiobotocore_comprehend.type_defs import AugmentedManifestsListItemTypeDef
 
-    data: AugmentedManifestsListItemOutputTypeDef = ...
+    data: AugmentedManifestsListItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -58,15 +58,14 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AugmentedManifestsListItemOutputTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDetectEntitiesRequestRequestTypeDef",
     "KeyPhraseTypeDef",
@@ -87,15 +86,14 @@
     "ErrorsListItemTypeDef",
     "WarningsListItemTypeDef",
     "ContainsPiiEntitiesRequestRequestTypeDef",
     "EntityLabelTypeDef",
     "TagTypeDef",
     "DocumentClassifierOutputDataConfigTypeDef",
     "VpcConfigTypeDef",
-    "VpcConfigOutputTypeDef",
     "DatasetAugmentedManifestsListItemTypeDef",
     "DatasetDocumentClassifierInputDataConfigTypeDef",
     "DatasetEntityRecognizerAnnotationsTypeDef",
     "DatasetEntityRecognizerDocumentsTypeDef",
     "DatasetEntityRecognizerEntityListTypeDef",
     "TimestampTypeDef",
     "DatasetPropertiesTypeDef",
@@ -124,19 +122,17 @@
     "DetectDominantLanguageRequestRequestTypeDef",
     "DetectKeyPhrasesRequestRequestTypeDef",
     "DetectPiiEntitiesRequestRequestTypeDef",
     "PiiEntityTypeDef",
     "DetectSentimentRequestRequestTypeDef",
     "DetectSyntaxRequestRequestTypeDef",
     "DetectTargetedSentimentRequestRequestTypeDef",
-    "DocumentClassificationConfigOutputTypeDef",
     "DocumentClassificationConfigTypeDef",
     "OutputDataConfigTypeDef",
     "DocumentClassifierDocumentsTypeDef",
-    "DocumentReaderConfigOutputTypeDef",
     "DocumentClassifierSummaryTypeDef",
     "ExtractedCharactersListItemTypeDef",
     "EntityTypesListItemTypeDef",
     "EntityRecognizerAnnotationsTypeDef",
     "EntityRecognizerDocumentsTypeDef",
     "EntityRecognizerEntityListTypeDef",
     "EntityRecognizerEvaluationMetricsTypeDef",
@@ -148,17 +144,16 @@
     "PointTypeDef",
     "PaginatorConfigTypeDef",
     "ListDocumentClassifierSummariesRequestRequestTypeDef",
     "ListEntityRecognizerSummariesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "PartOfSpeechTagTypeDef",
     "PiiOutputDataConfigTypeDef",
-    "RedactionConfigOutputTypeDef",
-    "PutResourcePolicyRequestRequestTypeDef",
     "RedactionConfigTypeDef",
+    "PutResourcePolicyRequestRequestTypeDef",
     "StartFlywheelIterationRequestRequestTypeDef",
     "StopDominantLanguageDetectionJobRequestRequestTypeDef",
     "StopEntitiesDetectionJobRequestRequestTypeDef",
     "StopEventsDetectionJobRequestRequestTypeDef",
     "StopKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StopPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StopSentimentDetectionJobRequestRequestTypeDef",
@@ -208,16 +203,14 @@
     "ContainsPiiEntitiesResponseTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "ImportModelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DataSecurityConfigTypeDef",
     "UpdateDataSecurityConfigTypeDef",
-    "DataSecurityConfigOutputTypeDef",
-    "VpcConfigUnionTypeDef",
     "DatasetEntityRecognizerInputDataConfigTypeDef",
     "DatasetFilterTypeDef",
     "DocumentClassificationJobFilterTypeDef",
     "DocumentClassifierFilterTypeDef",
     "DominantLanguageDetectionJobFilterTypeDef",
     "EndpointFilterTypeDef",
     "EntitiesDetectionJobFilterTypeDef",
@@ -232,46 +225,48 @@
     "TopicsDetectionJobFilterTypeDef",
     "DescribeDatasetResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "ListEndpointsResponseTypeDef",
     "DetectPiiEntitiesResponseTypeDef",
     "DocumentClassifierInputDataConfigTypeDef",
-    "DocumentClassifierInputDataConfigOutputTypeDef",
-    "DocumentReaderConfigUnionTypeDef",
-    "InputDataConfigOutputTypeDef",
     "ListDocumentClassifierSummariesResponseTypeDef",
     "DocumentMetadataTypeDef",
-    "EntityRecognitionConfigOutputTypeDef",
     "EntityRecognitionConfigTypeDef",
-    "EntityRecognizerInputDataConfigOutputTypeDef",
     "EntityRecognizerInputDataConfigTypeDef",
     "EntityRecognizerMetadataEntityTypesListItemTypeDef",
     "ListEntityRecognizerSummariesResponseTypeDef",
     "FlywheelIterationPropertiesTypeDef",
     "ListFlywheelsResponseTypeDef",
     "GeometryTypeDef",
     "SyntaxTokenTypeDef",
-    "RedactionConfigUnionTypeDef",
     "BatchDetectDominantLanguageResponseTypeDef",
     "BatchDetectKeyPhrasesResponseTypeDef",
     "BatchDetectSentimentResponseTypeDef",
     "TargetedSentimentMentionTypeDef",
     "EntityTypeDef",
+    "DocumentClassificationJobPropertiesTypeDef",
+    "DominantLanguageDetectionJobPropertiesTypeDef",
+    "EntitiesDetectionJobPropertiesTypeDef",
+    "EventsDetectionJobPropertiesTypeDef",
+    "KeyPhrasesDetectionJobPropertiesTypeDef",
+    "PiiEntitiesDetectionJobPropertiesTypeDef",
+    "SentimentDetectionJobPropertiesTypeDef",
     "StartDocumentClassificationJobRequestRequestTypeDef",
     "StartDominantLanguageDetectionJobRequestRequestTypeDef",
     "StartEntitiesDetectionJobRequestRequestTypeDef",
     "StartEventsDetectionJobRequestRequestTypeDef",
     "StartKeyPhrasesDetectionJobRequestRequestTypeDef",
     "StartPiiEntitiesDetectionJobRequestRequestTypeDef",
     "StartSentimentDetectionJobRequestRequestTypeDef",
     "StartTargetedSentimentDetectionJobRequestRequestTypeDef",
     "StartTopicsDetectionJobRequestRequestTypeDef",
+    "TargetedSentimentDetectionJobPropertiesTypeDef",
+    "TopicsDetectionJobPropertiesTypeDef",
     "UpdateFlywheelRequestRequestTypeDef",
-    "DataSecurityConfigUnionTypeDef",
     "DatasetInputDataConfigTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef",
     "ListDocumentClassificationJobsRequestRequestTypeDef",
     "ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef",
     "ListDocumentClassifiersRequestRequestTypeDef",
     "ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef",
@@ -291,42 +286,26 @@
     "ListPiiEntitiesDetectionJobsRequestRequestTypeDef",
     "ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef",
     "ListSentimentDetectionJobsRequestRequestTypeDef",
     "ListTargetedSentimentDetectionJobsRequestRequestTypeDef",
     "ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef",
     "ListTopicsDetectionJobsRequestRequestTypeDef",
     "CreateDocumentClassifierRequestRequestTypeDef",
-    "DocumentClassifierInputDataConfigUnionTypeDef",
     "DocumentClassifierPropertiesTypeDef",
-    "DocumentClassificationJobPropertiesTypeDef",
-    "DominantLanguageDetectionJobPropertiesTypeDef",
-    "EntitiesDetectionJobPropertiesTypeDef",
-    "EventsDetectionJobPropertiesTypeDef",
-    "InputDataConfigUnionTypeDef",
-    "KeyPhrasesDetectionJobPropertiesTypeDef",
-    "PiiEntitiesDetectionJobPropertiesTypeDef",
-    "SentimentDetectionJobPropertiesTypeDef",
-    "TargetedSentimentDetectionJobPropertiesTypeDef",
-    "TopicsDetectionJobPropertiesTypeDef",
     "ClassifyDocumentResponseTypeDef",
-    "TaskConfigOutputTypeDef",
     "TaskConfigTypeDef",
     "CreateEntityRecognizerRequestRequestTypeDef",
-    "EntityRecognizerInputDataConfigUnionTypeDef",
     "EntityRecognizerMetadataTypeDef",
     "DescribeFlywheelIterationResponseTypeDef",
     "ListFlywheelIterationHistoryResponseTypeDef",
     "BlockTypeDef",
     "BatchDetectSyntaxItemResultTypeDef",
     "DetectSyntaxResponseTypeDef",
     "TargetedSentimentEntityTypeDef",
     "BatchDetectEntitiesItemResultTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "DescribeDocumentClassifierResponseTypeDef",
-    "ListDocumentClassifiersResponseTypeDef",
     "DescribeDocumentClassificationJobResponseTypeDef",
     "ListDocumentClassificationJobsResponseTypeDef",
     "DescribeDominantLanguageDetectionJobResponseTypeDef",
     "ListDominantLanguageDetectionJobsResponseTypeDef",
     "DescribeEntitiesDetectionJobResponseTypeDef",
     "ListEntitiesDetectionJobsResponseTypeDef",
     "DescribeEventsDetectionJobResponseTypeDef",
@@ -337,54 +316,32 @@
     "ListPiiEntitiesDetectionJobsResponseTypeDef",
     "DescribeSentimentDetectionJobResponseTypeDef",
     "ListSentimentDetectionJobsResponseTypeDef",
     "DescribeTargetedSentimentDetectionJobResponseTypeDef",
     "ListTargetedSentimentDetectionJobsResponseTypeDef",
     "DescribeTopicsDetectionJobResponseTypeDef",
     "ListTopicsDetectionJobsResponseTypeDef",
-    "FlywheelPropertiesTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "DescribeDocumentClassifierResponseTypeDef",
+    "ListDocumentClassifiersResponseTypeDef",
     "CreateFlywheelRequestRequestTypeDef",
-    "TaskConfigUnionTypeDef",
+    "FlywheelPropertiesTypeDef",
     "EntityRecognizerPropertiesTypeDef",
     "DetectEntitiesResponseTypeDef",
     "BatchDetectSyntaxResponseTypeDef",
     "BatchDetectTargetedSentimentItemResultTypeDef",
     "DetectTargetedSentimentResponseTypeDef",
     "BatchDetectEntitiesResponseTypeDef",
     "DescribeFlywheelResponseTypeDef",
     "UpdateFlywheelResponseTypeDef",
     "DescribeEntityRecognizerResponseTypeDef",
     "ListEntityRecognizersResponseTypeDef",
     "BatchDetectTargetedSentimentResponseTypeDef",
 )
 
-_RequiredAugmentedManifestsListItemOutputTypeDef = TypedDict(
-    "_RequiredAugmentedManifestsListItemOutputTypeDef",
-    {
-        "S3Uri": str,
-        "AttributeNames": List[str],
-    },
-)
-_OptionalAugmentedManifestsListItemOutputTypeDef = TypedDict(
-    "_OptionalAugmentedManifestsListItemOutputTypeDef",
-    {
-        "Split": SplitType,
-        "AnnotationDataS3Uri": str,
-        "SourceDocumentsS3Uri": str,
-        "DocumentType": AugmentedManifestsDocumentTypeFormatType,
-    },
-    total=False,
-)
-
-class AugmentedManifestsListItemOutputTypeDef(
-    _RequiredAugmentedManifestsListItemOutputTypeDef,
-    _OptionalAugmentedManifestsListItemOutputTypeDef,
-):
-    pass
-
 _RequiredAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredAugmentedManifestsListItemTypeDef",
     {
         "S3Uri": str,
         "AttributeNames": Sequence[str],
     },
 )
@@ -666,22 +623,14 @@
     "VpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "Subnets": Sequence[str],
     },
 )
 
-VpcConfigOutputTypeDef = TypedDict(
-    "VpcConfigOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "Subnets": List[str],
-    },
-)
-
 _RequiredDatasetAugmentedManifestsListItemTypeDef = TypedDict(
     "_RequiredDatasetAugmentedManifestsListItemTypeDef",
     {
         "AttributeNames": Sequence[str],
         "S3Uri": str,
     },
 )
@@ -1007,34 +956,14 @@
     "DetectTargetedSentimentRequestRequestTypeDef",
     {
         "Text": str,
         "LanguageCode": LanguageCodeType,
     },
 )
 
-_RequiredDocumentClassificationConfigOutputTypeDef = TypedDict(
-    "_RequiredDocumentClassificationConfigOutputTypeDef",
-    {
-        "Mode": DocumentClassifierModeType,
-    },
-)
-_OptionalDocumentClassificationConfigOutputTypeDef = TypedDict(
-    "_OptionalDocumentClassificationConfigOutputTypeDef",
-    {
-        "Labels": List[str],
-    },
-    total=False,
-)
-
-class DocumentClassificationConfigOutputTypeDef(
-    _RequiredDocumentClassificationConfigOutputTypeDef,
-    _OptionalDocumentClassificationConfigOutputTypeDef,
-):
-    pass
-
 _RequiredDocumentClassificationConfigTypeDef = TypedDict(
     "_RequiredDocumentClassificationConfigTypeDef",
     {
         "Mode": DocumentClassifierModeType,
     },
 )
 _OptionalDocumentClassificationConfigTypeDef = TypedDict(
@@ -1082,34 +1011,14 @@
 )
 
 class DocumentClassifierDocumentsTypeDef(
     _RequiredDocumentClassifierDocumentsTypeDef, _OptionalDocumentClassifierDocumentsTypeDef
 ):
     pass
 
-_RequiredDocumentReaderConfigOutputTypeDef = TypedDict(
-    "_RequiredDocumentReaderConfigOutputTypeDef",
-    {
-        "DocumentReadAction": DocumentReadActionType,
-    },
-)
-_OptionalDocumentReaderConfigOutputTypeDef = TypedDict(
-    "_OptionalDocumentReaderConfigOutputTypeDef",
-    {
-        "DocumentReadMode": DocumentReadModeType,
-        "FeatureTypes": List[DocumentReadFeatureTypesType],
-    },
-    total=False,
-)
-
-class DocumentReaderConfigOutputTypeDef(
-    _RequiredDocumentReaderConfigOutputTypeDef, _OptionalDocumentReaderConfigOutputTypeDef
-):
-    pass
-
 DocumentClassifierSummaryTypeDef = TypedDict(
     "DocumentClassifierSummaryTypeDef",
     {
         "DocumentClassifierName": str,
         "NumberOfVersions": int,
         "LatestVersionCreatedAt": datetime,
         "LatestVersionName": str,
@@ -1315,16 +1224,16 @@
 )
 
 class PiiOutputDataConfigTypeDef(
     _RequiredPiiOutputDataConfigTypeDef, _OptionalPiiOutputDataConfigTypeDef
 ):
     pass
 
-RedactionConfigOutputTypeDef = TypedDict(
-    "RedactionConfigOutputTypeDef",
+RedactionConfigTypeDef = TypedDict(
+    "RedactionConfigTypeDef",
     {
         "PiiEntityTypes": List[PiiEntityTypeType],
         "MaskMode": PiiEntitiesDetectionMaskModeType,
         "MaskCharacter": str,
     },
     total=False,
 )
@@ -1345,24 +1254,14 @@
 )
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-RedactionConfigTypeDef = TypedDict(
-    "RedactionConfigTypeDef",
-    {
-        "PiiEntityTypes": Sequence[PiiEntityTypeType],
-        "MaskMode": PiiEntitiesDetectionMaskModeType,
-        "MaskCharacter": str,
-    },
-    total=False,
-)
-
 _RequiredStartFlywheelIterationRequestRequestTypeDef = TypedDict(
     "_RequiredStartFlywheelIterationRequestRequestTypeDef",
     {
         "FlywheelArn": str,
     },
 )
 _OptionalStartFlywheelIterationRequestRequestTypeDef = TypedDict(
@@ -1937,26 +1836,14 @@
         "ModelKmsKeyId": str,
         "VolumeKmsKeyId": str,
         "VpcConfig": VpcConfigTypeDef,
     },
     total=False,
 )
 
-DataSecurityConfigOutputTypeDef = TypedDict(
-    "DataSecurityConfigOutputTypeDef",
-    {
-        "ModelKmsKeyId": str,
-        "VolumeKmsKeyId": str,
-        "DataLakeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-VpcConfigUnionTypeDef = Union[VpcConfigTypeDef, VpcConfigOutputTypeDef]
 _RequiredDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredDatasetEntityRecognizerInputDataConfigTypeDef",
     {
         "Documents": DatasetEntityRecognizerDocumentsTypeDef,
     },
 )
 _OptionalDatasetEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2189,52 +2076,14 @@
         "DocumentType": DocumentClassifierDocumentTypeFormatType,
         "Documents": DocumentClassifierDocumentsTypeDef,
         "DocumentReaderConfig": DocumentReaderConfigTypeDef,
     },
     total=False,
 )
 
-DocumentClassifierInputDataConfigOutputTypeDef = TypedDict(
-    "DocumentClassifierInputDataConfigOutputTypeDef",
-    {
-        "DataFormat": DocumentClassifierDataFormatType,
-        "S3Uri": str,
-        "TestS3Uri": str,
-        "LabelDelimiter": str,
-        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
-        "DocumentType": DocumentClassifierDocumentTypeFormatType,
-        "Documents": DocumentClassifierDocumentsTypeDef,
-        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-DocumentReaderConfigUnionTypeDef = Union[
-    DocumentReaderConfigTypeDef, DocumentReaderConfigOutputTypeDef
-]
-_RequiredInputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredInputDataConfigOutputTypeDef",
-    {
-        "S3Uri": str,
-    },
-)
-_OptionalInputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalInputDataConfigOutputTypeDef",
-    {
-        "InputFormat": InputFormatType,
-        "DocumentReaderConfig": DocumentReaderConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class InputDataConfigOutputTypeDef(
-    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
-):
-    pass
-
 ListDocumentClassifierSummariesResponseTypeDef = TypedDict(
     "ListDocumentClassifierSummariesResponseTypeDef",
     {
         "DocumentClassifierSummariesList": List[DocumentClassifierSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2245,52 +2094,21 @@
     {
         "Pages": int,
         "ExtractedCharacters": List[ExtractedCharactersListItemTypeDef],
     },
     total=False,
 )
 
-EntityRecognitionConfigOutputTypeDef = TypedDict(
-    "EntityRecognitionConfigOutputTypeDef",
-    {
-        "EntityTypes": List[EntityTypesListItemTypeDef],
-    },
-)
-
 EntityRecognitionConfigTypeDef = TypedDict(
     "EntityRecognitionConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 
-_RequiredEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredEntityRecognizerInputDataConfigOutputTypeDef",
-    {
-        "EntityTypes": List[EntityTypesListItemTypeDef],
-    },
-)
-_OptionalEntityRecognizerInputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalEntityRecognizerInputDataConfigOutputTypeDef",
-    {
-        "DataFormat": EntityRecognizerDataFormatType,
-        "Documents": EntityRecognizerDocumentsTypeDef,
-        "Annotations": EntityRecognizerAnnotationsTypeDef,
-        "EntityList": EntityRecognizerEntityListTypeDef,
-        "AugmentedManifests": List[AugmentedManifestsListItemOutputTypeDef],
-    },
-    total=False,
-)
-
-class EntityRecognizerInputDataConfigOutputTypeDef(
-    _RequiredEntityRecognizerInputDataConfigOutputTypeDef,
-    _OptionalEntityRecognizerInputDataConfigOutputTypeDef,
-):
-    pass
-
 _RequiredEntityRecognizerInputDataConfigTypeDef = TypedDict(
     "_RequiredEntityRecognizerInputDataConfigTypeDef",
     {
         "EntityTypes": Sequence[EntityTypesListItemTypeDef],
     },
 )
 _OptionalEntityRecognizerInputDataConfigTypeDef = TypedDict(
@@ -2373,15 +2191,14 @@
         "BeginOffset": int,
         "EndOffset": int,
         "PartOfSpeech": PartOfSpeechTagTypeDef,
     },
     total=False,
 )
 
-RedactionConfigUnionTypeDef = Union[RedactionConfigTypeDef, RedactionConfigOutputTypeDef]
 BatchDetectDominantLanguageResponseTypeDef = TypedDict(
     "BatchDetectDominantLanguageResponseTypeDef",
     {
         "ResultList": List[BatchDetectDominantLanguageItemResultTypeDef],
         "ErrorList": List[BatchItemErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2428,14 +2245,155 @@
         "BeginOffset": int,
         "EndOffset": int,
         "BlockReferences": List[BlockReferenceTypeDef],
     },
     total=False,
 )
 
+DocumentClassificationJobPropertiesTypeDef = TypedDict(
+    "DocumentClassificationJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "DocumentClassifierArn": str,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
+    "DominantLanguageDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
+EntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "EntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "EntityRecognizerArn": str,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+        "FlywheelArn": str,
+    },
+    total=False,
+)
+
+EventsDetectionJobPropertiesTypeDef = TypedDict(
+    "EventsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "TargetEventTypes": List[str],
+    },
+    total=False,
+)
+
+KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
+    "KeyPhrasesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
+PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
+    "PiiEntitiesDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": PiiOutputDataConfigTypeDef,
+        "RedactionConfig": RedactionConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "Mode": PiiEntitiesDetectionModeType,
+    },
+    total=False,
+)
+
+SentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "SentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStartDocumentClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredStartDocumentClassificationJobRequestRequestTypeDef",
     {
         "InputDataConfig": InputDataConfigTypeDef,
         "OutputDataConfig": OutputDataConfigTypeDef,
         "DataAccessRoleArn": str,
     },
@@ -2672,14 +2630,54 @@
 
 class StartTopicsDetectionJobRequestRequestTypeDef(
     _RequiredStartTopicsDetectionJobRequestRequestTypeDef,
     _OptionalStartTopicsDetectionJobRequestRequestTypeDef,
 ):
     pass
 
+TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
+    "TargetedSentimentDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
+TopicsDetectionJobPropertiesTypeDef = TypedDict(
+    "TopicsDetectionJobPropertiesTypeDef",
+    {
+        "JobId": str,
+        "JobArn": str,
+        "JobName": str,
+        "JobStatus": JobStatusType,
+        "Message": str,
+        "SubmitTime": datetime,
+        "EndTime": datetime,
+        "InputDataConfig": InputDataConfigTypeDef,
+        "OutputDataConfig": OutputDataConfigTypeDef,
+        "NumberOfTopics": int,
+        "DataAccessRoleArn": str,
+        "VolumeKmsKeyId": str,
+        "VpcConfig": VpcConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlywheelRequestRequestTypeDef",
     {
         "FlywheelArn": str,
     },
 )
 _OptionalUpdateFlywheelRequestRequestTypeDef = TypedDict(
@@ -2693,15 +2691,14 @@
 )
 
 class UpdateFlywheelRequestRequestTypeDef(
     _RequiredUpdateFlywheelRequestRequestTypeDef, _OptionalUpdateFlywheelRequestRequestTypeDef
 ):
     pass
 
-DataSecurityConfigUnionTypeDef = Union[DataSecurityConfigTypeDef, DataSecurityConfigOutputTypeDef]
 DatasetInputDataConfigTypeDef = TypedDict(
     "DatasetInputDataConfigTypeDef",
     {
         "AugmentedManifests": Sequence[DatasetAugmentedManifestsListItemTypeDef],
         "DataFormat": DatasetDataFormatType,
         "DocumentClassifierInputDataConfig": DatasetDocumentClassifierInputDataConfigTypeDef,
         "EntityRecognizerInputDataConfig": DatasetEntityRecognizerInputDataConfigTypeDef,
@@ -2991,256 +2988,53 @@
 
 class CreateDocumentClassifierRequestRequestTypeDef(
     _RequiredCreateDocumentClassifierRequestRequestTypeDef,
     _OptionalCreateDocumentClassifierRequestRequestTypeDef,
 ):
     pass
 
-DocumentClassifierInputDataConfigUnionTypeDef = Union[
-    DocumentClassifierInputDataConfigTypeDef, DocumentClassifierInputDataConfigOutputTypeDef
-]
 DocumentClassifierPropertiesTypeDef = TypedDict(
     "DocumentClassifierPropertiesTypeDef",
     {
         "DocumentClassifierArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": DocumentClassifierInputDataConfigOutputTypeDef,
+        "InputDataConfig": DocumentClassifierInputDataConfigTypeDef,
         "OutputDataConfig": DocumentClassifierOutputDataConfigTypeDef,
         "ClassifierMetadata": ClassifierMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "Mode": DocumentClassifierModeType,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
     },
     total=False,
 )
 
-DocumentClassificationJobPropertiesTypeDef = TypedDict(
-    "DocumentClassificationJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "DocumentClassifierArn": str,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-DominantLanguageDetectionJobPropertiesTypeDef = TypedDict(
-    "DominantLanguageDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-EntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "EntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "EntityRecognizerArn": str,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-        "FlywheelArn": str,
-    },
-    total=False,
-)
-
-EventsDetectionJobPropertiesTypeDef = TypedDict(
-    "EventsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "TargetEventTypes": List[str],
-    },
-    total=False,
-)
-
-InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
-KeyPhrasesDetectionJobPropertiesTypeDef = TypedDict(
-    "KeyPhrasesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-PiiEntitiesDetectionJobPropertiesTypeDef = TypedDict(
-    "PiiEntitiesDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": PiiOutputDataConfigTypeDef,
-        "RedactionConfig": RedactionConfigOutputTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "Mode": PiiEntitiesDetectionModeType,
-    },
-    total=False,
-)
-
-SentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "SentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-TargetedSentimentDetectionJobPropertiesTypeDef = TypedDict(
-    "TargetedSentimentDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-TopicsDetectionJobPropertiesTypeDef = TypedDict(
-    "TopicsDetectionJobPropertiesTypeDef",
-    {
-        "JobId": str,
-        "JobArn": str,
-        "JobName": str,
-        "JobStatus": JobStatusType,
-        "Message": str,
-        "SubmitTime": datetime,
-        "EndTime": datetime,
-        "InputDataConfig": InputDataConfigOutputTypeDef,
-        "OutputDataConfig": OutputDataConfigTypeDef,
-        "NumberOfTopics": int,
-        "DataAccessRoleArn": str,
-        "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 ClassifyDocumentResponseTypeDef = TypedDict(
     "ClassifyDocumentResponseTypeDef",
     {
         "Classes": List[DocumentClassTypeDef],
         "Labels": List[DocumentLabelTypeDef],
         "DocumentMetadata": DocumentMetadataTypeDef,
         "DocumentType": List[DocumentTypeListItemTypeDef],
         "Errors": List[ErrorsListItemTypeDef],
         "Warnings": List[WarningsListItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredTaskConfigOutputTypeDef = TypedDict(
-    "_RequiredTaskConfigOutputTypeDef",
-    {
-        "LanguageCode": LanguageCodeType,
-    },
-)
-_OptionalTaskConfigOutputTypeDef = TypedDict(
-    "_OptionalTaskConfigOutputTypeDef",
-    {
-        "DocumentClassificationConfig": DocumentClassificationConfigOutputTypeDef,
-        "EntityRecognitionConfig": EntityRecognitionConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class TaskConfigOutputTypeDef(_RequiredTaskConfigOutputTypeDef, _OptionalTaskConfigOutputTypeDef):
-    pass
-
 _RequiredTaskConfigTypeDef = TypedDict(
     "_RequiredTaskConfigTypeDef",
     {
         "LanguageCode": LanguageCodeType,
     },
 )
 _OptionalTaskConfigTypeDef = TypedDict(
@@ -3280,17 +3074,14 @@
 
 class CreateEntityRecognizerRequestRequestTypeDef(
     _RequiredCreateEntityRecognizerRequestRequestTypeDef,
     _OptionalCreateEntityRecognizerRequestRequestTypeDef,
 ):
     pass
 
-EntityRecognizerInputDataConfigUnionTypeDef = Union[
-    EntityRecognizerInputDataConfigTypeDef, EntityRecognizerInputDataConfigOutputTypeDef
-]
 EntityRecognizerMetadataTypeDef = TypedDict(
     "EntityRecognizerMetadataTypeDef",
     {
         "NumberOfTrainedDocuments": int,
         "NumberOfTestDocuments": int,
         "EvaluationMetrics": EntityRecognizerEvaluationMetricsTypeDef,
         "EntityTypes": List[EntityRecognizerMetadataEntityTypesListItemTypeDef],
@@ -3359,55 +3150,14 @@
     {
         "Index": int,
         "Entities": List[EntityTypeDef],
     },
     total=False,
 )
 
-_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatasetRequestRequestTypeDef",
-    {
-        "FlywheelArn": str,
-        "DatasetName": str,
-        "InputDataConfig": DatasetInputDataConfigTypeDef,
-    },
-)
-_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatasetRequestRequestTypeDef",
-    {
-        "DatasetType": DatasetTypeType,
-        "Description": str,
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateDatasetRequestRequestTypeDef(
-    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
-):
-    pass
-
-DescribeDocumentClassifierResponseTypeDef = TypedDict(
-    "DescribeDocumentClassifierResponseTypeDef",
-    {
-        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDocumentClassifiersResponseTypeDef = TypedDict(
-    "ListDocumentClassifiersResponseTypeDef",
-    {
-        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeDocumentClassificationJobResponseTypeDef = TypedDict(
     "DescribeDocumentClassificationJobResponseTypeDef",
     {
         "DocumentClassificationJobProperties": DocumentClassificationJobPropertiesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3557,33 +3307,55 @@
     {
         "TopicsDetectionJobPropertiesList": List[TopicsDetectionJobPropertiesTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FlywheelPropertiesTypeDef = TypedDict(
-    "FlywheelPropertiesTypeDef",
+_RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "FlywheelArn": str,
-        "ActiveModelArn": str,
-        "DataAccessRoleArn": str,
-        "TaskConfig": TaskConfigOutputTypeDef,
-        "DataLakeS3Uri": str,
-        "DataSecurityConfig": DataSecurityConfigOutputTypeDef,
-        "Status": FlywheelStatusType,
-        "ModelType": ModelTypeType,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "LatestFlywheelIteration": str,
+        "DatasetName": str,
+        "InputDataConfig": DatasetInputDataConfigTypeDef,
+    },
+)
+_OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatasetRequestRequestTypeDef",
+    {
+        "DatasetType": DatasetTypeType,
+        "Description": str,
+        "ClientRequestToken": str,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+class CreateDatasetRequestRequestTypeDef(
+    _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
+):
+    pass
+
+DescribeDocumentClassifierResponseTypeDef = TypedDict(
+    "DescribeDocumentClassifierResponseTypeDef",
+    {
+        "DocumentClassifierProperties": DocumentClassifierPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDocumentClassifiersResponseTypeDef = TypedDict(
+    "ListDocumentClassifiersResponseTypeDef",
+    {
+        "DocumentClassifierPropertiesList": List[DocumentClassifierPropertiesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFlywheelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlywheelRequestRequestTypeDef",
     {
         "FlywheelName": str,
         "DataAccessRoleArn": str,
         "DataLakeS3Uri": str,
     },
@@ -3602,31 +3374,49 @@
 )
 
 class CreateFlywheelRequestRequestTypeDef(
     _RequiredCreateFlywheelRequestRequestTypeDef, _OptionalCreateFlywheelRequestRequestTypeDef
 ):
     pass
 
-TaskConfigUnionTypeDef = Union[TaskConfigTypeDef, TaskConfigOutputTypeDef]
+FlywheelPropertiesTypeDef = TypedDict(
+    "FlywheelPropertiesTypeDef",
+    {
+        "FlywheelArn": str,
+        "ActiveModelArn": str,
+        "DataAccessRoleArn": str,
+        "TaskConfig": TaskConfigTypeDef,
+        "DataLakeS3Uri": str,
+        "DataSecurityConfig": DataSecurityConfigTypeDef,
+        "Status": FlywheelStatusType,
+        "ModelType": ModelTypeType,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "LatestFlywheelIteration": str,
+    },
+    total=False,
+)
+
 EntityRecognizerPropertiesTypeDef = TypedDict(
     "EntityRecognizerPropertiesTypeDef",
     {
         "EntityRecognizerArn": str,
         "LanguageCode": LanguageCodeType,
         "Status": ModelStatusType,
         "Message": str,
         "SubmitTime": datetime,
         "EndTime": datetime,
         "TrainingStartTime": datetime,
         "TrainingEndTime": datetime,
-        "InputDataConfig": EntityRecognizerInputDataConfigOutputTypeDef,
+        "InputDataConfig": EntityRecognizerInputDataConfigTypeDef,
         "RecognizerMetadata": EntityRecognizerMetadataTypeDef,
         "DataAccessRoleArn": str,
         "VolumeKmsKeyId": str,
-        "VpcConfig": VpcConfigOutputTypeDef,
+        "VpcConfig": VpcConfigTypeDef,
         "ModelKmsKeyId": str,
         "VersionName": str,
         "SourceModelArn": str,
         "FlywheelArn": str,
         "OutputDataConfig": EntityRecognizerOutputDataConfigTypeDef,
     },
     total=False,
```

### Comparing `types-aiobotocore-comprehend-2.5.2.post1/types_aiobotocore_comprehend.egg-info/SOURCES.txt` & `types-aiobotocore-comprehend-2.5.2.post2/types_aiobotocore_comprehend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

