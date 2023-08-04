# Comparing `tmp/grai_source_looker-0.0.1a5.tar.gz` & `tmp/grai_source_looker-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_looker-0.0.1a5.tar", max compression
+gzip compressed data, was "grai_source_looker-0.0.1a6.tar", max compression
```

## Comparing `grai_source_looker-0.0.1a5.tar` & `grai_source_looker-0.0.1a6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      133 2023-08-03 09:33:45.520341 grai_source_looker-0.0.1a5/README.md
--rw-r--r--   0        0        0     1123 2023-08-04 09:50:35.328714 grai_source_looker-0.0.1a5/pyproject.toml
--rw-r--r--   0        0        0       97 2023-08-04 09:50:40.043390 grai_source_looker-0.0.1a5/src/grai_source_looker/__init__.py
--rw-r--r--   0        0        0    10902 2023-08-04 11:02:00.937900 grai_source_looker-0.0.1a5/src/grai_source_looker/adapters.py
--rw-r--r--   0        0        0       48 2023-08-03 09:59:32.956516 grai_source_looker-0.0.1a5/src/grai_source_looker/api/__init__.py
--rw-r--r--   0        0        0   642045 2023-08-03 09:33:45.526480 grai_source_looker-0.0.1a5/src/grai_source_looker/api/api_models.py
--rw-r--r--   0        0        0     1410 2023-08-03 17:17:53.769053 grai_source_looker-0.0.1a5/src/grai_source_looker/base.py
--rw-r--r--   0        0        0     5864 2023-08-04 11:01:52.833414 grai_source_looker-0.0.1a5/src/grai_source_looker/loader.py
--rw-r--r--   0        0        0     6065 2023-08-04 10:59:28.899712 grai_source_looker-0.0.1a5/src/grai_source_looker/models.py
--rw-r--r--   0        0        0      195 2023-08-03 09:33:45.526746 grai_source_looker-0.0.1a5/src/grai_source_looker/package_definitions.py
--rw-r--r--   0        0        0        0 2023-08-03 09:33:45.526767 grai_source_looker-0.0.1a5/src/grai_source_looker/py.typed
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 grai_source_looker-0.0.1a5/PKG-INFO
+-rw-r--r--   0        0        0      133 2023-08-03 09:33:45.520341 grai_source_looker-0.0.1a6/README.md
+-rw-r--r--   0        0        0     1123 2023-08-04 11:39:33.130555 grai_source_looker-0.0.1a6/pyproject.toml
+-rw-r--r--   0        0        0       97 2023-08-04 11:39:37.077075 grai_source_looker-0.0.1a6/src/grai_source_looker/__init__.py
+-rw-r--r--   0        0        0    10796 2023-08-04 11:04:46.861928 grai_source_looker-0.0.1a6/src/grai_source_looker/adapters.py
+-rw-r--r--   0        0        0       48 2023-08-03 09:59:32.956516 grai_source_looker-0.0.1a6/src/grai_source_looker/api/__init__.py
+-rw-r--r--   0        0        0   642045 2023-08-03 09:33:45.526480 grai_source_looker-0.0.1a6/src/grai_source_looker/api/api_models.py
+-rw-r--r--   0        0        0     1410 2023-08-03 17:17:53.769053 grai_source_looker-0.0.1a6/src/grai_source_looker/base.py
+-rw-r--r--   0        0        0     5864 2023-08-04 11:39:24.031221 grai_source_looker-0.0.1a6/src/grai_source_looker/loader.py
+-rw-r--r--   0        0        0     5963 2023-08-04 11:04:46.823946 grai_source_looker-0.0.1a6/src/grai_source_looker/models.py
+-rw-r--r--   0        0        0      195 2023-08-03 09:33:45.526746 grai_source_looker-0.0.1a6/src/grai_source_looker/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-08-03 09:33:45.526767 grai_source_looker-0.0.1a6/src/grai_source_looker/py.typed
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 grai_source_looker-0.0.1a6/PKG-INFO
```

### Comparing `grai_source_looker-0.0.1a5/pyproject.toml` & `grai_source_looker-0.0.1a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_looker"
-version = "0.0.1a5"
+version = "0.0.1a6"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_looker", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_looker-0.0.1a5/src/grai_source_looker/adapters.py` & `grai_source_looker-0.0.1a6/src/grai_source_looker/adapters.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,23 +44,19 @@
         desired (Any):
 
     Returns:
 
     Raises:
 
     """
-    raise NotImplementedError(
-        f"No adapter between {type(current)} and {type(desired)} for value {current}"
-    )
+    raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_dashboard(
-    current: Dashboard, version: Literal["v1"] = "v1"
-) -> TableMetadata:
+def build_grai_metadata_from_dashboard(current: Dashboard, version: Literal["v1"] = "v1") -> TableMetadata:
     """
 
     Args:
         current (Dashboard):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -75,17 +71,15 @@
         "tags": [config.metadata_id],
     }
 
     return TableMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_query(
-    current: Query, version: Literal["v1"] = "v1"
-) -> ColumnMetadata:
+def build_grai_metadata_from_query(current: Query, version: Literal["v1"] = "v1") -> ColumnMetadata:
     """
 
     Args:
         current (Query):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -100,17 +94,15 @@
         "tags": [config.metadata_id],
     }
 
     return ColumnMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_explore(
-    current: Explore, version: Literal["v1"] = "v1"
-) -> TableMetadata:
+def build_grai_metadata_from_explore(current: Explore, version: Literal["v1"] = "v1") -> TableMetadata:
     """
 
     Args:
         current (Explore):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -125,17 +117,15 @@
         "tags": [config.metadata_id],
     }
 
     return TableMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_dimension(
-    current: Dimension, version: Literal["v1"] = "v1"
-) -> ColumnMetadata:
+def build_grai_metadata_from_dimension(current: Dimension, version: Literal["v1"] = "v1") -> ColumnMetadata:
     """
 
     Args:
         current (Dimension):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -150,17 +140,15 @@
         "tags": [config.metadata_id],
     }
 
     return ColumnMetadata(**data)
 
 
 @build_grai_metadata.register
-def build_grai_metadata_from_edge(
-    current: Edge, version: Literal["v1"] = "v1"
-) -> GenericEdgeMetadataV1:
+def build_grai_metadata_from_edge(current: Edge, version: Literal["v1"] = "v1") -> GenericEdgeMetadataV1:
     """
 
     Args:
         current (Edge):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -195,23 +183,19 @@
         desired (Any):
 
     Returns:
 
     Raises:
 
     """
-    raise NotImplementedError(
-        f"No adapter between {type(current)} and {type(desired)} for value {current}"
-    )
+    raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)} for value {current}")
 
 
 @build_app_metadata.register
-def build_metadata_from_dashboard(
-    current: Dashboard, version: Literal["v1"] = "v1"
-) -> Dict:
+def build_metadata_from_dashboard(current: Dashboard, version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
         current (Dashboard):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -245,17 +229,15 @@
         "display_name": current.title,
     }
 
     return data
 
 
 @build_app_metadata.register
-def build_metadata_from_explore(
-    current: Explore, version: Literal["v1"] = "v1"
-) -> Dict:
+def build_metadata_from_explore(current: Explore, version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
         current (Explore):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -268,17 +250,15 @@
         "display_name": current.name,
     }
 
     return data
 
 
 @build_app_metadata.register
-def build_metadata_from_dimension(
-    current: Dimension, version: Literal["v1"] = "v1"
-) -> Dict:
+def build_metadata_from_dimension(current: Dimension, version: Literal["v1"] = "v1") -> Dict:
     """
 
     Args:
         current (Dimension):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -347,17 +327,15 @@
     Raises:
 
     """
     raise NotImplementedError(f"No adapter between {type(current)} and {type(desired)}")
 
 
 @adapt_to_client.register
-def adapt_dashboard_to_client(
-    current: Dashboard, source: SourceSpec, version: Literal["v1"]
-) -> SourcedNodeV1:
+def adapt_dashboard_to_client(current: Dashboard, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
         current (Dashboard):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -372,17 +350,15 @@
         "data_source": source,
         "metadata": build_metadata(current, version),
     }
     return SourcedNodeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_query_to_client(
-    current: Query, source: SourceSpec, version: Literal["v1"]
-) -> SourcedNodeV1:
+def adapt_query_to_client(current: Query, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
         current (Query):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -397,17 +373,15 @@
         "data_source": source,
         "metadata": build_metadata(current, version),
     }
     return SourcedNodeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_explore_to_client(
-    current: Explore, source: SourceSpec, version: Literal["v1"]
-) -> SourcedNodeV1:
+def adapt_explore_to_client(current: Explore, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
         current (Explore):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -422,17 +396,15 @@
         "data_source": source,
         "metadata": build_metadata(current, version),
     }
     return SourcedNodeV1.from_spec(spec_dict)
 
 
 @adapt_to_client.register
-def adapt_dimension_to_client(
-    current: Dimension, source: SourceSpec, version: Literal["v1"]
-) -> SourcedNodeV1:
+def adapt_dimension_to_client(current: Dimension, source: SourceSpec, version: Literal["v1"]) -> SourcedNodeV1:
     """
 
     Args:
         current (Dimension):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
@@ -464,17 +436,15 @@
     """
     node1_name = f"{node1.namespace}:{node1.full_name}"
     node2_name = f"{node2.namespace}:{node2.full_name}"
     return f"{node1_name} -> {node2_name}"
 
 
 @adapt_to_client.register
-def adapt_edge_to_client(
-    current: Edge, source: SourceSpec, version: Literal["v1"]
-) -> SourcedEdgeV1:
+def adapt_edge_to_client(current: Edge, source: SourceSpec, version: Literal["v1"]) -> SourcedEdgeV1:
     """
 
     Args:
         current (Edge):
         version (Literal["v1"], optional):  (Default value = "v1")
 
     Returns:
```

### Comparing `grai_source_looker-0.0.1a5/src/grai_source_looker/api/api_models.py` & `grai_source_looker-0.0.1a6/src/grai_source_looker/api/api_models.py`

 * *Files identical despite different names*

### Comparing `grai_source_looker-0.0.1a5/src/grai_source_looker/base.py` & `grai_source_looker-0.0.1a6/src/grai_source_looker/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_looker-0.0.1a5/src/grai_source_looker/loader.py` & `grai_source_looker-0.0.1a6/src/grai_source_looker/loader.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -188,21 +188,21 @@
                     )
 
                     edges.append(edge)
 
                     edge = Edge(
                         constraint_type=Constraint("f"),
                         source=FieldID(
-                            table_name=dashboard.name,
-                            name=query.title if query.title else query.id,
+                            table_name=explore.table_name,
+                            name=dimension.column_name,
                             namespace=self.config.namespace,
                         ),
                         destination=FieldID(
-                            table_name=explore.table_name,
-                            name=dimension.column_name,
+                            table_name=dashboard.name,
+                            name=query.title if query.title else query.id,
                             namespace=self.config.namespace,
                         ),
                     )
 
                     edges.append(edge)
 
         dashboards.extend(queries)
```

### Comparing `grai_source_looker-0.0.1a5/src/grai_source_looker/models.py` & `grai_source_looker-0.0.1a6/src/grai_source_looker/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import re, json
+import json
+import re
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, root_validator, validator
 
 
 class LookerNode(BaseModel):
@@ -224,20 +225,15 @@
 
         fields = []
 
         for element in self.dashboard_elements if self.dashboard_elements else []:
             query = self.get_query(element)
 
             if query:
-                fields.extend(
-                    [
-                        QueryField(namespace=self.namespace, name=field)
-                        for field in query.fields
-                    ]
-                )
+                fields.extend([QueryField(namespace=self.namespace, name=field) for field in query.fields])
 
         return fields
 
     def get_edges(self):
         """ """
 
         edges = []
```

### Comparing `grai_source_looker-0.0.1a5/PKG-INFO` & `grai_source_looker-0.0.1a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-looker
-Version: 0.0.1a5
+Version: 0.0.1a6
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.9.13,<4.0.0
 Classifier: License :: Other/Proprietary License
```

