# Comparing `tmp/types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:31 2023, max compression
```

## Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1.tar` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.681642 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-08-02 14:51:57.677642 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.681642 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.673642 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19300 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19272 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-08-02 14:34:08.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-08-02 14:34:08.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48594 2023-08-02 14:34:08.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48535 2023-08-02 14:34:08.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.677642 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.111331 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:20.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-08-04 12:00:31.111331 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11576 2023-08-04 11:41:20.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:31.111331 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-08-04 11:41:20.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.103330 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-04 11:41:20.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-04 11:41:20.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-08-04 11:41:20.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19230 2023-08-04 11:41:21.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19202 2023-08-04 11:41:20.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-08-04 11:41:21.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-08-04 11:41:21.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:20.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38685 2023-08-04 11:41:22.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38640 2023-08-04 11:41:21.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:20.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.111331 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/LICENSE` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/setup.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-media-pipelines",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_chime_sdk_media_pipelines"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__init__.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/__main__.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ChimeSDKMediaPipelines 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/client.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,36 +18,36 @@
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import MediaPipelineStatusUpdateType
 from .type_defs import (
-    ChimeSdkMeetingConfigurationUnionTypeDef,
+    ChimeSdkMeetingConfigurationTypeDef,
     ConcatenationSinkTypeDef,
     ConcatenationSourceTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaPipelineResponseTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
-    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
-    LiveConnectorSourceConfigurationUnionTypeDef,
-    MediaInsightsPipelineConfigurationElementUnionTypeDef,
-    RealTimeAlertConfigurationUnionTypeDef,
+    LiveConnectorSourceConfigurationTypeDef,
+    MediaInsightsPipelineConfigurationElementTypeDef,
+    RealTimeAlertConfigurationTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     TagTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -116,15 +116,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...,
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_capture_pipeline)
@@ -145,17 +145,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_concatenation_pipeline)
         """
 
     async def create_media_insights_pipeline(
         self,
         *,
         MediaInsightsPipelineConfigurationArn: str,
-        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = ...,
+        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationTypeDef = ...,
         MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
-        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = ...,
+        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = ...,
         S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineResponseTypeDef:
         """
         Creates a media insights pipeline.
 
@@ -164,31 +164,31 @@
         """
 
     async def create_media_insights_pipeline_configuration(
         self,
         *,
         MediaInsightsPipelineConfigurationName: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...,
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         A structure that contains the static configurations for a media insights
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline_configuration)
         """
 
     async def create_media_live_connector_pipeline(
         self,
         *,
-        Sources: Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
+        Sources: Sequence[LiveConnectorSourceConfigurationTypeDef],
         Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaLiveConnectorPipelineResponseTypeDef:
         """
         Creates a media live connector pipeline in an Amazon Chime SDK meeting.
 
@@ -323,16 +323,16 @@
         """
 
     async def update_media_insights_pipeline_configuration(
         self,
         *,
         Identifier: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...
     ) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Updates the media insights pipeline's configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_configuration)
         """
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/client.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,36 +18,36 @@
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import MediaPipelineStatusUpdateType
 from .type_defs import (
-    ChimeSdkMeetingConfigurationUnionTypeDef,
+    ChimeSdkMeetingConfigurationTypeDef,
     ConcatenationSinkTypeDef,
     ConcatenationSourceTypeDef,
     CreateMediaCapturePipelineResponseTypeDef,
     CreateMediaConcatenationPipelineResponseTypeDef,
     CreateMediaInsightsPipelineConfigurationResponseTypeDef,
     CreateMediaInsightsPipelineResponseTypeDef,
     CreateMediaLiveConnectorPipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetMediaCapturePipelineResponseTypeDef,
     GetMediaInsightsPipelineConfigurationResponseTypeDef,
     GetMediaPipelineResponseTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef,
-    KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef,
+    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
+    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
     ListMediaCapturePipelinesResponseTypeDef,
     ListMediaInsightsPipelineConfigurationsResponseTypeDef,
     ListMediaPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LiveConnectorSinkConfigurationTypeDef,
-    LiveConnectorSourceConfigurationUnionTypeDef,
-    MediaInsightsPipelineConfigurationElementUnionTypeDef,
-    RealTimeAlertConfigurationUnionTypeDef,
+    LiveConnectorSourceConfigurationTypeDef,
+    MediaInsightsPipelineConfigurationElementTypeDef,
+    RealTimeAlertConfigurationTypeDef,
     S3RecordingSinkRuntimeConfigurationTypeDef,
     TagTypeDef,
     UpdateMediaInsightsPipelineConfigurationResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -109,15 +109,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...,
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_capture_pipeline)
@@ -136,17 +136,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_concatenation_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_concatenation_pipeline)
         """
     async def create_media_insights_pipeline(
         self,
         *,
         MediaInsightsPipelineConfigurationArn: str,
-        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = ...,
+        KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationTypeDef = ...,
         MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
-        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = ...,
+        KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = ...,
         S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineResponseTypeDef:
         """
         Creates a media insights pipeline.
 
@@ -154,30 +154,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline)
         """
     async def create_media_insights_pipeline_configuration(
         self,
         *,
         MediaInsightsPipelineConfigurationName: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...,
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...
     ) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         A structure that contains the static configurations for a media insights
         pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#create_media_insights_pipeline_configuration)
         """
     async def create_media_live_connector_pipeline(
         self,
         *,
-        Sources: Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
+        Sources: Sequence[LiveConnectorSourceConfigurationTypeDef],
         Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMediaLiveConnectorPipelineResponseTypeDef:
         """
         Creates a media live connector pipeline in an Amazon Chime SDK meeting.
 
@@ -298,16 +298,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#untag_resource)
         """
     async def update_media_insights_pipeline_configuration(
         self,
         *,
         Identifier: str,
         ResourceAccessRoleArn: str,
-        Elements: Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
-        RealTimeAlertConfiguration: RealTimeAlertConfigurationUnionTypeDef = ...
+        Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
+        RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...
     ) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:
         """
         Updates the media insights pipeline's configuration settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_media_pipelines/client/#update_media_insights_pipeline_configuration)
         """
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/literals.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,21 +65,19 @@
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
-    "TimestampRangeOutputTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
     "PresenterOnlyConfigurationTypeDef",
     "IssueDetectionConfigurationTypeDef",
-    "KeywordMatchConfigurationOutputTypeDef",
     "KeywordMatchConfigurationTypeDef",
     "KinesisDataStreamSinkConfigurationTypeDef",
     "RecordingStreamConfigurationTypeDef",
     "LambdaFunctionSinkConfigurationTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "MediaCapturePipelineSummaryTypeDef",
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
@@ -89,87 +87,67 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "LiveConnectorRTMPConfigurationTypeDef",
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
     "SentimentConfigurationTypeDef",
-    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
-    "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
-    "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
     "ConcatenationSinkTypeDef",
     "TagResourceRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "FragmentSelectorOutputTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
-    "RealTimeAlertRuleOutputTypeDef",
     "RealTimeAlertRuleTypeDef",
-    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "TimestampRangeTypeDef",
-    "MediaInsightsPipelineConfigurationElementOutputTypeDef",
     "MediaInsightsPipelineConfigurationElementTypeDef",
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
-    "StreamConfigurationOutputTypeDef",
     "StreamConfigurationTypeDef",
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     "CompositedVideoArtifactsConfigurationTypeDef",
-    "RealTimeAlertConfigurationOutputTypeDef",
     "RealTimeAlertConfigurationTypeDef",
     "FragmentSelectorTypeDef",
-    "MediaInsightsPipelineConfigurationElementUnionTypeDef",
     "MediaCapturePipelineSourceConfigurationTypeDef",
-    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     "ArtifactsConfigurationTypeDef",
-    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationTypeDef",
-    "MediaInsightsPipelineConfigurationTypeDef",
-    "RealTimeAlertConfigurationUnionTypeDef",
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
+    "MediaInsightsPipelineConfigurationTypeDef",
     "UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     "ConcatenationSourceTypeDef",
-    "MediaInsightsPipelineTypeDef",
-    "KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef",
-    "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
-    "LiveConnectorSourceConfigurationOutputTypeDef",
     "LiveConnectorSourceConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     "CreateMediaInsightsPipelineRequestRequestTypeDef",
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef",
+    "MediaInsightsPipelineTypeDef",
     "CreateMediaConcatenationPipelineRequestRequestTypeDef",
     "MediaConcatenationPipelineTypeDef",
-    "CreateMediaInsightsPipelineResponseTypeDef",
-    "MediaCapturePipelineTypeDef",
-    "ChimeSdkMeetingConfigurationUnionTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
+    "MediaCapturePipelineTypeDef",
+    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "MediaLiveConnectorPipelineTypeDef",
-    "LiveConnectorSourceConfigurationUnionTypeDef",
+    "CreateMediaInsightsPipelineResponseTypeDef",
     "CreateMediaConcatenationPipelineResponseTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
-    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
@@ -394,22 +372,14 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
-TimestampRangeOutputTypeDef = TypedDict(
-    "TimestampRangeOutputTypeDef",
-    {
-        "StartTimestamp": datetime,
-        "EndTimestamp": datetime,
-    },
-)
-
 GetMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "GetMediaCapturePipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
@@ -438,36 +408,14 @@
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
-_RequiredKeywordMatchConfigurationOutputTypeDef = TypedDict(
-    "_RequiredKeywordMatchConfigurationOutputTypeDef",
-    {
-        "RuleName": str,
-        "Keywords": List[str],
-    },
-)
-_OptionalKeywordMatchConfigurationOutputTypeDef = TypedDict(
-    "_OptionalKeywordMatchConfigurationOutputTypeDef",
-    {
-        "Negate": bool,
-    },
-    total=False,
-)
-
-
-class KeywordMatchConfigurationOutputTypeDef(
-    _RequiredKeywordMatchConfigurationOutputTypeDef, _OptionalKeywordMatchConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -633,23 +581,14 @@
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
     },
 )
 
-SelectedVideoStreamsOutputTypeDef = TypedDict(
-    "SelectedVideoStreamsOutputTypeDef",
-    {
-        "AttendeeIds": List[str],
-        "ExternalUserIds": List[str],
-    },
-    total=False,
-)
-
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
@@ -668,47 +607,14 @@
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     {
         "Identifier": str,
         "UpdateStatus": MediaPipelineStatusUpdateType,
     },
 )
 
-_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
-    {
-        "LanguageCode": CallAnalyticsLanguageCodeType,
-    },
-)
-_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
-    {
-        "VocabularyName": str,
-        "VocabularyFilterName": str,
-        "VocabularyFilterMethod": VocabularyFilterMethodType,
-        "LanguageModelName": str,
-        "EnablePartialResultsStabilization": bool,
-        "PartialResultsStability": PartialResultsStabilityType,
-        "ContentIdentificationType": Literal["PII"],
-        "ContentRedactionType": Literal["PII"],
-        "PiiEntityTypes": str,
-        "FilterPartialResults": bool,
-        "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
-        "CallAnalyticsStreamCategories": List[str],
-    },
-    total=False,
-)
-
-
-class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
-    _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
-    _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -747,35 +653,14 @@
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
         "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationTypeDef,
         "MeetingEvents": MeetingEventsConcatenationConfigurationTypeDef,
         "CompositedVideo": CompositedVideoConcatenationConfigurationTypeDef,
     },
 )
 
-_RequiredStreamChannelDefinitionOutputTypeDef = TypedDict(
-    "_RequiredStreamChannelDefinitionOutputTypeDef",
-    {
-        "NumberOfChannels": int,
-    },
-)
-_OptionalStreamChannelDefinitionOutputTypeDef = TypedDict(
-    "_OptionalStreamChannelDefinitionOutputTypeDef",
-    {
-        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
-    },
-    total=False,
-)
-
-
-class StreamChannelDefinitionOutputTypeDef(
-    _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
-):
-    pass
-
-
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
@@ -820,22 +705,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FragmentSelectorOutputTypeDef = TypedDict(
-    "FragmentSelectorOutputTypeDef",
-    {
-        "FragmentSelectorType": FragmentSelectorTypeType,
-        "TimestampRange": TimestampRangeOutputTypeDef,
-    },
-)
-
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
@@ -886,37 +763,14 @@
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
         "RTMPConfiguration": LiveConnectorRTMPConfigurationTypeDef,
     },
 )
 
-_RequiredRealTimeAlertRuleOutputTypeDef = TypedDict(
-    "_RequiredRealTimeAlertRuleOutputTypeDef",
-    {
-        "Type": RealTimeAlertRuleTypeType,
-    },
-)
-_OptionalRealTimeAlertRuleOutputTypeDef = TypedDict(
-    "_OptionalRealTimeAlertRuleOutputTypeDef",
-    {
-        "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
-        "SentimentConfiguration": SentimentConfigurationTypeDef,
-        "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class RealTimeAlertRuleOutputTypeDef(
-    _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
-):
-    pass
-
-
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -932,22 +786,14 @@
 
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
 
-SourceConfigurationOutputTypeDef = TypedDict(
-    "SourceConfigurationOutputTypeDef",
-    {
-        "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
@@ -956,45 +802,14 @@
     "TimestampRangeTypeDef",
     {
         "StartTimestamp": TimestampTypeDef,
         "EndTimestamp": TimestampTypeDef,
     },
 )
 
-_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
-    "_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef",
-    {
-        "Type": MediaInsightsPipelineConfigurationElementTypeType,
-    },
-)
-_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
-    "_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef",
-    {
-        "AmazonTranscribeCallAnalyticsProcessorConfiguration": (
-            AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef
-        ),
-        "AmazonTranscribeProcessorConfiguration": AmazonTranscribeProcessorConfigurationTypeDef,
-        "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationTypeDef,
-        "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationTypeDef,
-        "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationTypeDef,
-        "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
-        "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
-        "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class MediaInsightsPipelineConfigurationElementOutputTypeDef(
-    _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
-    _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
-):
-    pass
-
-
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -1025,36 +840,14 @@
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
-_RequiredStreamConfigurationOutputTypeDef = TypedDict(
-    "_RequiredStreamConfigurationOutputTypeDef",
-    {
-        "StreamArn": str,
-        "StreamChannelDefinition": StreamChannelDefinitionOutputTypeDef,
-    },
-)
-_OptionalStreamConfigurationOutputTypeDef = TypedDict(
-    "_OptionalStreamConfigurationOutputTypeDef",
-    {
-        "FragmentNumber": str,
-    },
-    total=False,
-)
-
-
-class StreamConfigurationOutputTypeDef(
-    _RequiredStreamConfigurationOutputTypeDef, _OptionalStreamConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
 )
@@ -1069,22 +862,14 @@
 
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
 
-KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
-    {
-        "Streams": List[RecordingStreamConfigurationTypeDef],
-        "FragmentSelector": FragmentSelectorOutputTypeDef,
-    },
-)
-
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -1100,23 +885,14 @@
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
 
-RealTimeAlertConfigurationOutputTypeDef = TypedDict(
-    "RealTimeAlertConfigurationOutputTypeDef",
-    {
-        "Disabled": bool,
-        "Rules": List[RealTimeAlertRuleOutputTypeDef],
-    },
-    total=False,
-)
-
 RealTimeAlertConfigurationTypeDef = TypedDict(
     "RealTimeAlertConfigurationTypeDef",
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
@@ -1126,35 +902,22 @@
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeTypeDef,
     },
 )
 
-MediaInsightsPipelineConfigurationElementUnionTypeDef = Union[
-    MediaInsightsPipelineConfigurationElementTypeDef,
-    MediaInsightsPipelineConfigurationElementOutputTypeDef,
-]
 MediaCapturePipelineSourceConfigurationTypeDef = TypedDict(
     "MediaCapturePipelineSourceConfigurationTypeDef",
     {
         "MediaPipelineArn": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationTypeDef,
     },
 )
 
-KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef = TypedDict(
-    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
-    {
-        "Streams": List[StreamConfigurationOutputTypeDef],
-        "MediaEncoding": Literal["pcm"],
-        "MediaSampleRate": int,
-    },
-)
-
 KinesisVideoStreamSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[StreamConfigurationTypeDef],
         "MediaEncoding": Literal["pcm"],
         "MediaSampleRate": int,
     },
@@ -1179,38 +942,14 @@
 
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
 
-_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
-    "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
-    {
-        "Arn": str,
-        "MuxType": LiveConnectorMuxTypeType,
-    },
-)
-_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
-    "_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
-    {
-        "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
-        "SourceConfiguration": SourceConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
-    _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
-    _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1227,46 +966,20 @@
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
 
-MediaInsightsPipelineConfigurationTypeDef = TypedDict(
-    "MediaInsightsPipelineConfigurationTypeDef",
-    {
-        "MediaInsightsPipelineConfigurationName": str,
-        "MediaInsightsPipelineConfigurationArn": str,
-        "ResourceAccessRoleArn": str,
-        "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
-        "Elements": List[MediaInsightsPipelineConfigurationElementOutputTypeDef],
-        "MediaInsightsPipelineConfigurationId": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
-RealTimeAlertConfigurationUnionTypeDef = Union[
-    RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
-]
-KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
-    {
-        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
-        "FragmentSelector": FragmentSelectorTypeDef,
-    },
-)
-
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
     },
 )
 _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
@@ -1279,20 +992,35 @@
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+MediaInsightsPipelineConfigurationTypeDef = TypedDict(
+    "MediaInsightsPipelineConfigurationTypeDef",
+    {
+        "MediaInsightsPipelineConfigurationName": str,
+        "MediaInsightsPipelineConfigurationArn": str,
+        "ResourceAccessRoleArn": str,
+        "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
+        "Elements": List[MediaInsightsPipelineConfigurationElementTypeDef],
+        "MediaInsightsPipelineConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
 _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
     },
 )
 _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
@@ -1303,74 +1031,39 @@
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-ConcatenationSourceTypeDef = TypedDict(
-    "ConcatenationSourceTypeDef",
-    {
-        "Type": Literal["MediaCapturePipeline"],
-        "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
-    },
-)
-
-MediaInsightsPipelineTypeDef = TypedDict(
-    "MediaInsightsPipelineTypeDef",
+KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     {
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "MediaInsightsPipelineConfigurationArn": str,
-        "Status": MediaPipelineStatusType,
-        "KinesisVideoStreamSourceRuntimeConfiguration": (
-            KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef
-        ),
-        "MediaInsightsRuntimeMetadata": Dict[str, str],
-        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef
-        ),
-        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
-        "CreatedTimestamp": datetime,
+        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
+        "FragmentSelector": FragmentSelectorTypeDef,
     },
-    total=False,
 )
 
-KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = Union[
-    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
-    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
-]
-ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
-    "ChimeSdkMeetingConfigurationOutputTypeDef",
+ConcatenationSourceTypeDef = TypedDict(
+    "ConcatenationSourceTypeDef",
     {
-        "SourceConfiguration": SourceConfigurationOutputTypeDef,
-        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
+        "Type": Literal["MediaCapturePipeline"],
+        "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
-    total=False,
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
-LiveConnectorSourceConfigurationOutputTypeDef = TypedDict(
-    "LiveConnectorSourceConfigurationOutputTypeDef",
-    {
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "ChimeSdkMeetingLiveConnectorConfiguration": (
-            ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef
-        ),
-    },
-)
-
 LiveConnectorSourceConfigurationTypeDef = TypedDict(
     "LiveConnectorSourceConfigurationTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "ChimeSdkMeetingLiveConnectorConfiguration": (
             ChimeSdkMeetingLiveConnectorConfigurationTypeDef
         ),
@@ -1428,18 +1121,34 @@
 class CreateMediaInsightsPipelineRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
 ):
     pass
 
 
-KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = Union[
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
-]
+MediaInsightsPipelineTypeDef = TypedDict(
+    "MediaInsightsPipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "MediaInsightsPipelineConfigurationArn": str,
+        "Status": MediaPipelineStatusType,
+        "KinesisVideoStreamSourceRuntimeConfiguration": (
+            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
+        ),
+        "MediaInsightsRuntimeMetadata": Dict[str, str],
+        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
+        ),
+        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
+        "CreatedTimestamp": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
         "Sinks": Sequence[ConcatenationSinkTypeDef],
     },
 )
@@ -1470,86 +1179,104 @@
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
-    "CreateMediaInsightsPipelineResponseTypeDef",
+_RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
-        "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
     },
 )
+_OptionalCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaCapturePipelineRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateMediaCapturePipelineRequestRequestTypeDef(
+    _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
+    _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
+):
+    pass
+
 
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "Status": MediaPipelineStatusType,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
     },
     total=False,
 )
 
-ChimeSdkMeetingConfigurationUnionTypeDef = Union[
-    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
-]
-_RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
+_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
+        "Sources": Sequence[LiveConnectorSourceConfigurationTypeDef],
+        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
     },
 )
-_OptionalCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaCapturePipelineRequestRequestTypeDef",
+_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class CreateMediaCapturePipelineRequestRequestTypeDef(
-    _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
-    _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
+class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
+    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
 ):
     pass
 
 
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
-        "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
+        "Sources": List[LiveConnectorSourceConfigurationTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-LiveConnectorSourceConfigurationUnionTypeDef = Union[
-    LiveConnectorSourceConfigurationTypeDef, LiveConnectorSourceConfigurationOutputTypeDef
-]
+CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
+    "CreateMediaInsightsPipelineResponseTypeDef",
+    {
+        "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1585,38 +1312,14 @@
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
-    {
-        "Sources": Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
-        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
-    },
-)
-_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
-    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
-    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
-):
-    pass
-
-
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines/type_defs.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -64,21 +64,19 @@
     "S3BucketSinkConfigurationTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "S3RecordingSinkRuntimeConfigurationTypeDef",
     "DeleteMediaCapturePipelineRequestRequestTypeDef",
     "DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "DeleteMediaPipelineRequestRequestTypeDef",
-    "TimestampRangeOutputTypeDef",
     "GetMediaCapturePipelineRequestRequestTypeDef",
     "GetMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     "GetMediaPipelineRequestRequestTypeDef",
     "PresenterOnlyConfigurationTypeDef",
     "IssueDetectionConfigurationTypeDef",
-    "KeywordMatchConfigurationOutputTypeDef",
     "KeywordMatchConfigurationTypeDef",
     "KinesisDataStreamSinkConfigurationTypeDef",
     "RecordingStreamConfigurationTypeDef",
     "LambdaFunctionSinkConfigurationTypeDef",
     "ListMediaCapturePipelinesRequestRequestTypeDef",
     "MediaCapturePipelineSummaryTypeDef",
     "ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef",
@@ -88,87 +86,67 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "LiveConnectorRTMPConfigurationTypeDef",
     "S3RecordingSinkConfigurationTypeDef",
     "SnsTopicSinkConfigurationTypeDef",
     "SqsQueueSinkConfigurationTypeDef",
     "VoiceAnalyticsProcessorConfigurationTypeDef",
     "SentimentConfigurationTypeDef",
-    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
-    "AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
     "AmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     "ArtifactsConcatenationConfigurationTypeDef",
-    "StreamChannelDefinitionOutputTypeDef",
     "StreamChannelDefinitionTypeDef",
     "ConcatenationSinkTypeDef",
     "TagResourceRequestRequestTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "FragmentSelectorOutputTypeDef",
     "GridViewConfigurationTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
     "ListMediaInsightsPipelineConfigurationsResponseTypeDef",
     "ListMediaPipelinesResponseTypeDef",
     "LiveConnectorSinkConfigurationTypeDef",
-    "RealTimeAlertRuleOutputTypeDef",
     "RealTimeAlertRuleTypeDef",
-    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
     "TimestampRangeTypeDef",
-    "MediaInsightsPipelineConfigurationElementOutputTypeDef",
     "MediaInsightsPipelineConfigurationElementTypeDef",
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
-    "StreamConfigurationOutputTypeDef",
     "StreamConfigurationTypeDef",
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
     "CompositedVideoArtifactsConfigurationTypeDef",
-    "RealTimeAlertConfigurationOutputTypeDef",
     "RealTimeAlertConfigurationTypeDef",
     "FragmentSelectorTypeDef",
-    "MediaInsightsPipelineConfigurationElementUnionTypeDef",
     "MediaCapturePipelineSourceConfigurationTypeDef",
-    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     "ArtifactsConfigurationTypeDef",
-    "ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
     "ChimeSdkMeetingLiveConnectorConfigurationTypeDef",
-    "MediaInsightsPipelineConfigurationTypeDef",
-    "RealTimeAlertConfigurationUnionTypeDef",
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
+    "MediaInsightsPipelineConfigurationTypeDef",
     "UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     "ConcatenationSourceTypeDef",
-    "MediaInsightsPipelineTypeDef",
-    "KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef",
-    "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
-    "LiveConnectorSourceConfigurationOutputTypeDef",
     "LiveConnectorSourceConfigurationTypeDef",
     "CreateMediaInsightsPipelineConfigurationResponseTypeDef",
     "GetMediaInsightsPipelineConfigurationResponseTypeDef",
     "UpdateMediaInsightsPipelineConfigurationResponseTypeDef",
     "CreateMediaInsightsPipelineRequestRequestTypeDef",
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef",
+    "MediaInsightsPipelineTypeDef",
     "CreateMediaConcatenationPipelineRequestRequestTypeDef",
     "MediaConcatenationPipelineTypeDef",
-    "CreateMediaInsightsPipelineResponseTypeDef",
-    "MediaCapturePipelineTypeDef",
-    "ChimeSdkMeetingConfigurationUnionTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
+    "MediaCapturePipelineTypeDef",
+    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "MediaLiveConnectorPipelineTypeDef",
-    "LiveConnectorSourceConfigurationUnionTypeDef",
+    "CreateMediaInsightsPipelineResponseTypeDef",
     "CreateMediaConcatenationPipelineResponseTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "CreateMediaLiveConnectorPipelineResponseTypeDef",
     "MediaPipelineTypeDef",
-    "CreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     "GetMediaPipelineResponseTypeDef",
 )
 
 _RequiredPostCallAnalyticsSettingsTypeDef = TypedDict(
     "_RequiredPostCallAnalyticsSettingsTypeDef",
     {
         "OutputLocation": str,
@@ -383,22 +361,14 @@
 DeleteMediaPipelineRequestRequestTypeDef = TypedDict(
     "DeleteMediaPipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
-TimestampRangeOutputTypeDef = TypedDict(
-    "TimestampRangeOutputTypeDef",
-    {
-        "StartTimestamp": datetime,
-        "EndTimestamp": datetime,
-    },
-)
-
 GetMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "GetMediaCapturePipelineRequestRequestTypeDef",
     {
         "MediaPipelineId": str,
     },
 )
 
@@ -427,34 +397,14 @@
 IssueDetectionConfigurationTypeDef = TypedDict(
     "IssueDetectionConfigurationTypeDef",
     {
         "RuleName": str,
     },
 )
 
-_RequiredKeywordMatchConfigurationOutputTypeDef = TypedDict(
-    "_RequiredKeywordMatchConfigurationOutputTypeDef",
-    {
-        "RuleName": str,
-        "Keywords": List[str],
-    },
-)
-_OptionalKeywordMatchConfigurationOutputTypeDef = TypedDict(
-    "_OptionalKeywordMatchConfigurationOutputTypeDef",
-    {
-        "Negate": bool,
-    },
-    total=False,
-)
-
-class KeywordMatchConfigurationOutputTypeDef(
-    _RequiredKeywordMatchConfigurationOutputTypeDef, _OptionalKeywordMatchConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredKeywordMatchConfigurationTypeDef = TypedDict(
     "_RequiredKeywordMatchConfigurationTypeDef",
     {
         "RuleName": str,
         "Keywords": Sequence[str],
     },
 )
@@ -616,23 +566,14 @@
     {
         "RuleName": str,
         "SentimentType": Literal["NEGATIVE"],
         "TimePeriod": int,
     },
 )
 
-SelectedVideoStreamsOutputTypeDef = TypedDict(
-    "SelectedVideoStreamsOutputTypeDef",
-    {
-        "AttendeeIds": List[str],
-        "ExternalUserIds": List[str],
-    },
-    total=False,
-)
-
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
@@ -651,45 +592,14 @@
     "UpdateMediaInsightsPipelineStatusRequestRequestTypeDef",
     {
         "Identifier": str,
         "UpdateStatus": MediaPipelineStatusUpdateType,
     },
 )
 
-_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
-    {
-        "LanguageCode": CallAnalyticsLanguageCodeType,
-    },
-)
-_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef",
-    {
-        "VocabularyName": str,
-        "VocabularyFilterName": str,
-        "VocabularyFilterMethod": VocabularyFilterMethodType,
-        "LanguageModelName": str,
-        "EnablePartialResultsStabilization": bool,
-        "PartialResultsStability": PartialResultsStabilityType,
-        "ContentIdentificationType": Literal["PII"],
-        "ContentRedactionType": Literal["PII"],
-        "PiiEntityTypes": str,
-        "FilterPartialResults": bool,
-        "PostCallAnalyticsSettings": PostCallAnalyticsSettingsTypeDef,
-        "CallAnalyticsStreamCategories": List[str],
-    },
-    total=False,
-)
-
-class AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef(
-    _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
-    _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
     "_RequiredAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef",
     {
         "LanguageCode": CallAnalyticsLanguageCodeType,
     },
 )
 _OptionalAmazonTranscribeCallAnalyticsProcessorConfigurationTypeDef = TypedDict(
@@ -726,33 +636,14 @@
         "DataChannel": DataChannelConcatenationConfigurationTypeDef,
         "TranscriptionMessages": TranscriptionMessagesConcatenationConfigurationTypeDef,
         "MeetingEvents": MeetingEventsConcatenationConfigurationTypeDef,
         "CompositedVideo": CompositedVideoConcatenationConfigurationTypeDef,
     },
 )
 
-_RequiredStreamChannelDefinitionOutputTypeDef = TypedDict(
-    "_RequiredStreamChannelDefinitionOutputTypeDef",
-    {
-        "NumberOfChannels": int,
-    },
-)
-_OptionalStreamChannelDefinitionOutputTypeDef = TypedDict(
-    "_OptionalStreamChannelDefinitionOutputTypeDef",
-    {
-        "ChannelDefinitions": List[ChannelDefinitionTypeDef],
-    },
-    total=False,
-)
-
-class StreamChannelDefinitionOutputTypeDef(
-    _RequiredStreamChannelDefinitionOutputTypeDef, _OptionalStreamChannelDefinitionOutputTypeDef
-):
-    pass
-
 _RequiredStreamChannelDefinitionTypeDef = TypedDict(
     "_RequiredStreamChannelDefinitionTypeDef",
     {
         "NumberOfChannels": int,
     },
 )
 _OptionalStreamChannelDefinitionTypeDef = TypedDict(
@@ -795,22 +686,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FragmentSelectorOutputTypeDef = TypedDict(
-    "FragmentSelectorOutputTypeDef",
-    {
-        "FragmentSelectorType": FragmentSelectorTypeType,
-        "TimestampRange": TimestampRangeOutputTypeDef,
-    },
-)
-
 _RequiredGridViewConfigurationTypeDef = TypedDict(
     "_RequiredGridViewConfigurationTypeDef",
     {
         "ContentShareLayout": ContentShareLayoutOptionType,
     },
 )
 _OptionalGridViewConfigurationTypeDef = TypedDict(
@@ -859,35 +742,14 @@
     "LiveConnectorSinkConfigurationTypeDef",
     {
         "SinkType": Literal["RTMP"],
         "RTMPConfiguration": LiveConnectorRTMPConfigurationTypeDef,
     },
 )
 
-_RequiredRealTimeAlertRuleOutputTypeDef = TypedDict(
-    "_RequiredRealTimeAlertRuleOutputTypeDef",
-    {
-        "Type": RealTimeAlertRuleTypeType,
-    },
-)
-_OptionalRealTimeAlertRuleOutputTypeDef = TypedDict(
-    "_OptionalRealTimeAlertRuleOutputTypeDef",
-    {
-        "KeywordMatchConfiguration": KeywordMatchConfigurationOutputTypeDef,
-        "SentimentConfiguration": SentimentConfigurationTypeDef,
-        "IssueDetectionConfiguration": IssueDetectionConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class RealTimeAlertRuleOutputTypeDef(
-    _RequiredRealTimeAlertRuleOutputTypeDef, _OptionalRealTimeAlertRuleOutputTypeDef
-):
-    pass
-
 _RequiredRealTimeAlertRuleTypeDef = TypedDict(
     "_RequiredRealTimeAlertRuleTypeDef",
     {
         "Type": RealTimeAlertRuleTypeType,
     },
 )
 _OptionalRealTimeAlertRuleTypeDef = TypedDict(
@@ -901,22 +763,14 @@
 )
 
 class RealTimeAlertRuleTypeDef(
     _RequiredRealTimeAlertRuleTypeDef, _OptionalRealTimeAlertRuleTypeDef
 ):
     pass
 
-SourceConfigurationOutputTypeDef = TypedDict(
-    "SourceConfigurationOutputTypeDef",
-    {
-        "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
@@ -925,43 +779,14 @@
     "TimestampRangeTypeDef",
     {
         "StartTimestamp": TimestampTypeDef,
         "EndTimestamp": TimestampTypeDef,
     },
 )
 
-_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
-    "_RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef",
-    {
-        "Type": MediaInsightsPipelineConfigurationElementTypeType,
-    },
-)
-_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef = TypedDict(
-    "_OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef",
-    {
-        "AmazonTranscribeCallAnalyticsProcessorConfiguration": (
-            AmazonTranscribeCallAnalyticsProcessorConfigurationOutputTypeDef
-        ),
-        "AmazonTranscribeProcessorConfiguration": AmazonTranscribeProcessorConfigurationTypeDef,
-        "KinesisDataStreamSinkConfiguration": KinesisDataStreamSinkConfigurationTypeDef,
-        "S3RecordingSinkConfiguration": S3RecordingSinkConfigurationTypeDef,
-        "VoiceAnalyticsProcessorConfiguration": VoiceAnalyticsProcessorConfigurationTypeDef,
-        "LambdaFunctionSinkConfiguration": LambdaFunctionSinkConfigurationTypeDef,
-        "SqsQueueSinkConfiguration": SqsQueueSinkConfigurationTypeDef,
-        "SnsTopicSinkConfiguration": SnsTopicSinkConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class MediaInsightsPipelineConfigurationElementOutputTypeDef(
-    _RequiredMediaInsightsPipelineConfigurationElementOutputTypeDef,
-    _OptionalMediaInsightsPipelineConfigurationElementOutputTypeDef,
-):
-    pass
-
 _RequiredMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
     "_RequiredMediaInsightsPipelineConfigurationElementTypeDef",
     {
         "Type": MediaInsightsPipelineConfigurationElementTypeType,
     },
 )
 _OptionalMediaInsightsPipelineConfigurationElementTypeDef = TypedDict(
@@ -990,34 +815,14 @@
 ChimeSdkMeetingConcatenationConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConcatenationConfigurationTypeDef",
     {
         "ArtifactsConfiguration": ArtifactsConcatenationConfigurationTypeDef,
     },
 )
 
-_RequiredStreamConfigurationOutputTypeDef = TypedDict(
-    "_RequiredStreamConfigurationOutputTypeDef",
-    {
-        "StreamArn": str,
-        "StreamChannelDefinition": StreamChannelDefinitionOutputTypeDef,
-    },
-)
-_OptionalStreamConfigurationOutputTypeDef = TypedDict(
-    "_OptionalStreamConfigurationOutputTypeDef",
-    {
-        "FragmentNumber": str,
-    },
-    total=False,
-)
-
-class StreamConfigurationOutputTypeDef(
-    _RequiredStreamConfigurationOutputTypeDef, _OptionalStreamConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredStreamConfigurationTypeDef = TypedDict(
     "_RequiredStreamConfigurationTypeDef",
     {
         "StreamArn": str,
         "StreamChannelDefinition": StreamChannelDefinitionTypeDef,
     },
 )
@@ -1030,22 +835,14 @@
 )
 
 class StreamConfigurationTypeDef(
     _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
-KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef = TypedDict(
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef",
-    {
-        "Streams": List[RecordingStreamConfigurationTypeDef],
-        "FragmentSelector": FragmentSelectorOutputTypeDef,
-    },
-)
-
 _RequiredCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
     "_RequiredCompositedVideoArtifactsConfigurationTypeDef",
     {
         "GridViewConfiguration": GridViewConfigurationTypeDef,
     },
 )
 _OptionalCompositedVideoArtifactsConfigurationTypeDef = TypedDict(
@@ -1059,23 +856,14 @@
 
 class CompositedVideoArtifactsConfigurationTypeDef(
     _RequiredCompositedVideoArtifactsConfigurationTypeDef,
     _OptionalCompositedVideoArtifactsConfigurationTypeDef,
 ):
     pass
 
-RealTimeAlertConfigurationOutputTypeDef = TypedDict(
-    "RealTimeAlertConfigurationOutputTypeDef",
-    {
-        "Disabled": bool,
-        "Rules": List[RealTimeAlertRuleOutputTypeDef],
-    },
-    total=False,
-)
-
 RealTimeAlertConfigurationTypeDef = TypedDict(
     "RealTimeAlertConfigurationTypeDef",
     {
         "Disabled": bool,
         "Rules": Sequence[RealTimeAlertRuleTypeDef],
     },
     total=False,
@@ -1085,35 +873,22 @@
     "FragmentSelectorTypeDef",
     {
         "FragmentSelectorType": FragmentSelectorTypeType,
         "TimestampRange": TimestampRangeTypeDef,
     },
 )
 
-MediaInsightsPipelineConfigurationElementUnionTypeDef = Union[
-    MediaInsightsPipelineConfigurationElementTypeDef,
-    MediaInsightsPipelineConfigurationElementOutputTypeDef,
-]
 MediaCapturePipelineSourceConfigurationTypeDef = TypedDict(
     "MediaCapturePipelineSourceConfigurationTypeDef",
     {
         "MediaPipelineArn": str,
         "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConcatenationConfigurationTypeDef,
     },
 )
 
-KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef = TypedDict(
-    "KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef",
-    {
-        "Streams": List[StreamConfigurationOutputTypeDef],
-        "MediaEncoding": Literal["pcm"],
-        "MediaSampleRate": int,
-    },
-)
-
 KinesisVideoStreamSourceRuntimeConfigurationTypeDef = TypedDict(
     "KinesisVideoStreamSourceRuntimeConfigurationTypeDef",
     {
         "Streams": Sequence[StreamConfigurationTypeDef],
         "MediaEncoding": Literal["pcm"],
         "MediaSampleRate": int,
     },
@@ -1136,36 +911,14 @@
 )
 
 class ArtifactsConfigurationTypeDef(
     _RequiredArtifactsConfigurationTypeDef, _OptionalArtifactsConfigurationTypeDef
 ):
     pass
 
-_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
-    "_RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
-    {
-        "Arn": str,
-        "MuxType": LiveConnectorMuxTypeType,
-    },
-)
-_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef = TypedDict(
-    "_OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef",
-    {
-        "CompositedVideo": CompositedVideoArtifactsConfigurationTypeDef,
-        "SourceConfiguration": SourceConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-class ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef(
-    _RequiredChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
-    _OptionalChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef = TypedDict(
     "_RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef",
     {
         "Arn": str,
         "MuxType": LiveConnectorMuxTypeType,
     },
 )
@@ -1180,46 +933,20 @@
 
 class ChimeSdkMeetingLiveConnectorConfigurationTypeDef(
     _RequiredChimeSdkMeetingLiveConnectorConfigurationTypeDef,
     _OptionalChimeSdkMeetingLiveConnectorConfigurationTypeDef,
 ):
     pass
 
-MediaInsightsPipelineConfigurationTypeDef = TypedDict(
-    "MediaInsightsPipelineConfigurationTypeDef",
-    {
-        "MediaInsightsPipelineConfigurationName": str,
-        "MediaInsightsPipelineConfigurationArn": str,
-        "ResourceAccessRoleArn": str,
-        "RealTimeAlertConfiguration": RealTimeAlertConfigurationOutputTypeDef,
-        "Elements": List[MediaInsightsPipelineConfigurationElementOutputTypeDef],
-        "MediaInsightsPipelineConfigurationId": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-    },
-    total=False,
-)
-
-RealTimeAlertConfigurationUnionTypeDef = Union[
-    RealTimeAlertConfigurationTypeDef, RealTimeAlertConfigurationOutputTypeDef
-]
-KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
-    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
-    {
-        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
-        "FragmentSelector": FragmentSelectorTypeDef,
-    },
-)
-
 _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "MediaInsightsPipelineConfigurationName": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
     },
 )
 _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
@@ -1230,20 +957,35 @@
 
 class CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
+MediaInsightsPipelineConfigurationTypeDef = TypedDict(
+    "MediaInsightsPipelineConfigurationTypeDef",
+    {
+        "MediaInsightsPipelineConfigurationName": str,
+        "MediaInsightsPipelineConfigurationArn": str,
+        "ResourceAccessRoleArn": str,
+        "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
+        "Elements": List[MediaInsightsPipelineConfigurationElementTypeDef],
+        "MediaInsightsPipelineConfigurationId": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+    },
+    total=False,
+)
+
 _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "Identifier": str,
         "ResourceAccessRoleArn": str,
-        "Elements": Sequence[MediaInsightsPipelineConfigurationElementUnionTypeDef],
+        "Elements": Sequence[MediaInsightsPipelineConfigurationElementTypeDef],
     },
 )
 _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef",
     {
         "RealTimeAlertConfiguration": RealTimeAlertConfigurationTypeDef,
     },
@@ -1252,74 +994,39 @@
 
 class UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef(
     _RequiredUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
     _OptionalUpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef,
 ):
     pass
 
-ConcatenationSourceTypeDef = TypedDict(
-    "ConcatenationSourceTypeDef",
-    {
-        "Type": Literal["MediaCapturePipeline"],
-        "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
-    },
-)
-
-MediaInsightsPipelineTypeDef = TypedDict(
-    "MediaInsightsPipelineTypeDef",
+KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = TypedDict(
+    "KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef",
     {
-        "MediaPipelineId": str,
-        "MediaPipelineArn": str,
-        "MediaInsightsPipelineConfigurationArn": str,
-        "Status": MediaPipelineStatusType,
-        "KinesisVideoStreamSourceRuntimeConfiguration": (
-            KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef
-        ),
-        "MediaInsightsRuntimeMetadata": Dict[str, str],
-        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
-            KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef
-        ),
-        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
-        "CreatedTimestamp": datetime,
+        "Streams": Sequence[RecordingStreamConfigurationTypeDef],
+        "FragmentSelector": FragmentSelectorTypeDef,
     },
-    total=False,
 )
 
-KinesisVideoStreamSourceRuntimeConfigurationUnionTypeDef = Union[
-    KinesisVideoStreamSourceRuntimeConfigurationTypeDef,
-    KinesisVideoStreamSourceRuntimeConfigurationOutputTypeDef,
-]
-ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
-    "ChimeSdkMeetingConfigurationOutputTypeDef",
+ConcatenationSourceTypeDef = TypedDict(
+    "ConcatenationSourceTypeDef",
     {
-        "SourceConfiguration": SourceConfigurationOutputTypeDef,
-        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
+        "Type": Literal["MediaCapturePipeline"],
+        "MediaCapturePipelineSourceConfiguration": MediaCapturePipelineSourceConfigurationTypeDef,
     },
-    total=False,
 )
 
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
-LiveConnectorSourceConfigurationOutputTypeDef = TypedDict(
-    "LiveConnectorSourceConfigurationOutputTypeDef",
-    {
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "ChimeSdkMeetingLiveConnectorConfiguration": (
-            ChimeSdkMeetingLiveConnectorConfigurationOutputTypeDef
-        ),
-    },
-)
-
 LiveConnectorSourceConfigurationTypeDef = TypedDict(
     "LiveConnectorSourceConfigurationTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "ChimeSdkMeetingLiveConnectorConfiguration": (
             ChimeSdkMeetingLiveConnectorConfigurationTypeDef
         ),
@@ -1375,18 +1082,34 @@
 
 class CreateMediaInsightsPipelineRequestRequestTypeDef(
     _RequiredCreateMediaInsightsPipelineRequestRequestTypeDef,
     _OptionalCreateMediaInsightsPipelineRequestRequestTypeDef,
 ):
     pass
 
-KinesisVideoStreamRecordingSourceRuntimeConfigurationUnionTypeDef = Union[
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef,
-    KinesisVideoStreamRecordingSourceRuntimeConfigurationOutputTypeDef,
-]
+MediaInsightsPipelineTypeDef = TypedDict(
+    "MediaInsightsPipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "MediaPipelineArn": str,
+        "MediaInsightsPipelineConfigurationArn": str,
+        "Status": MediaPipelineStatusType,
+        "KinesisVideoStreamSourceRuntimeConfiguration": (
+            KinesisVideoStreamSourceRuntimeConfigurationTypeDef
+        ),
+        "MediaInsightsRuntimeMetadata": Dict[str, str],
+        "KinesisVideoStreamRecordingSourceRuntimeConfiguration": (
+            KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef
+        ),
+        "S3RecordingSinkRuntimeConfiguration": S3RecordingSinkRuntimeConfigurationTypeDef,
+        "CreatedTimestamp": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaConcatenationPipelineRequestRequestTypeDef",
     {
         "Sources": Sequence[ConcatenationSourceTypeDef],
         "Sinks": Sequence[ConcatenationSinkTypeDef],
     },
 )
@@ -1415,84 +1138,100 @@
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
-    "CreateMediaInsightsPipelineResponseTypeDef",
+_RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
-        "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
     },
 )
+_OptionalCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaCapturePipelineRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateMediaCapturePipelineRequestRequestTypeDef(
+    _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
+    _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
+):
+    pass
 
 MediaCapturePipelineTypeDef = TypedDict(
     "MediaCapturePipelineTypeDef",
     {
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "Status": MediaPipelineStatusType,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
     },
     total=False,
 )
 
-ChimeSdkMeetingConfigurationUnionTypeDef = Union[
-    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
-]
-_RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
+_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
+        "Sources": Sequence[LiveConnectorSourceConfigurationTypeDef],
+        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
     },
 )
-_OptionalCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaCapturePipelineRequestRequestTypeDef",
+_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class CreateMediaCapturePipelineRequestRequestTypeDef(
-    _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
-    _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
+class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
+    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
+    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
 ):
     pass
 
 MediaLiveConnectorPipelineTypeDef = TypedDict(
     "MediaLiveConnectorPipelineTypeDef",
     {
-        "Sources": List[LiveConnectorSourceConfigurationOutputTypeDef],
+        "Sources": List[LiveConnectorSourceConfigurationTypeDef],
         "Sinks": List[LiveConnectorSinkConfigurationTypeDef],
         "MediaPipelineId": str,
         "MediaPipelineArn": str,
         "Status": MediaPipelineStatusType,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-LiveConnectorSourceConfigurationUnionTypeDef = Union[
-    LiveConnectorSourceConfigurationTypeDef, LiveConnectorSourceConfigurationOutputTypeDef
-]
+CreateMediaInsightsPipelineResponseTypeDef = TypedDict(
+    "CreateMediaInsightsPipelineResponseTypeDef",
+    {
+        "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateMediaConcatenationPipelineResponseTypeDef = TypedDict(
     "CreateMediaConcatenationPipelineResponseTypeDef",
     {
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1528,36 +1267,14 @@
         "MediaLiveConnectorPipeline": MediaLiveConnectorPipelineTypeDef,
         "MediaConcatenationPipeline": MediaConcatenationPipelineTypeDef,
         "MediaInsightsPipeline": MediaInsightsPipelineTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
-    {
-        "Sources": Sequence[LiveConnectorSourceConfigurationUnionTypeDef],
-        "Sinks": Sequence[LiveConnectorSinkConfigurationTypeDef],
-    },
-)
-_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateMediaLiveConnectorPipelineRequestRequestTypeDef(
-    _RequiredCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
-    _OptionalCreateMediaLiveConnectorPipelineRequestRequestTypeDef,
-):
-    pass
-
 GetMediaPipelineResponseTypeDef = TypedDict(
     "GetMediaPipelineResponseTypeDef",
     {
         "MediaPipeline": MediaPipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post1/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-media-pipelines-2.5.2.post2/types_aiobotocore_chime_sdk_media_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

