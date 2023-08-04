# Comparing `tmp/dbt-graph-builder-0.6.1.tar.gz` & `tmp/dbt-graph-builder-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-graph-builder-0.6.1.tar", last modified: Thu Aug  3 12:11:03 2023, max compression
+gzip compressed data, was "dbt-graph-builder-0.6.2.tar", last modified: Thu Aug  3 13:05:14 2023, max compression
```

## Comparing `dbt-graph-builder-0.6.1.tar` & `dbt-graph-builder-0.6.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/src/dbt_graph_builder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/node_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-08-03 12:10:45.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:11:03.509156 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 12:11:03.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-03 12:11:03.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:11:03.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 12:11:03.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 12:11:03.000000 dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:05:14.271789 dbt-graph-builder-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 13:05:14.271789 dbt-graph-builder-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 13:05:14.271789 dbt-graph-builder-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:05:14.267789 dbt-graph-builder-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:05:14.271789 dbt-graph-builder-0.6.2/src/dbt_graph_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14841 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-08-03 13:04:58.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 13:05:14.271789 dbt-graph-builder-0.6.2/src/dbt_graph_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-08-03 13:05:14.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-03 13:05:14.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 13:05:14.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 13:05:14.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 13:05:14.000000 dbt-graph-builder-0.6.2/src/dbt_graph_builder.egg-info/top_level.txt
```

### Comparing `dbt-graph-builder-0.6.1/LICENSE` & `dbt-graph-builder-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.1/PKG-INFO` & `dbt-graph-builder-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.6.1
+Version: 0.6.2
 Summary: DBT Graph Builder
 Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Andrzej Swatowski <andrzej.swatowski@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dbt-graph-builder-0.6.1/README.md` & `dbt-graph-builder-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.1/pyproject.toml` & `dbt-graph-builder-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.1/src/dbt_graph_builder/builder.py` & `dbt-graph-builder-0.6.2/src/dbt_graph_builder/builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,22 +28,22 @@
         graph_config = GraphConfiguration()
     LOGGER.info("Creating tasks graph")
     dbt_airflow_graph = DbtManifestGraph(graph_config)
     dbt_airflow_graph.add_execution_tasks(manifest)
     if graph_config.enable_dags_dependencies:
         LOGGER.debug("Adding external dependencies")
         dbt_airflow_graph.add_external_dependencies(manifest)
-    dbt_airflow_graph.create_edges_from_dependencies(graph_config.enable_dags_dependencies)
+    dbt_airflow_graph.create_edges_from_dependencies()
     if not graph_config.show_ephemeral_models:
         LOGGER.debug("Removing ephemeral nodes from graph")
         dbt_airflow_graph.remove_ephemeral_nodes_from_graph()
     LOGGER.debug("Contracting test nodes")
     dbt_airflow_graph.contract_test_nodes()
     LOGGER.debug("Creating multple deps tests dependencies")
-    dbt_airflow_graph.create_multiple_deps_test_dependencies(graph_config.check_all_deps_for_multiple_deps_tests)
+    dbt_airflow_graph.create_multiple_deps_test_dependencies()
     return dbt_airflow_graph
 
 
 def load_dbt_manifest(manifest_path: os.PathLike[str] | str) -> dict[str, Any]:
     """Load dbt manifest.
 
     Args:
```

### Comparing `dbt-graph-builder-0.6.1/src/dbt_graph_builder/gateway.py` & `dbt-graph-builder-0.6.2/src/dbt_graph_builder/gateway.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.1/src/dbt_graph_builder/graph.py` & `dbt-graph-builder-0.6.2/src/dbt_graph_builder/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,23 +102,19 @@
         """
         manifest_child_map = manifest["child_map"]
         for source_name, manifest_source in manifest["sources"].items():
             if "dag" in manifest_source["source_meta"] and len(manifest_child_map[source_name]) > 0:
                 logging.info("Creating source sensor for: " + source_name)
                 self._add_sensor_source_node(source_name, manifest_source)
 
-    def create_edges_from_dependencies(self, include_sensors: bool = False) -> None:
-        """Create edges from dependencies.
-
-        Args:
-            include_sensors (bool, optional): If True, include sensors in the graph. Defaults to False.
-        """
+    def create_edges_from_dependencies(self) -> None:
+        """Create edges from dependencies."""
         for graph_node_name, graph_node in self.get_graph_nodes():
             for dependency in graph_node.get("depends_on", []):
-                if is_source_sensor_task(dependency) and not include_sensors:
+                if is_source_sensor_task(dependency) and not self._configuration.enable_dags_dependencies:
                     continue
                 if not self._graph.has_node(dependency):
                     continue
                 self._graph.add_edge(dependency, graph_node_name)
 
     def get_graph_nodes(self) -> NodeDataView:
         """Get graph nodes.
@@ -162,49 +158,43 @@
                 itertools.product(
                     list(self._graph.predecessors(node_name)),
                     list(self._graph.successors(node_name)),
                 )
             )
             self._graph.remove_node(node_name)
 
-    def create_multiple_deps_test_dependencies(self, check_all_predecessors: bool) -> None:
-        """Create edges from dependencies to multiple deps test.
-
-        Args:
-            check_all_predecessors (bool): If True, check all predecessors when creating dependencies.
-                Defaults to False.
-        """
+    def create_multiple_deps_test_dependencies(self) -> None:
+        """Create edges from dependencies to multiple deps test."""
         for test_node_name, node in self._graph.nodes(data=True):
             if node["node_type"] != NodeType.MULTIPLE_DEPS_TEST:
                 continue
             for node_name in self._graph.nodes():
                 if self._check_if_node_predecessors_are_superset_of_test_deps(
-                    node_name, test_node_name, check_all_predecessors=check_all_predecessors
+                    node_name,
+                    test_node_name,
                 ):
                     self._graph.add_edge(test_node_name, node_name)
 
     def _get_all_node_predecessors(self, node_name: str) -> set[str]:
         predecessors: set[str] = set()
         node_predecessors = set(self._graph.predecessors(node_name))
         predecessors |= node_predecessors
         for predecessor in node_predecessors:
             predecessors |= self._get_all_node_predecessors(predecessor)
         return predecessors
 
-    def _check_if_node_predecessors_are_superset_of_test_deps(
-        self, node_name: str, test_node_name: str, check_all_predecessors: bool
-    ) -> bool:
+    def _check_if_node_predecessors_are_superset_of_test_deps(self, node_name: str, test_node_name: str) -> bool:
         node = self._graph.nodes[node_name]
         test_node = self._graph.nodes[test_node_name]
         if node["node_type"] != NodeType.RUN_TEST:
             return False
         test_deps: set[str] = set(test_node["depends_on"])
         if node_name in test_deps:
             return False
-        if not check_all_predecessors:
+        if not self._configuration.check_all_deps_for_multiple_deps_tests:
             if not test_deps.issubset(set(node["depends_on"])):
                 return False
             if test_node_name in self._get_all_node_predecessors(node_name):
                 return False
             return True
         predecessors = self._get_all_node_predecessors(node_name)
         if not test_deps.issubset(predecessors):
```

### Comparing `dbt-graph-builder-0.6.1/src/dbt_graph_builder/utils.py` & `dbt-graph-builder-0.6.2/src/dbt_graph_builder/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.1/src/dbt_graph_builder/workflow.py` & `dbt-graph-builder-0.6.2/src/dbt_graph_builder/workflow.py`

 * *Files identical despite different names*

### Comparing `dbt-graph-builder-0.6.1/src/dbt_graph_builder.egg-info/PKG-INFO` & `dbt-graph-builder-0.6.2/src/dbt_graph_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-graph-builder
-Version: 0.6.1
+Version: 0.6.2
 Summary: DBT Graph Builder
 Author-email: Piotr Pękala <piotr.pekala@getindata.com>, Andrzej Swatowski <andrzej.swatowski@getindata.com>, Piotr Tutak <piotr.tutak@getindata.com>
 License:     MIT License
         
             Copyright (c) Microsoft Corporation.
         
             Permission is hereby granted, free of charge, to any person obtaining a copy
```

