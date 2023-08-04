# Comparing `tmp/databricks_vectorsearch_preview-0.16-py3-none-any.whl.zip` & `tmp/databricks_vectorsearch_preview-0.17-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,9 @@
-Zip file size: 20386 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 16:27 databricks/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 16:27 databricks/vector_search/__init__.py
--rw-r--r--  2.0 unx    10267 b- defN 23-Jul-18 16:31 databricks/vector_search/client.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 16:27 databricks/vector_search/proto/__init__.py
--rw-r--r--  2.0 unx    76905 b- defN 23-Jul-18 21:29 databricks/vector_search/proto/messages_pb2.py
--rw-r--r--  2.0 unx     9837 b- defN 23-Jul-18 21:32 databricks/vector_search/proto/service_pb2.py
--rw-r--r--  2.0 unx    38292 b- defN 23-Jul-18 16:27 databricks/vector_search/proto/taxonomy_pb2.py
--rw-r--r--  2.0 unx    13028 b- defN 23-Jul-18 21:36 databricks/vector_search/proto/well_known_types_pb2.py
--rw-r--r--  2.0 unx      570 b- defN 23-Jul-18 21:41 databricks_vectorsearch_preview-0.16.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 21:41 databricks_vectorsearch_preview-0.16.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-18 21:41 databricks_vectorsearch_preview-0.16.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1165 b- defN 23-Jul-18 21:41 databricks_vectorsearch_preview-0.16.dist-info/RECORD
-12 files, 150167 bytes uncompressed, 18362 bytes compressed:  87.8%
+Zip file size: 4086 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-20 17:44 databricks/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-20 17:44 databricks/vector_search/__init__.py
+-rw-r--r--  2.0 unx     9017 b- defN 23-Aug-04 00:05 databricks/vector_search/client.py
+-rw-r--r--  2.0 unx      570 b- defN 23-Aug-04 00:16 databricks_vectorsearch_preview-0.17.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 00:16 databricks_vectorsearch_preview-0.17.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Aug-04 00:16 databricks_vectorsearch_preview-0.17.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      646 b- defN 23-Aug-04 00:16 databricks_vectorsearch_preview-0.17.dist-info/RECORD
+7 files, 10336 bytes uncompressed, 2908 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -3,35 +3,20 @@
 
 Filename: databricks/vector_search/__init__.py
 Comment: 
 
 Filename: databricks/vector_search/client.py
 Comment: 
 
-Filename: databricks/vector_search/proto/__init__.py
+Filename: databricks_vectorsearch_preview-0.17.dist-info/METADATA
 Comment: 
 
-Filename: databricks/vector_search/proto/messages_pb2.py
+Filename: databricks_vectorsearch_preview-0.17.dist-info/WHEEL
 Comment: 
 
-Filename: databricks/vector_search/proto/service_pb2.py
+Filename: databricks_vectorsearch_preview-0.17.dist-info/top_level.txt
 Comment: 
 
-Filename: databricks/vector_search/proto/taxonomy_pb2.py
-Comment: 
-
-Filename: databricks/vector_search/proto/well_known_types_pb2.py
-Comment: 
-
-Filename: databricks_vectorsearch_preview-0.16.dist-info/METADATA
-Comment: 
-
-Filename: databricks_vectorsearch_preview-0.16.dist-info/WHEEL
-Comment: 
-
-Filename: databricks_vectorsearch_preview-0.16.dist-info/top_level.txt
-Comment: 
-
-Filename: databricks_vectorsearch_preview-0.16.dist-info/RECORD
+Filename: databricks_vectorsearch_preview-0.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databricks/vector_search/client.py

```diff
@@ -2,31 +2,14 @@
 import logging
 from typing import Dict, List, Optional
 
 import requests
 from google.protobuf.json_format import MessageToJson
 from mlflow.utils import databricks_utils
 
-from databricks.vector_search.proto.messages_pb2 import (
-    CreateVectorSearchCatalogRequest,
-    CreateVectorSearchIndexRequest,
-    QueryVectorSearchIndexRequest,
-    VectorSearchIndexPipelineSpec,
-    ListVectorSearchIndexRequest,
-)
-
-# logging.basicConfig(level=logging.WARNING)
-# log = logging.getLogger("databricks.vector_search.client")
-# log.setLevel(logging.INFO)
-
-
-# Assign the class VectorSearchIndexPipelineSpec.VectorIndex to VectorIndex
-VectorIndex = VectorSearchIndexPipelineSpec.VectorIndex
-
-
 class VectorSearchClient:
     """
     Client for interacting with the Vector Search API for Databricks.
 
     Example usage:
 
         client = VectorSearchClient()
@@ -73,22 +56,21 @@
         """
         Creates a Vector Search catalog.
 
         :param catalog_name: The name of the vector search catalog to be created.
 
         :return: The response from the API call.
         """
-        catalog_request = CreateVectorSearchCatalogRequest()
-        catalog_request.name = catalog_name
+        json_data = {
+            "name": catalog_name
+        }
         return self._call_endpoint(
             "/api/2.0/vector-search/catalog",
             "POST",
-            json=json.loads(
-                MessageToJson(catalog_request, preserving_proto_field_name=True)
-            ),
+            json=json_data,
         )
 
     ### This method will delete the vector search catalog in UC
     # catalog_name is the vector search catalog name to be deleted
     def delete_catalog(self, catalog_name):
         """
         Deletes the specified Vector Search catalog.
@@ -147,32 +129,29 @@
             source_table_name="my_catalog.schema1.table1",
             dest_index_name="vector.schema1.table1_index",
             primary_key="doc_id",
             index_column="text",
             embedding_model_endpoint_name="e5-large-v2")
         print(response)
         """
-        index_request = CreateVectorSearchIndexRequest()
-
-        vector_index_column = VectorIndex()
-        vector_index_column.column = index_column
-        vector_index_column.embedding_model_endpoint_name = (
-            embedding_model_endpoint_name
-        )
-
-        index_request.index_pipeline_spec.src_table = source_table_name
-        index_request.index_pipeline_spec.dest_index = dest_index_name
-        index_request.index_pipeline_spec.primary_key = primary_key
-        index_request.index_pipeline_spec.vector_index.MergeFrom(vector_index_column)
-        index_request.index_pipeline_spec.continuous.SetInParent()
-
-        json_str = MessageToJson(index_request, preserving_proto_field_name=True)
+        json_data = {
+            "index_pipeline_spec": {
+                "continuous": {},
+                "src_table": source_table_name,
+                "dest_index": dest_index_name,
+                "primary_key": primary_key,
+                "vector_index": {
+                    "column": index_column,
+                    "embedding_model_endpoint_name": embedding_model_endpoint_name
+                }
+            }
+        }
 
         return self._call_endpoint(
-            "/api/2.0/vector-search/index", "POST", json=json.loads(json_str)
+            "/api/2.0/vector-search/index", "POST", json=json_data
         )
 
     ### This method will get the index definition
     # index_name is the index name created under the online catalog, this must be in the format of <vector search catalog>.<schema>.<table>
     def get_index(self, index_name):
         """
         Retrieves the specified index.
@@ -215,27 +194,25 @@
             index_name="vector.schema1.table1_index",
             query_text="What is spark connect?",
             columns=["text", "source"],
             filter={"id NOT": ("10", "1")},
             num_results=3)
         print(response)
         """
-        query_request = QueryVectorSearchIndexRequest()
-        query_request.query = query_text
-        if filter is not None:
-            query_request.filters_json = json.dumps(filter)
-        query_request.columns.extend(columns)
-        query_request.num_results = num_results
-
-        json_str = MessageToJson(query_request, preserving_proto_field_name=True)
+        json_data = {
+            "query": query_text,
+            "num_results": num_results,
+            "columns": columns,
+            "filters_json": json.dumps(filter) if filter else None
+        }
 
         return self._call_endpoint(
             f"/api/2.0/vector-search/index/{index_name}/query",
             "GET",
-            json=json.loads(json_str),
+            json=json_data,
         )
 
     # index_name is the index name created under the online catalog, this must be in the format of <vector search catalog>.<schema>.<table>
     def delete_index(self, index_name):
         """
         Deletes the specified index in the Vector Search cluster.
 
@@ -253,14 +230,13 @@
         """
         Lists all existing indexes created under the specified catalog.
 
         :param catalog_name: The name of the catalog.
 
         :return: The response from the API call.
         """
-        list_index_request = ListVectorSearchIndexRequest()
-        list_index_request.catalog_name = catalog_name
-        json_str = MessageToJson(list_index_request, preserving_proto_field_name=True)
-
+        json_data = {
+            "catalog_name": catalog_name
+        }
         return self._call_endpoint(
-            f"/api/2.0/vector-search/index", "GET", json=json.loads(json_str)
+            f"/api/2.0/vector-search/index", "GET", json=json_data
         )
```

## Comparing `databricks_vectorsearch_preview-0.16.dist-info/METADATA` & `databricks_vectorsearch_preview-0.17.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-vectorsearch-preview
-Version: 0.16
+Version: 0.17
 Summary: Databricks Vector Search Client
 Home-page: UNKNOWN
 Author: Databirkcs
 Author-email: feedback@databricks.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

