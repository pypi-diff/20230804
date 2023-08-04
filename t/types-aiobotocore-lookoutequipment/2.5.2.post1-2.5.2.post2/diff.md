# Comparing `tmp/types-aiobotocore-lookoutequipment-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-lookoutequipment-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lookoutequipment-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-lookoutequipment-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
```

## Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1.tar` & `types-aiobotocore-lookoutequipment-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.941533 types-aiobotocore-lookoutequipment-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:31.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-08-02 14:52:35.941533 types-aiobotocore-lookoutequipment-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-08-02 14:42:31.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:35.941533 types-aiobotocore-lookoutequipment-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:42:31.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.937533 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-02 14:42:31.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-02 14:42:31.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:42:31.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27543 2023-08-02 14:42:32.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27502 2023-08-02 14:42:32.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-08-02 14:42:32.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-08-02 14:42:32.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:31.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35940 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35899 2023-08-02 14:42:32.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:31.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.937533 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.126643 types-aiobotocore-lookoutequipment-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:23.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12681 2023-08-04 13:59:16.106643 types-aiobotocore-lookoutequipment-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11127 2023-08-04 13:43:23.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.126643 types-aiobotocore-lookoutequipment-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2135 2023-08-04 13:43:23.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.106643 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      514 2023-08-04 13:43:23.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      513 2023-08-04 13:43:23.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      979 2023-08-04 13:43:23.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33235 2023-08-04 13:43:23.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    33186 2023-08-04 13:43:23.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9243 2023-08-04 13:43:24.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9241 2023-08-04 13:43:24.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:23.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43815 2023-08-04 13:43:26.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43766 2023-08-04 13:43:24.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:23.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.106643 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12681 2023-08-04 13:59:15.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      887 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       35 2023-08-04 13:59:16.000000 types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/LICENSE` & `types-aiobotocore-lookoutequipment-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/setup.py` & `types-aiobotocore-lookoutequipment-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lookoutequipment",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_lookoutequipment"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LookoutEquipment 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/__init__.py` & `types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/__init__.pyi` & `types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/__main__.py` & `types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LookoutEquipment 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment\nOther"
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

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/client.py` & `types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from .literals import (
     DataUploadFrequencyType,
     InferenceExecutionStatusType,
     InferenceSchedulerStatusType,
     IngestionJobStatusType,
     LabelRatingType,
     ModelStatusType,
+    ModelVersionSourceTypeType,
+    ModelVersionStatusType,
 )
 from .type_defs import (
     CreateDatasetResponseTypeDef,
     CreateInferenceSchedulerResponseTypeDef,
     CreateLabelGroupResponseTypeDef,
     CreateLabelResponseTypeDef,
     CreateModelResponseTypeDef,
@@ -37,34 +39,41 @@
     DatasetSchemaTypeDef,
     DescribeDataIngestionJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeInferenceSchedulerResponseTypeDef,
     DescribeLabelGroupResponseTypeDef,
     DescribeLabelResponseTypeDef,
     DescribeModelResponseTypeDef,
+    DescribeModelVersionResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    ImportDatasetResponseTypeDef,
+    ImportModelVersionResponseTypeDef,
     InferenceInputConfigurationTypeDef,
     InferenceOutputConfigurationTypeDef,
     IngestionInputConfigurationTypeDef,
     LabelsInputConfigurationTypeDef,
     ListDataIngestionJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     ListInferenceExecutionsResponseTypeDef,
     ListInferenceSchedulersResponseTypeDef,
     ListLabelGroupsResponseTypeDef,
     ListLabelsResponseTypeDef,
     ListModelsResponseTypeDef,
+    ListModelVersionsResponseTypeDef,
     ListSensorStatisticsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
     StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
+    UpdateActiveModelVersionResponseTypeDef,
 )
 
 __all__ = ("LookoutEquipmentClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -254,14 +263,22 @@
         """
         Deletes an ML model currently available for Amazon Lookout for Equipment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#delete_model)
         """
 
+    async def delete_resource_policy(self, *, ResourceArn: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes the resource policy attached to the resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_resource_policy)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#delete_resource_policy)
+        """
+
     async def describe_data_ingestion_job(
         self, *, JobId: str
     ) -> DescribeDataIngestionJobResponseTypeDef:
         """
         Provides information on a specific data ingestion job such as creation time,
         dataset ARN, and status.
 
@@ -316,28 +333,83 @@
         including model name and ARN, dataset, training and evaluation information,
         status, and so on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#describe_model)
         """
 
+    async def describe_model_version(
+        self, *, ModelName: str, ModelVersion: int
+    ) -> DescribeModelVersionResponseTypeDef:
+        """
+        Retrieves information about a specific machine learning model version.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_model_version)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#describe_model_version)
+        """
+
+    async def describe_resource_policy(
+        self, *, ResourceArn: str
+    ) -> DescribeResourcePolicyResponseTypeDef:
+        """
+        Provides the details of a resource policy attached to a resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_resource_policy)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#describe_resource_policy)
+        """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#generate_presigned_url)
         """
 
+    async def import_dataset(
+        self,
+        *,
+        SourceDatasetArn: str,
+        ClientToken: str,
+        DatasetName: str = ...,
+        ServerSideKmsKeyId: str = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> ImportDatasetResponseTypeDef:
+        """
+        Imports a dataset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.import_dataset)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#import_dataset)
+        """
+
+    async def import_model_version(
+        self,
+        *,
+        SourceModelVersionArn: str,
+        DatasetName: str,
+        ClientToken: str,
+        ModelName: str = ...,
+        LabelsInputConfiguration: LabelsInputConfigurationTypeDef = ...,
+        RoleArn: str = ...,
+        ServerSideKmsKeyId: str = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> ImportModelVersionResponseTypeDef:
+        """
+        Imports a model that has been trained successfully.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.import_model_version)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#import_model_version)
+        """
+
     async def list_data_ingestion_jobs(
         self,
         *,
         DatasetName: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: IngestionJobStatusType = ...
@@ -437,14 +509,35 @@
         """
         Provides a list of labels.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_labels)
         """
 
+    async def list_model_versions(
+        self,
+        *,
+        ModelName: str,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        Status: ModelVersionStatusType = ...,
+        SourceType: ModelVersionSourceTypeType = ...,
+        CreatedAtEndTime: TimestampTypeDef = ...,
+        CreatedAtStartTime: TimestampTypeDef = ...,
+        MaxModelVersion: int = ...,
+        MinModelVersion: int = ...
+    ) -> ListModelVersionsResponseTypeDef:
+        """
+        Generates a list of all model versions for a given model, including the model
+        version, model version ARN, and status.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_model_versions)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_model_versions)
+        """
+
     async def list_models(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: ModelStatusType = ...,
         ModelNameBeginsWith: str = ...,
@@ -480,14 +573,29 @@
         """
         Lists all the tags for a specified resource, including key and value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_tags_for_resource)
         """
 
+    async def put_resource_policy(
+        self,
+        *,
+        ResourceArn: str,
+        ResourcePolicy: str,
+        ClientToken: str,
+        PolicyRevisionId: str = ...
+    ) -> PutResourcePolicyResponseTypeDef:
+        """
+        Creates a resource control policy for a given resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.put_resource_policy)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#put_resource_policy)
+        """
+
     async def start_data_ingestion_job(
         self,
         *,
         DatasetName: str,
         IngestionInputConfiguration: IngestionInputConfigurationTypeDef,
         RoleArn: str,
         ClientToken: str
@@ -531,14 +639,24 @@
         """
         Removes a specific tag from a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#untag_resource)
         """
 
+    async def update_active_model_version(
+        self, *, ModelName: str, ModelVersion: int
+    ) -> UpdateActiveModelVersionResponseTypeDef:
+        """
+        Sets the active model version for a given machine learning model.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_active_model_version)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#update_active_model_version)
+        """
+
     async def update_inference_scheduler(
         self,
         *,
         InferenceSchedulerName: str,
         DataDelayOffsetInMinutes: int = ...,
         DataUploadFrequency: DataUploadFrequencyType = ...,
         DataInputConfiguration: InferenceInputConfigurationTypeDef = ...,
```

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/client.pyi` & `types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/client.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from .literals import (
     DataUploadFrequencyType,
     InferenceExecutionStatusType,
     InferenceSchedulerStatusType,
     IngestionJobStatusType,
     LabelRatingType,
     ModelStatusType,
+    ModelVersionSourceTypeType,
+    ModelVersionStatusType,
 )
 from .type_defs import (
     CreateDatasetResponseTypeDef,
     CreateInferenceSchedulerResponseTypeDef,
     CreateLabelGroupResponseTypeDef,
     CreateLabelResponseTypeDef,
     CreateModelResponseTypeDef,
@@ -37,34 +39,41 @@
     DatasetSchemaTypeDef,
     DescribeDataIngestionJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeInferenceSchedulerResponseTypeDef,
     DescribeLabelGroupResponseTypeDef,
     DescribeLabelResponseTypeDef,
     DescribeModelResponseTypeDef,
+    DescribeModelVersionResponseTypeDef,
+    DescribeResourcePolicyResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    ImportDatasetResponseTypeDef,
+    ImportModelVersionResponseTypeDef,
     InferenceInputConfigurationTypeDef,
     InferenceOutputConfigurationTypeDef,
     IngestionInputConfigurationTypeDef,
     LabelsInputConfigurationTypeDef,
     ListDataIngestionJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListInferenceEventsResponseTypeDef,
     ListInferenceExecutionsResponseTypeDef,
     ListInferenceSchedulersResponseTypeDef,
     ListLabelGroupsResponseTypeDef,
     ListLabelsResponseTypeDef,
     ListModelsResponseTypeDef,
+    ListModelVersionsResponseTypeDef,
     ListSensorStatisticsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
     StartDataIngestionJobResponseTypeDef,
     StartInferenceSchedulerResponseTypeDef,
     StopInferenceSchedulerResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
+    UpdateActiveModelVersionResponseTypeDef,
 )
 
 __all__ = ("LookoutEquipmentClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -238,14 +247,21 @@
     async def delete_model(self, *, ModelName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes an ML model currently available for Amazon Lookout for Equipment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#delete_model)
         """
+    async def delete_resource_policy(self, *, ResourceArn: str) -> EmptyResponseMetadataTypeDef:
+        """
+        Deletes the resource policy attached to the resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.delete_resource_policy)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#delete_resource_policy)
+        """
     async def describe_data_ingestion_job(
         self, *, JobId: str
     ) -> DescribeDataIngestionJobResponseTypeDef:
         """
         Provides information on a specific data ingestion job such as creation time,
         dataset ARN, and status.
 
@@ -294,27 +310,78 @@
         Provides a JSON containing the overall information about a specific ML model,
         including model name and ARN, dataset, training and evaluation information,
         status, and so on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#describe_model)
         """
+    async def describe_model_version(
+        self, *, ModelName: str, ModelVersion: int
+    ) -> DescribeModelVersionResponseTypeDef:
+        """
+        Retrieves information about a specific machine learning model version.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_model_version)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#describe_model_version)
+        """
+    async def describe_resource_policy(
+        self, *, ResourceArn: str
+    ) -> DescribeResourcePolicyResponseTypeDef:
+        """
+        Provides the details of a resource policy attached to a resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.describe_resource_policy)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#describe_resource_policy)
+        """
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#generate_presigned_url)
         """
+    async def import_dataset(
+        self,
+        *,
+        SourceDatasetArn: str,
+        ClientToken: str,
+        DatasetName: str = ...,
+        ServerSideKmsKeyId: str = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> ImportDatasetResponseTypeDef:
+        """
+        Imports a dataset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.import_dataset)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#import_dataset)
+        """
+    async def import_model_version(
+        self,
+        *,
+        SourceModelVersionArn: str,
+        DatasetName: str,
+        ClientToken: str,
+        ModelName: str = ...,
+        LabelsInputConfiguration: LabelsInputConfigurationTypeDef = ...,
+        RoleArn: str = ...,
+        ServerSideKmsKeyId: str = ...,
+        Tags: Sequence[TagTypeDef] = ...
+    ) -> ImportModelVersionResponseTypeDef:
+        """
+        Imports a model that has been trained successfully.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.import_model_version)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#import_model_version)
+        """
     async def list_data_ingestion_jobs(
         self,
         *,
         DatasetName: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: IngestionJobStatusType = ...
@@ -407,14 +474,34 @@
     ) -> ListLabelsResponseTypeDef:
         """
         Provides a list of labels.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_labels)
         """
+    async def list_model_versions(
+        self,
+        *,
+        ModelName: str,
+        NextToken: str = ...,
+        MaxResults: int = ...,
+        Status: ModelVersionStatusType = ...,
+        SourceType: ModelVersionSourceTypeType = ...,
+        CreatedAtEndTime: TimestampTypeDef = ...,
+        CreatedAtStartTime: TimestampTypeDef = ...,
+        MaxModelVersion: int = ...,
+        MinModelVersion: int = ...
+    ) -> ListModelVersionsResponseTypeDef:
+        """
+        Generates a list of all model versions for a given model, including the model
+        version, model version ARN, and status.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_model_versions)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_model_versions)
+        """
     async def list_models(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         Status: ModelStatusType = ...,
         ModelNameBeginsWith: str = ...,
@@ -447,14 +534,28 @@
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists all the tags for a specified resource, including key and value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#list_tags_for_resource)
         """
+    async def put_resource_policy(
+        self,
+        *,
+        ResourceArn: str,
+        ResourcePolicy: str,
+        ClientToken: str,
+        PolicyRevisionId: str = ...
+    ) -> PutResourcePolicyResponseTypeDef:
+        """
+        Creates a resource control policy for a given resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.put_resource_policy)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#put_resource_policy)
+        """
     async def start_data_ingestion_job(
         self,
         *,
         DatasetName: str,
         IngestionInputConfiguration: IngestionInputConfigurationTypeDef,
         RoleArn: str,
         ClientToken: str
@@ -493,14 +594,23 @@
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes a specific tag from a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#untag_resource)
         """
+    async def update_active_model_version(
+        self, *, ModelName: str, ModelVersion: int
+    ) -> UpdateActiveModelVersionResponseTypeDef:
+        """
+        Sets the active model version for a given machine learning model.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#LookoutEquipment.Client.update_active_model_version)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutequipment/client/#update_active_model_version)
+        """
     async def update_inference_scheduler(
         self,
         *,
         InferenceSchedulerName: str,
         DataDelayOffsetInMinutes: int = ...,
         DataUploadFrequency: DataUploadFrequencyType = ...,
         DataInputConfiguration: InferenceInputConfigurationTypeDef = ...,
```

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/literals.py` & `types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/literals.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,32 +24,38 @@
     "DatasetStatusType",
     "InferenceExecutionStatusType",
     "InferenceSchedulerStatusType",
     "IngestionJobStatusType",
     "LabelRatingType",
     "LatestInferenceResultType",
     "ModelStatusType",
+    "ModelVersionSourceTypeType",
+    "ModelVersionStatusType",
     "MonotonicityType",
     "StatisticalIssueStatusType",
     "TargetSamplingRateType",
     "LookoutEquipmentServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
 DataUploadFrequencyType = Literal["PT10M", "PT15M", "PT1H", "PT30M", "PT5M"]
-DatasetStatusType = Literal["ACTIVE", "CREATED", "INGESTION_IN_PROGRESS"]
+DatasetStatusType = Literal["ACTIVE", "CREATED", "IMPORT_IN_PROGRESS", "INGESTION_IN_PROGRESS"]
 InferenceExecutionStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 InferenceSchedulerStatusType = Literal["PENDING", "RUNNING", "STOPPED", "STOPPING"]
-IngestionJobStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
+IngestionJobStatusType = Literal["FAILED", "IMPORT_IN_PROGRESS", "IN_PROGRESS", "SUCCESS"]
 LabelRatingType = Literal["ANOMALY", "NEUTRAL", "NO_ANOMALY"]
 LatestInferenceResultType = Literal["ANOMALOUS", "NORMAL"]
-ModelStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
+ModelStatusType = Literal["FAILED", "IMPORT_IN_PROGRESS", "IN_PROGRESS", "SUCCESS"]
+ModelVersionSourceTypeType = Literal["IMPORT", "RETRAINING", "TRAINING"]
+ModelVersionStatusType = Literal[
+    "CANCELED", "FAILED", "IMPORT_IN_PROGRESS", "IN_PROGRESS", "SUCCESS"
+]
 MonotonicityType = Literal["DECREASING", "INCREASING", "STATIC"]
 StatisticalIssueStatusType = Literal["NO_ISSUE_DETECTED", "POTENTIAL_ISSUE_DETECTED"]
 TargetSamplingRateType = Literal[
     "PT10M", "PT10S", "PT15M", "PT15S", "PT1H", "PT1M", "PT1S", "PT30M", "PT30S", "PT5M", "PT5S"
 ]
 LookoutEquipmentServiceName = Literal["lookoutequipment"]
 ServiceName = Literal[
@@ -63,14 +69,15 @@
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
@@ -166,14 +173,15 @@
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
@@ -252,26 +260,28 @@
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

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/literals.pyi` & `types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/literals.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -23,31 +23,37 @@
     "DatasetStatusType",
     "InferenceExecutionStatusType",
     "InferenceSchedulerStatusType",
     "IngestionJobStatusType",
     "LabelRatingType",
     "LatestInferenceResultType",
     "ModelStatusType",
+    "ModelVersionSourceTypeType",
+    "ModelVersionStatusType",
     "MonotonicityType",
     "StatisticalIssueStatusType",
     "TargetSamplingRateType",
     "LookoutEquipmentServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 DataUploadFrequencyType = Literal["PT10M", "PT15M", "PT1H", "PT30M", "PT5M"]
-DatasetStatusType = Literal["ACTIVE", "CREATED", "INGESTION_IN_PROGRESS"]
+DatasetStatusType = Literal["ACTIVE", "CREATED", "IMPORT_IN_PROGRESS", "INGESTION_IN_PROGRESS"]
 InferenceExecutionStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
 InferenceSchedulerStatusType = Literal["PENDING", "RUNNING", "STOPPED", "STOPPING"]
-IngestionJobStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
+IngestionJobStatusType = Literal["FAILED", "IMPORT_IN_PROGRESS", "IN_PROGRESS", "SUCCESS"]
 LabelRatingType = Literal["ANOMALY", "NEUTRAL", "NO_ANOMALY"]
 LatestInferenceResultType = Literal["ANOMALOUS", "NORMAL"]
-ModelStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCESS"]
+ModelStatusType = Literal["FAILED", "IMPORT_IN_PROGRESS", "IN_PROGRESS", "SUCCESS"]
+ModelVersionSourceTypeType = Literal["IMPORT", "RETRAINING", "TRAINING"]
+ModelVersionStatusType = Literal[
+    "CANCELED", "FAILED", "IMPORT_IN_PROGRESS", "IN_PROGRESS", "SUCCESS"
+]
 MonotonicityType = Literal["DECREASING", "INCREASING", "STATIC"]
 StatisticalIssueStatusType = Literal["NO_ISSUE_DETECTED", "POTENTIAL_ISSUE_DETECTED"]
 TargetSamplingRateType = Literal[
     "PT10M", "PT10S", "PT15M", "PT15S", "PT1H", "PT1M", "PT1S", "PT30M", "PT30S", "PT5M", "PT5S"
 ]
 LookoutEquipmentServiceName = Literal["lookoutequipment"]
 ServiceName = Literal[
@@ -61,14 +67,15 @@
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
@@ -164,14 +171,15 @@
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
@@ -250,26 +258,28 @@
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

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/type_defs.py` & `types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     DataUploadFrequencyType,
     InferenceExecutionStatusType,
     InferenceSchedulerStatusType,
     IngestionJobStatusType,
     LabelRatingType,
     LatestInferenceResultType,
     ModelStatusType,
+    ModelVersionSourceTypeType,
+    ModelVersionStatusType,
     MonotonicityType,
     StatisticalIssueStatusType,
     TargetSamplingRateType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -49,20 +51,23 @@
     "UnsupportedTimestampsTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteInferenceSchedulerRequestRequestTypeDef",
     "DeleteLabelGroupRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
+    "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeDataIngestionJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeInferenceSchedulerRequestRequestTypeDef",
     "DescribeLabelGroupRequestRequestTypeDef",
     "DescribeLabelRequestRequestTypeDef",
     "DescribeModelRequestRequestTypeDef",
+    "DescribeModelVersionRequestRequestTypeDef",
+    "DescribeResourcePolicyRequestRequestTypeDef",
     "InferenceEventSummaryTypeDef",
     "S3ObjectTypeDef",
     "InferenceInputNameConfigurationTypeDef",
     "InferenceS3InputConfigurationTypeDef",
     "InferenceS3OutputConfigurationTypeDef",
     "InferenceSchedulerSummaryTypeDef",
     "IngestionS3InputConfigurationTypeDef",
@@ -72,65 +77,78 @@
     "LabelSummaryTypeDef",
     "LabelsS3InputConfigurationTypeDef",
     "LargeTimestampGapsTypeDef",
     "ListDataIngestionJobsRequestRequestTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListInferenceSchedulersRequestRequestTypeDef",
     "ListLabelGroupsRequestRequestTypeDef",
+    "ModelVersionSummaryTypeDef",
     "ListModelsRequestRequestTypeDef",
     "ModelSummaryTypeDef",
     "ListSensorStatisticsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MonotonicValuesTypeDef",
     "MultipleOperatingModesTypeDef",
+    "PutResourcePolicyRequestRequestTypeDef",
     "StartInferenceSchedulerRequestRequestTypeDef",
     "StopInferenceSchedulerRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateActiveModelVersionRequestRequestTypeDef",
     "UpdateLabelGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateLabelGroupRequestRequestTypeDef",
+    "ImportDatasetRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateInferenceSchedulerResponseTypeDef",
     "CreateLabelGroupResponseTypeDef",
     "CreateLabelResponseTypeDef",
     "CreateModelResponseTypeDef",
     "DescribeLabelGroupResponseTypeDef",
     "DescribeLabelResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "ImportDatasetResponseTypeDef",
+    "ImportModelVersionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
     "StartDataIngestionJobResponseTypeDef",
     "StartInferenceSchedulerResponseTypeDef",
     "StopInferenceSchedulerResponseTypeDef",
+    "UpdateActiveModelVersionResponseTypeDef",
     "CreateLabelRequestRequestTypeDef",
     "ListInferenceEventsRequestRequestTypeDef",
     "ListInferenceExecutionsRequestRequestTypeDef",
     "ListLabelsRequestRequestTypeDef",
+    "ListModelVersionsRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
     "ListInferenceEventsResponseTypeDef",
     "IngestedFilesSummaryTypeDef",
     "InferenceInputConfigurationTypeDef",
     "InferenceOutputConfigurationTypeDef",
     "ListInferenceSchedulersResponseTypeDef",
     "IngestionInputConfigurationTypeDef",
     "InsufficientSensorDataTypeDef",
     "ListLabelGroupsResponseTypeDef",
     "ListLabelsResponseTypeDef",
     "LabelsInputConfigurationTypeDef",
+    "ListModelVersionsResponseTypeDef",
     "ListModelsResponseTypeDef",
     "SensorStatisticsSummaryTypeDef",
     "CreateInferenceSchedulerRequestRequestTypeDef",
     "DescribeInferenceSchedulerResponseTypeDef",
     "InferenceExecutionSummaryTypeDef",
     "UpdateInferenceSchedulerRequestRequestTypeDef",
     "DataIngestionJobSummaryTypeDef",
     "StartDataIngestionJobRequestRequestTypeDef",
     "DataQualitySummaryTypeDef",
     "CreateModelRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
+    "DescribeModelVersionResponseTypeDef",
+    "ImportModelVersionRequestRequestTypeDef",
     "ListSensorStatisticsResponseTypeDef",
     "ListInferenceExecutionsResponseTypeDef",
     "ListDataIngestionJobsResponseTypeDef",
     "DescribeDataIngestionJobResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
 )
 
@@ -272,14 +290,21 @@
 DeleteModelRequestRequestTypeDef = TypedDict(
     "DeleteModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
+DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
+    "DeleteResourcePolicyRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+
 DescribeDataIngestionJobRequestRequestTypeDef = TypedDict(
     "DescribeDataIngestionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -315,14 +340,29 @@
 DescribeModelRequestRequestTypeDef = TypedDict(
     "DescribeModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
+DescribeModelVersionRequestRequestTypeDef = TypedDict(
+    "DescribeModelVersionRequestRequestTypeDef",
+    {
+        "ModelName": str,
+        "ModelVersion": int,
+    },
+)
+
+DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
+    "DescribeResourcePolicyRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+
 InferenceEventSummaryTypeDef = TypedDict(
     "InferenceEventSummaryTypeDef",
     {
         "InferenceSchedulerArn": str,
         "InferenceSchedulerName": str,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
@@ -551,14 +591,28 @@
         "LabelGroupNameBeginsWith": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ModelVersionSummaryTypeDef = TypedDict(
+    "ModelVersionSummaryTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "ModelVersion": int,
+        "ModelVersionArn": str,
+        "CreatedAt": datetime,
+        "Status": ModelVersionStatusType,
+        "SourceType": ModelVersionSourceTypeType,
+    },
+    total=False,
+)
+
 ListModelsRequestRequestTypeDef = TypedDict(
     "ListModelsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Status": ModelStatusType,
         "ModelNameBeginsWith": str,
@@ -572,14 +626,16 @@
     {
         "ModelName": str,
         "ModelArn": str,
         "DatasetName": str,
         "DatasetArn": str,
         "Status": ModelStatusType,
         "CreatedAt": datetime,
+        "ActiveModelVersion": int,
+        "ActiveModelVersionArn": str,
     },
     total=False,
 )
 
 _RequiredListSensorStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredListSensorStatisticsRequestRequestTypeDef",
     {
@@ -633,14 +689,37 @@
 MultipleOperatingModesTypeDef = TypedDict(
     "MultipleOperatingModesTypeDef",
     {
         "Status": StatisticalIssueStatusType,
     },
 )
 
+_RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourcePolicyRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ClientToken": str,
+    },
+)
+_OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourcePolicyRequestRequestTypeDef",
+    {
+        "PolicyRevisionId": str,
+    },
+    total=False,
+)
+
+
+class PutResourcePolicyRequestRequestTypeDef(
+    _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
+):
+    pass
+
+
 StartInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "StartInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 
@@ -655,14 +734,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateActiveModelVersionRequestRequestTypeDef = TypedDict(
+    "UpdateActiveModelVersionRequestRequestTypeDef",
+    {
+        "ModelName": str,
+        "ModelVersion": int,
+    },
+)
+
 _RequiredUpdateLabelGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLabelGroupRequestRequestTypeDef",
     {
         "LabelGroupName": str,
     },
 )
 _OptionalUpdateLabelGroupRequestRequestTypeDef = TypedDict(
@@ -723,14 +810,38 @@
 
 class CreateLabelGroupRequestRequestTypeDef(
     _RequiredCreateLabelGroupRequestRequestTypeDef, _OptionalCreateLabelGroupRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredImportDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredImportDatasetRequestRequestTypeDef",
+    {
+        "SourceDatasetArn": str,
+        "ClientToken": str,
+    },
+)
+_OptionalImportDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalImportDatasetRequestRequestTypeDef",
+    {
+        "DatasetName": str,
+        "ServerSideKmsKeyId": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class ImportDatasetRequestRequestTypeDef(
+    _RequiredImportDatasetRequestRequestTypeDef, _OptionalImportDatasetRequestRequestTypeDef
+):
+    pass
+
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -806,29 +917,72 @@
         "Notes": str,
         "Equipment": str,
         "CreatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "PolicyRevisionId": str,
+        "ResourcePolicy": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImportDatasetResponseTypeDef = TypedDict(
+    "ImportDatasetResponseTypeDef",
+    {
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Status": DatasetStatusType,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportModelVersionResponseTypeDef = TypedDict(
+    "ImportModelVersionResponseTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "ModelVersionArn": str,
+        "ModelVersion": int,
+        "Status": ModelVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartDataIngestionJobResponseTypeDef = TypedDict(
     "StartDataIngestionJobResponseTypeDef",
     {
         "JobId": str,
         "Status": IngestionJobStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -854,14 +1008,27 @@
         "InferenceSchedulerName": str,
         "InferenceSchedulerArn": str,
         "Status": InferenceSchedulerStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateActiveModelVersionResponseTypeDef = TypedDict(
+    "UpdateActiveModelVersionResponseTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "CurrentActiveVersion": int,
+        "PreviousActiveVersion": int,
+        "CurrentActiveVersionArn": str,
+        "PreviousActiveVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLabelRequestRequestTypeDef",
     {
         "LabelGroupName": str,
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
         "Rating": LabelRatingType,
@@ -958,14 +1125,42 @@
 
 class ListLabelsRequestRequestTypeDef(
     _RequiredListLabelsRequestRequestTypeDef, _OptionalListLabelsRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredListModelVersionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListModelVersionsRequestRequestTypeDef",
+    {
+        "ModelName": str,
+    },
+)
+_OptionalListModelVersionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListModelVersionsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "Status": ModelVersionStatusType,
+        "SourceType": ModelVersionSourceTypeType,
+        "CreatedAtEndTime": TimestampTypeDef,
+        "CreatedAtStartTime": TimestampTypeDef,
+        "MaxModelVersion": int,
+        "MinModelVersion": int,
+    },
+    total=False,
+)
+
+
+class ListModelVersionsRequestRequestTypeDef(
+    _RequiredListModelVersionsRequestRequestTypeDef, _OptionalListModelVersionsRequestRequestTypeDef
+):
+    pass
+
+
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "NextToken": str,
         "DatasetSummaries": List[DatasetSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1080,14 +1275,23 @@
     {
         "S3InputConfiguration": LabelsS3InputConfigurationTypeDef,
         "LabelGroupName": str,
     },
     total=False,
 )
 
+ListModelVersionsResponseTypeDef = TypedDict(
+    "ListModelVersionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "ModelVersionSummaries": List[ModelVersionSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListModelsResponseTypeDef = TypedDict(
     "ListModelsResponseTypeDef",
     {
         "NextToken": str,
         "ModelSummaries": List[ModelSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1295,18 +1499,90 @@
         "TrainingExecutionEndTime": datetime,
         "FailedReason": str,
         "ModelMetrics": str,
         "LastUpdatedTime": datetime,
         "CreatedAt": datetime,
         "ServerSideKmsKeyId": str,
         "OffCondition": str,
+        "SourceModelVersionArn": str,
+        "ImportJobStartTime": datetime,
+        "ImportJobEndTime": datetime,
+        "ActiveModelVersion": int,
+        "ActiveModelVersionArn": str,
+        "ModelVersionActivatedAt": datetime,
+        "PreviousActiveModelVersion": int,
+        "PreviousActiveModelVersionArn": str,
+        "PreviousModelVersionActivatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeModelVersionResponseTypeDef = TypedDict(
+    "DescribeModelVersionResponseTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "ModelVersion": int,
+        "ModelVersionArn": str,
+        "Status": ModelVersionStatusType,
+        "SourceType": ModelVersionSourceTypeType,
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Schema": str,
+        "LabelsInputConfiguration": LabelsInputConfigurationTypeDef,
+        "TrainingDataStartTime": datetime,
+        "TrainingDataEndTime": datetime,
+        "EvaluationDataStartTime": datetime,
+        "EvaluationDataEndTime": datetime,
+        "RoleArn": str,
+        "DataPreProcessingConfiguration": DataPreProcessingConfigurationTypeDef,
+        "TrainingExecutionStartTime": datetime,
+        "TrainingExecutionEndTime": datetime,
+        "FailedReason": str,
+        "ModelMetrics": str,
+        "LastUpdatedTime": datetime,
+        "CreatedAt": datetime,
+        "ServerSideKmsKeyId": str,
+        "OffCondition": str,
+        "SourceModelVersionArn": str,
+        "ImportJobStartTime": datetime,
+        "ImportJobEndTime": datetime,
+        "ImportedDataSizeInBytes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredImportModelVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredImportModelVersionRequestRequestTypeDef",
+    {
+        "SourceModelVersionArn": str,
+        "DatasetName": str,
+        "ClientToken": str,
+    },
+)
+_OptionalImportModelVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalImportModelVersionRequestRequestTypeDef",
+    {
+        "ModelName": str,
+        "LabelsInputConfiguration": LabelsInputConfigurationTypeDef,
+        "RoleArn": str,
+        "ServerSideKmsKeyId": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class ImportModelVersionRequestRequestTypeDef(
+    _RequiredImportModelVersionRequestRequestTypeDef,
+    _OptionalImportModelVersionRequestRequestTypeDef,
+):
+    pass
+
+
 ListSensorStatisticsResponseTypeDef = TypedDict(
     "ListSensorStatisticsResponseTypeDef",
     {
         "SensorStatisticsSummaries": List[SensorStatisticsSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1342,14 +1618,15 @@
         "FailedReason": str,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "StatusDetail": str,
         "IngestedDataSize": int,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
+        "SourceDatasetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
@@ -1362,10 +1639,11 @@
         "ServerSideKmsKeyId": str,
         "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "RoleArn": str,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
+        "SourceDatasetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment/type_defs.pyi` & `types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     DataUploadFrequencyType,
     InferenceExecutionStatusType,
     InferenceSchedulerStatusType,
     IngestionJobStatusType,
     LabelRatingType,
     LatestInferenceResultType,
     ModelStatusType,
+    ModelVersionSourceTypeType,
+    ModelVersionStatusType,
     MonotonicityType,
     StatisticalIssueStatusType,
     TargetSamplingRateType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -48,20 +50,23 @@
     "UnsupportedTimestampsTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteInferenceSchedulerRequestRequestTypeDef",
     "DeleteLabelGroupRequestRequestTypeDef",
     "DeleteLabelRequestRequestTypeDef",
     "DeleteModelRequestRequestTypeDef",
+    "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeDataIngestionJobRequestRequestTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeInferenceSchedulerRequestRequestTypeDef",
     "DescribeLabelGroupRequestRequestTypeDef",
     "DescribeLabelRequestRequestTypeDef",
     "DescribeModelRequestRequestTypeDef",
+    "DescribeModelVersionRequestRequestTypeDef",
+    "DescribeResourcePolicyRequestRequestTypeDef",
     "InferenceEventSummaryTypeDef",
     "S3ObjectTypeDef",
     "InferenceInputNameConfigurationTypeDef",
     "InferenceS3InputConfigurationTypeDef",
     "InferenceS3OutputConfigurationTypeDef",
     "InferenceSchedulerSummaryTypeDef",
     "IngestionS3InputConfigurationTypeDef",
@@ -71,65 +76,78 @@
     "LabelSummaryTypeDef",
     "LabelsS3InputConfigurationTypeDef",
     "LargeTimestampGapsTypeDef",
     "ListDataIngestionJobsRequestRequestTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListInferenceSchedulersRequestRequestTypeDef",
     "ListLabelGroupsRequestRequestTypeDef",
+    "ModelVersionSummaryTypeDef",
     "ListModelsRequestRequestTypeDef",
     "ModelSummaryTypeDef",
     "ListSensorStatisticsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MonotonicValuesTypeDef",
     "MultipleOperatingModesTypeDef",
+    "PutResourcePolicyRequestRequestTypeDef",
     "StartInferenceSchedulerRequestRequestTypeDef",
     "StopInferenceSchedulerRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateActiveModelVersionRequestRequestTypeDef",
     "UpdateLabelGroupRequestRequestTypeDef",
     "CreateDatasetRequestRequestTypeDef",
     "CreateLabelGroupRequestRequestTypeDef",
+    "ImportDatasetRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatasetResponseTypeDef",
     "CreateInferenceSchedulerResponseTypeDef",
     "CreateLabelGroupResponseTypeDef",
     "CreateLabelResponseTypeDef",
     "CreateModelResponseTypeDef",
     "DescribeLabelGroupResponseTypeDef",
     "DescribeLabelResponseTypeDef",
+    "DescribeResourcePolicyResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "ImportDatasetResponseTypeDef",
+    "ImportModelVersionResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
     "StartDataIngestionJobResponseTypeDef",
     "StartInferenceSchedulerResponseTypeDef",
     "StopInferenceSchedulerResponseTypeDef",
+    "UpdateActiveModelVersionResponseTypeDef",
     "CreateLabelRequestRequestTypeDef",
     "ListInferenceEventsRequestRequestTypeDef",
     "ListInferenceExecutionsRequestRequestTypeDef",
     "ListLabelsRequestRequestTypeDef",
+    "ListModelVersionsRequestRequestTypeDef",
     "ListDatasetsResponseTypeDef",
     "ListInferenceEventsResponseTypeDef",
     "IngestedFilesSummaryTypeDef",
     "InferenceInputConfigurationTypeDef",
     "InferenceOutputConfigurationTypeDef",
     "ListInferenceSchedulersResponseTypeDef",
     "IngestionInputConfigurationTypeDef",
     "InsufficientSensorDataTypeDef",
     "ListLabelGroupsResponseTypeDef",
     "ListLabelsResponseTypeDef",
     "LabelsInputConfigurationTypeDef",
+    "ListModelVersionsResponseTypeDef",
     "ListModelsResponseTypeDef",
     "SensorStatisticsSummaryTypeDef",
     "CreateInferenceSchedulerRequestRequestTypeDef",
     "DescribeInferenceSchedulerResponseTypeDef",
     "InferenceExecutionSummaryTypeDef",
     "UpdateInferenceSchedulerRequestRequestTypeDef",
     "DataIngestionJobSummaryTypeDef",
     "StartDataIngestionJobRequestRequestTypeDef",
     "DataQualitySummaryTypeDef",
     "CreateModelRequestRequestTypeDef",
     "DescribeModelResponseTypeDef",
+    "DescribeModelVersionResponseTypeDef",
+    "ImportModelVersionRequestRequestTypeDef",
     "ListSensorStatisticsResponseTypeDef",
     "ListInferenceExecutionsResponseTypeDef",
     "ListDataIngestionJobsResponseTypeDef",
     "DescribeDataIngestionJobResponseTypeDef",
     "DescribeDatasetResponseTypeDef",
 )
 
@@ -269,14 +287,21 @@
 DeleteModelRequestRequestTypeDef = TypedDict(
     "DeleteModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
+DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
+    "DeleteResourcePolicyRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+
 DescribeDataIngestionJobRequestRequestTypeDef = TypedDict(
     "DescribeDataIngestionJobRequestRequestTypeDef",
     {
         "JobId": str,
     },
 )
 
@@ -312,14 +337,29 @@
 DescribeModelRequestRequestTypeDef = TypedDict(
     "DescribeModelRequestRequestTypeDef",
     {
         "ModelName": str,
     },
 )
 
+DescribeModelVersionRequestRequestTypeDef = TypedDict(
+    "DescribeModelVersionRequestRequestTypeDef",
+    {
+        "ModelName": str,
+        "ModelVersion": int,
+    },
+)
+
+DescribeResourcePolicyRequestRequestTypeDef = TypedDict(
+    "DescribeResourcePolicyRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+
 InferenceEventSummaryTypeDef = TypedDict(
     "InferenceEventSummaryTypeDef",
     {
         "InferenceSchedulerArn": str,
         "InferenceSchedulerName": str,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
@@ -538,14 +578,28 @@
         "LabelGroupNameBeginsWith": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ModelVersionSummaryTypeDef = TypedDict(
+    "ModelVersionSummaryTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "ModelVersion": int,
+        "ModelVersionArn": str,
+        "CreatedAt": datetime,
+        "Status": ModelVersionStatusType,
+        "SourceType": ModelVersionSourceTypeType,
+    },
+    total=False,
+)
+
 ListModelsRequestRequestTypeDef = TypedDict(
     "ListModelsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Status": ModelStatusType,
         "ModelNameBeginsWith": str,
@@ -559,14 +613,16 @@
     {
         "ModelName": str,
         "ModelArn": str,
         "DatasetName": str,
         "DatasetArn": str,
         "Status": ModelStatusType,
         "CreatedAt": datetime,
+        "ActiveModelVersion": int,
+        "ActiveModelVersionArn": str,
     },
     total=False,
 )
 
 _RequiredListSensorStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredListSensorStatisticsRequestRequestTypeDef",
     {
@@ -616,14 +672,35 @@
 MultipleOperatingModesTypeDef = TypedDict(
     "MultipleOperatingModesTypeDef",
     {
         "Status": StatisticalIssueStatusType,
     },
 )
 
+_RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourcePolicyRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourcePolicy": str,
+        "ClientToken": str,
+    },
+)
+_OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourcePolicyRequestRequestTypeDef",
+    {
+        "PolicyRevisionId": str,
+    },
+    total=False,
+)
+
+class PutResourcePolicyRequestRequestTypeDef(
+    _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
+):
+    pass
+
 StartInferenceSchedulerRequestRequestTypeDef = TypedDict(
     "StartInferenceSchedulerRequestRequestTypeDef",
     {
         "InferenceSchedulerName": str,
     },
 )
 
@@ -638,14 +715,22 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateActiveModelVersionRequestRequestTypeDef = TypedDict(
+    "UpdateActiveModelVersionRequestRequestTypeDef",
+    {
+        "ModelName": str,
+        "ModelVersion": int,
+    },
+)
+
 _RequiredUpdateLabelGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLabelGroupRequestRequestTypeDef",
     {
         "LabelGroupName": str,
     },
 )
 _OptionalUpdateLabelGroupRequestRequestTypeDef = TypedDict(
@@ -700,14 +785,36 @@
 )
 
 class CreateLabelGroupRequestRequestTypeDef(
     _RequiredCreateLabelGroupRequestRequestTypeDef, _OptionalCreateLabelGroupRequestRequestTypeDef
 ):
     pass
 
+_RequiredImportDatasetRequestRequestTypeDef = TypedDict(
+    "_RequiredImportDatasetRequestRequestTypeDef",
+    {
+        "SourceDatasetArn": str,
+        "ClientToken": str,
+    },
+)
+_OptionalImportDatasetRequestRequestTypeDef = TypedDict(
+    "_OptionalImportDatasetRequestRequestTypeDef",
+    {
+        "DatasetName": str,
+        "ServerSideKmsKeyId": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class ImportDatasetRequestRequestTypeDef(
+    _RequiredImportDatasetRequestRequestTypeDef, _OptionalImportDatasetRequestRequestTypeDef
+):
+    pass
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -783,29 +890,72 @@
         "Notes": str,
         "Equipment": str,
         "CreatedAt": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeResourcePolicyResponseTypeDef = TypedDict(
+    "DescribeResourcePolicyResponseTypeDef",
+    {
+        "PolicyRevisionId": str,
+        "ResourcePolicy": str,
+        "CreationTime": datetime,
+        "LastModifiedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImportDatasetResponseTypeDef = TypedDict(
+    "ImportDatasetResponseTypeDef",
+    {
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Status": DatasetStatusType,
+        "JobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportModelVersionResponseTypeDef = TypedDict(
+    "ImportModelVersionResponseTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "ModelVersionArn": str,
+        "ModelVersion": int,
+        "Status": ModelVersionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "ResourceArn": str,
+        "PolicyRevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartDataIngestionJobResponseTypeDef = TypedDict(
     "StartDataIngestionJobResponseTypeDef",
     {
         "JobId": str,
         "Status": IngestionJobStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -831,14 +981,27 @@
         "InferenceSchedulerName": str,
         "InferenceSchedulerArn": str,
         "Status": InferenceSchedulerStatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateActiveModelVersionResponseTypeDef = TypedDict(
+    "UpdateActiveModelVersionResponseTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "CurrentActiveVersion": int,
+        "PreviousActiveVersion": int,
+        "CurrentActiveVersionArn": str,
+        "PreviousActiveVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateLabelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLabelRequestRequestTypeDef",
     {
         "LabelGroupName": str,
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
         "Rating": LabelRatingType,
@@ -927,14 +1090,40 @@
 )
 
 class ListLabelsRequestRequestTypeDef(
     _RequiredListLabelsRequestRequestTypeDef, _OptionalListLabelsRequestRequestTypeDef
 ):
     pass
 
+_RequiredListModelVersionsRequestRequestTypeDef = TypedDict(
+    "_RequiredListModelVersionsRequestRequestTypeDef",
+    {
+        "ModelName": str,
+    },
+)
+_OptionalListModelVersionsRequestRequestTypeDef = TypedDict(
+    "_OptionalListModelVersionsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "MaxResults": int,
+        "Status": ModelVersionStatusType,
+        "SourceType": ModelVersionSourceTypeType,
+        "CreatedAtEndTime": TimestampTypeDef,
+        "CreatedAtStartTime": TimestampTypeDef,
+        "MaxModelVersion": int,
+        "MinModelVersion": int,
+    },
+    total=False,
+)
+
+class ListModelVersionsRequestRequestTypeDef(
+    _RequiredListModelVersionsRequestRequestTypeDef, _OptionalListModelVersionsRequestRequestTypeDef
+):
+    pass
+
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "NextToken": str,
         "DatasetSummaries": List[DatasetSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1045,14 +1234,23 @@
     {
         "S3InputConfiguration": LabelsS3InputConfigurationTypeDef,
         "LabelGroupName": str,
     },
     total=False,
 )
 
+ListModelVersionsResponseTypeDef = TypedDict(
+    "ListModelVersionsResponseTypeDef",
+    {
+        "NextToken": str,
+        "ModelVersionSummaries": List[ModelVersionSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListModelsResponseTypeDef = TypedDict(
     "ListModelsResponseTypeDef",
     {
         "NextToken": str,
         "ModelSummaries": List[ModelSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1254,18 +1452,88 @@
         "TrainingExecutionEndTime": datetime,
         "FailedReason": str,
         "ModelMetrics": str,
         "LastUpdatedTime": datetime,
         "CreatedAt": datetime,
         "ServerSideKmsKeyId": str,
         "OffCondition": str,
+        "SourceModelVersionArn": str,
+        "ImportJobStartTime": datetime,
+        "ImportJobEndTime": datetime,
+        "ActiveModelVersion": int,
+        "ActiveModelVersionArn": str,
+        "ModelVersionActivatedAt": datetime,
+        "PreviousActiveModelVersion": int,
+        "PreviousActiveModelVersionArn": str,
+        "PreviousModelVersionActivatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeModelVersionResponseTypeDef = TypedDict(
+    "DescribeModelVersionResponseTypeDef",
+    {
+        "ModelName": str,
+        "ModelArn": str,
+        "ModelVersion": int,
+        "ModelVersionArn": str,
+        "Status": ModelVersionStatusType,
+        "SourceType": ModelVersionSourceTypeType,
+        "DatasetName": str,
+        "DatasetArn": str,
+        "Schema": str,
+        "LabelsInputConfiguration": LabelsInputConfigurationTypeDef,
+        "TrainingDataStartTime": datetime,
+        "TrainingDataEndTime": datetime,
+        "EvaluationDataStartTime": datetime,
+        "EvaluationDataEndTime": datetime,
+        "RoleArn": str,
+        "DataPreProcessingConfiguration": DataPreProcessingConfigurationTypeDef,
+        "TrainingExecutionStartTime": datetime,
+        "TrainingExecutionEndTime": datetime,
+        "FailedReason": str,
+        "ModelMetrics": str,
+        "LastUpdatedTime": datetime,
+        "CreatedAt": datetime,
+        "ServerSideKmsKeyId": str,
+        "OffCondition": str,
+        "SourceModelVersionArn": str,
+        "ImportJobStartTime": datetime,
+        "ImportJobEndTime": datetime,
+        "ImportedDataSizeInBytes": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredImportModelVersionRequestRequestTypeDef = TypedDict(
+    "_RequiredImportModelVersionRequestRequestTypeDef",
+    {
+        "SourceModelVersionArn": str,
+        "DatasetName": str,
+        "ClientToken": str,
+    },
+)
+_OptionalImportModelVersionRequestRequestTypeDef = TypedDict(
+    "_OptionalImportModelVersionRequestRequestTypeDef",
+    {
+        "ModelName": str,
+        "LabelsInputConfiguration": LabelsInputConfigurationTypeDef,
+        "RoleArn": str,
+        "ServerSideKmsKeyId": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class ImportModelVersionRequestRequestTypeDef(
+    _RequiredImportModelVersionRequestRequestTypeDef,
+    _OptionalImportModelVersionRequestRequestTypeDef,
+):
+    pass
+
 ListSensorStatisticsResponseTypeDef = TypedDict(
     "ListSensorStatisticsResponseTypeDef",
     {
         "SensorStatisticsSummaries": List[SensorStatisticsSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1301,14 +1569,15 @@
         "FailedReason": str,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "StatusDetail": str,
         "IngestedDataSize": int,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
+        "SourceDatasetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatasetResponseTypeDef = TypedDict(
     "DescribeDatasetResponseTypeDef",
     {
@@ -1321,10 +1590,11 @@
         "ServerSideKmsKeyId": str,
         "IngestionInputConfiguration": IngestionInputConfigurationTypeDef,
         "DataQualitySummary": DataQualitySummaryTypeDef,
         "IngestedFilesSummary": IngestedFilesSummaryTypeDef,
         "RoleArn": str,
         "DataStartTime": datetime,
         "DataEndTime": datetime,
+        "SourceDatasetArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-lookoutequipment-2.5.2.post1/types_aiobotocore_lookoutequipment.egg-info/SOURCES.txt` & `types-aiobotocore-lookoutequipment-2.5.2.post2/types_aiobotocore_lookoutequipment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

