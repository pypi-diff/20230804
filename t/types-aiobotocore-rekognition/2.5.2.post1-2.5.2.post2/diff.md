# Comparing `tmp/types-aiobotocore-rekognition-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-rekognition-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rekognition-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-rekognition-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
```

## Comparing `types-aiobotocore-rekognition-2.5.2.post1.tar` & `types-aiobotocore-rekognition-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.393483 types-aiobotocore-rekognition-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27180 2023-08-02 14:52:52.393483 types-aiobotocore-rekognition-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25646 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.393483 types-aiobotocore-rekognition-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.385483 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60562 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    60470 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-08-02 14:47:47.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    98991 2023-08-02 14:47:48.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98870 2023-08-02 14:47:47.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-08-02 14:47:46.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.393483 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27180 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:52.000000 types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-rekognition-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15268 2023-08-04 13:59:22.906643 types-aiobotocore-rekognition-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13734 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.906643 types-aiobotocore-rekognition-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2859 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2858 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    60517 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    60425 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14856 2023-08-04 13:50:35.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14854 2023-08-04 13:50:35.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11430 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11419 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    97024 2023-08-04 13:50:40.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    96905 2023-08-04 13:50:36.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3088 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3086 2023-08-04 13:50:34.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.906643 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15268 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      970 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:22.000000 types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/LICENSE` & `types-aiobotocore-rekognition-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/setup.py` & `types-aiobotocore-rekognition-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rekognition",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Rekognition 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__init__.py` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__init__.pyi` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/__main__.py` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Rekognition 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Rekognition 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
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

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/client.py` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
-    RegionOfInterestUnionTypeDef,
+    RegionOfInterestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
@@ -127,17 +127,17 @@
     StreamProcessingStartSelectorTypeDef,
     StreamProcessingStopSelectorTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorInputTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     StreamProcessorOutputTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
-    StreamProcessorSettingsUnionTypeDef,
-    TestingDataUnionTypeDef,
-    TrainingDataUnionTypeDef,
+    StreamProcessorSettingsTypeDef,
+    TestingDataTypeDef,
+    TrainingDataTypeDef,
     VideoTypeDef,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -313,16 +313,16 @@
 
     async def create_project_version(
         self,
         *,
         ProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
-        TrainingData: TrainingDataUnionTypeDef = ...,
-        TestingData: TestingDataUnionTypeDef = ...,
+        TrainingData: TrainingDataTypeDef = ...,
+        TestingData: TestingDataTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of a model and begins training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
@@ -331,20 +331,20 @@
 
     async def create_stream_processor(
         self,
         *,
         Input: StreamProcessorInputTypeDef,
         Output: StreamProcessorOutputTypeDef,
         Name: str,
-        Settings: StreamProcessorSettingsUnionTypeDef,
+        Settings: StreamProcessorSettingsTypeDef,
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
-        RegionsOfInterest: Sequence[RegionOfInterestUnionTypeDef] = ...,
+        RegionsOfInterest: Sequence[RegionOfInterestTypeDef] = ...,
         DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
@@ -1142,15 +1142,15 @@
         """
 
     async def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
-        RegionsOfInterestForUpdate: Sequence[RegionOfInterestUnionTypeDef] = ...,
+        RegionsOfInterestForUpdate: Sequence[RegionOfInterestTypeDef] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
         ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
```

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/client.pyi` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     NotificationChannelTypeDef,
     OutputConfigTypeDef,
     ProtectiveEquipmentSummarizationAttributesTypeDef,
     PutProjectPolicyResponseTypeDef,
     RecognizeCelebritiesResponseTypeDef,
-    RegionOfInterestUnionTypeDef,
+    RegionOfInterestTypeDef,
     SearchFacesByImageResponseTypeDef,
     SearchFacesResponseTypeDef,
     SearchUsersByImageResponseTypeDef,
     SearchUsersResponseTypeDef,
     StartCelebrityRecognitionResponseTypeDef,
     StartContentModerationResponseTypeDef,
     StartFaceDetectionResponseTypeDef,
@@ -127,17 +127,17 @@
     StreamProcessingStartSelectorTypeDef,
     StreamProcessingStopSelectorTypeDef,
     StreamProcessorDataSharingPreferenceTypeDef,
     StreamProcessorInputTypeDef,
     StreamProcessorNotificationChannelTypeDef,
     StreamProcessorOutputTypeDef,
     StreamProcessorSettingsForUpdateTypeDef,
-    StreamProcessorSettingsUnionTypeDef,
-    TestingDataUnionTypeDef,
-    TrainingDataUnionTypeDef,
+    StreamProcessorSettingsTypeDef,
+    TestingDataTypeDef,
+    TrainingDataTypeDef,
     VideoTypeDef,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -299,16 +299,16 @@
         """
     async def create_project_version(
         self,
         *,
         ProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
-        TrainingData: TrainingDataUnionTypeDef = ...,
-        TestingData: TestingDataUnionTypeDef = ...,
+        TrainingData: TrainingDataTypeDef = ...,
+        TestingData: TestingDataTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of a model and begins training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
@@ -316,20 +316,20 @@
         """
     async def create_stream_processor(
         self,
         *,
         Input: StreamProcessorInputTypeDef,
         Output: StreamProcessorOutputTypeDef,
         Name: str,
-        Settings: StreamProcessorSettingsUnionTypeDef,
+        Settings: StreamProcessorSettingsTypeDef,
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
-        RegionsOfInterest: Sequence[RegionOfInterestUnionTypeDef] = ...,
+        RegionsOfInterest: Sequence[RegionOfInterestTypeDef] = ...,
         DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
@@ -1063,15 +1063,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#update_dataset_entries)
         """
     async def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
-        RegionsOfInterestForUpdate: Sequence[RegionOfInterestUnionTypeDef] = ...,
+        RegionsOfInterestForUpdate: Sequence[RegionOfInterestTypeDef] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
         ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
```

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/literals.py` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,14 +235,15 @@
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
@@ -338,14 +339,15 @@
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
@@ -424,26 +426,28 @@
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

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/literals.pyi` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -233,14 +233,15 @@
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
@@ -336,14 +337,15 @@
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
@@ -422,26 +424,28 @@
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

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/paginator.py` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/paginator.pyi` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/type_defs.py` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AgeRangeTypeDef",
     "AssociateFacesRequestRequestTypeDef",
     "AssociatedFaceTypeDef",
     "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
@@ -83,15 +82,14 @@
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
-    "ConnectedHomeSettingsOutputTypeDef",
     "ConnectedHomeSettingsTypeDef",
     "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
     "LivenessOutputConfigTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -251,18 +249,16 @@
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
     "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
     "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
-    "StreamProcessorSettingsOutputTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
-    "RegionOfInterestOutputTypeDef",
     "RegionOfInterestTypeDef",
     "HumanLoopConfigTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -306,30 +302,28 @@
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
-    "StreamProcessorSettingsUnionTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
     "DetectTextFiltersTypeDef",
-    "RegionOfInterestUnionTypeDef",
     "StartTextDetectionFiltersTypeDef",
+    "UpdateStreamProcessorRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
     "SearchUsersResponseTypeDef",
+    "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
-    "TestingDataOutputTypeDef",
     "TestingDataTypeDef",
-    "TrainingDataOutputTypeDef",
     "TrainingDataTypeDef",
     "ValidationDataTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
@@ -341,20 +335,16 @@
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
     "DetectTextRequestRequestTypeDef",
-    "CreateStreamProcessorRequestRequestTypeDef",
-    "UpdateStreamProcessorRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
-    "TestingDataUnionTypeDef",
     "CreateProjectVersionRequestRequestTypeDef",
-    "TrainingDataUnionTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
@@ -385,21 +375,19 @@
     {
         "UserMatchThreshold": float,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class AssociateFacesRequestRequestTypeDef(
     _RequiredAssociateFacesRequestRequestTypeDef, _OptionalAssociateFacesRequestRequestTypeDef
 ):
     pass
 
-
 AssociatedFaceTypeDef = TypedDict(
     "AssociatedFaceTypeDef",
     {
         "FaceId": str,
     },
     total=False,
 )
@@ -537,56 +525,33 @@
     {
         "Labels": Sequence[str],
         "MinConfidence": float,
     },
     total=False,
 )
 
-_RequiredConnectedHomeSettingsOutputTypeDef = TypedDict(
-    "_RequiredConnectedHomeSettingsOutputTypeDef",
-    {
-        "Labels": List[str],
-    },
-)
-_OptionalConnectedHomeSettingsOutputTypeDef = TypedDict(
-    "_OptionalConnectedHomeSettingsOutputTypeDef",
-    {
-        "MinConfidence": float,
-    },
-    total=False,
-)
-
-
-class ConnectedHomeSettingsOutputTypeDef(
-    _RequiredConnectedHomeSettingsOutputTypeDef, _OptionalConnectedHomeSettingsOutputTypeDef
-):
-    pass
-
-
 _RequiredConnectedHomeSettingsTypeDef = TypedDict(
     "_RequiredConnectedHomeSettingsTypeDef",
     {
         "Labels": Sequence[str],
     },
 )
 _OptionalConnectedHomeSettingsTypeDef = TypedDict(
     "_OptionalConnectedHomeSettingsTypeDef",
     {
         "MinConfidence": float,
     },
     total=False,
 )
 
-
 class ConnectedHomeSettingsTypeDef(
     _RequiredConnectedHomeSettingsTypeDef, _OptionalConnectedHomeSettingsTypeDef
 ):
     pass
 
-
 ModerationLabelTypeDef = TypedDict(
     "ModerationLabelTypeDef",
     {
         "Confidence": float,
         "Name": str,
         "ParentName": str,
     },
@@ -621,42 +586,38 @@
     "_OptionalCreateCollectionRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredLivenessOutputConfigTypeDef = TypedDict(
     "_RequiredLivenessOutputConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalLivenessOutputConfigTypeDef = TypedDict(
     "_OptionalLivenessOutputConfigTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-
 class LivenessOutputConfigTypeDef(
     _RequiredLivenessOutputConfigTypeDef, _OptionalLivenessOutputConfigTypeDef
 ):
     pass
 
-
 CreateProjectRequestRequestTypeDef = TypedDict(
     "CreateProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 
@@ -685,21 +646,19 @@
     "_OptionalCreateUserRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-
 DatasetStatsTypeDef = TypedDict(
     "DatasetStatsTypeDef",
     {
         "LabeledEntries": int,
         "TotalEntries": int,
         "TotalLabels": int,
         "ErrorEntries": int,
@@ -772,22 +731,20 @@
     "_OptionalDeleteProjectPolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
-
 class DeleteProjectPolicyRequestRequestTypeDef(
     _RequiredDeleteProjectPolicyRequestRequestTypeDef,
     _OptionalDeleteProjectPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 
@@ -816,21 +773,19 @@
     "_OptionalDeleteUserRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DeleteUserRequestRequestTypeDef(
     _RequiredDeleteUserRequestRequestTypeDef, _OptionalDeleteUserRequestRequestTypeDef
 ):
     pass
 
-
 DescribeCollectionRequestRequestTypeDef = TypedDict(
     "DescribeCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
@@ -872,22 +827,20 @@
         "VersionNames": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class DescribeProjectVersionsRequestRequestTypeDef(
     _RequiredDescribeProjectVersionsRequestRequestTypeDef,
     _OptionalDescribeProjectVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeProjectsRequestRequestTypeDef = TypedDict(
     "DescribeProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProjectNames": Sequence[str],
     },
@@ -994,21 +947,19 @@
     "_OptionalDisassociateFacesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
-
 class DisassociateFacesRequestRequestTypeDef(
     _RequiredDisassociateFacesRequestRequestTypeDef, _OptionalDisassociateFacesRequestRequestTypeDef
 ):
     pass
 
-
 DisassociatedFaceTypeDef = TypedDict(
     "DisassociatedFaceTypeDef",
     {
         "FaceId": str,
     },
     total=False,
 )
@@ -1140,22 +1091,20 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": CelebrityRecognitionSortByType,
     },
     total=False,
 )
 
-
 class GetCelebrityRecognitionRequestRequestTypeDef(
     _RequiredGetCelebrityRecognitionRequestRequestTypeDef,
     _OptionalGetCelebrityRecognitionRequestRequestTypeDef,
 ):
     pass
 
-
 VideoMetadataTypeDef = TypedDict(
     "VideoMetadataTypeDef",
     {
         "Codec": str,
         "DurationMillis": int,
         "Format": str,
         "FrameRate": float,
@@ -1188,22 +1137,20 @@
         "NextToken": str,
         "SortBy": ContentModerationSortByType,
         "AggregateBy": ContentModerationAggregateByType,
     },
     total=False,
 )
 
-
 class GetContentModerationRequestRequestTypeDef(
     _RequiredGetContentModerationRequestRequestTypeDef,
     _OptionalGetContentModerationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetFaceDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetFaceDetectionRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetFaceDetectionRequestRequestTypeDef = TypedDict(
@@ -1211,21 +1158,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetFaceDetectionRequestRequestTypeDef(
     _RequiredGetFaceDetectionRequestRequestTypeDef, _OptionalGetFaceDetectionRequestRequestTypeDef
 ):
     pass
 
-
 GetFaceLivenessSessionResultsRequestRequestTypeDef = TypedDict(
     "GetFaceLivenessSessionResultsRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
@@ -1241,21 +1186,19 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": FaceSearchSortByType,
     },
     total=False,
 )
 
-
 class GetFaceSearchRequestRequestTypeDef(
     _RequiredGetFaceSearchRequestRequestTypeDef, _OptionalGetFaceSearchRequestRequestTypeDef
 ):
     pass
 
-
 GetLabelDetectionRequestMetadataTypeDef = TypedDict(
     "GetLabelDetectionRequestMetadataTypeDef",
     {
         "SortBy": LabelDetectionSortByType,
         "AggregateBy": LabelDetectionAggregateByType,
     },
     total=False,
@@ -1274,21 +1217,19 @@
         "NextToken": str,
         "SortBy": LabelDetectionSortByType,
         "AggregateBy": LabelDetectionAggregateByType,
     },
     total=False,
 )
 
-
 class GetLabelDetectionRequestRequestTypeDef(
     _RequiredGetLabelDetectionRequestRequestTypeDef, _OptionalGetLabelDetectionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetPersonTrackingRequestRequestTypeDef = TypedDict(
     "_RequiredGetPersonTrackingRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetPersonTrackingRequestRequestTypeDef = TypedDict(
@@ -1297,21 +1238,19 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": PersonTrackingSortByType,
     },
     total=False,
 )
 
-
 class GetPersonTrackingRequestRequestTypeDef(
     _RequiredGetPersonTrackingRequestRequestTypeDef, _OptionalGetPersonTrackingRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentDetectionRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetSegmentDetectionRequestRequestTypeDef = TypedDict(
@@ -1319,22 +1258,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetSegmentDetectionRequestRequestTypeDef(
     _RequiredGetSegmentDetectionRequestRequestTypeDef,
     _OptionalGetSegmentDetectionRequestRequestTypeDef,
 ):
     pass
 
-
 SegmentTypeInfoTypeDef = TypedDict(
     "SegmentTypeInfoTypeDef",
     {
         "Type": SegmentTypeType,
         "ModelVersion": str,
     },
     total=False,
@@ -1351,21 +1288,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetTextDetectionRequestRequestTypeDef(
     _RequiredGetTextDetectionRequestRequestTypeDef, _OptionalGetTextDetectionRequestRequestTypeDef
 ):
     pass
 
-
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
     total=False,
 )
@@ -1443,22 +1378,20 @@
         "HasErrors": bool,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDatasetLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetLabelsRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetLabelsRequestRequestTypeDef = TypedDict(
@@ -1466,21 +1399,19 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDatasetLabelsRequestRequestTypeDef(
     _RequiredListDatasetLabelsRequestRequestTypeDef, _OptionalListDatasetLabelsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListFacesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListFacesRequestRequestTypeDef = TypedDict(
@@ -1490,21 +1421,19 @@
         "MaxResults": int,
         "UserId": str,
         "FaceIds": Sequence[str],
     },
     total=False,
 )
 
-
 class ListFacesRequestRequestTypeDef(
     _RequiredListFacesRequestRequestTypeDef, _OptionalListFacesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListProjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectPoliciesRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalListProjectPoliciesRequestRequestTypeDef = TypedDict(
@@ -1512,22 +1441,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListProjectPoliciesRequestRequestTypeDef(
     _RequiredListProjectPoliciesRequestRequestTypeDef,
     _OptionalListProjectPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 ProjectPolicyTypeDef = TypedDict(
     "ProjectPolicyTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
         "PolicyRevisionId": str,
         "PolicyDocument": str,
@@ -1573,21 +1500,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
-
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "UserId": str,
         "UserStatus": UserStatusType,
     },
     total=False,
@@ -1622,21 +1547,19 @@
     "_OptionalPutProjectPolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
-
 class PutProjectPolicyRequestRequestTypeDef(
     _RequiredPutProjectPolicyRequestRequestTypeDef, _OptionalPutProjectPolicyRequestRequestTypeDef
 ):
     pass
 
-
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "Bucket": str,
         "KeyPrefix": str,
     },
     total=False,
@@ -1654,21 +1577,19 @@
     {
         "MaxFaces": int,
         "FaceMatchThreshold": float,
     },
     total=False,
 )
 
-
 class SearchFacesRequestRequestTypeDef(
     _RequiredSearchFacesRequestRequestTypeDef, _OptionalSearchFacesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredSearchUsersRequestRequestTypeDef = TypedDict(
     "_RequiredSearchUsersRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalSearchUsersRequestRequestTypeDef = TypedDict(
@@ -1678,21 +1599,19 @@
         "FaceId": str,
         "UserMatchThreshold": float,
         "MaxUsers": int,
     },
     total=False,
 )
 
-
 class SearchUsersRequestRequestTypeDef(
     _RequiredSearchUsersRequestRequestTypeDef, _OptionalSearchUsersRequestRequestTypeDef
 ):
     pass
 
-
 SearchedFaceTypeDef = TypedDict(
     "SearchedFaceTypeDef",
     {
         "FaceId": str,
     },
     total=False,
 )
@@ -1734,22 +1653,20 @@
     "_OptionalStartProjectVersionRequestRequestTypeDef",
     {
         "MaxInferenceUnits": int,
     },
     total=False,
 )
 
-
 class StartProjectVersionRequestRequestTypeDef(
     _RequiredStartProjectVersionRequestRequestTypeDef,
     _OptionalStartProjectVersionRequestRequestTypeDef,
 ):
     pass
 
-
 StartShotDetectionFilterTypeDef = TypedDict(
     "StartShotDetectionFilterTypeDef",
     {
         "MinSegmentConfidence": float,
     },
     total=False,
 )
@@ -2160,22 +2077,20 @@
     {
         "Tags": Mapping[str, str],
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class CopyProjectVersionRequestRequestTypeDef(
     _RequiredCopyProjectVersionRequestRequestTypeDef,
     _OptionalCopyProjectVersionRequestRequestTypeDef,
 ):
     pass
 
-
 EquipmentDetectionTypeDef = TypedDict(
     "EquipmentDetectionTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "Type": ProtectiveEquipmentTypeType,
         "CoversBodyPart": CoversBodyPartTypeDef,
@@ -2245,22 +2160,20 @@
     {
         "VersionNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
     _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
     _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
 ):
     pass
 
-
 DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
     "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
     {
         "ProjectNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2288,44 +2201,40 @@
         "SourceRefContains": str,
         "HasErrors": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
     _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
     "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
     "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
     _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
     "_RequiredListFacesRequestListFacesPaginateTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
@@ -2334,44 +2243,40 @@
         "UserId": str,
         "FaceIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListFacesRequestListFacesPaginateTypeDef(
     _RequiredListFacesRequestListFacesPaginateTypeDef,
     _OptionalListFacesRequestListFacesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
     _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
 ):
     pass
 
-
 ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
     "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2386,22 +2291,20 @@
     "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
@@ -2411,22 +2314,20 @@
         "NextToken": str,
         "MaxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef(
     _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     _OptionalDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
 ):
     pass
 
-
 _RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef = TypedDict(
@@ -2436,22 +2337,20 @@
         "NextToken": str,
         "MaxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef(
     _RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     _OptionalDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
 ):
     pass
 
-
 DetectLabelsImageBackgroundTypeDef = TypedDict(
     "DetectLabelsImageBackgroundTypeDef",
     {
         "Quality": DetectLabelsImageQualityTypeDef,
         "DominantColors": List[DominantColorTypeDef],
     },
     total=False,
@@ -2540,23 +2439,14 @@
         "Confidence": float,
         "FaceOccluded": FaceOccludedTypeDef,
         "EyeDirection": EyeDirectionTypeDef,
     },
     total=False,
 )
 
-StreamProcessorSettingsOutputTypeDef = TypedDict(
-    "StreamProcessorSettingsOutputTypeDef",
-    {
-        "FaceSearch": FaceSearchSettingsTypeDef,
-        "ConnectedHome": ConnectedHomeSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
     {
         "FaceSearch": FaceSearchSettingsTypeDef,
         "ConnectedHome": ConnectedHomeSettingsTypeDef,
     },
     total=False,
@@ -2567,23 +2457,14 @@
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-RegionOfInterestOutputTypeDef = TypedDict(
-    "RegionOfInterestOutputTypeDef",
-    {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Polygon": List[PointTypeDef],
-    },
-    total=False,
-)
-
 RegionOfInterestTypeDef = TypedDict(
     "RegionOfInterestTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": Sequence[PointTypeDef],
     },
     total=False,
@@ -2600,19 +2481,17 @@
     "_OptionalHumanLoopConfigTypeDef",
     {
         "DataAttributes": HumanLoopDataAttributesTypeDef,
     },
     total=False,
 )
 
-
 class HumanLoopConfigTypeDef(_RequiredHumanLoopConfigTypeDef, _OptionalHumanLoopConfigTypeDef):
     pass
 
-
 StreamProcessingStartSelectorTypeDef = TypedDict(
     "StreamProcessingStartSelectorTypeDef",
     {
         "KVSStreamStartSelector": KinesisVideoStreamStartSelectorTypeDef,
     },
     total=False,
 )
@@ -2758,22 +2637,20 @@
         "ClientRequestToken": str,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
-
 class StartCelebrityRecognitionRequestRequestTypeDef(
     _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
     _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
     "_RequiredStartContentModerationRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
@@ -2783,22 +2660,20 @@
         "ClientRequestToken": str,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
-
 class StartContentModerationRequestRequestTypeDef(
     _RequiredStartContentModerationRequestRequestTypeDef,
     _OptionalStartContentModerationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartFaceDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
@@ -2808,22 +2683,20 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "FaceAttributes": FaceAttributesType,
         "JobTag": str,
     },
     total=False,
 )
 
-
 class StartFaceDetectionRequestRequestTypeDef(
     _RequiredStartFaceDetectionRequestRequestTypeDef,
     _OptionalStartFaceDetectionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
     "_RequiredStartFaceSearchRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "CollectionId": str,
     },
 )
@@ -2834,21 +2707,19 @@
         "FaceMatchThreshold": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
-
 class StartFaceSearchRequestRequestTypeDef(
     _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
     "_RequiredStartPersonTrackingRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
@@ -2857,22 +2728,20 @@
         "ClientRequestToken": str,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
-
 class StartPersonTrackingRequestRequestTypeDef(
     _RequiredStartPersonTrackingRequestRequestTypeDef,
     _OptionalStartPersonTrackingRequestRequestTypeDef,
 ):
     pass
 
-
 StartSegmentDetectionFiltersTypeDef = TypedDict(
     "StartSegmentDetectionFiltersTypeDef",
     {
         "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
         "ShotFilter": StartShotDetectionFilterTypeDef,
     },
     total=False,
@@ -2898,21 +2767,19 @@
     {
         "SimilarityThreshold": float,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
-
 class CompareFacesRequestRequestTypeDef(
     _RequiredCompareFacesRequestRequestTypeDef, _OptionalCompareFacesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDetectCustomLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectCustomLabelsRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
         "Image": ImageTypeDef,
     },
 )
@@ -2921,65 +2788,59 @@
     {
         "MaxResults": int,
         "MinConfidence": float,
     },
     total=False,
 )
 
-
 class DetectCustomLabelsRequestRequestTypeDef(
     _RequiredDetectCustomLabelsRequestRequestTypeDef,
     _OptionalDetectCustomLabelsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDetectFacesRequestRequestTypeDef = TypedDict(
     "_RequiredDetectFacesRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectFacesRequestRequestTypeDef = TypedDict(
     "_OptionalDetectFacesRequestRequestTypeDef",
     {
         "Attributes": Sequence[AttributeType],
     },
     total=False,
 )
 
-
 class DetectFacesRequestRequestTypeDef(
     _RequiredDetectFacesRequestRequestTypeDef, _OptionalDetectFacesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_RequiredDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_OptionalDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "SummarizationAttributes": ProtectiveEquipmentSummarizationAttributesTypeDef,
     },
     total=False,
 )
 
-
 class DetectProtectiveEquipmentRequestRequestTypeDef(
     _RequiredDetectProtectiveEquipmentRequestRequestTypeDef,
     _OptionalDetectProtectiveEquipmentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredIndexFacesRequestRequestTypeDef = TypedDict(
     "_RequiredIndexFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
         "Image": ImageTypeDef,
     },
 )
@@ -2990,21 +2851,19 @@
         "DetectionAttributes": Sequence[AttributeType],
         "MaxFaces": int,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
-
 class IndexFacesRequestRequestTypeDef(
     _RequiredIndexFacesRequestRequestTypeDef, _OptionalIndexFacesRequestRequestTypeDef
 ):
     pass
 
-
 RecognizeCelebritiesRequestRequestTypeDef = TypedDict(
     "RecognizeCelebritiesRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 
@@ -3021,22 +2880,20 @@
         "MaxFaces": int,
         "FaceMatchThreshold": float,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
-
 class SearchFacesByImageRequestRequestTypeDef(
     _RequiredSearchFacesByImageRequestRequestTypeDef,
     _OptionalSearchFacesByImageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSearchUsersByImageRequestRequestTypeDef = TypedDict(
     "_RequiredSearchUsersByImageRequestRequestTypeDef",
     {
         "CollectionId": str,
         "Image": ImageTypeDef,
     },
 )
@@ -3046,22 +2903,20 @@
         "UserMatchThreshold": float,
         "MaxUsers": int,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
-
 class SearchUsersByImageRequestRequestTypeDef(
     _RequiredSearchUsersByImageRequestRequestTypeDef,
     _OptionalSearchUsersByImageRequestRequestTypeDef,
 ):
     pass
 
-
 CelebrityTypeDef = TypedDict(
     "CelebrityTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "Id": str,
         "Face": ComparedFaceTypeDef,
@@ -3180,21 +3035,19 @@
         "MinConfidence": float,
         "Features": Sequence[DetectLabelsFeatureNameType],
         "Settings": DetectLabelsSettingsTypeDef,
     },
     total=False,
 )
 
-
 class DetectLabelsRequestRequestTypeDef(
     _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartLabelDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
@@ -3206,22 +3059,20 @@
         "JobTag": str,
         "Features": Sequence[Literal["GENERAL_LABELS"]],
         "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
-
 class StartLabelDetectionRequestRequestTypeDef(
     _RequiredStartLabelDetectionRequestRequestTypeDef,
     _OptionalStartLabelDetectionRequestRequestTypeDef,
 ):
     pass
 
-
 CelebrityDetailTypeDef = TypedDict(
     "CelebrityDetailTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "Id": str,
         "Confidence": float,
@@ -3291,17 +3142,14 @@
     {
         "FaceDetails": FaceDetailTypeDef,
         "Reasons": List[UnsearchedFaceReasonType],
     },
     total=False,
 )
 
-StreamProcessorSettingsUnionTypeDef = Union[
-    StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef
-]
 CustomLabelTypeDef = TypedDict(
     "CustomLabelTypeDef",
     {
         "Name": str,
         "Confidence": float,
         "Geometry": GeometryTypeDef,
     },
@@ -3326,24 +3174,46 @@
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
-RegionOfInterestUnionTypeDef = Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
 StartTextDetectionFiltersTypeDef = TypedDict(
     "StartTextDetectionFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
+        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
+        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
+        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+    },
+    total=False,
+)
+
+class UpdateStreamProcessorRequestRequestTypeDef(
+    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
+    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
 _RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
@@ -3351,22 +3221,20 @@
     {
         "MinConfidence": float,
         "HumanLoopConfig": HumanLoopConfigTypeDef,
     },
     total=False,
 )
 
-
 class DetectModerationLabelsRequestRequestTypeDef(
     _RequiredDetectModerationLabelsRequestRequestTypeDef,
     _OptionalDetectModerationLabelsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
     "_RequiredStartStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
@@ -3374,49 +3242,75 @@
     {
         "StartSelector": StreamProcessingStartSelectorTypeDef,
         "StopSelector": StreamProcessingStopSelectorTypeDef,
     },
     total=False,
 )
 
-
 class StartStreamProcessorRequestRequestTypeDef(
     _RequiredStartStreamProcessorRequestRequestTypeDef,
     _OptionalStartStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
-
 SearchUsersResponseTypeDef = TypedDict(
     "SearchUsersResponseTypeDef",
     {
         "UserMatches": List[UserMatchTypeDef],
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceTypeDef,
         "SearchedUser": SearchedUserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Input": StreamProcessorInputTypeDef,
+        "Output": StreamProcessorOutputTypeDef,
+        "Name": str,
+        "Settings": StreamProcessorSettingsTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
+        "KmsKeyId": str,
+        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
+    },
+    total=False,
+)
+
+class CreateStreamProcessorRequestRequestTypeDef(
+    _RequiredCreateStreamProcessorRequestRequestTypeDef,
+    _OptionalCreateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
 DescribeStreamProcessorResponseTypeDef = TypedDict(
     "DescribeStreamProcessorResponseTypeDef",
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
-        "Settings": StreamProcessorSettingsOutputTypeDef,
+        "Settings": StreamProcessorSettingsTypeDef,
         "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
-        "RegionsOfInterest": List[RegionOfInterestOutputTypeDef],
+        "RegionsOfInterest": List[RegionOfInterestTypeDef],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
@@ -3452,40 +3346,23 @@
         "SearchedFaceId": str,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TestingDataOutputTypeDef = TypedDict(
-    "TestingDataOutputTypeDef",
-    {
-        "Assets": List[AssetTypeDef],
-        "AutoCreate": bool,
-    },
-    total=False,
-)
-
 TestingDataTypeDef = TypedDict(
     "TestingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
         "AutoCreate": bool,
     },
     total=False,
 )
 
-TrainingDataOutputTypeDef = TypedDict(
-    "TrainingDataOutputTypeDef",
-    {
-        "Assets": List[AssetTypeDef],
-    },
-    total=False,
-)
-
 TrainingDataTypeDef = TypedDict(
     "TrainingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
     },
     total=False,
 )
@@ -3509,21 +3386,19 @@
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "DatasetSource": DatasetSourceTypeDef,
     },
     total=False,
 )
 
-
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredStartSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSegmentDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "SegmentTypes": Sequence[SegmentTypeType],
     },
 )
@@ -3534,22 +3409,20 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
         "Filters": StartSegmentDetectionFiltersTypeDef,
     },
     total=False,
 )
 
-
 class StartSegmentDetectionRequestRequestTypeDef(
     _RequiredStartSegmentDetectionRequestRequestTypeDef,
     _OptionalStartSegmentDetectionRequestRequestTypeDef,
 ):
     pass
 
-
 RecognizeCelebritiesResponseTypeDef = TypedDict(
     "RecognizeCelebritiesResponseTypeDef",
     {
         "CelebrityFaces": List[CelebrityTypeDef],
         "UnrecognizedFaces": List[ComparedFaceTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3703,76 +3576,19 @@
     "_OptionalDetectTextRequestRequestTypeDef",
     {
         "Filters": DetectTextFiltersTypeDef,
     },
     total=False,
 )
 
-
 class DetectTextRequestRequestTypeDef(
     _RequiredDetectTextRequestRequestTypeDef, _OptionalDetectTextRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Input": StreamProcessorInputTypeDef,
-        "Output": StreamProcessorOutputTypeDef,
-        "Name": str,
-        "Settings": StreamProcessorSettingsTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
-        "KmsKeyId": str,
-        "RegionsOfInterest": Sequence[RegionOfInterestUnionTypeDef],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateStreamProcessorRequestRequestTypeDef(
-    _RequiredCreateStreamProcessorRequestRequestTypeDef,
-    _OptionalCreateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestUnionTypeDef],
-        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
-        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
-    },
-    total=False,
-)
-
-
-class UpdateStreamProcessorRequestRequestTypeDef(
-    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
-    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredStartTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartTextDetectionRequestRequestTypeDef = TypedDict(
@@ -3782,23 +3598,20 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
         "Filters": StartTextDetectionFiltersTypeDef,
     },
     total=False,
 )
 
-
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
-
-TestingDataUnionTypeDef = Union[TestingDataTypeDef, TestingDataOutputTypeDef]
 _RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectVersionRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "VersionName": str,
         "OutputConfig": OutputConfigTypeDef,
     },
@@ -3810,38 +3623,35 @@
         "TestingData": TestingDataTypeDef,
         "Tags": Mapping[str, str],
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class CreateProjectVersionRequestRequestTypeDef(
     _RequiredCreateProjectVersionRequestRequestTypeDef,
     _OptionalCreateProjectVersionRequestRequestTypeDef,
 ):
     pass
 
-
-TrainingDataUnionTypeDef = Union[TrainingDataTypeDef, TrainingDataOutputTypeDef]
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
-        "Input": TestingDataOutputTypeDef,
-        "Output": TestingDataOutputTypeDef,
+        "Input": TestingDataTypeDef,
+        "Output": TestingDataTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 TrainingDataResultTypeDef = TypedDict(
     "TrainingDataResultTypeDef",
     {
-        "Input": TrainingDataOutputTypeDef,
-        "Output": TrainingDataOutputTypeDef,
+        "Input": TrainingDataTypeDef,
+        "Output": TrainingDataTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 DetectProtectiveEquipmentResponseTypeDef = TypedDict(
     "DetectProtectiveEquipmentResponseTypeDef",
```

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/type_defs.pyi` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AgeRangeTypeDef",
     "AssociateFacesRequestRequestTypeDef",
     "AssociatedFaceTypeDef",
     "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
@@ -82,15 +83,14 @@
     "KnownGenderTypeDef",
     "EmotionTypeDef",
     "ImageQualityTypeDef",
     "LandmarkTypeDef",
     "PoseTypeDef",
     "SmileTypeDef",
     "ConnectedHomeSettingsForUpdateTypeDef",
-    "ConnectedHomeSettingsOutputTypeDef",
     "ConnectedHomeSettingsTypeDef",
     "ModerationLabelTypeDef",
     "OutputConfigTypeDef",
     "CoversBodyPartTypeDef",
     "CreateCollectionRequestRequestTypeDef",
     "LivenessOutputConfigTypeDef",
     "CreateProjectRequestRequestTypeDef",
@@ -250,18 +250,16 @@
     "InstanceTypeDef",
     "DetectLabelsSettingsTypeDef",
     "LabelDetectionSettingsTypeDef",
     "DetectModerationLabelsResponseTypeDef",
     "DisassociateFacesResponseTypeDef",
     "DistributeDatasetEntriesRequestRequestTypeDef",
     "FaceDetailTypeDef",
-    "StreamProcessorSettingsOutputTypeDef",
     "StreamProcessorSettingsTypeDef",
     "GeometryTypeDef",
-    "RegionOfInterestOutputTypeDef",
     "RegionOfInterestTypeDef",
     "HumanLoopConfigTypeDef",
     "StreamProcessingStartSelectorTypeDef",
     "StreamProcessorInputTypeDef",
     "ListProjectPoliciesResponseTypeDef",
     "ListStreamProcessorsResponseTypeDef",
     "ListUsersResponseTypeDef",
@@ -305,30 +303,28 @@
     "DetectFacesResponseTypeDef",
     "FaceDetectionTypeDef",
     "FaceRecordTypeDef",
     "PersonDetailTypeDef",
     "SearchedFaceDetailsTypeDef",
     "UnindexedFaceTypeDef",
     "UnsearchedFaceTypeDef",
-    "StreamProcessorSettingsUnionTypeDef",
     "CustomLabelTypeDef",
     "TextDetectionTypeDef",
     "DetectTextFiltersTypeDef",
-    "RegionOfInterestUnionTypeDef",
     "StartTextDetectionFiltersTypeDef",
+    "UpdateStreamProcessorRequestRequestTypeDef",
     "DetectModerationLabelsRequestRequestTypeDef",
     "StartStreamProcessorRequestRequestTypeDef",
     "SearchUsersResponseTypeDef",
+    "CreateStreamProcessorRequestRequestTypeDef",
     "DescribeStreamProcessorResponseTypeDef",
     "GetSegmentDetectionResponseTypeDef",
     "SearchFacesByImageResponseTypeDef",
     "SearchFacesResponseTypeDef",
-    "TestingDataOutputTypeDef",
     "TestingDataTypeDef",
-    "TrainingDataOutputTypeDef",
     "TrainingDataTypeDef",
     "ValidationDataTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "StartSegmentDetectionRequestRequestTypeDef",
     "RecognizeCelebritiesResponseTypeDef",
     "CompareFacesResponseTypeDef",
     "ProtectiveEquipmentPersonTypeDef",
@@ -340,20 +336,16 @@
     "PersonMatchTypeDef",
     "IndexFacesResponseTypeDef",
     "SearchUsersByImageResponseTypeDef",
     "DetectCustomLabelsResponseTypeDef",
     "DetectTextResponseTypeDef",
     "TextDetectionResultTypeDef",
     "DetectTextRequestRequestTypeDef",
-    "CreateStreamProcessorRequestRequestTypeDef",
-    "UpdateStreamProcessorRequestRequestTypeDef",
     "StartTextDetectionRequestRequestTypeDef",
-    "TestingDataUnionTypeDef",
     "CreateProjectVersionRequestRequestTypeDef",
-    "TrainingDataUnionTypeDef",
     "TestingDataResultTypeDef",
     "TrainingDataResultTypeDef",
     "DetectProtectiveEquipmentResponseTypeDef",
     "GetLabelDetectionResponseTypeDef",
     "GetCelebrityRecognitionResponseTypeDef",
     "GetPersonTrackingResponseTypeDef",
     "GetFaceSearchResponseTypeDef",
@@ -384,19 +376,21 @@
     {
         "UserMatchThreshold": float,
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class AssociateFacesRequestRequestTypeDef(
     _RequiredAssociateFacesRequestRequestTypeDef, _OptionalAssociateFacesRequestRequestTypeDef
 ):
     pass
 
+
 AssociatedFaceTypeDef = TypedDict(
     "AssociatedFaceTypeDef",
     {
         "FaceId": str,
     },
     total=False,
 )
@@ -534,52 +528,35 @@
     {
         "Labels": Sequence[str],
         "MinConfidence": float,
     },
     total=False,
 )
 
-_RequiredConnectedHomeSettingsOutputTypeDef = TypedDict(
-    "_RequiredConnectedHomeSettingsOutputTypeDef",
-    {
-        "Labels": List[str],
-    },
-)
-_OptionalConnectedHomeSettingsOutputTypeDef = TypedDict(
-    "_OptionalConnectedHomeSettingsOutputTypeDef",
-    {
-        "MinConfidence": float,
-    },
-    total=False,
-)
-
-class ConnectedHomeSettingsOutputTypeDef(
-    _RequiredConnectedHomeSettingsOutputTypeDef, _OptionalConnectedHomeSettingsOutputTypeDef
-):
-    pass
-
 _RequiredConnectedHomeSettingsTypeDef = TypedDict(
     "_RequiredConnectedHomeSettingsTypeDef",
     {
         "Labels": Sequence[str],
     },
 )
 _OptionalConnectedHomeSettingsTypeDef = TypedDict(
     "_OptionalConnectedHomeSettingsTypeDef",
     {
         "MinConfidence": float,
     },
     total=False,
 )
 
+
 class ConnectedHomeSettingsTypeDef(
     _RequiredConnectedHomeSettingsTypeDef, _OptionalConnectedHomeSettingsTypeDef
 ):
     pass
 
+
 ModerationLabelTypeDef = TypedDict(
     "ModerationLabelTypeDef",
     {
         "Confidence": float,
         "Name": str,
         "ParentName": str,
     },
@@ -614,38 +591,42 @@
     "_OptionalCreateCollectionRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateCollectionRequestRequestTypeDef(
     _RequiredCreateCollectionRequestRequestTypeDef, _OptionalCreateCollectionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredLivenessOutputConfigTypeDef = TypedDict(
     "_RequiredLivenessOutputConfigTypeDef",
     {
         "S3Bucket": str,
     },
 )
 _OptionalLivenessOutputConfigTypeDef = TypedDict(
     "_OptionalLivenessOutputConfigTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
+
 class LivenessOutputConfigTypeDef(
     _RequiredLivenessOutputConfigTypeDef, _OptionalLivenessOutputConfigTypeDef
 ):
     pass
 
+
 CreateProjectRequestRequestTypeDef = TypedDict(
     "CreateProjectRequestRequestTypeDef",
     {
         "ProjectName": str,
     },
 )
 
@@ -674,19 +655,21 @@
     "_OptionalCreateUserRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
+
 DatasetStatsTypeDef = TypedDict(
     "DatasetStatsTypeDef",
     {
         "LabeledEntries": int,
         "TotalEntries": int,
         "TotalLabels": int,
         "ErrorEntries": int,
@@ -759,20 +742,22 @@
     "_OptionalDeleteProjectPolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
+
 class DeleteProjectPolicyRequestRequestTypeDef(
     _RequiredDeleteProjectPolicyRequestRequestTypeDef,
     _OptionalDeleteProjectPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 
@@ -801,19 +786,21 @@
     "_OptionalDeleteUserRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DeleteUserRequestRequestTypeDef(
     _RequiredDeleteUserRequestRequestTypeDef, _OptionalDeleteUserRequestRequestTypeDef
 ):
     pass
 
+
 DescribeCollectionRequestRequestTypeDef = TypedDict(
     "DescribeCollectionRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 
@@ -855,20 +842,22 @@
         "VersionNames": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class DescribeProjectVersionsRequestRequestTypeDef(
     _RequiredDescribeProjectVersionsRequestRequestTypeDef,
     _OptionalDescribeProjectVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeProjectsRequestRequestTypeDef = TypedDict(
     "DescribeProjectsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ProjectNames": Sequence[str],
     },
@@ -975,19 +964,21 @@
     "_OptionalDisassociateFacesRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
     },
     total=False,
 )
 
+
 class DisassociateFacesRequestRequestTypeDef(
     _RequiredDisassociateFacesRequestRequestTypeDef, _OptionalDisassociateFacesRequestRequestTypeDef
 ):
     pass
 
+
 DisassociatedFaceTypeDef = TypedDict(
     "DisassociatedFaceTypeDef",
     {
         "FaceId": str,
     },
     total=False,
 )
@@ -1119,20 +1110,22 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": CelebrityRecognitionSortByType,
     },
     total=False,
 )
 
+
 class GetCelebrityRecognitionRequestRequestTypeDef(
     _RequiredGetCelebrityRecognitionRequestRequestTypeDef,
     _OptionalGetCelebrityRecognitionRequestRequestTypeDef,
 ):
     pass
 
+
 VideoMetadataTypeDef = TypedDict(
     "VideoMetadataTypeDef",
     {
         "Codec": str,
         "DurationMillis": int,
         "Format": str,
         "FrameRate": float,
@@ -1165,20 +1158,22 @@
         "NextToken": str,
         "SortBy": ContentModerationSortByType,
         "AggregateBy": ContentModerationAggregateByType,
     },
     total=False,
 )
 
+
 class GetContentModerationRequestRequestTypeDef(
     _RequiredGetContentModerationRequestRequestTypeDef,
     _OptionalGetContentModerationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetFaceDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetFaceDetectionRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetFaceDetectionRequestRequestTypeDef = TypedDict(
@@ -1186,19 +1181,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetFaceDetectionRequestRequestTypeDef(
     _RequiredGetFaceDetectionRequestRequestTypeDef, _OptionalGetFaceDetectionRequestRequestTypeDef
 ):
     pass
 
+
 GetFaceLivenessSessionResultsRequestRequestTypeDef = TypedDict(
     "GetFaceLivenessSessionResultsRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
@@ -1214,19 +1211,21 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": FaceSearchSortByType,
     },
     total=False,
 )
 
+
 class GetFaceSearchRequestRequestTypeDef(
     _RequiredGetFaceSearchRequestRequestTypeDef, _OptionalGetFaceSearchRequestRequestTypeDef
 ):
     pass
 
+
 GetLabelDetectionRequestMetadataTypeDef = TypedDict(
     "GetLabelDetectionRequestMetadataTypeDef",
     {
         "SortBy": LabelDetectionSortByType,
         "AggregateBy": LabelDetectionAggregateByType,
     },
     total=False,
@@ -1245,19 +1244,21 @@
         "NextToken": str,
         "SortBy": LabelDetectionSortByType,
         "AggregateBy": LabelDetectionAggregateByType,
     },
     total=False,
 )
 
+
 class GetLabelDetectionRequestRequestTypeDef(
     _RequiredGetLabelDetectionRequestRequestTypeDef, _OptionalGetLabelDetectionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetPersonTrackingRequestRequestTypeDef = TypedDict(
     "_RequiredGetPersonTrackingRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetPersonTrackingRequestRequestTypeDef = TypedDict(
@@ -1266,19 +1267,21 @@
         "MaxResults": int,
         "NextToken": str,
         "SortBy": PersonTrackingSortByType,
     },
     total=False,
 )
 
+
 class GetPersonTrackingRequestRequestTypeDef(
     _RequiredGetPersonTrackingRequestRequestTypeDef, _OptionalGetPersonTrackingRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSegmentDetectionRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetSegmentDetectionRequestRequestTypeDef = TypedDict(
@@ -1286,20 +1289,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetSegmentDetectionRequestRequestTypeDef(
     _RequiredGetSegmentDetectionRequestRequestTypeDef,
     _OptionalGetSegmentDetectionRequestRequestTypeDef,
 ):
     pass
 
+
 SegmentTypeInfoTypeDef = TypedDict(
     "SegmentTypeInfoTypeDef",
     {
         "Type": SegmentTypeType,
         "ModelVersion": str,
     },
     total=False,
@@ -1316,19 +1321,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetTextDetectionRequestRequestTypeDef(
     _RequiredGetTextDetectionRequestRequestTypeDef, _OptionalGetTextDetectionRequestRequestTypeDef
 ):
     pass
 
+
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
     total=False,
 )
@@ -1406,20 +1413,22 @@
         "HasErrors": bool,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDatasetEntriesRequestRequestTypeDef(
     _RequiredListDatasetEntriesRequestRequestTypeDef,
     _OptionalListDatasetEntriesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDatasetLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredListDatasetLabelsRequestRequestTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetLabelsRequestRequestTypeDef = TypedDict(
@@ -1427,19 +1436,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDatasetLabelsRequestRequestTypeDef(
     _RequiredListDatasetLabelsRequestRequestTypeDef, _OptionalListDatasetLabelsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListFacesRequestRequestTypeDef = TypedDict(
     "_RequiredListFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListFacesRequestRequestTypeDef = TypedDict(
@@ -1449,19 +1460,21 @@
         "MaxResults": int,
         "UserId": str,
         "FaceIds": Sequence[str],
     },
     total=False,
 )
 
+
 class ListFacesRequestRequestTypeDef(
     _RequiredListFacesRequestRequestTypeDef, _OptionalListFacesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListProjectPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListProjectPoliciesRequestRequestTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalListProjectPoliciesRequestRequestTypeDef = TypedDict(
@@ -1469,20 +1482,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListProjectPoliciesRequestRequestTypeDef(
     _RequiredListProjectPoliciesRequestRequestTypeDef,
     _OptionalListProjectPoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 ProjectPolicyTypeDef = TypedDict(
     "ProjectPolicyTypeDef",
     {
         "ProjectArn": str,
         "PolicyName": str,
         "PolicyRevisionId": str,
         "PolicyDocument": str,
@@ -1528,19 +1543,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListUsersRequestRequestTypeDef(
     _RequiredListUsersRequestRequestTypeDef, _OptionalListUsersRequestRequestTypeDef
 ):
     pass
 
+
 UserTypeDef = TypedDict(
     "UserTypeDef",
     {
         "UserId": str,
         "UserStatus": UserStatusType,
     },
     total=False,
@@ -1575,19 +1592,21 @@
     "_OptionalPutProjectPolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
+
 class PutProjectPolicyRequestRequestTypeDef(
     _RequiredPutProjectPolicyRequestRequestTypeDef, _OptionalPutProjectPolicyRequestRequestTypeDef
 ):
     pass
 
+
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "Bucket": str,
         "KeyPrefix": str,
     },
     total=False,
@@ -1605,19 +1624,21 @@
     {
         "MaxFaces": int,
         "FaceMatchThreshold": float,
     },
     total=False,
 )
 
+
 class SearchFacesRequestRequestTypeDef(
     _RequiredSearchFacesRequestRequestTypeDef, _OptionalSearchFacesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredSearchUsersRequestRequestTypeDef = TypedDict(
     "_RequiredSearchUsersRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalSearchUsersRequestRequestTypeDef = TypedDict(
@@ -1627,19 +1648,21 @@
         "FaceId": str,
         "UserMatchThreshold": float,
         "MaxUsers": int,
     },
     total=False,
 )
 
+
 class SearchUsersRequestRequestTypeDef(
     _RequiredSearchUsersRequestRequestTypeDef, _OptionalSearchUsersRequestRequestTypeDef
 ):
     pass
 
+
 SearchedFaceTypeDef = TypedDict(
     "SearchedFaceTypeDef",
     {
         "FaceId": str,
     },
     total=False,
 )
@@ -1681,20 +1704,22 @@
     "_OptionalStartProjectVersionRequestRequestTypeDef",
     {
         "MaxInferenceUnits": int,
     },
     total=False,
 )
 
+
 class StartProjectVersionRequestRequestTypeDef(
     _RequiredStartProjectVersionRequestRequestTypeDef,
     _OptionalStartProjectVersionRequestRequestTypeDef,
 ):
     pass
 
+
 StartShotDetectionFilterTypeDef = TypedDict(
     "StartShotDetectionFilterTypeDef",
     {
         "MinSegmentConfidence": float,
     },
     total=False,
 )
@@ -2105,20 +2130,22 @@
     {
         "Tags": Mapping[str, str],
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class CopyProjectVersionRequestRequestTypeDef(
     _RequiredCopyProjectVersionRequestRequestTypeDef,
     _OptionalCopyProjectVersionRequestRequestTypeDef,
 ):
     pass
 
+
 EquipmentDetectionTypeDef = TypedDict(
     "EquipmentDetectionTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Confidence": float,
         "Type": ProtectiveEquipmentTypeType,
         "CoversBodyPart": CoversBodyPartTypeDef,
@@ -2188,20 +2215,22 @@
     {
         "VersionNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef(
     _RequiredDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
     _OptionalDescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef,
 ):
     pass
 
+
 DescribeProjectsRequestDescribeProjectsPaginateTypeDef = TypedDict(
     "DescribeProjectsRequestDescribeProjectsPaginateTypeDef",
     {
         "ProjectNames": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -2229,40 +2258,44 @@
         "SourceRefContains": str,
         "HasErrors": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef(
     _RequiredListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
     _OptionalListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
     "_RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
     {
         "DatasetArn": str,
     },
 )
 _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = TypedDict(
     "_OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef(
     _RequiredListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
     _OptionalListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListFacesRequestListFacesPaginateTypeDef = TypedDict(
     "_RequiredListFacesRequestListFacesPaginateTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListFacesRequestListFacesPaginateTypeDef = TypedDict(
@@ -2271,40 +2304,44 @@
         "UserId": str,
         "FaceIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListFacesRequestListFacesPaginateTypeDef(
     _RequiredListFacesRequestListFacesPaginateTypeDef,
     _OptionalListFacesRequestListFacesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
     "_RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef(
     _RequiredListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
     _OptionalListProjectPoliciesRequestListProjectPoliciesPaginateTypeDef,
 ):
     pass
 
+
 ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = TypedDict(
     "ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -2319,20 +2356,22 @@
     "_OptionalListUsersRequestListUsersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListUsersRequestListUsersPaginateTypeDef(
     _RequiredListUsersRequestListUsersPaginateTypeDef,
     _OptionalListUsersRequestListUsersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef = TypedDict(
@@ -2342,20 +2381,22 @@
         "NextToken": str,
         "MaxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef(
     _RequiredDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
     _OptionalDescribeProjectVersionsRequestProjectVersionRunningWaitTypeDef,
 ):
     pass
 
+
 _RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef = TypedDict(
     "_RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef",
     {
         "ProjectArn": str,
     },
 )
 _OptionalDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef = TypedDict(
@@ -2365,20 +2406,22 @@
         "NextToken": str,
         "MaxResults": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef(
     _RequiredDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
     _OptionalDescribeProjectVersionsRequestProjectVersionTrainingCompletedWaitTypeDef,
 ):
     pass
 
+
 DetectLabelsImageBackgroundTypeDef = TypedDict(
     "DetectLabelsImageBackgroundTypeDef",
     {
         "Quality": DetectLabelsImageQualityTypeDef,
         "DominantColors": List[DominantColorTypeDef],
     },
     total=False,
@@ -2467,23 +2510,14 @@
         "Confidence": float,
         "FaceOccluded": FaceOccludedTypeDef,
         "EyeDirection": EyeDirectionTypeDef,
     },
     total=False,
 )
 
-StreamProcessorSettingsOutputTypeDef = TypedDict(
-    "StreamProcessorSettingsOutputTypeDef",
-    {
-        "FaceSearch": FaceSearchSettingsTypeDef,
-        "ConnectedHome": ConnectedHomeSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 StreamProcessorSettingsTypeDef = TypedDict(
     "StreamProcessorSettingsTypeDef",
     {
         "FaceSearch": FaceSearchSettingsTypeDef,
         "ConnectedHome": ConnectedHomeSettingsTypeDef,
     },
     total=False,
@@ -2494,23 +2528,14 @@
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": List[PointTypeDef],
     },
     total=False,
 )
 
-RegionOfInterestOutputTypeDef = TypedDict(
-    "RegionOfInterestOutputTypeDef",
-    {
-        "BoundingBox": BoundingBoxTypeDef,
-        "Polygon": List[PointTypeDef],
-    },
-    total=False,
-)
-
 RegionOfInterestTypeDef = TypedDict(
     "RegionOfInterestTypeDef",
     {
         "BoundingBox": BoundingBoxTypeDef,
         "Polygon": Sequence[PointTypeDef],
     },
     total=False,
@@ -2527,17 +2552,19 @@
     "_OptionalHumanLoopConfigTypeDef",
     {
         "DataAttributes": HumanLoopDataAttributesTypeDef,
     },
     total=False,
 )
 
+
 class HumanLoopConfigTypeDef(_RequiredHumanLoopConfigTypeDef, _OptionalHumanLoopConfigTypeDef):
     pass
 
+
 StreamProcessingStartSelectorTypeDef = TypedDict(
     "StreamProcessingStartSelectorTypeDef",
     {
         "KVSStreamStartSelector": KinesisVideoStreamStartSelectorTypeDef,
     },
     total=False,
 )
@@ -2683,20 +2710,22 @@
         "ClientRequestToken": str,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
+
 class StartCelebrityRecognitionRequestRequestTypeDef(
     _RequiredStartCelebrityRecognitionRequestRequestTypeDef,
     _OptionalStartCelebrityRecognitionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartContentModerationRequestRequestTypeDef = TypedDict(
     "_RequiredStartContentModerationRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartContentModerationRequestRequestTypeDef = TypedDict(
@@ -2706,20 +2735,22 @@
         "ClientRequestToken": str,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
+
 class StartContentModerationRequestRequestTypeDef(
     _RequiredStartContentModerationRequestRequestTypeDef,
     _OptionalStartContentModerationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartFaceDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartFaceDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartFaceDetectionRequestRequestTypeDef = TypedDict(
@@ -2729,20 +2760,22 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "FaceAttributes": FaceAttributesType,
         "JobTag": str,
     },
     total=False,
 )
 
+
 class StartFaceDetectionRequestRequestTypeDef(
     _RequiredStartFaceDetectionRequestRequestTypeDef,
     _OptionalStartFaceDetectionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartFaceSearchRequestRequestTypeDef = TypedDict(
     "_RequiredStartFaceSearchRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "CollectionId": str,
     },
 )
@@ -2753,19 +2786,21 @@
         "FaceMatchThreshold": float,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
+
 class StartFaceSearchRequestRequestTypeDef(
     _RequiredStartFaceSearchRequestRequestTypeDef, _OptionalStartFaceSearchRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStartPersonTrackingRequestRequestTypeDef = TypedDict(
     "_RequiredStartPersonTrackingRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartPersonTrackingRequestRequestTypeDef = TypedDict(
@@ -2774,20 +2809,22 @@
         "ClientRequestToken": str,
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
     },
     total=False,
 )
 
+
 class StartPersonTrackingRequestRequestTypeDef(
     _RequiredStartPersonTrackingRequestRequestTypeDef,
     _OptionalStartPersonTrackingRequestRequestTypeDef,
 ):
     pass
 
+
 StartSegmentDetectionFiltersTypeDef = TypedDict(
     "StartSegmentDetectionFiltersTypeDef",
     {
         "TechnicalCueFilter": StartTechnicalCueDetectionFilterTypeDef,
         "ShotFilter": StartShotDetectionFilterTypeDef,
     },
     total=False,
@@ -2813,19 +2850,21 @@
     {
         "SimilarityThreshold": float,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
+
 class CompareFacesRequestRequestTypeDef(
     _RequiredCompareFacesRequestRequestTypeDef, _OptionalCompareFacesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDetectCustomLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectCustomLabelsRequestRequestTypeDef",
     {
         "ProjectVersionArn": str,
         "Image": ImageTypeDef,
     },
 )
@@ -2834,59 +2873,65 @@
     {
         "MaxResults": int,
         "MinConfidence": float,
     },
     total=False,
 )
 
+
 class DetectCustomLabelsRequestRequestTypeDef(
     _RequiredDetectCustomLabelsRequestRequestTypeDef,
     _OptionalDetectCustomLabelsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDetectFacesRequestRequestTypeDef = TypedDict(
     "_RequiredDetectFacesRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectFacesRequestRequestTypeDef = TypedDict(
     "_OptionalDetectFacesRequestRequestTypeDef",
     {
         "Attributes": Sequence[AttributeType],
     },
     total=False,
 )
 
+
 class DetectFacesRequestRequestTypeDef(
     _RequiredDetectFacesRequestRequestTypeDef, _OptionalDetectFacesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_RequiredDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectProtectiveEquipmentRequestRequestTypeDef = TypedDict(
     "_OptionalDetectProtectiveEquipmentRequestRequestTypeDef",
     {
         "SummarizationAttributes": ProtectiveEquipmentSummarizationAttributesTypeDef,
     },
     total=False,
 )
 
+
 class DetectProtectiveEquipmentRequestRequestTypeDef(
     _RequiredDetectProtectiveEquipmentRequestRequestTypeDef,
     _OptionalDetectProtectiveEquipmentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredIndexFacesRequestRequestTypeDef = TypedDict(
     "_RequiredIndexFacesRequestRequestTypeDef",
     {
         "CollectionId": str,
         "Image": ImageTypeDef,
     },
 )
@@ -2897,19 +2942,21 @@
         "DetectionAttributes": Sequence[AttributeType],
         "MaxFaces": int,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
+
 class IndexFacesRequestRequestTypeDef(
     _RequiredIndexFacesRequestRequestTypeDef, _OptionalIndexFacesRequestRequestTypeDef
 ):
     pass
 
+
 RecognizeCelebritiesRequestRequestTypeDef = TypedDict(
     "RecognizeCelebritiesRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 
@@ -2926,20 +2973,22 @@
         "MaxFaces": int,
         "FaceMatchThreshold": float,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
+
 class SearchFacesByImageRequestRequestTypeDef(
     _RequiredSearchFacesByImageRequestRequestTypeDef,
     _OptionalSearchFacesByImageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSearchUsersByImageRequestRequestTypeDef = TypedDict(
     "_RequiredSearchUsersByImageRequestRequestTypeDef",
     {
         "CollectionId": str,
         "Image": ImageTypeDef,
     },
 )
@@ -2949,20 +2998,22 @@
         "UserMatchThreshold": float,
         "MaxUsers": int,
         "QualityFilter": QualityFilterType,
     },
     total=False,
 )
 
+
 class SearchUsersByImageRequestRequestTypeDef(
     _RequiredSearchUsersByImageRequestRequestTypeDef,
     _OptionalSearchUsersByImageRequestRequestTypeDef,
 ):
     pass
 
+
 CelebrityTypeDef = TypedDict(
     "CelebrityTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "Id": str,
         "Face": ComparedFaceTypeDef,
@@ -3081,19 +3132,21 @@
         "MinConfidence": float,
         "Features": Sequence[DetectLabelsFeatureNameType],
         "Settings": DetectLabelsSettingsTypeDef,
     },
     total=False,
 )
 
+
 class DetectLabelsRequestRequestTypeDef(
     _RequiredDetectLabelsRequestRequestTypeDef, _OptionalDetectLabelsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStartLabelDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartLabelDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
 _OptionalStartLabelDetectionRequestRequestTypeDef = TypedDict(
@@ -3105,20 +3158,22 @@
         "JobTag": str,
         "Features": Sequence[Literal["GENERAL_LABELS"]],
         "Settings": LabelDetectionSettingsTypeDef,
     },
     total=False,
 )
 
+
 class StartLabelDetectionRequestRequestTypeDef(
     _RequiredStartLabelDetectionRequestRequestTypeDef,
     _OptionalStartLabelDetectionRequestRequestTypeDef,
 ):
     pass
 
+
 CelebrityDetailTypeDef = TypedDict(
     "CelebrityDetailTypeDef",
     {
         "Urls": List[str],
         "Name": str,
         "Id": str,
         "Confidence": float,
@@ -3188,17 +3243,14 @@
     {
         "FaceDetails": FaceDetailTypeDef,
         "Reasons": List[UnsearchedFaceReasonType],
     },
     total=False,
 )
 
-StreamProcessorSettingsUnionTypeDef = Union[
-    StreamProcessorSettingsTypeDef, StreamProcessorSettingsOutputTypeDef
-]
 CustomLabelTypeDef = TypedDict(
     "CustomLabelTypeDef",
     {
         "Name": str,
         "Confidence": float,
         "Geometry": GeometryTypeDef,
     },
@@ -3223,24 +3275,48 @@
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
-RegionOfInterestUnionTypeDef = Union[RegionOfInterestTypeDef, RegionOfInterestOutputTypeDef]
 StartTextDetectionFiltersTypeDef = TypedDict(
     "StartTextDetectionFiltersTypeDef",
     {
         "WordFilter": DetectionFilterTypeDef,
         "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
+    {
+        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
+        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestTypeDef],
+        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
+        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
+    },
+    total=False,
+)
+
+
+class UpdateStreamProcessorRequestRequestTypeDef(
+    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
+    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredDetectModerationLabelsRequestRequestTypeDef = TypedDict(
     "_RequiredDetectModerationLabelsRequestRequestTypeDef",
     {
         "Image": ImageTypeDef,
     },
 )
 _OptionalDetectModerationLabelsRequestRequestTypeDef = TypedDict(
@@ -3248,20 +3324,22 @@
     {
         "MinConfidence": float,
         "HumanLoopConfig": HumanLoopConfigTypeDef,
     },
     total=False,
 )
 
+
 class DetectModerationLabelsRequestRequestTypeDef(
     _RequiredDetectModerationLabelsRequestRequestTypeDef,
     _OptionalDetectModerationLabelsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartStreamProcessorRequestRequestTypeDef = TypedDict(
     "_RequiredStartStreamProcessorRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalStartStreamProcessorRequestRequestTypeDef = TypedDict(
@@ -3269,47 +3347,79 @@
     {
         "StartSelector": StreamProcessingStartSelectorTypeDef,
         "StopSelector": StreamProcessingStopSelectorTypeDef,
     },
     total=False,
 )
 
+
 class StartStreamProcessorRequestRequestTypeDef(
     _RequiredStartStreamProcessorRequestRequestTypeDef,
     _OptionalStartStreamProcessorRequestRequestTypeDef,
 ):
     pass
 
+
 SearchUsersResponseTypeDef = TypedDict(
     "SearchUsersResponseTypeDef",
     {
         "UserMatches": List[UserMatchTypeDef],
         "FaceModelVersion": str,
         "SearchedFace": SearchedFaceTypeDef,
         "SearchedUser": SearchedUserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Input": StreamProcessorInputTypeDef,
+        "Output": StreamProcessorOutputTypeDef,
+        "Name": str,
+        "Settings": StreamProcessorSettingsTypeDef,
+        "RoleArn": str,
+    },
+)
+_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
+    {
+        "Tags": Mapping[str, str],
+        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
+        "KmsKeyId": str,
+        "RegionsOfInterest": Sequence[RegionOfInterestTypeDef],
+        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateStreamProcessorRequestRequestTypeDef(
+    _RequiredCreateStreamProcessorRequestRequestTypeDef,
+    _OptionalCreateStreamProcessorRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeStreamProcessorResponseTypeDef = TypedDict(
     "DescribeStreamProcessorResponseTypeDef",
     {
         "Name": str,
         "StreamProcessorArn": str,
         "Status": StreamProcessorStatusType,
         "StatusMessage": str,
         "CreationTimestamp": datetime,
         "LastUpdateTimestamp": datetime,
         "Input": StreamProcessorInputTypeDef,
         "Output": StreamProcessorOutputTypeDef,
         "RoleArn": str,
-        "Settings": StreamProcessorSettingsOutputTypeDef,
+        "Settings": StreamProcessorSettingsTypeDef,
         "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
         "KmsKeyId": str,
-        "RegionsOfInterest": List[RegionOfInterestOutputTypeDef],
+        "RegionsOfInterest": List[RegionOfInterestTypeDef],
         "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSegmentDetectionResponseTypeDef = TypedDict(
     "GetSegmentDetectionResponseTypeDef",
@@ -3345,40 +3455,23 @@
         "SearchedFaceId": str,
         "FaceMatches": List[FaceMatchTypeDef],
         "FaceModelVersion": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TestingDataOutputTypeDef = TypedDict(
-    "TestingDataOutputTypeDef",
-    {
-        "Assets": List[AssetTypeDef],
-        "AutoCreate": bool,
-    },
-    total=False,
-)
-
 TestingDataTypeDef = TypedDict(
     "TestingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
         "AutoCreate": bool,
     },
     total=False,
 )
 
-TrainingDataOutputTypeDef = TypedDict(
-    "TrainingDataOutputTypeDef",
-    {
-        "Assets": List[AssetTypeDef],
-    },
-    total=False,
-)
-
 TrainingDataTypeDef = TypedDict(
     "TrainingDataTypeDef",
     {
         "Assets": Sequence[AssetTypeDef],
     },
     total=False,
 )
@@ -3402,19 +3495,21 @@
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "DatasetSource": DatasetSourceTypeDef,
     },
     total=False,
 )
 
+
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredStartSegmentDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSegmentDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
         "SegmentTypes": Sequence[SegmentTypeType],
     },
 )
@@ -3425,20 +3520,22 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
         "Filters": StartSegmentDetectionFiltersTypeDef,
     },
     total=False,
 )
 
+
 class StartSegmentDetectionRequestRequestTypeDef(
     _RequiredStartSegmentDetectionRequestRequestTypeDef,
     _OptionalStartSegmentDetectionRequestRequestTypeDef,
 ):
     pass
 
+
 RecognizeCelebritiesResponseTypeDef = TypedDict(
     "RecognizeCelebritiesResponseTypeDef",
     {
         "CelebrityFaces": List[CelebrityTypeDef],
         "UnrecognizedFaces": List[ComparedFaceTypeDef],
         "OrientationCorrection": OrientationCorrectionType,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3592,69 +3689,20 @@
     "_OptionalDetectTextRequestRequestTypeDef",
     {
         "Filters": DetectTextFiltersTypeDef,
     },
     total=False,
 )
 
+
 class DetectTextRequestRequestTypeDef(
     _RequiredDetectTextRequestRequestTypeDef, _OptionalDetectTextRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Input": StreamProcessorInputTypeDef,
-        "Output": StreamProcessorOutputTypeDef,
-        "Name": str,
-        "Settings": StreamProcessorSettingsTypeDef,
-        "RoleArn": str,
-    },
-)
-_OptionalCreateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateStreamProcessorRequestRequestTypeDef",
-    {
-        "Tags": Mapping[str, str],
-        "NotificationChannel": StreamProcessorNotificationChannelTypeDef,
-        "KmsKeyId": str,
-        "RegionsOfInterest": Sequence[RegionOfInterestUnionTypeDef],
-        "DataSharingPreference": StreamProcessorDataSharingPreferenceTypeDef,
-    },
-    total=False,
-)
-
-class CreateStreamProcessorRequestRequestTypeDef(
-    _RequiredCreateStreamProcessorRequestRequestTypeDef,
-    _OptionalCreateStreamProcessorRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateStreamProcessorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateStreamProcessorRequestRequestTypeDef",
-    {
-        "SettingsForUpdate": StreamProcessorSettingsForUpdateTypeDef,
-        "RegionsOfInterestForUpdate": Sequence[RegionOfInterestUnionTypeDef],
-        "DataSharingPreferenceForUpdate": StreamProcessorDataSharingPreferenceTypeDef,
-        "ParametersToDelete": Sequence[StreamProcessorParameterToDeleteType],
-    },
-    total=False,
-)
-
-class UpdateStreamProcessorRequestRequestTypeDef(
-    _RequiredUpdateStreamProcessorRequestRequestTypeDef,
-    _OptionalUpdateStreamProcessorRequestRequestTypeDef,
-):
-    pass
 
 _RequiredStartTextDetectionRequestRequestTypeDef = TypedDict(
     "_RequiredStartTextDetectionRequestRequestTypeDef",
     {
         "Video": VideoTypeDef,
     },
 )
@@ -3665,21 +3713,22 @@
         "NotificationChannel": NotificationChannelTypeDef,
         "JobTag": str,
         "Filters": StartTextDetectionFiltersTypeDef,
     },
     total=False,
 )
 
+
 class StartTextDetectionRequestRequestTypeDef(
     _RequiredStartTextDetectionRequestRequestTypeDef,
     _OptionalStartTextDetectionRequestRequestTypeDef,
 ):
     pass
 
-TestingDataUnionTypeDef = Union[TestingDataTypeDef, TestingDataOutputTypeDef]
+
 _RequiredCreateProjectVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProjectVersionRequestRequestTypeDef",
     {
         "ProjectArn": str,
         "VersionName": str,
         "OutputConfig": OutputConfigTypeDef,
     },
@@ -3691,36 +3740,37 @@
         "TestingData": TestingDataTypeDef,
         "Tags": Mapping[str, str],
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class CreateProjectVersionRequestRequestTypeDef(
     _RequiredCreateProjectVersionRequestRequestTypeDef,
     _OptionalCreateProjectVersionRequestRequestTypeDef,
 ):
     pass
 
-TrainingDataUnionTypeDef = Union[TrainingDataTypeDef, TrainingDataOutputTypeDef]
+
 TestingDataResultTypeDef = TypedDict(
     "TestingDataResultTypeDef",
     {
-        "Input": TestingDataOutputTypeDef,
-        "Output": TestingDataOutputTypeDef,
+        "Input": TestingDataTypeDef,
+        "Output": TestingDataTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 TrainingDataResultTypeDef = TypedDict(
     "TrainingDataResultTypeDef",
     {
-        "Input": TrainingDataOutputTypeDef,
-        "Output": TrainingDataOutputTypeDef,
+        "Input": TrainingDataTypeDef,
+        "Output": TrainingDataTypeDef,
         "Validation": ValidationDataTypeDef,
     },
     total=False,
 )
 
 DetectProtectiveEquipmentResponseTypeDef = TypedDict(
     "DetectProtectiveEquipmentResponseTypeDef",
```

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/waiter.py` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition/waiter.pyi` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.5.2.post1/types_aiobotocore_rekognition.egg-info/SOURCES.txt` & `types-aiobotocore-rekognition-2.5.2.post2/types_aiobotocore_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

