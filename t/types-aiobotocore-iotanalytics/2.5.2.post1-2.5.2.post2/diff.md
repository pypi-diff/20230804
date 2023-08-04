# Comparing `tmp/types-aiobotocore-iotanalytics-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iotanalytics-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotanalytics-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotanalytics-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
```

## Comparing `types-aiobotocore-iotanalytics-2.5.2.post1.tar` & `types-aiobotocore-iotanalytics-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.417563 types-aiobotocore-iotanalytics-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-08-02 14:52:26.409563 types-aiobotocore-iotanalytics-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18086 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.417563 types-aiobotocore-iotanalytics-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.409563 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28217 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28169 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9106 2023-08-02 14:40:42.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-08-02 14:40:42.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52421 2023-08-02 14:40:43.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52341 2023-08-02 14:40:42.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:41.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.409563 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:26.000000 types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.386643 types-aiobotocore-iotanalytics-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13735 2023-08-04 13:59:12.386643 types-aiobotocore-iotanalytics-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12197 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.386643 types-aiobotocore-iotanalytics-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.386643 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1473 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1472 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28127 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    28079 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9201 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9199 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6582 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6575 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    46249 2023-08-04 13:40:55.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    46178 2023-08-04 13:40:54.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:53.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.386643 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13735 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:12.000000 types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/LICENSE` & `types-aiobotocore-iotanalytics-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/setup.py` & `types-aiobotocore-iotanalytics-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotanalytics",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iotanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTAnalytics 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__init__.py` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__init__.pyi` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/__main__.py` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTAnalytics 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IoTAnalytics 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics\nOther"
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

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/client.py` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,43 +27,43 @@
     ListDatastoresPaginator,
     ListPipelinesPaginator,
 )
 from .type_defs import (
     BatchPutMessageResponseTypeDef,
     BlobTypeDef,
     ChannelMessagesTypeDef,
-    ChannelStorageUnionTypeDef,
+    ChannelStorageTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     CreatePipelineResponseTypeDef,
-    DatasetActionUnionTypeDef,
+    DatasetActionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetTriggerTypeDef,
-    DatastorePartitionsUnionTypeDef,
-    DatastoreStorageUnionTypeDef,
+    DatastorePartitionsTypeDef,
+    DatastoreStorageTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     DescribePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    FileFormatConfigurationUnionTypeDef,
+    FileFormatConfigurationTypeDef,
     GetDatasetContentResponseTypeDef,
     LateDataRuleTypeDef,
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LoggingOptionsTypeDef,
     MessageTypeDef,
-    PipelineActivityUnionTypeDef,
+    PipelineActivityTypeDef,
     RetentionPeriodTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     VersioningConfigurationTypeDef,
@@ -150,30 +150,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#close)
         """
 
     async def create_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageUnionTypeDef = ...,
+        channelStorage: ChannelStorageTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Used to create a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_channel)
         """
 
     async def create_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionUnionTypeDef],
+        actions: Sequence[DatasetActionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
@@ -195,32 +195,32 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_dataset_content)
         """
 
     async def create_datastore(
         self,
         *,
         datastoreName: str,
-        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
+        datastoreStorage: DatastoreStorageTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...,
-        datastorePartitions: DatastorePartitionsUnionTypeDef = ...
+        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...,
+        datastorePartitions: DatastorePartitionsTypeDef = ...
     ) -> CreateDatastoreResponseTypeDef:
         """
         Creates a data store, which is a repository for messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_datastore)
         """
 
     async def create_pipeline(
         self,
         *,
         pipelineName: str,
-        pipelineActivities: Sequence[PipelineActivityUnionTypeDef],
+        pipelineActivities: Sequence[PipelineActivityTypeDef],
         tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_pipeline)
@@ -409,15 +409,15 @@
         Sets or updates the IoT Analytics logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.put_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#put_logging_options)
         """
 
     async def run_pipeline_activity(
-        self, *, pipelineActivity: PipelineActivityUnionTypeDef, payloads: Sequence[BlobTypeDef]
+        self, *, pipelineActivity: PipelineActivityTypeDef, payloads: Sequence[BlobTypeDef]
     ) -> RunPipelineActivityResponseTypeDef:
         """
         Simulates the results of running a pipeline activity on a message payload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.run_pipeline_activity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#run_pipeline_activity)
         """
@@ -469,29 +469,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#untag_resource)
         """
 
     async def update_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageUnionTypeDef = ...,
+        channelStorage: ChannelStorageTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_channel)
         """
 
     async def update_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionUnionTypeDef],
+        actions: Sequence[DatasetActionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
@@ -502,26 +502,26 @@
         """
 
     async def update_datastore(
         self,
         *,
         datastoreName: str,
         retentionPeriod: RetentionPeriodTypeDef = ...,
-        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
-        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...
+        datastoreStorage: DatastoreStorageTypeDef = ...,
+        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_datastore)
         """
 
     async def update_pipeline(
-        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityUnionTypeDef]
+        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/client.pyi` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,43 +27,43 @@
     ListDatastoresPaginator,
     ListPipelinesPaginator,
 )
 from .type_defs import (
     BatchPutMessageResponseTypeDef,
     BlobTypeDef,
     ChannelMessagesTypeDef,
-    ChannelStorageUnionTypeDef,
+    ChannelStorageTypeDef,
     CreateChannelResponseTypeDef,
     CreateDatasetContentResponseTypeDef,
     CreateDatasetResponseTypeDef,
     CreateDatastoreResponseTypeDef,
     CreatePipelineResponseTypeDef,
-    DatasetActionUnionTypeDef,
+    DatasetActionTypeDef,
     DatasetContentDeliveryRuleTypeDef,
     DatasetTriggerTypeDef,
-    DatastorePartitionsUnionTypeDef,
-    DatastoreStorageUnionTypeDef,
+    DatastorePartitionsTypeDef,
+    DatastoreStorageTypeDef,
     DescribeChannelResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeDatastoreResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
     DescribePipelineResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    FileFormatConfigurationUnionTypeDef,
+    FileFormatConfigurationTypeDef,
     GetDatasetContentResponseTypeDef,
     LateDataRuleTypeDef,
     ListChannelsResponseTypeDef,
     ListDatasetContentsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListDatastoresResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LoggingOptionsTypeDef,
     MessageTypeDef,
-    PipelineActivityUnionTypeDef,
+    PipelineActivityTypeDef,
     RetentionPeriodTypeDef,
     RunPipelineActivityResponseTypeDef,
     SampleChannelDataResponseTypeDef,
     StartPipelineReprocessingResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     VersioningConfigurationTypeDef,
@@ -141,29 +141,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#close)
         """
     async def create_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageUnionTypeDef = ...,
+        channelStorage: ChannelStorageTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Used to create a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_channel)
         """
     async def create_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionUnionTypeDef],
+        actions: Sequence[DatasetActionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
@@ -183,31 +183,31 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_dataset_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_dataset_content)
         """
     async def create_datastore(
         self,
         *,
         datastoreName: str,
-        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
+        datastoreStorage: DatastoreStorageTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...,
-        datastorePartitions: DatastorePartitionsUnionTypeDef = ...
+        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...,
+        datastorePartitions: DatastorePartitionsTypeDef = ...
     ) -> CreateDatastoreResponseTypeDef:
         """
         Creates a data store, which is a repository for messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_datastore)
         """
     async def create_pipeline(
         self,
         *,
         pipelineName: str,
-        pipelineActivities: Sequence[PipelineActivityUnionTypeDef],
+        pipelineActivities: Sequence[PipelineActivityTypeDef],
         tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#create_pipeline)
@@ -376,15 +376,15 @@
         """
         Sets or updates the IoT Analytics logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.put_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#put_logging_options)
         """
     async def run_pipeline_activity(
-        self, *, pipelineActivity: PipelineActivityUnionTypeDef, payloads: Sequence[BlobTypeDef]
+        self, *, pipelineActivity: PipelineActivityTypeDef, payloads: Sequence[BlobTypeDef]
     ) -> RunPipelineActivityResponseTypeDef:
         """
         Simulates the results of running a pipeline activity on a message payload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.run_pipeline_activity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#run_pipeline_activity)
         """
@@ -431,28 +431,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#untag_resource)
         """
     async def update_channel(
         self,
         *,
         channelName: str,
-        channelStorage: ChannelStorageUnionTypeDef = ...,
+        channelStorage: ChannelStorageTypeDef = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_channel)
         """
     async def update_dataset(
         self,
         *,
         datasetName: str,
-        actions: Sequence[DatasetActionUnionTypeDef],
+        actions: Sequence[DatasetActionTypeDef],
         triggers: Sequence[DatasetTriggerTypeDef] = ...,
         contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,
         retentionPeriod: RetentionPeriodTypeDef = ...,
         versioningConfiguration: VersioningConfigurationTypeDef = ...,
         lateDataRules: Sequence[LateDataRuleTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
@@ -462,25 +462,25 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_dataset)
         """
     async def update_datastore(
         self,
         *,
         datastoreName: str,
         retentionPeriod: RetentionPeriodTypeDef = ...,
-        datastoreStorage: DatastoreStorageUnionTypeDef = ...,
-        fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...
+        datastoreStorage: DatastoreStorageTypeDef = ...,
+        fileFormatConfiguration: FileFormatConfigurationTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to update the settings of a data store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_datastore)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_datastore)
         """
     async def update_pipeline(
-        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityUnionTypeDef]
+        self, *, pipelineName: str, pipelineActivities: Sequence[PipelineActivityTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the settings of a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/literals.py` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
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
@@ -171,14 +172,15 @@
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
@@ -257,26 +259,28 @@
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

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/literals.pyi` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
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
@@ -169,14 +170,15 @@
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
@@ -255,26 +257,28 @@
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

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/paginator.py` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/paginator.pyi` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/type_defs.py` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotanalytics service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityOutputTypeDef
+    from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityTypeDef
 
-    data: AddAttributesActivityOutputTypeDef = ...
+    data: AddAttributesActivityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -35,25 +35,24 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AddAttributesActivityOutputTypeDef",
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "ResponseMetadataTypeDef",
     "BlobTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
-    "CustomerManagedChannelS3StorageTypeDef",
     "CustomerManagedChannelS3StorageSummaryTypeDef",
+    "CustomerManagedChannelS3StorageTypeDef",
     "RetentionPeriodTypeDef",
     "ColumnTypeDef",
     "ResourceConfigurationTypeDef",
     "TagTypeDef",
     "CreateDatasetContentRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
@@ -93,37 +92,33 @@
     "TimestampTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListDatastoresRequestRequestTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MathActivityTypeDef",
     "OutputFileUriValueTypeDef",
-    "RemoveAttributesActivityOutputTypeDef",
-    "SelectAttributesActivityOutputTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchPutMessageResponseTypeDef",
     "CreateDatasetContentResponseTypeDef",
     "CreatePipelineResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "RunPipelineActivityResponseTypeDef",
     "SampleChannelDataResponseTypeDef",
     "StartPipelineReprocessingResponseTypeDef",
     "MessageTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
-    "ChannelStorageOutputTypeDef",
-    "ChannelStorageTypeDef",
     "ChannelStorageSummaryTypeDef",
+    "ChannelStorageTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
-    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatasetContentSummaryTypeDef",
     "GetDatasetContentResponseTypeDef",
     "DatasetTriggerTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
@@ -139,91 +134,55 @@
     "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     "ListDatasetContentsRequestRequestTypeDef",
     "SampleChannelDataRequestRequestTypeDef",
     "StartPipelineReprocessingRequestRequestTypeDef",
     "VariableTypeDef",
-    "PipelineActivityOutputTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
     "BatchPutMessageRequestRequestTypeDef",
+    "ChannelSummaryTypeDef",
     "ChannelTypeDef",
-    "ChannelStorageUnionTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "ChannelSummaryTypeDef",
-    "ParquetConfigurationOutputTypeDef",
     "ParquetConfigurationTypeDef",
     "ListDatasetContentsResponseTypeDef",
     "DatasetSummaryTypeDef",
     "DatastoreStorageSummaryTypeDef",
-    "DatastoreStorageOutputTypeDef",
     "DatastoreStorageTypeDef",
-    "DatastorePartitionsOutputTypeDef",
     "DatastorePartitionsTypeDef",
     "LateDataRuleTypeDef",
-    "SqlQueryDatasetActionOutputTypeDef",
     "SqlQueryDatasetActionTypeDef",
     "DatasetContentDeliveryDestinationTypeDef",
-    "ContainerDatasetActionOutputTypeDef",
     "ContainerDatasetActionTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
     "PipelineTypeDef",
-    "PipelineActivityUnionTypeDef",
     "RunPipelineActivityRequestRequestTypeDef",
+    "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
-    "DescribeChannelResponseTypeDef",
     "ListChannelsResponseTypeDef",
-    "FileFormatConfigurationOutputTypeDef",
+    "DescribeChannelResponseTypeDef",
     "FileFormatConfigurationTypeDef",
     "ListDatasetsResponseTypeDef",
-    "DatastoreStorageUnionTypeDef",
     "DatastoreSummaryTypeDef",
-    "DatastorePartitionsUnionTypeDef",
     "DatasetContentDeliveryRuleTypeDef",
-    "DatasetActionOutputTypeDef",
     "DatasetActionTypeDef",
     "DescribePipelineResponseTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
-    "UpdatePipelineRequestRequestTypeDef",
-    "DatastoreTypeDef",
     "CreateDatastoreRequestRequestTypeDef",
-    "FileFormatConfigurationUnionTypeDef",
+    "DatastoreTypeDef",
     "UpdateDatastoreRequestRequestTypeDef",
     "ListDatastoresResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
-    "DatasetActionUnionTypeDef",
+    "UpdateDatasetRequestRequestTypeDef",
     "DescribeDatastoreResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "UpdateDatasetRequestRequestTypeDef",
 )
 
-_RequiredAddAttributesActivityOutputTypeDef = TypedDict(
-    "_RequiredAddAttributesActivityOutputTypeDef",
-    {
-        "name": str,
-        "attributes": Dict[str, str],
-    },
-)
-_OptionalAddAttributesActivityOutputTypeDef = TypedDict(
-    "_OptionalAddAttributesActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-
-class AddAttributesActivityOutputTypeDef(
-    _RequiredAddAttributesActivityOutputTypeDef, _OptionalAddAttributesActivityOutputTypeDef
-):
-    pass
-
-
 _RequiredAddAttributesActivityTypeDef = TypedDict(
     "_RequiredAddAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
 )
@@ -305,14 +264,24 @@
     {
         "estimatedSizeInBytes": float,
         "estimatedOn": datetime,
     },
     total=False,
 )
 
+CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
+    "CustomerManagedChannelS3StorageSummaryTypeDef",
+    {
+        "bucket": str,
+        "keyPrefix": str,
+        "roleArn": str,
+    },
+    total=False,
+)
+
 _RequiredCustomerManagedChannelS3StorageTypeDef = TypedDict(
     "_RequiredCustomerManagedChannelS3StorageTypeDef",
     {
         "bucket": str,
         "roleArn": str,
     },
 )
@@ -327,24 +296,14 @@
 
 class CustomerManagedChannelS3StorageTypeDef(
     _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
 ):
     pass
 
 
-CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
-    "CustomerManagedChannelS3StorageSummaryTypeDef",
-    {
-        "bucket": str,
-        "keyPrefix": str,
-        "roleArn": str,
-    },
-    total=False,
-)
-
 RetentionPeriodTypeDef = TypedDict(
     "RetentionPeriodTypeDef",
     {
         "unlimited": bool,
         "numberOfDays": int,
     },
     total=False,
@@ -888,58 +847,14 @@
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
     },
 )
 
-_RequiredRemoveAttributesActivityOutputTypeDef = TypedDict(
-    "_RequiredRemoveAttributesActivityOutputTypeDef",
-    {
-        "name": str,
-        "attributes": List[str],
-    },
-)
-_OptionalRemoveAttributesActivityOutputTypeDef = TypedDict(
-    "_OptionalRemoveAttributesActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-
-class RemoveAttributesActivityOutputTypeDef(
-    _RequiredRemoveAttributesActivityOutputTypeDef, _OptionalRemoveAttributesActivityOutputTypeDef
-):
-    pass
-
-
-_RequiredSelectAttributesActivityOutputTypeDef = TypedDict(
-    "_RequiredSelectAttributesActivityOutputTypeDef",
-    {
-        "name": str,
-        "attributes": List[str],
-    },
-)
-_OptionalSelectAttributesActivityOutputTypeDef = TypedDict(
-    "_OptionalSelectAttributesActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-
-class SelectAttributesActivityOutputTypeDef(
-    _RequiredSelectAttributesActivityOutputTypeDef, _OptionalSelectAttributesActivityOutputTypeDef
-):
-    pass
-
-
 _RequiredRemoveAttributesActivityTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -1075,41 +990,32 @@
     "DatastoreStatisticsTypeDef",
     {
         "size": EstimatedResourceSizeTypeDef,
     },
     total=False,
 )
 
-ChannelStorageOutputTypeDef = TypedDict(
-    "ChannelStorageOutputTypeDef",
+ChannelStorageSummaryTypeDef = TypedDict(
+    "ChannelStorageSummaryTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
+        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
     },
     total=False,
 )
 
 ChannelStorageTypeDef = TypedDict(
     "ChannelStorageTypeDef",
     {
         "serviceManagedS3": Mapping[str, Any],
         "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
     },
     total=False,
 )
 
-ChannelStorageSummaryTypeDef = TypedDict(
-    "ChannelStorageSummaryTypeDef",
-    {
-        "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
-    },
-    total=False,
-)
-
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channelName": str,
         "channelArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1132,22 +1038,14 @@
         "datastoreName": str,
         "datastoreArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SchemaDefinitionOutputTypeDef = TypedDict(
-    "SchemaDefinitionOutputTypeDef",
-    {
-        "columns": List[ColumnTypeDef],
-    },
-    total=False,
-)
-
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnTypeDef],
     },
     total=False,
 )
@@ -1423,31 +1321,14 @@
 )
 
 
 class VariableTypeDef(_RequiredVariableTypeDef, _OptionalVariableTypeDef):
     pass
 
 
-PipelineActivityOutputTypeDef = TypedDict(
-    "PipelineActivityOutputTypeDef",
-    {
-        "channel": ChannelActivityTypeDef,
-        "lambda": LambdaActivityTypeDef,
-        "datastore": DatastoreActivityTypeDef,
-        "addAttributes": AddAttributesActivityOutputTypeDef,
-        "removeAttributes": RemoveAttributesActivityOutputTypeDef,
-        "selectAttributes": SelectAttributesActivityOutputTypeDef,
-        "filter": FilterActivityTypeDef,
-        "math": MathActivityTypeDef,
-        "deviceRegistryEnrich": DeviceRegistryEnrichActivityTypeDef,
-        "deviceShadowEnrich": DeviceShadowEnrichActivityTypeDef,
-    },
-    total=False,
-)
-
 PipelineActivityTypeDef = TypedDict(
     "PipelineActivityTypeDef",
     {
         "channel": ChannelActivityTypeDef,
         "lambda": LambdaActivityTypeDef,
         "datastore": DatastoreActivityTypeDef,
         "addAttributes": AddAttributesActivityTypeDef,
@@ -1476,30 +1357,42 @@
     "BatchPutMessageRequestRequestTypeDef",
     {
         "channelName": str,
         "messages": Sequence[MessageTypeDef],
     },
 )
 
+ChannelSummaryTypeDef = TypedDict(
+    "ChannelSummaryTypeDef",
+    {
+        "channelName": str,
+        "channelStorage": ChannelStorageSummaryTypeDef,
+        "status": ChannelStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "lastMessageArrivalTime": datetime,
+    },
+    total=False,
+)
+
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "name": str,
-        "storage": ChannelStorageOutputTypeDef,
+        "storage": ChannelStorageTypeDef,
         "arn": str,
         "status": ChannelStatusType,
         "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
-ChannelStorageUnionTypeDef = Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef]
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalCreateChannelRequestRequestTypeDef = TypedDict(
@@ -1537,35 +1430,14 @@
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
 
-ChannelSummaryTypeDef = TypedDict(
-    "ChannelSummaryTypeDef",
-    {
-        "channelName": str,
-        "channelStorage": ChannelStorageSummaryTypeDef,
-        "status": ChannelStatusType,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "lastMessageArrivalTime": datetime,
-    },
-    total=False,
-)
-
-ParquetConfigurationOutputTypeDef = TypedDict(
-    "ParquetConfigurationOutputTypeDef",
-    {
-        "schemaDefinition": SchemaDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
 ParquetConfigurationTypeDef = TypedDict(
     "ParquetConfigurationTypeDef",
     {
         "schemaDefinition": SchemaDefinitionTypeDef,
     },
     total=False,
 )
@@ -1598,42 +1470,24 @@
         "serviceManagedS3": Dict[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageSummaryTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     },
     total=False,
 )
 
-DatastoreStorageOutputTypeDef = TypedDict(
-    "DatastoreStorageOutputTypeDef",
-    {
-        "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
-        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
-    },
-    total=False,
-)
-
 DatastoreStorageTypeDef = TypedDict(
     "DatastoreStorageTypeDef",
     {
         "serviceManagedS3": Mapping[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     },
     total=False,
 )
 
-DatastorePartitionsOutputTypeDef = TypedDict(
-    "DatastorePartitionsOutputTypeDef",
-    {
-        "partitions": List[DatastorePartitionTypeDef],
-    },
-    total=False,
-)
-
 DatastorePartitionsTypeDef = TypedDict(
     "DatastorePartitionsTypeDef",
     {
         "partitions": Sequence[DatastorePartitionTypeDef],
     },
     total=False,
 )
@@ -1653,35 +1507,14 @@
 )
 
 
 class LateDataRuleTypeDef(_RequiredLateDataRuleTypeDef, _OptionalLateDataRuleTypeDef):
     pass
 
 
-_RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
-    "_RequiredSqlQueryDatasetActionOutputTypeDef",
-    {
-        "sqlQuery": str,
-    },
-)
-_OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
-    "_OptionalSqlQueryDatasetActionOutputTypeDef",
-    {
-        "filters": List[QueryFilterTypeDef],
-    },
-    total=False,
-)
-
-
-class SqlQueryDatasetActionOutputTypeDef(
-    _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
-):
-    pass
-
-
 _RequiredSqlQueryDatasetActionTypeDef = TypedDict(
     "_RequiredSqlQueryDatasetActionTypeDef",
     {
         "sqlQuery": str,
     },
 )
 _OptionalSqlQueryDatasetActionTypeDef = TypedDict(
@@ -1704,116 +1537,113 @@
     {
         "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationTypeDef,
         "s3DestinationConfiguration": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredContainerDatasetActionOutputTypeDef = TypedDict(
-    "_RequiredContainerDatasetActionOutputTypeDef",
+_RequiredContainerDatasetActionTypeDef = TypedDict(
+    "_RequiredContainerDatasetActionTypeDef",
     {
         "image": str,
         "executionRoleArn": str,
         "resourceConfiguration": ResourceConfigurationTypeDef,
     },
 )
-_OptionalContainerDatasetActionOutputTypeDef = TypedDict(
-    "_OptionalContainerDatasetActionOutputTypeDef",
+_OptionalContainerDatasetActionTypeDef = TypedDict(
+    "_OptionalContainerDatasetActionTypeDef",
     {
-        "variables": List[VariableTypeDef],
+        "variables": Sequence[VariableTypeDef],
     },
     total=False,
 )
 
 
-class ContainerDatasetActionOutputTypeDef(
-    _RequiredContainerDatasetActionOutputTypeDef, _OptionalContainerDatasetActionOutputTypeDef
+class ContainerDatasetActionTypeDef(
+    _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
 ):
     pass
 
 
-_RequiredContainerDatasetActionTypeDef = TypedDict(
-    "_RequiredContainerDatasetActionTypeDef",
+_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePipelineRequestRequestTypeDef",
     {
-        "image": str,
-        "executionRoleArn": str,
-        "resourceConfiguration": ResourceConfigurationTypeDef,
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityTypeDef],
     },
 )
-_OptionalContainerDatasetActionTypeDef = TypedDict(
-    "_OptionalContainerDatasetActionTypeDef",
+_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePipelineRequestRequestTypeDef",
     {
-        "variables": Sequence[VariableTypeDef],
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class ContainerDatasetActionTypeDef(
-    _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
+class CreatePipelineRequestRequestTypeDef(
+    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
 
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "name": str,
         "arn": str,
-        "activities": List[PipelineActivityOutputTypeDef],
+        "activities": List[PipelineActivityTypeDef],
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
-PipelineActivityUnionTypeDef = Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
 RunPipelineActivityRequestRequestTypeDef = TypedDict(
     "RunPipelineActivityRequestRequestTypeDef",
     {
         "pipelineActivity": PipelineActivityTypeDef,
         "payloads": Sequence[BlobTypeDef],
     },
 )
 
-ListPipelinesResponseTypeDef = TypedDict(
-    "ListPipelinesResponseTypeDef",
+UpdatePipelineRequestRequestTypeDef = TypedDict(
+    "UpdatePipelineRequestRequestTypeDef",
     {
-        "pipelineSummaries": List[PipelineSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityTypeDef],
     },
 )
 
-DescribeChannelResponseTypeDef = TypedDict(
-    "DescribeChannelResponseTypeDef",
+ListPipelinesResponseTypeDef = TypedDict(
+    "ListPipelinesResponseTypeDef",
     {
-        "channel": ChannelTypeDef,
-        "statistics": ChannelStatisticsTypeDef,
+        "pipelineSummaries": List[PipelineSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channelSummaries": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FileFormatConfigurationOutputTypeDef = TypedDict(
-    "FileFormatConfigurationOutputTypeDef",
+DescribeChannelResponseTypeDef = TypedDict(
+    "DescribeChannelResponseTypeDef",
     {
-        "jsonConfiguration": Dict[str, Any],
-        "parquetConfiguration": ParquetConfigurationOutputTypeDef,
+        "channel": ChannelTypeDef,
+        "statistics": ChannelStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 FileFormatConfigurationTypeDef = TypedDict(
     "FileFormatConfigurationTypeDef",
     {
         "jsonConfiguration": Mapping[str, Any],
         "parquetConfiguration": ParquetConfigurationTypeDef,
@@ -1826,33 +1656,29 @@
     {
         "datasetSummaries": List[DatasetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatastoreStorageUnionTypeDef = Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef]
 DatastoreSummaryTypeDef = TypedDict(
     "DatastoreSummaryTypeDef",
     {
         "datastoreName": str,
         "datastoreStorage": DatastoreStorageSummaryTypeDef,
         "status": DatastoreStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
         "fileFormatType": FileFormatTypeType,
-        "datastorePartitions": DatastorePartitionsOutputTypeDef,
+        "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
-DatastorePartitionsUnionTypeDef = Union[
-    DatastorePartitionsTypeDef, DatastorePartitionsOutputTypeDef
-]
 _RequiredDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_RequiredDatasetContentDeliveryRuleTypeDef",
     {
         "destination": DatasetContentDeliveryDestinationTypeDef,
     },
 )
 _OptionalDatasetContentDeliveryRuleTypeDef = TypedDict(
@@ -1866,24 +1692,14 @@
 
 class DatasetContentDeliveryRuleTypeDef(
     _RequiredDatasetContentDeliveryRuleTypeDef, _OptionalDatasetContentDeliveryRuleTypeDef
 ):
     pass
 
 
-DatasetActionOutputTypeDef = TypedDict(
-    "DatasetActionOutputTypeDef",
-    {
-        "actionName": str,
-        "queryAction": SqlQueryDatasetActionOutputTypeDef,
-        "containerAction": ContainerDatasetActionOutputTypeDef,
-    },
-    total=False,
-)
-
 DatasetActionTypeDef = TypedDict(
     "DatasetActionTypeDef",
     {
         "actionName": str,
         "queryAction": SqlQueryDatasetActionTypeDef,
         "containerAction": ContainerDatasetActionTypeDef,
     },
@@ -1894,89 +1710,56 @@
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePipelineRequestRequestTypeDef",
+_RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatastoreRequestRequestTypeDef",
     {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
+        "datastoreName": str,
     },
 )
-_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePipelineRequestRequestTypeDef",
+_OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatastoreRequestRequestTypeDef",
     {
+        "datastoreStorage": DatastoreStorageTypeDef,
+        "retentionPeriod": RetentionPeriodTypeDef,
         "tags": Sequence[TagTypeDef],
+        "fileFormatConfiguration": FileFormatConfigurationTypeDef,
+        "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
 
-class CreatePipelineRequestRequestTypeDef(
-    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
+class CreateDatastoreRequestRequestTypeDef(
+    _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
 ):
     pass
 
 
-UpdatePipelineRequestRequestTypeDef = TypedDict(
-    "UpdatePipelineRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
-    },
-)
-
 DatastoreTypeDef = TypedDict(
     "DatastoreTypeDef",
     {
         "name": str,
-        "storage": DatastoreStorageOutputTypeDef,
+        "storage": DatastoreStorageTypeDef,
         "arn": str,
         "status": DatastoreStatusType,
         "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
-        "fileFormatConfiguration": FileFormatConfigurationOutputTypeDef,
-        "datastorePartitions": DatastorePartitionsOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatastoreRequestRequestTypeDef",
-    {
-        "datastoreName": str,
-    },
-)
-_OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatastoreRequestRequestTypeDef",
-    {
-        "datastoreStorage": DatastoreStorageTypeDef,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "tags": Sequence[TagTypeDef],
         "fileFormatConfiguration": FileFormatConfigurationTypeDef,
         "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
-
-class CreateDatastoreRequestRequestTypeDef(
-    _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
-):
-    pass
-
-
-FileFormatConfigurationUnionTypeDef = Union[
-    FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
-]
 _RequiredUpdateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
     },
 )
 _OptionalUpdateDatastoreRequestRequestTypeDef = TypedDict(
@@ -2001,55 +1784,19 @@
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "actions": List[DatasetActionOutputTypeDef],
-        "triggers": List[DatasetTriggerTypeDef],
-        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
-        "status": DatasetStatusType,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "versioningConfiguration": VersioningConfigurationTypeDef,
-        "lateDataRules": List[LateDataRuleTypeDef],
-    },
-    total=False,
-)
-
-DatasetActionUnionTypeDef = Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]
-DescribeDatastoreResponseTypeDef = TypedDict(
-    "DescribeDatastoreResponseTypeDef",
-    {
-        "datastore": DatastoreTypeDef,
-        "statistics": DatastoreStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionUnionTypeDef],
+        "actions": Sequence[DatasetActionTypeDef],
     },
 )
 _OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
@@ -2064,19 +1811,37 @@
 
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
 
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "actions": List[DatasetActionTypeDef],
+        "triggers": List[DatasetTriggerTypeDef],
+        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
+        "status": DatasetStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "versioningConfiguration": VersioningConfigurationTypeDef,
+        "lateDataRules": List[LateDataRuleTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionUnionTypeDef],
+        "actions": Sequence[DatasetActionTypeDef],
     },
 )
 _OptionalUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
@@ -2088,7 +1853,25 @@
 )
 
 
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
+
+
+DescribeDatastoreResponseTypeDef = TypedDict(
+    "DescribeDatastoreResponseTypeDef",
+    {
+        "datastore": DatastoreTypeDef,
+        "statistics": DatastoreStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "dataset": DatasetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics/type_defs.pyi` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iotanalytics service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotanalytics/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityOutputTypeDef
+    from types_aiobotocore_iotanalytics.type_defs import AddAttributesActivityTypeDef
 
-    data: AddAttributesActivityOutputTypeDef = ...
+    data: AddAttributesActivityTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -34,25 +34,24 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AddAttributesActivityOutputTypeDef",
     "AddAttributesActivityTypeDef",
     "BatchPutMessageErrorEntryTypeDef",
     "ResponseMetadataTypeDef",
     "BlobTypeDef",
     "CancelPipelineReprocessingRequestRequestTypeDef",
     "ChannelActivityTypeDef",
     "ChannelMessagesTypeDef",
     "EstimatedResourceSizeTypeDef",
-    "CustomerManagedChannelS3StorageTypeDef",
     "CustomerManagedChannelS3StorageSummaryTypeDef",
+    "CustomerManagedChannelS3StorageTypeDef",
     "RetentionPeriodTypeDef",
     "ColumnTypeDef",
     "ResourceConfigurationTypeDef",
     "TagTypeDef",
     "CreateDatasetContentRequestRequestTypeDef",
     "VersioningConfigurationTypeDef",
     "CustomerManagedDatastoreS3StorageSummaryTypeDef",
@@ -92,37 +91,33 @@
     "TimestampTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListDatastoresRequestRequestTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MathActivityTypeDef",
     "OutputFileUriValueTypeDef",
-    "RemoveAttributesActivityOutputTypeDef",
-    "SelectAttributesActivityOutputTypeDef",
     "RemoveAttributesActivityTypeDef",
     "SelectAttributesActivityTypeDef",
     "ReprocessingSummaryTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchPutMessageResponseTypeDef",
     "CreateDatasetContentResponseTypeDef",
     "CreatePipelineResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "RunPipelineActivityResponseTypeDef",
     "SampleChannelDataResponseTypeDef",
     "StartPipelineReprocessingResponseTypeDef",
     "MessageTypeDef",
     "ChannelStatisticsTypeDef",
     "DatastoreStatisticsTypeDef",
-    "ChannelStorageOutputTypeDef",
-    "ChannelStorageTypeDef",
     "ChannelStorageSummaryTypeDef",
+    "ChannelStorageTypeDef",
     "CreateChannelResponseTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateDatastoreResponseTypeDef",
-    "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatasetContentSummaryTypeDef",
     "GetDatasetContentResponseTypeDef",
     "DatasetTriggerTypeDef",
     "DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef",
@@ -138,89 +133,55 @@
     "ListDatastoresRequestListDatastoresPaginateTypeDef",
     "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListDatasetContentsRequestListDatasetContentsPaginateTypeDef",
     "ListDatasetContentsRequestRequestTypeDef",
     "SampleChannelDataRequestRequestTypeDef",
     "StartPipelineReprocessingRequestRequestTypeDef",
     "VariableTypeDef",
-    "PipelineActivityOutputTypeDef",
     "PipelineActivityTypeDef",
     "PipelineSummaryTypeDef",
     "BatchPutMessageRequestRequestTypeDef",
+    "ChannelSummaryTypeDef",
     "ChannelTypeDef",
-    "ChannelStorageUnionTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
-    "ChannelSummaryTypeDef",
-    "ParquetConfigurationOutputTypeDef",
     "ParquetConfigurationTypeDef",
     "ListDatasetContentsResponseTypeDef",
     "DatasetSummaryTypeDef",
     "DatastoreStorageSummaryTypeDef",
-    "DatastoreStorageOutputTypeDef",
     "DatastoreStorageTypeDef",
-    "DatastorePartitionsOutputTypeDef",
     "DatastorePartitionsTypeDef",
     "LateDataRuleTypeDef",
-    "SqlQueryDatasetActionOutputTypeDef",
     "SqlQueryDatasetActionTypeDef",
     "DatasetContentDeliveryDestinationTypeDef",
-    "ContainerDatasetActionOutputTypeDef",
     "ContainerDatasetActionTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
     "PipelineTypeDef",
-    "PipelineActivityUnionTypeDef",
     "RunPipelineActivityRequestRequestTypeDef",
+    "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
-    "DescribeChannelResponseTypeDef",
     "ListChannelsResponseTypeDef",
-    "FileFormatConfigurationOutputTypeDef",
+    "DescribeChannelResponseTypeDef",
     "FileFormatConfigurationTypeDef",
     "ListDatasetsResponseTypeDef",
-    "DatastoreStorageUnionTypeDef",
     "DatastoreSummaryTypeDef",
-    "DatastorePartitionsUnionTypeDef",
     "DatasetContentDeliveryRuleTypeDef",
-    "DatasetActionOutputTypeDef",
     "DatasetActionTypeDef",
     "DescribePipelineResponseTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
-    "UpdatePipelineRequestRequestTypeDef",
-    "DatastoreTypeDef",
     "CreateDatastoreRequestRequestTypeDef",
-    "FileFormatConfigurationUnionTypeDef",
+    "DatastoreTypeDef",
     "UpdateDatastoreRequestRequestTypeDef",
     "ListDatastoresResponseTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
     "DatasetTypeDef",
-    "DatasetActionUnionTypeDef",
+    "UpdateDatasetRequestRequestTypeDef",
     "DescribeDatastoreResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "UpdateDatasetRequestRequestTypeDef",
-)
-
-_RequiredAddAttributesActivityOutputTypeDef = TypedDict(
-    "_RequiredAddAttributesActivityOutputTypeDef",
-    {
-        "name": str,
-        "attributes": Dict[str, str],
-    },
-)
-_OptionalAddAttributesActivityOutputTypeDef = TypedDict(
-    "_OptionalAddAttributesActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
 )
 
-class AddAttributesActivityOutputTypeDef(
-    _RequiredAddAttributesActivityOutputTypeDef, _OptionalAddAttributesActivityOutputTypeDef
-):
-    pass
-
 _RequiredAddAttributesActivityTypeDef = TypedDict(
     "_RequiredAddAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Mapping[str, str],
     },
 )
@@ -298,14 +259,24 @@
     {
         "estimatedSizeInBytes": float,
         "estimatedOn": datetime,
     },
     total=False,
 )
 
+CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
+    "CustomerManagedChannelS3StorageSummaryTypeDef",
+    {
+        "bucket": str,
+        "keyPrefix": str,
+        "roleArn": str,
+    },
+    total=False,
+)
+
 _RequiredCustomerManagedChannelS3StorageTypeDef = TypedDict(
     "_RequiredCustomerManagedChannelS3StorageTypeDef",
     {
         "bucket": str,
         "roleArn": str,
     },
 )
@@ -318,24 +289,14 @@
 )
 
 class CustomerManagedChannelS3StorageTypeDef(
     _RequiredCustomerManagedChannelS3StorageTypeDef, _OptionalCustomerManagedChannelS3StorageTypeDef
 ):
     pass
 
-CustomerManagedChannelS3StorageSummaryTypeDef = TypedDict(
-    "CustomerManagedChannelS3StorageSummaryTypeDef",
-    {
-        "bucket": str,
-        "keyPrefix": str,
-        "roleArn": str,
-    },
-    total=False,
-)
-
 RetentionPeriodTypeDef = TypedDict(
     "RetentionPeriodTypeDef",
     {
         "unlimited": bool,
         "numberOfDays": int,
     },
     total=False,
@@ -853,54 +814,14 @@
 OutputFileUriValueTypeDef = TypedDict(
     "OutputFileUriValueTypeDef",
     {
         "fileName": str,
     },
 )
 
-_RequiredRemoveAttributesActivityOutputTypeDef = TypedDict(
-    "_RequiredRemoveAttributesActivityOutputTypeDef",
-    {
-        "name": str,
-        "attributes": List[str],
-    },
-)
-_OptionalRemoveAttributesActivityOutputTypeDef = TypedDict(
-    "_OptionalRemoveAttributesActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-class RemoveAttributesActivityOutputTypeDef(
-    _RequiredRemoveAttributesActivityOutputTypeDef, _OptionalRemoveAttributesActivityOutputTypeDef
-):
-    pass
-
-_RequiredSelectAttributesActivityOutputTypeDef = TypedDict(
-    "_RequiredSelectAttributesActivityOutputTypeDef",
-    {
-        "name": str,
-        "attributes": List[str],
-    },
-)
-_OptionalSelectAttributesActivityOutputTypeDef = TypedDict(
-    "_OptionalSelectAttributesActivityOutputTypeDef",
-    {
-        "next": str,
-    },
-    total=False,
-)
-
-class SelectAttributesActivityOutputTypeDef(
-    _RequiredSelectAttributesActivityOutputTypeDef, _OptionalSelectAttributesActivityOutputTypeDef
-):
-    pass
-
 _RequiredRemoveAttributesActivityTypeDef = TypedDict(
     "_RequiredRemoveAttributesActivityTypeDef",
     {
         "name": str,
         "attributes": Sequence[str],
     },
 )
@@ -1032,41 +953,32 @@
     "DatastoreStatisticsTypeDef",
     {
         "size": EstimatedResourceSizeTypeDef,
     },
     total=False,
 )
 
-ChannelStorageOutputTypeDef = TypedDict(
-    "ChannelStorageOutputTypeDef",
+ChannelStorageSummaryTypeDef = TypedDict(
+    "ChannelStorageSummaryTypeDef",
     {
         "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
+        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
     },
     total=False,
 )
 
 ChannelStorageTypeDef = TypedDict(
     "ChannelStorageTypeDef",
     {
         "serviceManagedS3": Mapping[str, Any],
         "customerManagedS3": CustomerManagedChannelS3StorageTypeDef,
     },
     total=False,
 )
 
-ChannelStorageSummaryTypeDef = TypedDict(
-    "ChannelStorageSummaryTypeDef",
-    {
-        "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedChannelS3StorageSummaryTypeDef,
-    },
-    total=False,
-)
-
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "channelName": str,
         "channelArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1089,22 +1001,14 @@
         "datastoreName": str,
         "datastoreArn": str,
         "retentionPeriod": RetentionPeriodTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SchemaDefinitionOutputTypeDef = TypedDict(
-    "SchemaDefinitionOutputTypeDef",
-    {
-        "columns": List[ColumnTypeDef],
-    },
-    total=False,
-)
-
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
     {
         "columns": Sequence[ColumnTypeDef],
     },
     total=False,
 )
@@ -1368,31 +1272,14 @@
     },
     total=False,
 )
 
 class VariableTypeDef(_RequiredVariableTypeDef, _OptionalVariableTypeDef):
     pass
 
-PipelineActivityOutputTypeDef = TypedDict(
-    "PipelineActivityOutputTypeDef",
-    {
-        "channel": ChannelActivityTypeDef,
-        "lambda": LambdaActivityTypeDef,
-        "datastore": DatastoreActivityTypeDef,
-        "addAttributes": AddAttributesActivityOutputTypeDef,
-        "removeAttributes": RemoveAttributesActivityOutputTypeDef,
-        "selectAttributes": SelectAttributesActivityOutputTypeDef,
-        "filter": FilterActivityTypeDef,
-        "math": MathActivityTypeDef,
-        "deviceRegistryEnrich": DeviceRegistryEnrichActivityTypeDef,
-        "deviceShadowEnrich": DeviceShadowEnrichActivityTypeDef,
-    },
-    total=False,
-)
-
 PipelineActivityTypeDef = TypedDict(
     "PipelineActivityTypeDef",
     {
         "channel": ChannelActivityTypeDef,
         "lambda": LambdaActivityTypeDef,
         "datastore": DatastoreActivityTypeDef,
         "addAttributes": AddAttributesActivityTypeDef,
@@ -1421,30 +1308,42 @@
     "BatchPutMessageRequestRequestTypeDef",
     {
         "channelName": str,
         "messages": Sequence[MessageTypeDef],
     },
 )
 
+ChannelSummaryTypeDef = TypedDict(
+    "ChannelSummaryTypeDef",
+    {
+        "channelName": str,
+        "channelStorage": ChannelStorageSummaryTypeDef,
+        "status": ChannelStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "lastMessageArrivalTime": datetime,
+    },
+    total=False,
+)
+
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "name": str,
-        "storage": ChannelStorageOutputTypeDef,
+        "storage": ChannelStorageTypeDef,
         "arn": str,
         "status": ChannelStatusType,
         "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
     },
     total=False,
 )
 
-ChannelStorageUnionTypeDef = Union[ChannelStorageTypeDef, ChannelStorageOutputTypeDef]
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "channelName": str,
     },
 )
 _OptionalCreateChannelRequestRequestTypeDef = TypedDict(
@@ -1478,35 +1377,14 @@
 )
 
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-ChannelSummaryTypeDef = TypedDict(
-    "ChannelSummaryTypeDef",
-    {
-        "channelName": str,
-        "channelStorage": ChannelStorageSummaryTypeDef,
-        "status": ChannelStatusType,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "lastMessageArrivalTime": datetime,
-    },
-    total=False,
-)
-
-ParquetConfigurationOutputTypeDef = TypedDict(
-    "ParquetConfigurationOutputTypeDef",
-    {
-        "schemaDefinition": SchemaDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
 ParquetConfigurationTypeDef = TypedDict(
     "ParquetConfigurationTypeDef",
     {
         "schemaDefinition": SchemaDefinitionTypeDef,
     },
     total=False,
 )
@@ -1539,42 +1417,24 @@
         "serviceManagedS3": Dict[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageSummaryTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageSummaryTypeDef,
     },
     total=False,
 )
 
-DatastoreStorageOutputTypeDef = TypedDict(
-    "DatastoreStorageOutputTypeDef",
-    {
-        "serviceManagedS3": Dict[str, Any],
-        "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
-        "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
-    },
-    total=False,
-)
-
 DatastoreStorageTypeDef = TypedDict(
     "DatastoreStorageTypeDef",
     {
         "serviceManagedS3": Mapping[str, Any],
         "customerManagedS3": CustomerManagedDatastoreS3StorageTypeDef,
         "iotSiteWiseMultiLayerStorage": DatastoreIotSiteWiseMultiLayerStorageTypeDef,
     },
     total=False,
 )
 
-DatastorePartitionsOutputTypeDef = TypedDict(
-    "DatastorePartitionsOutputTypeDef",
-    {
-        "partitions": List[DatastorePartitionTypeDef],
-    },
-    total=False,
-)
-
 DatastorePartitionsTypeDef = TypedDict(
     "DatastorePartitionsTypeDef",
     {
         "partitions": Sequence[DatastorePartitionTypeDef],
     },
     total=False,
 )
@@ -1592,33 +1452,14 @@
     },
     total=False,
 )
 
 class LateDataRuleTypeDef(_RequiredLateDataRuleTypeDef, _OptionalLateDataRuleTypeDef):
     pass
 
-_RequiredSqlQueryDatasetActionOutputTypeDef = TypedDict(
-    "_RequiredSqlQueryDatasetActionOutputTypeDef",
-    {
-        "sqlQuery": str,
-    },
-)
-_OptionalSqlQueryDatasetActionOutputTypeDef = TypedDict(
-    "_OptionalSqlQueryDatasetActionOutputTypeDef",
-    {
-        "filters": List[QueryFilterTypeDef],
-    },
-    total=False,
-)
-
-class SqlQueryDatasetActionOutputTypeDef(
-    _RequiredSqlQueryDatasetActionOutputTypeDef, _OptionalSqlQueryDatasetActionOutputTypeDef
-):
-    pass
-
 _RequiredSqlQueryDatasetActionTypeDef = TypedDict(
     "_RequiredSqlQueryDatasetActionTypeDef",
     {
         "sqlQuery": str,
     },
 )
 _OptionalSqlQueryDatasetActionTypeDef = TypedDict(
@@ -1639,112 +1480,109 @@
     {
         "iotEventsDestinationConfiguration": IotEventsDestinationConfigurationTypeDef,
         "s3DestinationConfiguration": S3DestinationConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredContainerDatasetActionOutputTypeDef = TypedDict(
-    "_RequiredContainerDatasetActionOutputTypeDef",
+_RequiredContainerDatasetActionTypeDef = TypedDict(
+    "_RequiredContainerDatasetActionTypeDef",
     {
         "image": str,
         "executionRoleArn": str,
         "resourceConfiguration": ResourceConfigurationTypeDef,
     },
 )
-_OptionalContainerDatasetActionOutputTypeDef = TypedDict(
-    "_OptionalContainerDatasetActionOutputTypeDef",
+_OptionalContainerDatasetActionTypeDef = TypedDict(
+    "_OptionalContainerDatasetActionTypeDef",
     {
-        "variables": List[VariableTypeDef],
+        "variables": Sequence[VariableTypeDef],
     },
     total=False,
 )
 
-class ContainerDatasetActionOutputTypeDef(
-    _RequiredContainerDatasetActionOutputTypeDef, _OptionalContainerDatasetActionOutputTypeDef
+class ContainerDatasetActionTypeDef(
+    _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
 ):
     pass
 
-_RequiredContainerDatasetActionTypeDef = TypedDict(
-    "_RequiredContainerDatasetActionTypeDef",
+_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_RequiredCreatePipelineRequestRequestTypeDef",
     {
-        "image": str,
-        "executionRoleArn": str,
-        "resourceConfiguration": ResourceConfigurationTypeDef,
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityTypeDef],
     },
 )
-_OptionalContainerDatasetActionTypeDef = TypedDict(
-    "_OptionalContainerDatasetActionTypeDef",
+_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
+    "_OptionalCreatePipelineRequestRequestTypeDef",
     {
-        "variables": Sequence[VariableTypeDef],
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class ContainerDatasetActionTypeDef(
-    _RequiredContainerDatasetActionTypeDef, _OptionalContainerDatasetActionTypeDef
+class CreatePipelineRequestRequestTypeDef(
+    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "name": str,
         "arn": str,
-        "activities": List[PipelineActivityOutputTypeDef],
+        "activities": List[PipelineActivityTypeDef],
         "reprocessingSummaries": List[ReprocessingSummaryTypeDef],
         "creationTime": datetime,
         "lastUpdateTime": datetime,
     },
     total=False,
 )
 
-PipelineActivityUnionTypeDef = Union[PipelineActivityTypeDef, PipelineActivityOutputTypeDef]
 RunPipelineActivityRequestRequestTypeDef = TypedDict(
     "RunPipelineActivityRequestRequestTypeDef",
     {
         "pipelineActivity": PipelineActivityTypeDef,
         "payloads": Sequence[BlobTypeDef],
     },
 )
 
-ListPipelinesResponseTypeDef = TypedDict(
-    "ListPipelinesResponseTypeDef",
+UpdatePipelineRequestRequestTypeDef = TypedDict(
+    "UpdatePipelineRequestRequestTypeDef",
     {
-        "pipelineSummaries": List[PipelineSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "pipelineName": str,
+        "pipelineActivities": Sequence[PipelineActivityTypeDef],
     },
 )
 
-DescribeChannelResponseTypeDef = TypedDict(
-    "DescribeChannelResponseTypeDef",
+ListPipelinesResponseTypeDef = TypedDict(
+    "ListPipelinesResponseTypeDef",
     {
-        "channel": ChannelTypeDef,
-        "statistics": ChannelStatisticsTypeDef,
+        "pipelineSummaries": List[PipelineSummaryTypeDef],
+        "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChannelsResponseTypeDef = TypedDict(
     "ListChannelsResponseTypeDef",
     {
         "channelSummaries": List[ChannelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FileFormatConfigurationOutputTypeDef = TypedDict(
-    "FileFormatConfigurationOutputTypeDef",
+DescribeChannelResponseTypeDef = TypedDict(
+    "DescribeChannelResponseTypeDef",
     {
-        "jsonConfiguration": Dict[str, Any],
-        "parquetConfiguration": ParquetConfigurationOutputTypeDef,
+        "channel": ChannelTypeDef,
+        "statistics": ChannelStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 FileFormatConfigurationTypeDef = TypedDict(
     "FileFormatConfigurationTypeDef",
     {
         "jsonConfiguration": Mapping[str, Any],
         "parquetConfiguration": ParquetConfigurationTypeDef,
@@ -1757,33 +1595,29 @@
     {
         "datasetSummaries": List[DatasetSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatastoreStorageUnionTypeDef = Union[DatastoreStorageTypeDef, DatastoreStorageOutputTypeDef]
 DatastoreSummaryTypeDef = TypedDict(
     "DatastoreSummaryTypeDef",
     {
         "datastoreName": str,
         "datastoreStorage": DatastoreStorageSummaryTypeDef,
         "status": DatastoreStatusType,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
         "fileFormatType": FileFormatTypeType,
-        "datastorePartitions": DatastorePartitionsOutputTypeDef,
+        "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
-DatastorePartitionsUnionTypeDef = Union[
-    DatastorePartitionsTypeDef, DatastorePartitionsOutputTypeDef
-]
 _RequiredDatasetContentDeliveryRuleTypeDef = TypedDict(
     "_RequiredDatasetContentDeliveryRuleTypeDef",
     {
         "destination": DatasetContentDeliveryDestinationTypeDef,
     },
 )
 _OptionalDatasetContentDeliveryRuleTypeDef = TypedDict(
@@ -1795,24 +1629,14 @@
 )
 
 class DatasetContentDeliveryRuleTypeDef(
     _RequiredDatasetContentDeliveryRuleTypeDef, _OptionalDatasetContentDeliveryRuleTypeDef
 ):
     pass
 
-DatasetActionOutputTypeDef = TypedDict(
-    "DatasetActionOutputTypeDef",
-    {
-        "actionName": str,
-        "queryAction": SqlQueryDatasetActionOutputTypeDef,
-        "containerAction": ContainerDatasetActionOutputTypeDef,
-    },
-    total=False,
-)
-
 DatasetActionTypeDef = TypedDict(
     "DatasetActionTypeDef",
     {
         "actionName": str,
         "queryAction": SqlQueryDatasetActionTypeDef,
         "containerAction": ContainerDatasetActionTypeDef,
     },
@@ -1823,85 +1647,54 @@
     "DescribePipelineResponseTypeDef",
     {
         "pipeline": PipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_RequiredCreatePipelineRequestRequestTypeDef",
+_RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDatastoreRequestRequestTypeDef",
     {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
+        "datastoreName": str,
     },
 )
-_OptionalCreatePipelineRequestRequestTypeDef = TypedDict(
-    "_OptionalCreatePipelineRequestRequestTypeDef",
+_OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDatastoreRequestRequestTypeDef",
     {
+        "datastoreStorage": DatastoreStorageTypeDef,
+        "retentionPeriod": RetentionPeriodTypeDef,
         "tags": Sequence[TagTypeDef],
+        "fileFormatConfiguration": FileFormatConfigurationTypeDef,
+        "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
-class CreatePipelineRequestRequestTypeDef(
-    _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
+class CreateDatastoreRequestRequestTypeDef(
+    _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
 ):
     pass
 
-UpdatePipelineRequestRequestTypeDef = TypedDict(
-    "UpdatePipelineRequestRequestTypeDef",
-    {
-        "pipelineName": str,
-        "pipelineActivities": Sequence[PipelineActivityUnionTypeDef],
-    },
-)
-
 DatastoreTypeDef = TypedDict(
     "DatastoreTypeDef",
     {
         "name": str,
-        "storage": DatastoreStorageOutputTypeDef,
+        "storage": DatastoreStorageTypeDef,
         "arn": str,
         "status": DatastoreStatusType,
         "retentionPeriod": RetentionPeriodTypeDef,
         "creationTime": datetime,
         "lastUpdateTime": datetime,
         "lastMessageArrivalTime": datetime,
-        "fileFormatConfiguration": FileFormatConfigurationOutputTypeDef,
-        "datastorePartitions": DatastorePartitionsOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredCreateDatastoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDatastoreRequestRequestTypeDef",
-    {
-        "datastoreName": str,
-    },
-)
-_OptionalCreateDatastoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDatastoreRequestRequestTypeDef",
-    {
-        "datastoreStorage": DatastoreStorageTypeDef,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "tags": Sequence[TagTypeDef],
         "fileFormatConfiguration": FileFormatConfigurationTypeDef,
         "datastorePartitions": DatastorePartitionsTypeDef,
     },
     total=False,
 )
 
-class CreateDatastoreRequestRequestTypeDef(
-    _RequiredCreateDatastoreRequestRequestTypeDef, _OptionalCreateDatastoreRequestRequestTypeDef
-):
-    pass
-
-FileFormatConfigurationUnionTypeDef = Union[
-    FileFormatConfigurationTypeDef, FileFormatConfigurationOutputTypeDef
-]
 _RequiredUpdateDatastoreRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatastoreRequestRequestTypeDef",
     {
         "datastoreName": str,
     },
 )
 _OptionalUpdateDatastoreRequestRequestTypeDef = TypedDict(
@@ -1924,55 +1717,19 @@
     {
         "datastoreSummaries": List[DatastoreSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DatasetTypeDef = TypedDict(
-    "DatasetTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "actions": List[DatasetActionOutputTypeDef],
-        "triggers": List[DatasetTriggerTypeDef],
-        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
-        "status": DatasetStatusType,
-        "creationTime": datetime,
-        "lastUpdateTime": datetime,
-        "retentionPeriod": RetentionPeriodTypeDef,
-        "versioningConfiguration": VersioningConfigurationTypeDef,
-        "lateDataRules": List[LateDataRuleTypeDef],
-    },
-    total=False,
-)
-
-DatasetActionUnionTypeDef = Union[DatasetActionTypeDef, DatasetActionOutputTypeDef]
-DescribeDatastoreResponseTypeDef = TypedDict(
-    "DescribeDatastoreResponseTypeDef",
-    {
-        "datastore": DatastoreTypeDef,
-        "statistics": DatastoreStatisticsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "dataset": DatasetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionUnionTypeDef],
+        "actions": Sequence[DatasetActionTypeDef],
     },
 )
 _OptionalCreateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalCreateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
@@ -1985,19 +1742,37 @@
 )
 
 class CreateDatasetRequestRequestTypeDef(
     _RequiredCreateDatasetRequestRequestTypeDef, _OptionalCreateDatasetRequestRequestTypeDef
 ):
     pass
 
+DatasetTypeDef = TypedDict(
+    "DatasetTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "actions": List[DatasetActionTypeDef],
+        "triggers": List[DatasetTriggerTypeDef],
+        "contentDeliveryRules": List[DatasetContentDeliveryRuleTypeDef],
+        "status": DatasetStatusType,
+        "creationTime": datetime,
+        "lastUpdateTime": datetime,
+        "retentionPeriod": RetentionPeriodTypeDef,
+        "versioningConfiguration": VersioningConfigurationTypeDef,
+        "lateDataRules": List[LateDataRuleTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDatasetRequestRequestTypeDef",
     {
         "datasetName": str,
-        "actions": Sequence[DatasetActionUnionTypeDef],
+        "actions": Sequence[DatasetActionTypeDef],
     },
 )
 _OptionalUpdateDatasetRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateDatasetRequestRequestTypeDef",
     {
         "triggers": Sequence[DatasetTriggerTypeDef],
         "contentDeliveryRules": Sequence[DatasetContentDeliveryRuleTypeDef],
@@ -2008,7 +1783,24 @@
     total=False,
 )
 
 class UpdateDatasetRequestRequestTypeDef(
     _RequiredUpdateDatasetRequestRequestTypeDef, _OptionalUpdateDatasetRequestRequestTypeDef
 ):
     pass
+
+DescribeDatastoreResponseTypeDef = TypedDict(
+    "DescribeDatastoreResponseTypeDef",
+    {
+        "datastore": DatastoreTypeDef,
+        "statistics": DatastoreStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "dataset": DatasetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-iotanalytics-2.5.2.post1/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt` & `types-aiobotocore-iotanalytics-2.5.2.post2/types_aiobotocore_iotanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

