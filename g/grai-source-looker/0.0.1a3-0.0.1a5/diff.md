# Comparing `tmp/grai_source_looker-0.0.1a3.tar.gz` & `tmp/grai_source_looker-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_looker-0.0.1a3.tar", max compression
+gzip compressed data, was "grai_source_looker-0.0.1a5.tar", max compression
```

## Comparing `grai_source_looker-0.0.1a3.tar` & `grai_source_looker-0.0.1a5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      133 2023-08-03 09:33:45.520341 grai_source_looker-0.0.1a3/README.md
--rw-r--r--   0        0        0     1123 2023-08-03 13:29:53.571827 grai_source_looker-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0       97 2023-08-03 13:29:56.894502 grai_source_looker-0.0.1a3/src/grai_source_looker/__init__.py
--rw-r--r--   0        0        0     7947 2023-08-03 13:03:53.516927 grai_source_looker-0.0.1a3/src/grai_source_looker/adapters.py
--rw-r--r--   0        0        0       48 2023-08-03 09:59:32.956516 grai_source_looker-0.0.1a3/src/grai_source_looker/api/__init__.py
--rw-r--r--   0        0        0   642045 2023-08-03 09:33:45.526480 grai_source_looker-0.0.1a3/src/grai_source_looker/api/api_models.py
--rw-r--r--   0        0        0     2215 2023-08-03 13:03:53.418465 grai_source_looker-0.0.1a3/src/grai_source_looker/base.py
--rw-r--r--   0        0        0     3015 2023-08-03 13:17:33.954769 grai_source_looker-0.0.1a3/src/grai_source_looker/loader.py
--rw-r--r--   0        0        0     3454 2023-08-03 13:15:52.413917 grai_source_looker-0.0.1a3/src/grai_source_looker/models.py
--rw-r--r--   0        0        0      195 2023-08-03 09:33:45.526746 grai_source_looker-0.0.1a3/src/grai_source_looker/package_definitions.py
--rw-r--r--   0        0        0        0 2023-08-03 09:33:45.526767 grai_source_looker-0.0.1a3/src/grai_source_looker/py.typed
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 grai_source_looker-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      133 2023-08-03 09:33:45.520341 grai_source_looker-0.0.1a5/README.md
+-rw-r--r--   0        0        0     1123 2023-08-04 09:50:35.328714 grai_source_looker-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-08-04 09:50:40.043390 grai_source_looker-0.0.1a5/src/grai_source_looker/__init__.py
+-rw-r--r--   0        0        0    10902 2023-08-04 11:02:00.937900 grai_source_looker-0.0.1a5/src/grai_source_looker/adapters.py
+-rw-r--r--   0        0        0       48 2023-08-03 09:59:32.956516 grai_source_looker-0.0.1a5/src/grai_source_looker/api/__init__.py
+-rw-r--r--   0        0        0   642045 2023-08-03 09:33:45.526480 grai_source_looker-0.0.1a5/src/grai_source_looker/api/api_models.py
+-rw-r--r--   0        0        0     1410 2023-08-03 17:17:53.769053 grai_source_looker-0.0.1a5/src/grai_source_looker/base.py
+-rw-r--r--   0        0        0     5864 2023-08-04 11:01:52.833414 grai_source_looker-0.0.1a5/src/grai_source_looker/loader.py
+-rw-r--r--   0        0        0     6065 2023-08-04 10:59:28.899712 grai_source_looker-0.0.1a5/src/grai_source_looker/models.py
+-rw-r--r--   0        0        0      195 2023-08-03 09:33:45.526746 grai_source_looker-0.0.1a5/src/grai_source_looker/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-08-03 09:33:45.526767 grai_source_looker-0.0.1a5/src/grai_source_looker/py.typed
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 grai_source_looker-0.0.1a5/PKG-INFO
```

### Comparing `grai_source_looker-0.0.1a3/pyproject.toml` & `grai_source_looker-0.0.1a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_looker"
-version = "0.0.1a3"
+version = "0.0.1a5"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_looker", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_looker-0.0.1a3/src/grai_source_looker/adapters.py` & `grai_source_looker-0.0.1a5/src/grai_source_looker/adapters.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,25 @@
     ColumnMetadata,
     NodeMetadataTypeLabels,
     TableMetadata,
 )
 from grai_schemas.v1.source import SourceSpec
 from multimethod import multimethod
 
-from grai_source_looker.models import ID, Dashboard, Edge, FieldID, QueryField, TableID
+from grai_source_looker.models import (
+    ID,
+    Dashboard,
+    Dimension,
+    Edge,
+    Explore,
+    FieldID,
+    Query,
+    QueryField,
+    TableID,
+)
 from grai_source_looker.package_definitions import config
 
 T = TypeVar("T")
 X = TypeVar("X")
 Y = TypeVar("Y")
 
 
@@ -34,19 +44,23 @@
         desired (Any):
 
     Returns:
 
     Raises:
 
     """
-    raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
+    raise NotImplementedError(
+        f"No adapter between {type(current)} and {type(desired)} for value {current}"
+    )
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_dashboard(current: Dashboard, version: Literal["v1"] = "v1") -> TableMetadata:
+def build_grai_metadata_from_dashboard(
+    current: Dashboard, version: Literal["v1"] = "v1"
+) -> TableMetadata:
     """
 
     Args:
         current (Dashboard):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -61,19 +75,71 @@
         "tags": [config.metadata_id],
     }
 
     return TableMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_field(current: QueryField, version: Literal["v1"] = "v1") -> ColumnMetadata:
+def build_grai_metadata_from_query(
+    current: Query, version: Literal["v1"] = "v1"
+) -> ColumnMetadata:
+    """
+
+    Args:
+        current (Query):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
+    data = {
+        "version": version,
+        "node_type": NodeMetadataTypeLabels.column.value,
+        "node_attributes": {},
+        "tags": [config.metadata_id],
+    }
+
+    return ColumnMetadata(**data)
+
+
+@build_grai_metadata.register
+def build_grai_metadata_from_explore(
+    current: Explore, version: Literal["v1"] = "v1"
+) -> TableMetadata:
+    """
+
+    Args:
+        current (Explore):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
+    data = {
+        "version": version,
+        "node_type": NodeMetadataTypeLabels.table.value,
+        "node_attributes": {},
+        "tags": [config.metadata_id],
+    }
+
+    return TableMetadata(**data)
+
+
+@build_grai_metadata.register
+def build_grai_metadata_from_dimension(
+    current: Dimension, version: Literal["v1"] = "v1"
+) -> ColumnMetadata:
     """
 
     Args:
-        current (QueryField):
+        current (Dimension):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
@@ -84,15 +150,17 @@
         "tags": [config.metadata_id],
     }
 
     return ColumnMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> GenericEdgeMetadataV1:
+def build_grai_metadata_from_edge(
+    current: Edge, version: Literal["v1"] = "v1"
+) -> GenericEdgeMetadataV1:
     """
 
     Args:
         current (Edge):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -127,19 +195,23 @@
         desired (Any):
 
     Returns:
 
     Raises:
 
     """
-    raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
+    raise NotImplementedError(
+        f"No adapter between {type(current)} and {type(desired)} for value {current}"
+    )
 
 
 @build_app_metadata.register
-def build_metadata_from_dashboard(current: Dashboard, version: Literal["v1"] = "v1") -> Dict:
+def build_metadata_from_dashboard(
+    current: Dashboard, version: Literal["v1"] = "v1"
+) -> Dict:
     """
 
     Args:
         current (Dashboard):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -152,35 +224,81 @@
         "display_name": current.display_name,
     }
 
     return data
 
 
 @build_app_metadata.register
-def build_metadata_from_field(current: QueryField, version: Literal["v1"] = "v1") -> Dict:
+def build_metadata_from_query(current: Query, version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
         current (Dashboard):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     data = {
-        "name": current.name,
+        "name": current.title,
+        "display_name": current.title,
+    }
+
+    return data
+
+
+@build_app_metadata.register
+def build_metadata_from_explore(
+    current: Explore, version: Literal["v1"] = "v1"
+) -> Dict:
+    """
+
+    Args:
+        current (Explore):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
+    data = {
+        "name": current.table_name,
         "display_name": current.name,
     }
 
     return data
 
 
 @build_app_metadata.register
+def build_metadata_from_dimension(
+    current: Dimension, version: Literal["v1"] = "v1"
+) -> Dict:
+    """
+
+    Args:
+        current (Dimension):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
+    data = {
+        "name": current.column_name,
+        "display_name": current.label,
+    }
+
+    return data
+
+
+@build_app_metadata.register
 def build_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
         current (Edge):
         version (Literal["v1"], optional):  (Default value = "v1")
 
@@ -229,61 +347,113 @@
     Raises:
 
     """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
 
 
 @adapt_to_client.register
-def adapt_dashboard_to_client(current: Dashboard, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
+def adapt_dashboard_to_client(
+    current: Dashboard, source: SourceSpec, version: Literal["v1"]
+) -> SourcedNodeV1:
     """
 
     Args:
         current (Dashboard):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
         "name": current.name,
-        # "namespace": current.namespace,
-        "namespace": "looker",
+        "namespace": current.namespace,
         "display_name": current.display_name,
         "data_source": source,
         "metadata": build_metadata(current, version),
     }
     return SourcedNodeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_field_to_client(current: QueryField, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
+def adapt_query_to_client(
+    current: Query, source: SourceSpec, version: Literal["v1"]
+) -> SourcedNodeV1:
     """
 
     Args:
-        current (Dashboard):
+        current (Query):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
 
     Raises:
 
     """
     spec_dict = {
-        "name": current.name,
-        # "namespace": current.namespace,
-        "namespace": "looker",
+        "name": current.title,
+        "namespace": current.namespace,
+        "display_name": current.title,
+        "data_source": source,
+        "metadata": build_metadata(current, version),
+    }
+    return SourcedNodeV1.from_spec(spec_dict)
+
+
+@adapt_to_client.register
+def adapt_explore_to_client(
+    current: Explore, source: SourceSpec, version: Literal["v1"]
+) -> SourcedNodeV1:
+    """
+
+    Args:
+        current (Explore):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
+    spec_dict = {
+        "name": current.table_name,
+        "namespace": current.namespace,
         "display_name": current.name,
         "data_source": source,
         "metadata": build_metadata(current, version),
     }
     return SourcedNodeV1.from_spec(spec_dict)
 
 
+@adapt_to_client.register
+def adapt_dimension_to_client(
+    current: Dimension, source: SourceSpec, version: Literal["v1"]
+) -> SourcedNodeV1:
+    """
+
+    Args:
+        current (Dimension):
+        version (Literal["v1"], optional):  (Default value = "v1")
+
+    Returns:
+
+    Raises:
+
+    """
+    spec_dict = {
+        "name": current.column_name,
+        "namespace": current.namespace,
+        "display_name": current.label,
+        "data_source": source,
+        "metadata": build_metadata(current, version),
+    }
+    return SourcedNodeV1.from_spec(spec_dict)
+
+
 def make_name(node1: ID, node2: ID) -> str:
     """
 
     Args:
         node1 (ID):
         node2 (ID):
 
@@ -294,15 +464,17 @@
     """
     node1_name = f"{node1.namespace}:{node1.full_name}"
     node2_name = f"{node2.namespace}:{node2.full_name}"
     return f"{node1_name} -> {node2_name}"
 
 
 @adapt_to_client.register
-def adapt_edge_to_client(current: Edge, source: SourceSpec, version: Literal["v1"]) -> SourcedEdgeV1:
+def adapt_edge_to_client(
+    current: Edge, source: SourceSpec, version: Literal["v1"]
+) -> SourcedEdgeV1:
     """
 
     Args:
         current (Edge):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -311,19 +483,19 @@
 
     """
     spec_dict = {
         "data_source": source,
         "name": make_name(current.source, current.destination),
         "namespace": current.source.namespace,
         "source": {
-            "name": current.source.full_name,
+            "name": current.source.name,
             "namespace": current.source.namespace,
         },
         "destination": {
-            "name": current.destination.full_name,
+            "name": current.destination.name,
             "namespace": current.destination.namespace,
         },
         "metadata": build_metadata(current, version),
     }
 
     return SourcedEdgeV1.from_spec(spec_dict)
```

### Comparing `grai_source_looker-0.0.1a3/src/grai_source_looker/api/api_models.py` & `grai_source_looker-0.0.1a5/src/grai_source_looker/api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_looker-0.0.1a3/PKG-INFO` & `grai_source_looker-0.0.1a5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-looker
-Version: 0.0.1a3
+Version: 0.0.1a5
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
```

