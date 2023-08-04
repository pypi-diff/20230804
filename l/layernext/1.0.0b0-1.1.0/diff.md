# Comparing `tmp/layernext-1.0.0b0.tar.gz` & `tmp/layernext-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layernext-1.0.0b0.tar", last modified: Thu Jul 13 20:03:38 2023, max compression
+gzip compressed data, was "layernext-1.1.0.tar", last modified: Fri Aug  4 06:35:44 2023, max compression
```

## Comparing `layernext-1.0.0b0.tar` & `layernext-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-13 20:03:38.448120 layernext-1.0.0b0/
--rw-r--r--   0 channawijerathna   (501) staff       (20)     5651 2023-07-13 20:03:38.447928 layernext-1.0.0b0/PKG-INFO
--rw-r--r--   0 channawijerathna   (501) staff       (20)     5046 2023-07-13 19:59:20.000000 layernext-1.0.0b0/README.md
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-13 20:03:38.439955 layernext-1.0.0b0/layernext/
--rw-r--r--   0 channawijerathna   (501) staff       (20)    49823 2023-07-13 20:01:43.000000 layernext-1.0.0b0/layernext/__init__.py
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-13 20:03:38.445859 layernext-1.0.0b0/layernext/datalake/
--rw-r--r--   0 channawijerathna   (501) staff       (20)     9330 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/__init__.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     8820 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/annotation.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      873 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/aws_s3_client.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1001 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/azure_client.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      889 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/constants.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)    36049 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/datalakeinterface.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)        0 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/dataset.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      519 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/file_trash.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)    10724 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/file_upload.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      915 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/gcs_client.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1516 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/ground_truth.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1286 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/keys.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     3514 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/label.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/logger.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1801 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/metadata.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      849 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/model_run.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1301 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/query.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      287 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/storage_client.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     2566 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/storage_interface.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     7504 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/datalake/storage_upload.py
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-13 20:03:38.446877 layernext-1.0.0b0/layernext/dataset/
--rw-r--r--   0 channawijerathna   (501) staff       (20)     3111 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/dataset/__init__.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     4790 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/dataset/dataset.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     8999 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/dataset/datasetinterface.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/dataset/logger.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)    15591 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/dataset/sync.py
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-13 20:03:38.447636 layernext-1.0.0b0/layernext/studio/
--rw-r--r--   0 channawijerathna   (501) staff       (20)     2561 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/studio/__init__.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/studio/logger.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     3435 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/studio/project.py
--rw-r--r--   0 channawijerathna   (501) staff       (20)     9624 2023-07-13 19:59:20.000000 layernext-1.0.0b0/layernext/studio/studiointerface.py
-drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-07-13 20:03:38.440882 layernext-1.0.0b0/layernext.egg-info/
--rw-r--r--   0 channawijerathna   (501) staff       (20)     5651 2023-07-13 20:03:38.000000 layernext-1.0.0b0/layernext.egg-info/PKG-INFO
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1136 2023-07-13 20:03:38.000000 layernext-1.0.0b0/layernext.egg-info/SOURCES.txt
--rw-r--r--   0 channawijerathna   (501) staff       (20)        1 2023-07-13 20:03:38.000000 layernext-1.0.0b0/layernext.egg-info/dependency_links.txt
--rw-r--r--   0 channawijerathna   (501) staff       (20)       47 2023-07-13 20:03:38.000000 layernext-1.0.0b0/layernext.egg-info/requires.txt
--rw-r--r--   0 channawijerathna   (501) staff       (20)       10 2023-07-13 20:03:38.000000 layernext-1.0.0b0/layernext.egg-info/top_level.txt
--rw-r--r--   0 channawijerathna   (501) staff       (20)       38 2023-07-13 20:03:38.448174 layernext-1.0.0b0/setup.cfg
--rw-r--r--   0 channawijerathna   (501) staff       (20)     1665 2023-07-13 20:02:53.000000 layernext-1.0.0b0/setup.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-04 06:35:44.342084 layernext-1.1.0/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1073 2023-08-04 06:18:17.000000 layernext-1.1.0/LICENSE
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     5671 2023-08-04 06:35:44.341903 layernext-1.1.0/PKG-INFO
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     5046 2023-07-13 19:59:20.000000 layernext-1.1.0/README.md
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-04 06:35:44.330163 layernext-1.1.0/layernext/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    52713 2023-08-04 06:35:14.000000 layernext-1.1.0/layernext/__init__.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-04 06:35:44.339377 layernext-1.1.0/layernext/datalake/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    10172 2023-08-04 06:18:17.000000 layernext-1.1.0/layernext/datalake/__init__.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    12260 2023-08-04 06:32:48.000000 layernext-1.1.0/layernext/datalake/annotation.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      873 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/aws_s3_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1001 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/azure_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1028 2023-08-04 06:18:17.000000 layernext-1.1.0/layernext/datalake/constants.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    36049 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/datalakeinterface.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)        0 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/dataset.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      519 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/file_trash.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    10724 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/file_upload.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      915 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/gcs_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1714 2023-08-04 06:18:17.000000 layernext-1.1.0/layernext/datalake/ground_truth.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1387 2023-08-04 06:18:17.000000 layernext-1.1.0/layernext/datalake/keys.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     4806 2023-08-04 06:18:17.000000 layernext-1.1.0/layernext/datalake/label.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/logger.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1801 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/metadata.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      973 2023-08-04 06:18:17.000000 layernext-1.1.0/layernext/datalake/model_run.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1301 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/query.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      287 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/storage_client.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     2566 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/storage_interface.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     7504 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/datalake/storage_upload.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-04 06:35:44.340900 layernext-1.1.0/layernext/dataset/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     3111 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/dataset/__init__.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     4790 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/dataset/dataset.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     8999 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/dataset/datasetinterface.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/dataset/logger.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)    15591 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/dataset/sync.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-04 06:35:44.341601 layernext-1.1.0/layernext/studio/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     2561 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/studio/__init__.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)      417 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/studio/logger.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     3435 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/studio/project.py
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     9624 2023-07-13 19:59:20.000000 layernext-1.1.0/layernext/studio/studiointerface.py
+drwxr-xr-x   0 channawijerathna   (501) staff       (20)        0 2023-08-04 06:35:44.330960 layernext-1.1.0/layernext.egg-info/
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     5671 2023-08-04 06:35:44.000000 layernext-1.1.0/layernext.egg-info/PKG-INFO
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1144 2023-08-04 06:35:44.000000 layernext-1.1.0/layernext.egg-info/SOURCES.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)        1 2023-08-04 06:35:44.000000 layernext-1.1.0/layernext.egg-info/dependency_links.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)       47 2023-08-04 06:35:44.000000 layernext-1.1.0/layernext.egg-info/requires.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)       10 2023-08-04 06:35:44.000000 layernext-1.1.0/layernext.egg-info/top_level.txt
+-rw-r--r--   0 channawijerathna   (501) staff       (20)       38 2023-08-04 06:35:44.342132 layernext-1.1.0/setup.cfg
+-rw-r--r--   0 channawijerathna   (501) staff       (20)     1665 2023-08-04 06:35:26.000000 layernext-1.1.0/setup.py
```

### Comparing `layernext-1.0.0b0/PKG-INFO` & `layernext-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: layernext
-Version: 1.0.0b0
+Version: 1.1.0
 Summary: LayerNext Python SDK
 Home-page: UNKNOWN
 Author: LayerNext
 Author-email: <support@layernext.ai>
 License: UNKNOWN
 Keywords: python,datalake,datasetsync,ai,annotation,layernext,layernext,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # layernext-python-sdk
 
 LayerNext Python API Client
 Sync (upload/download) with LayerNext stacks via APIs from your local machine
```

### Comparing `layernext-1.0.0b0/README.md` & `layernext-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/__init__.py` & `layernext-1.1.0/layernext/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 
 from layernext import datalake, dataset, studio
-from layernext.datalake.constants import MediaType, ObjectType
+from layernext.datalake.constants import AnnotationUploadType, MediaType, ObjectType
 
-__version__ = '1.0.0b0'
+__version__ = '1.1.0'
 
 
 class LayerNextClient:
     """
     Python SDK of LayerNext
     """
 
@@ -26,48 +26,151 @@
         _datalake_client = datalake.DatalakeClient(
             self.encoded_key_secret, self.layernext_url)
 
         version_id = __version__.split('b')[0]
 
         _datalake_client.check_sdk_version_compatibility(version_id)
 
-    def upload_annoations_for_folder(
+    """
+    Annotation data upload from json file with new format and unique_name
+    """
+    def upload_annotations_by_unique_name    (
+            self,
+            operation_unique_id: str,
+            json_data_file_path: str,
+            is_normalized: bool,
+            is_model_run: bool
+    ):
+        
+        self.__upload_annotations(
+            None,
+            operation_unique_id,
+            json_data_file_path,
+            None,
+            is_normalized,
+            is_model_run,
+            upload_type=AnnotationUploadType.BY_UNIQUE_NAME
+        )
+
+    """
+    Annotation data upload from json file with new format and bucket name
+    """
+    def upload_annotations_by_storage_path    (
+            self,
+            operation_unique_id: str,
+            json_data_file_path: str,
+            is_normalized: bool,
+            is_model_run: bool,
+            bucket_name: str = None
+    ):
+        
+        self.__upload_annotations(
+            None,
+            operation_unique_id,
+            json_data_file_path,
+            None,
+            is_normalized,
+            is_model_run,
+            bucket_name=bucket_name,
+            upload_type=AnnotationUploadType.BY_STORAGE_PATH
+        )
+
+    """
+    Old annotation data upload from json file
+    """
+    def upload_annoations_for_folder    (
             self,
             collection_base_path: str,
             operation_unique_id: str,
             json_data_file_path: str,
             shape_type: str,
             is_normalized: bool,
             is_model_run: bool,
             destination_project_id: str = None
     ):
+        
+        self.__upload_annotations(
+            collection_base_path,
+            operation_unique_id,
+            json_data_file_path,
+            shape_type,
+            is_normalized,
+            is_model_run,
+            destination_project_id,
+            None,
+            upload_type=AnnotationUploadType.BY_FILE_NAME_OR_UNIQUE_NAME
+        )
+
+    """
+    New annotation data upload from json file with new format and file name
+    """
+    def upload_annotations_for_folder    (
+            self,
+            collection_name: str,
+            operation_unique_id: str,
+            json_data_file_path: str,
+            is_normalized: bool,
+            is_model_run: bool
+    ):
+        
+        self.__upload_annotations(
+            collection_name,
+            operation_unique_id,
+            json_data_file_path,
+            None,
+            is_normalized,
+            is_model_run,
+            upload_type=AnnotationUploadType.BY_FILE_NAME
+        )
+        
+
+    def __upload_annotations(
+            self,
+            collection_base_path: str,
+            operation_unique_id: str,
+            json_data_file_path: str,
+            shape_type: str,
+            is_normalized: bool,
+            is_model_run: bool,
+            destination_project_id: str = None,
+            version: str = "v2",
+            bucket_name: str = None,
+            upload_type: AnnotationUploadType = 1
+    ):
         """
         Upload annotation data from a json file
         """
         # init datalake client
         _datalake_client = datalake.DatalakeClient(
             self.encoded_key_secret, self.layernext_url)
 
         if is_model_run:
             _datalake_client.upload_modelrun_from_json(
                 collection_base_path,
                 operation_unique_id,
                 json_data_file_path,
                 shape_type,
                 is_normalized,
-                destination_project_id
+                destination_project_id,
+                version,
+                bucket_name,
+                upload_type
             )
         else:
             _datalake_client.upload_groundtruth_from_json(
                 collection_base_path,
                 operation_unique_id,
                 json_data_file_path,
                 shape_type,
                 is_normalized,
-                destination_project_id)
+                destination_project_id,
+                version,
+                bucket_name,
+                upload_type
+            )
 
     """
     Download dataset
     """
 
     def download_dataset(self, version_id: str, export_type: str, custom_download_path: str = None):
         # init dataset client
@@ -340,15 +443,15 @@
                 file_path, MediaType.IMAGE.value, collection_name, meta_data_object, False)
 
         if (json_data_file_path == None):
             print('annotation upload cannot be done')
         else:
             job_id = upload_details["job_id"]
             self.wait_for_job_complete(job_id)
-            self.upload_annoations_for_folder(
+            self.__upload_annotations(
                 collection_name, operation_unique_id, json_data_file_path, shape_type, is_normalized, is_model_run)
 
         return upload_details
 
     """"
     get upload progress
     """
```

### Comparing `layernext-1.0.0b0/layernext/datalake/__init__.py` & `layernext-1.1.0/layernext/datalake/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import time
 
 from layernext.datalake.annotation import Annotation
 from layernext.datalake.metadata import Metadata
 from layernext.datalake.query import Query
 
 from .ground_truth import GroundTruth
-from .constants import BOX_ANNOTATION, POLYGON_ANNOTATION, LINE_ANNOTATION, MediaType, JobStatus
+from .constants import BOX_ANNOTATION, POLYGON_ANNOTATION, LINE_ANNOTATION, AnnotationUploadType, MediaType, JobStatus
 from .datalakeinterface import DatalakeInterface
 from .file_upload import FileUpload
 from .file_trash import FileTrash
 from .logger import get_debug_logger
 from .model_run import ModelRun
 
 datalake_logger = get_debug_logger('DatalakeClient')
@@ -54,46 +54,57 @@
     def upload_modelrun_from_json(
             self,
             storage_base_path: str,
             model_id: str,
             file_path: str,
             annotation_geometry: str,
             is_normalized: bool,
-            dest_project_id: str
+            dest_project_id: str,
+            version: str,
+            bucket_name: str,
+            upload_type: AnnotationUploadType
+
     ):
         datalake_logger.debug(f'upload_modelrun_from_json file_path={file_path}, '
                               f'annotation_geometry={annotation_geometry}')
         _model = ModelRun(client=self)
         if annotation_geometry == BOX_ANNOTATION:
-            _model.upload_modelrun_json(storage_base_path, model_id, file_path, BOX_ANNOTATION, is_normalized, dest_project_id)
+            _model.upload_modelrun_json(storage_base_path, model_id, file_path, BOX_ANNOTATION, is_normalized, dest_project_id, version, bucket_name, upload_type)
         elif annotation_geometry == POLYGON_ANNOTATION:
-            _model.upload_modelrun_json(storage_base_path, model_id, file_path, POLYGON_ANNOTATION, is_normalized, dest_project_id)
+            _model.upload_modelrun_json(storage_base_path, model_id, file_path, POLYGON_ANNOTATION, is_normalized, dest_project_id, version, bucket_name, upload_type)
         elif annotation_geometry == LINE_ANNOTATION:
-            _model.upload_modelrun_json(storage_base_path, model_id, file_path, LINE_ANNOTATION, is_normalized, dest_project_id)
+            _model.upload_modelrun_json(storage_base_path, model_id, file_path, LINE_ANNOTATION, is_normalized, dest_project_id, version, bucket_name, upload_type)
+        elif annotation_geometry is None:
+            _model.upload_modelrun_json(storage_base_path, model_id, file_path, None, is_normalized, dest_project_id, version, bucket_name, upload_type)
         else:
             datalake_logger.debug(f'unsupported annotation_geometry={annotation_geometry}')
 
     def upload_groundtruth_from_json(
             self,
             storage_base_path: str,
             operation_id: str,
             file_path: str,
             annotation_geometry: str,
             is_normalized: bool,
-            dest_project_id: str
+            dest_project_id: str,
+            version: str,
+            bucket_name: str,
+            upload_type: AnnotationUploadType
     ):
         datalake_logger.debug(f'upload_groundtruth_from_json file_path={file_path}, '
                               f'annotation_geometry={annotation_geometry}')
         _groundTruth = GroundTruth(client=self)
         if annotation_geometry == BOX_ANNOTATION:
-            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, BOX_ANNOTATION, is_normalized, dest_project_id)
+            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, BOX_ANNOTATION, is_normalized, dest_project_id, version, bucket_name, upload_type)
         elif annotation_geometry == POLYGON_ANNOTATION:
-            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, POLYGON_ANNOTATION, is_normalized, dest_project_id)
+            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, POLYGON_ANNOTATION, is_normalized, dest_project_id, version, bucket_name, upload_type)
         elif annotation_geometry == LINE_ANNOTATION:
-            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, LINE_ANNOTATION, is_normalized, dest_project_id)
+            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, LINE_ANNOTATION, is_normalized, dest_project_id, version, bucket_name, upload_type)
+        elif annotation_geometry is None:
+            _groundTruth.upload_groundtruth_json(storage_base_path, operation_id, file_path, None, is_normalized, dest_project_id, version, bucket_name, upload_type)
         else:
             datalake_logger.debug(f'unsupported annotation_geometry={annotation_geometry}')
 
     def file_upload(self, path: str, collection_type, collection_name, meta_data_object, application_code, meta_data_override, storage_prefix_path):
         _upload = FileUpload(client=self, application_code=application_code)
         upload_res = _upload.file_upload_initiate(path, collection_type, collection_name, meta_data_object, meta_data_override, storage_prefix_path)
         return upload_res
```

### Comparing `layernext-1.0.0b0/layernext/datalake/annotation.py` & `layernext-1.1.0/layernext/datalake/annotation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import json
 import uuid
 from typing import TYPE_CHECKING
 import time
 
-from .constants import BOX_ANNOTATION, OPERATION_TYPE_ANNOTATION, OPERATION_MODE_AUTO, META_UPDATE_REQUEST_BATCH_SIZE, \
-    POLYGON_ANNOTATION, LINE_ANNOTATION
-from .keys import IMAGES, IMAGE, ANNOTATIONS, BBOX, BOX_BOUNDARIES_AND_DIMENSIONS, X, Y, W, H, POINTS, LABEL, \
+from .constants import BOX_ANNOTATION, OPERATION_MODE_HUMAN, OPERATION_TYPE_ANNOTATION, OPERATION_MODE_AUTO, META_UPDATE_REQUEST_BATCH_SIZE, \
+    POLYGON_ANNOTATION, LINE_ANNOTATION, AnnotationUploadType
+from .keys import ATTRIBUTES, BUCKET_NAME, IMAGES, IMAGE, ANNOTATIONS, BBOX, BOX_BOUNDARIES_AND_DIMENSIONS, STORAGE_NAME, STORAGE_PATH, VALUE, X, Y, W, H, POINTS, LABEL, \
     LABEL_TEXT, REF, KEY, COLOR, ATTRIBUTE_VALUES, METADATA, TEXTS, TYPE, ID, SHAPE_ID, CREATED_AT, OBJECT_KEY, \
     ANNOTATION_OBJECTS, DATA, IS_USER_ANNOTATED, UPDATED_AT, LINE, POLYGON, CONFIDENCE
 from .logger import get_debug_logger
 from .label import Label
 
 if TYPE_CHECKING:
     from . import DatalakeClient
@@ -59,46 +59,75 @@
             self,
             storage_base_path: str,
             operation_id: str,
             file_path: str,
             annotation_geometry: str,
             operation_mode: int,
             is_normalized: bool,
-            dest_project_id: str
+            dest_project_id: str,
+            version: str,
+            bucket_name: str,
+            upload_type: AnnotationUploadType
     ):
 
         session_uuid = str(datetime.datetime.now().timestamp())
+        storage_path = None
 
         # load json file
         f = open(file_path)
         annotation_data = json.load(f)
         f.close()
 
         # get labels,attributes,values in the json files as a dictionary
-        label_attribute_values_dict = Label.get_label_attribute_values_dict(annotation_data)
+        if version is None:
+            label_attribute_values_dict = Label.get_label_attribute_values_dict(annotation_data)
+        elif version == 'v2':
+            label_attribute_values_dict = Label.get_label_attribute_values_dict_v2(annotation_data)
+        else:
+            raise Exception(f'Invalid version: {version}')
         annotation_logger.debug('retrieving datalake label references started')
         label_references = self._client.datalake_interface.find_datalake_label_references(label_attribute_values_dict)
         annotation_logger.debug('retrieving datalake label references finished')
 
         # format data to call datalake operation data update API
         meta_updates_list = []
         request_batch_size = META_UPDATE_REQUEST_BATCH_SIZE
         total_images_count = len(annotation_data[IMAGES])
         uploaded_images_count = 0
         annotation_logger.debug(f'total images count with annotation data: {total_images_count}')
 
         for image in annotation_data[IMAGES]:
-            if storage_base_path is None:
+            if upload_type == AnnotationUploadType.BY_FILE_NAME:
+                object_key = f'{storage_base_path}_{image[IMAGE]}'
+            elif upload_type == AnnotationUploadType.BY_STORAGE_PATH:
+                object_key = None
+                storage_path = f'{image[IMAGE]}'
+            elif upload_type == AnnotationUploadType.BY_UNIQUE_NAME:
                 object_key = f'{image[IMAGE]}'
+            elif upload_type == AnnotationUploadType.BY_FILE_NAME_OR_UNIQUE_NAME:
+                if storage_base_path is None:
+                    object_key = f'{image[IMAGE]}'
+                else:
+                    object_key = f'{storage_base_path}_{image[IMAGE]}'
             else:
-                object_key = f'{storage_base_path}_{image[IMAGE]}'
+                raise Exception(f'Invalid upload type: {upload_type}')
+            
+            if STORAGE_NAME in image:
+                bucket_name = image[STORAGE_NAME]
+            
             annotation_objects = []
             i = 1
             for annotation in image[ANNOTATIONS]:
                 annotation_object = {}
+                if annotation_geometry is None and TYPE not in annotation:
+                    raise Exception(f'Invalid annotation data. Annotation type not found in annotation {annotation}')
+                    
+                if TYPE in annotation:
+                    annotation_geometry = annotation[TYPE]
+
                 # calculate coordinates and other dimensions
                 if annotation_geometry == BOX_ANNOTATION:
                     self.format_bbox_annotation(annotation, annotation_object)
                 elif annotation_geometry == POLYGON_ANNOTATION:
                     self.format_polygon_annotation(annotation, annotation_object)
                 elif annotation_geometry == LINE_ANNOTATION:
                     self.format_line_annotation(annotation, annotation_object)
@@ -116,41 +145,70 @@
                     annotation_object[CONFIDENCE] = annotation[CONFIDENCE]
 
                 try:
                     # assign label class
                     annotation_object[LABEL] = {
                         LABEL: label_references[annotation[LABEL]][REF],
                         LABEL_TEXT: annotation[LABEL],
+                        METADATA: {},
                         KEY: label_references[annotation[LABEL]][REF],
                         COLOR: label_references[annotation[LABEL]][COLOR],
                         ATTRIBUTE_VALUES: {}
                     }
                     # assign label attribute and values
-                    if METADATA in annotation:
-                        for attr, val in annotation[METADATA].items():
-                            try:
-                                attr_ref = label_references[annotation[LABEL]][TEXTS][attr][REF]
-                                val_ref = label_references[annotation[LABEL]][TEXTS][attr][TEXTS][val]
-                                annotation_object[LABEL][ATTRIBUTE_VALUES][attr_ref] = val_ref
-                            except (TypeError, KeyError, Exception) as te:
-                                print(f"An Error Occurred at attribute value reference finding for object_key: "
-                                      f"{object_key}", te)
-                                continue
+                    if version is None:
+                        if METADATA in annotation:
+                            for attr, val in annotation[METADATA].items():
+                                try:
+                                    attr_ref = label_references[annotation[LABEL]][TEXTS][attr][REF]
+                                    val_ref = label_references[annotation[LABEL]][TEXTS][attr][TEXTS][val]
+                                    if attr_ref not in annotation_object[LABEL][ATTRIBUTE_VALUES]:
+                                        annotation_object[LABEL][ATTRIBUTE_VALUES][attr_ref] = []
+                                    annotation_object[LABEL][ATTRIBUTE_VALUES][attr_ref].append(
+                                        {
+                                            VALUE: val_ref, 
+                                            CONFIDENCE: 1 if operation_mode == OPERATION_MODE_HUMAN else annotation[CONFIDENCE]
+                                        }
+                                    )
+                                except (TypeError, KeyError, Exception) as te:
+                                    print(f"An Error Occurred at attribute value reference finding for object_key: "
+                                        f"{object_key}", te)
+                                    continue
+                    elif version == 'v2':
+                        if ATTRIBUTES in annotation:
+                            if METADATA in annotation:
+                                annotation_object[LABEL][METADATA] = annotation[METADATA]
+                            for attr, val_array in annotation[ATTRIBUTES].items():
+                                try:
+                                    attr_ref = label_references[annotation[LABEL]][TEXTS][attr][REF]
+                                    
+                                    for val_obj in val_array:
+                                        val_ref = label_references[annotation[LABEL]][TEXTS][attr][TEXTS][val_obj[VALUE]]
+                                        val_obj[VALUE] = val_ref
+                                    annotation_object[LABEL][ATTRIBUTE_VALUES][attr_ref] = val_array
+                                except (TypeError, KeyError, Exception) as te:
+                                    print(f"An Error Occurred at attribute value reference finding for object_key: "
+                                        f"{object_key}", te)
+                                    continue
+                    else:
+                        raise Exception(f'Invalid version: {version}')
 
                     annotation_objects.append(annotation_object)
                 except (TypeError, KeyError, Exception) as te:
                     print(f"An Error Occurred at label class reference finding for object_key: {object_key}", te)
                     continue
 
             meta_update_data = {
                 ANNOTATION_OBJECTS: annotation_objects,
                 IS_USER_ANNOTATED: False,
             }
             meta_updates = {
                 OBJECT_KEY: object_key,
+                STORAGE_PATH: storage_path,
+                BUCKET_NAME: bucket_name,
                 DATA: meta_update_data
             }
             meta_updates_list.append(meta_updates)
 
             # call datalake operation data update API if batch size equals,
             # this is to reduce memory consumption & to stop request body size exceeding
             if len(meta_updates_list) == request_batch_size:
```

### Comparing `layernext-1.0.0b0/layernext/datalake/aws_s3_client.py` & `layernext-1.1.0/layernext/datalake/aws_s3_client.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/datalake/azure_client.py` & `layernext-1.1.0/layernext/datalake/azure_client.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/datalake/constants.py` & `layernext-1.1.0/layernext/datalake/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,8 +39,14 @@
     IN_PROGRESS = 1
     COMPLETED = 2
     QUEUED = 3
     FAILED = 4
 
 class MetadataUploadType(Enum):
     BY_JSON = 1
-    BY_META_OBJECT = 2
+    BY_META_OBJECT = 2
+
+class AnnotationUploadType(Enum):
+    BY_FILE_NAME = 1
+    BY_STORAGE_PATH = 2
+    BY_UNIQUE_NAME = 3
+    BY_FILE_NAME_OR_UNIQUE_NAME = 4
```

### Comparing `layernext-1.0.0b0/layernext/datalake/datalakeinterface.py` & `layernext-1.1.0/layernext/datalake/datalakeinterface.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/datalake/file_trash.py` & `layernext-1.1.0/layernext/datalake/file_trash.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/datalake/file_upload.py` & `layernext-1.1.0/layernext/datalake/file_upload.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/datalake/gcs_client.py` & `layernext-1.1.0/layernext/datalake/gcs_client.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/datalake/ground_truth.py` & `layernext-1.1.0/layernext/datalake/ground_truth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import TYPE_CHECKING
 
 from .annotation import Annotation
-from .constants import OPERATION_MODE_HUMAN
+from .constants import OPERATION_MODE_HUMAN, AnnotationUploadType
 from .keys import CATEGORIES
 from .label import Label
 from .logger import get_debug_logger
 
 if TYPE_CHECKING:
     from . import DatalakeClient
 
@@ -20,25 +20,31 @@
     def upload_groundtruth_json(
             self,
             storage_base_path: str,
             operation_id: str,
             file_path: str,
             annotation_geometry: str,
             is_normalized: bool,
-            dest_project_id: str
+            dest_project_id: str,
+            version: str,
+            bucket_name: str,
+            upload_type: AnnotationUploadType,
     ):
         ground_truth_logger.debug(f'Started uploading ground truth data for model_id: {operation_id}')
         self.upload_annotation_json(
             storage_base_path,
             operation_id,
             file_path,
             annotation_geometry,
             OPERATION_MODE_HUMAN,
             is_normalized,
-            dest_project_id
+            dest_project_id,
+            version,
+            bucket_name,
+            upload_type,
         )
         ground_truth_logger.debug(f'Finished uploading ground truth data for model_id: {operation_id}')
 
     def upload_coco(self, file_path: str):
         # load json file
         f = open(file_path)
         coco_data = json.load(f)
```

### Comparing `layernext-1.0.0b0/layernext/datalake/keys.py` & `layernext-1.1.0/layernext/datalake/keys.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,19 +36,23 @@
 SHAPE_ID = 'shapeId'
 SUPERCATEGORY = 'supercategory'
 TEXTS = 'texts'
 TYPE = 'type'
 USERNAME = 'userName'
 VALUE_TEXT = 'valueText'
 VALUES = 'values'
+VALUE = 'value'
 W = 'w'
 X = 'x'
 Y = 'y'
 SESSION_ID = "sessionId"
 TOTAL_IMAGE_COUNT = "totalImageCount"
 UPLOADED_IMAGE_COUNT = "uploadedImageCount"
 SELECTION_ID = "selectionId"
 USER_ID = "userId"
 COLLECTION_NAME = "collectionName"
 IS_APPLY_TO_ALL_FILES = "isApplyToAllFiles"
 FILES = "files"
-OBJECT_TYPE = "objectType"
+OBJECT_TYPE = "objectType"
+STORAGE_PATH = "storagePath"
+BUCKET_NAME = "bucketName"
+STORAGE_NAME = "storageName"
```

### Comparing `layernext-1.0.0b0/layernext/datalake/label.py` & `layernext-1.1.0/layernext/datalake/label.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,48 @@
 from typing import TYPE_CHECKING
 
 from .constants import LABEL_CLASS_WITH_ATTRIBUTES
-from .keys import SUPERCATEGORY, NAME, LABEL_TEXT, VALUES, VALUE_TEXT, DESCRIPTION, IMG_FILES, ATTRIBUTES, TYPE, \
+from .keys import SUPERCATEGORY, NAME, LABEL_TEXT, VALUE, VALUES, VALUE_TEXT, DESCRIPTION, IMG_FILES, ATTRIBUTES, TYPE, \
     LABEL_REF, LABEL, LABEL_COLOR, COLOR, IMAGES, ANNOTATIONS, METADATA
 
 if TYPE_CHECKING:
     from . import DatalakeClient
 
 
 class Label:
     def __init__(self, client: "DatalakeClient"):
         self._client = client
 
     @staticmethod
+    def get_label_attribute_values_dict_v2(modelrun_data):
+        label_attribute_values_dict = {}
+
+        # iterate through images
+        for image in modelrun_data[IMAGES]:
+            for annotation in image[ANNOTATIONS]:
+                # if label class not exists in label_attribute_values_dict, then add it
+                if annotation[LABEL] not in label_attribute_values_dict:
+                    label_attribute_values_dict[annotation[LABEL]] = {}
+
+                # add attributes and values to dict from metadata
+                _attribute_value = label_attribute_values_dict[annotation[LABEL]]
+                if ATTRIBUTES in annotation:
+                    _attributes = annotation[ATTRIBUTES]
+                    for attr, val in _attributes.items():
+                        # if attribute not exist, then add it
+                        if attr not in _attribute_value:
+                            _attribute_value[attr] = []
+                        # values array iterate and if value not exist, then add it
+                        for _val in val:
+                            if _val[VALUE] not in _attribute_value[attr]:
+                                _attribute_value[attr].append(_val[VALUE])
+
+        return label_attribute_values_dict
+    
+    @staticmethod
     def get_label_attribute_values_dict(modelrun_data):
         label_attribute_values_dict = {}
 
         # iterate through images
         for image in modelrun_data[IMAGES]:
             for annotation in image[ANNOTATIONS]:
                 # if label class not exists in label_attribute_values_dict, then add it
```

### Comparing `layernext-1.0.0b0/layernext/datalake/metadata.py` & `layernext-1.1.0/layernext/datalake/metadata.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/datalake/model_run.py` & `layernext-1.1.0/layernext/datalake/model_run.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 from typing import TYPE_CHECKING
 
 from .annotation import Annotation
-from .constants import OPERATION_MODE_AUTO
+from .constants import OPERATION_MODE_AUTO, AnnotationUploadType
 from .logger import get_debug_logger
 
 
 if TYPE_CHECKING:
     from . import DatalakeClient
 
 model_logger = get_debug_logger('Model')
 
 
 class ModelRun(Annotation):
     def __init__(self, client: "DatalakeClient"):
         super().__init__(client)
 
-    def upload_modelrun_json(self, storage_base_path: str, model_id: str, file_path: str, annotation_geometry: str, is_normalized: bool, dest_project_id: str):
+    def upload_modelrun_json(self, storage_base_path: str, model_id: str, file_path: str, annotation_geometry: str, is_normalized: bool, dest_project_id: str, version: str, bucket_name: str, upload_type: AnnotationUploadType):
         model_logger.debug(f'Started uploading model run data for model_id: {model_id}')
-        self.upload_annotation_json(storage_base_path, model_id, file_path, annotation_geometry, OPERATION_MODE_AUTO, is_normalized, dest_project_id)
+        self.upload_annotation_json(storage_base_path, model_id, file_path, annotation_geometry, OPERATION_MODE_AUTO, is_normalized, dest_project_id, version, bucket_name, upload_type)
         model_logger.debug(f'Finished uploading model run data for model_id: {model_id}')
```

### Comparing `layernext-1.0.0b0/layernext/datalake/query.py` & `layernext-1.1.0/layernext/datalake/query.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/datalake/storage_interface.py` & `layernext-1.1.0/layernext/datalake/storage_interface.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/datalake/storage_upload.py` & `layernext-1.1.0/layernext/datalake/storage_upload.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/dataset/__init__.py` & `layernext-1.1.0/layernext/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/dataset/dataset.py` & `layernext-1.1.0/layernext/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/dataset/datasetinterface.py` & `layernext-1.1.0/layernext/dataset/datasetinterface.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/dataset/sync.py` & `layernext-1.1.0/layernext/dataset/sync.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/studio/__init__.py` & `layernext-1.1.0/layernext/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/studio/project.py` & `layernext-1.1.0/layernext/studio/project.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext/studio/studiointerface.py` & `layernext-1.1.0/layernext/studio/studiointerface.py`

 * *Files identical despite different names*

### Comparing `layernext-1.0.0b0/layernext.egg-info/PKG-INFO` & `layernext-1.1.0/layernext.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: layernext
-Version: 1.0.0b0
+Version: 1.1.0
 Summary: LayerNext Python SDK
 Home-page: UNKNOWN
 Author: LayerNext
 Author-email: <support@layernext.ai>
 License: UNKNOWN
 Keywords: python,datalake,datasetsync,ai,annotation,layernext,layernext,machine learning
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 # layernext-python-sdk
 
 LayerNext Python API Client
 Sync (upload/download) with LayerNext stacks via APIs from your local machine
```

### Comparing `layernext-1.0.0b0/layernext.egg-info/SOURCES.txt` & `layernext-1.1.0/layernext.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 layernext/__init__.py
 layernext.egg-info/PKG-INFO
 layernext.egg-info/SOURCES.txt
 layernext.egg-info/dependency_links.txt
 layernext.egg-info/requires.txt
```

### Comparing `layernext-1.0.0b0/setup.py` & `layernext-1.1.0/setup.py`

 * *Files identical despite different names*

