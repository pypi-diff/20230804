# Comparing `tmp/pyed-1.0.0.tar.gz` & `tmp/pyed-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyed-1.0.0.tar", last modified: Tue Jul 18 12:27:41 2023, max compression
+gzip compressed data, was "pyed-1.1.0.tar", last modified: Fri Aug  4 13:44:04 2023, max compression
```

## Comparing `pyed-1.0.0.tar` & `pyed-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-07-18 12:27:41.597359 pyed-1.0.0/
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1069 2023-07-17 06:32:44.000000 pyed-1.0.0/LICENSE.txt
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)       19 2023-07-17 06:32:44.000000 pyed-1.0.0/MANIFEST.in
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      289 2023-07-18 12:27:41.597359 pyed-1.0.0/PKG-INFO
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)    15876 2023-07-18 12:15:23.000000 pyed-1.0.0/README.adoc
-drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-07-18 12:27:41.597359 pyed-1.0.0/pyed/
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      136 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/__init__.py
-drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-07-18 12:27:41.597359 pyed-1.0.0/pyed/core/
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)        0 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/core/__init__.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1270 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/core/constants.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4295 2023-07-17 13:40:35.000000 pyed-1.0.0/pyed/core/node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      452 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/core/utils.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      837 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/core/xml_item.py
-drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-07-18 12:27:41.597359 pyed-1.0.0/pyed/elements/
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      234 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/elements/__init__.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4653 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/elements/edge.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     2564 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/elements/generic_node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     5175 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/elements/graph.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     7196 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/elements/group.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4285 2023-07-17 12:11:14.000000 pyed-1.0.0/pyed/elements/label.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1368 2023-07-17 13:40:49.000000 pyed-1.0.0/pyed/elements/shape_node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     3886 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/elements/table_node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1339 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/elements/uml_node.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)     7257 2023-07-17 06:32:44.000000 pyed-1.0.0/pyed/utils.py
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)       22 2023-07-18 12:08:16.000000 pyed-1.0.0/pyed/version.py
-drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-07-18 12:27:41.597359 pyed-1.0.0/pyed.egg-info/
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      289 2023-07-18 12:27:41.000000 pyed-1.0.0/pyed.egg-info/PKG-INFO
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      588 2023-07-18 12:27:41.000000 pyed-1.0.0/pyed.egg-info/SOURCES.txt
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)        1 2023-07-18 12:27:41.000000 pyed-1.0.0/pyed.egg-info/dependency_links.txt
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)       18 2023-07-18 12:27:41.000000 pyed-1.0.0/pyed.egg-info/requires.txt
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)        5 2023-07-18 12:27:41.000000 pyed-1.0.0/pyed.egg-info/top_level.txt
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      105 2023-07-17 06:32:44.000000 pyed-1.0.0/pyproject.toml
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      430 2023-07-18 12:27:41.601359 pyed-1.0.0/setup.cfg
--rw-r-----   0 ccossou  (14983) idediplilas  (1348)      174 2023-07-17 06:32:44.000000 pyed-1.0.0/setup.py
+drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-04 13:44:04.265254 pyed-1.1.0/
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1069 2023-07-17 06:32:44.000000 pyed-1.1.0/LICENSE.txt
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)       19 2023-07-17 06:32:44.000000 pyed-1.1.0/MANIFEST.in
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1939 2023-08-04 13:44:04.265254 pyed-1.1.0/PKG-INFO
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)    16844 2023-08-04 13:40:53.000000 pyed-1.1.0/README.adoc
+drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-04 13:44:04.261254 pyed-1.1.0/pyed/
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      136 2023-07-24 07:40:55.000000 pyed-1.1.0/pyed/__init__.py
+drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-04 13:44:04.265254 pyed-1.1.0/pyed/core/
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)        0 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/core/__init__.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1270 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/core/constants.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4365 2023-07-24 07:54:54.000000 pyed-1.1.0/pyed/core/node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      452 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/core/utils.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      837 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/core/xml_item.py
+drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-04 13:44:04.265254 pyed-1.1.0/pyed/elements/
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      264 2023-08-04 08:30:26.000000 pyed-1.1.0/pyed/elements/__init__.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4653 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/elements/edge.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     2564 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/elements/generic_node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     6354 2023-08-04 09:52:41.000000 pyed-1.1.0/pyed/elements/graph.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     7196 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/elements/group.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     4285 2023-07-17 12:11:14.000000 pyed-1.1.0/pyed/elements/label.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      851 2023-08-04 12:42:07.000000 pyed-1.1.0/pyed/elements/resource.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1368 2023-07-17 13:40:49.000000 pyed-1.1.0/pyed/elements/shape_node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1320 2023-08-04 08:30:26.000000 pyed-1.1.0/pyed/elements/svg_node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     3886 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/elements/table_node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1339 2023-07-17 06:32:44.000000 pyed-1.1.0/pyed/elements/uml_node.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     7257 2023-07-24 07:41:12.000000 pyed-1.1.0/pyed/utils.py
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)       22 2023-08-04 13:43:51.000000 pyed-1.1.0/pyed/version.py
+drwxr-x---   0 ccossou  (14983) idediplilas  (1348)        0 2023-08-04 13:44:04.261254 pyed-1.1.0/pyed.egg-info/
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1939 2023-08-04 13:44:04.000000 pyed-1.1.0/pyed.egg-info/PKG-INFO
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      648 2023-08-04 13:44:04.000000 pyed-1.1.0/pyed.egg-info/SOURCES.txt
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)        1 2023-08-04 13:44:04.000000 pyed-1.1.0/pyed.egg-info/dependency_links.txt
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)       18 2023-08-04 13:44:04.000000 pyed-1.1.0/pyed.egg-info/requires.txt
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)        5 2023-08-04 13:44:04.000000 pyed-1.1.0/pyed.egg-info/top_level.txt
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)     1610 2023-08-04 13:40:53.000000 pyed-1.1.0/pypi.md
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      105 2023-07-17 06:32:44.000000 pyed-1.1.0/pyproject.toml
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      508 2023-08-04 13:44:04.265254 pyed-1.1.0/setup.cfg
+-rw-r-----   0 ccossou  (14983) idediplilas  (1348)      174 2023-07-17 06:32:44.000000 pyed-1.1.0/setup.py
```

### Comparing `pyed-1.0.0/LICENSE.txt` & `pyed-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/README.adoc` & `pyed-1.1.0/README.adoc`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,27 @@
 * https://networkx.org/documentation/stable/reference/readwrite/graphml.html[NetworkX]
 
 My package focus on drawing simple graph to quickly visualise relations between informations. It's a crude subset of what graphs are capable of. My intent is to have a kind of https://inkscape.org/release[Inkscape], but for graph. https://www.yworks.com/products/yed[Yed] is that, but I don't want to add and draw manually dozen of nodes when trying to understand a datastructure or a code.
 
 These pages are thought to provide quick documentation on what you can do with this package, especially the different types of nodes and the parameter and values available.
 
 === Why another package?
-I wanted functionalities that do not exist in those packages. I wanted a way to create package with enhanced data visualisation, in particular node with list of information (GenericNode in Pyed ; see <<generic_node>>) and node with table of data (TableNode in Pyed ; see <<table_node>>)
+I wanted functionalities that do not exist in those packages. I wanted a way to create package with enhanced data visualisation, in particular node with list of information (GenericNode in Pyed ; see <<generic_node>>), node with table of data (TableNode in Pyed ; see <<table_node>>) and custom nodes with any .svg file as a shape (SvgNode in Pyed ; see <<svg_node>>).
 
 === Principle
 This package will not create finalized graph on its own. You'll have to use https://www.yworks.com/products/yed[Yed] or another GUI that support .graphml to render the graph correctly. By default, node size is not adapted to its content, and all nodes are on top of eachother.
 
 
 
 === How to install
 Without downloading the project, one can do:
 [source]
 ----
-pip install git+URL
+pip install pyed
 ----
-(URL being the github repository front page)
 
 For developer that have the git repository, one can do:
 [source,bash]
 ----
 pip install .
 pip install -e .
 ----
@@ -217,14 +216,37 @@
 [frame="all",options="header"]
 |===
 | Parameter Name | Possible values | Description
 | description | str | Description text
 | desc_style | dict | dict of all values passed to the description label (see <<label_parameters>>)
 |===
 
+[[svg_node]]
+==== SvgNode
+.Example of SvgNode. Script used to make the plot is examples/plot_indiv_element.py.
+image::svg_node.svg[align="center"]
+
+[source]
+----
+import pyed
+
+g = pyed.Graph()
+
+n = g.add_node(pyed.SvgNode, "SvgNode", svg_filename="yed_regular_hexagon.svg")
+----
+
+.GenericNode parameters (see <<node_parameters>> for common parameters also applicable):
+[frame="all",options="header"]
+|===
+| Parameter Name | Possible values | Description
+| svg_filename | str | Absolute or relative path to an SVG file that will be used as node representation.
+|===
+
+In Yed, you have an option menu:SVG[Apply SVG size], to make sure the ratio if kept, but this is a one time only option. If you resize, that option is deactivated because you can only keep the original SVG size, and not the original ratio. You can, however, resize while pressing btn:[Shift]. Another option is to set *width* and *height* when defining the *SvgNode*.
+
 === Edge
 .Example of Edge. Script used to make the plot is examples/plot_indiv_element.py.
 image::edge.svg[align="center"]
 
 [source]
 ----
 import pyed
```

### Comparing `pyed-1.0.0/pyed/core/constants.py` & `pyed-1.1.0/pyed/core/constants.py`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/pyed/core/node.py` & `pyed-1.1.0/pyed/core/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 LOG = logging.getLogger(__name__)
 
 
 class Node(XmlItem, metaclass=ABCMeta):
     node_type = None
 
     default_title_style = dict(alignment="center", font_family="Dialog",
-                               underlined_text="false", font_style="plain", font_size="12", )
+                               underlined_text="false", font_style="plain", font_size="12",
+                               modelName="internal", modelPosition="c")
 
     def __init__(self, name, title_style={}, background="#ffffff", transparent="false", border_color="#000000",
                  border_type="line", border_width="1.0", height=False, width=False, x=False, y=False, description="",
                  url="", **kwargs):
         """
 
         :param str name: Node name (title)
```

### Comparing `pyed-1.0.0/pyed/core/xml_item.py` & `pyed-1.1.0/pyed/core/xml_item.py`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/pyed/elements/edge.py` & `pyed-1.1.0/pyed/elements/edge.py`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/pyed/elements/generic_node.py` & `pyed-1.1.0/pyed/elements/generic_node.py`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/pyed/elements/graph.py` & `pyed-1.1.0/pyed/elements/graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import logging
 
 import xml.etree.ElementTree as ET
 
 from ..core.xml_item import XmlItem
 from .edge import Edge
 from .group import Group
+from .resource import Resource
 
 LOG = logging.getLogger(__name__)
 
 
 class Graph(XmlItem):
     def __init__(self):
         """
         Top Graph object of which every other nodes must depend
         """
         super().__init__(parent=None)
 
         self.nodes = {}
         self.edges = {}
         self.groups = {}
+        # Used to store svg files for instance
+        self.resources = {}
+        self._ressources_hash = {}  # Corresponding hash for a given ressource (to avoid storing it twice)
 
         # Yed only support directed graph, so masking this value
         self.directed = "directed"
         self.existing_entities = {self.id: self}
 
         self.graphml = None
 
@@ -46,14 +50,19 @@
 
         # Definition: url for Node
         node_key = ET.SubElement(graphml, "key", id="url_node")
         node_key.set("for", "node")
         node_key.set("attr.name", "url")
         node_key.set("attr.type", "string")
 
+        # Definition: resource for graphml
+        node_key = ET.SubElement(graphml, "key", id="resource_node")
+        node_key.set("for", "graphml")
+        node_key.set("yfiles.type", "resources")
+
         # Definition: description for Node
         node_key = ET.SubElement(graphml, "key", id="description_node")
         node_key.set("for", "node")
         node_key.set("attr.name", "description")
         node_key.set("attr.type", "string")
 
         # Definition: url for Edge
@@ -68,37 +77,65 @@
         node_key.set("attr.name", "description")
         node_key.set("attr.type", "string")
 
         edge_key = ET.SubElement(graphml, "key", id="data_edge")
         edge_key.set("for", "edge")
         edge_key.set("yfiles.type", "edgegraphics")
 
+
+
         graph = ET.SubElement(graphml, "graph", edgedefault=self.directed,
                               id=self.id)
 
         for node in self.nodes.values():
             graph.append(node.to_xml())
 
         for grp in self.groups.values():
             graph.append(grp.to_xml())
 
         for edge in self.edges.values():
             graph.append(edge.to_xml())
 
+        data_key = ET.SubElement(graphml, "data", key="resource_node")
+        resources_key = ET.SubElement(data_key, 'y:Resources')
+
+        for resource in self.resources.values():
+            t = resource.to_xml()
+            resources_key.append(t)
+
         self.graphml = graphml
 
+
+    def add_resource(self, resource):
+        r_hash = hash(resource)
+
+        # Check if this ressource is already stored and return corresponding index if so
+        for (idx, res) in self.resources.items():
+            if r_hash == res.hash:
+                return idx
+
+        # New ressource
+        r_obj = Resource(resource, parent=self)
+
+        self.resources[r_obj.id] = r_obj
+        self.existing_entities[r_obj.id] = r_obj
+
+        return r_obj.id
+
     def write_graph(self, filename):
         """
         Write current graph object to file (Syntax is GraphML, compatible with Yed)
 
         :param str filename: absolute or relative path for output file (expect .graphml extension).
         """
         self._construct_graphml()
 
         tree = ET.ElementTree(self.graphml)
+
+        print(f"Write graph to {filename}")
         tree.write(filename)
 
     def get_graph(self):
         """
         Render current object as xml code
 
         :return: XML code
```

### Comparing `pyed-1.0.0/pyed/elements/group.py` & `pyed-1.1.0/pyed/elements/group.py`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/pyed/elements/label.py` & `pyed-1.1.0/pyed/elements/label.py`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/pyed/elements/shape_node.py` & `pyed-1.1.0/pyed/elements/shape_node.py`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/pyed/elements/table_node.py` & `pyed-1.1.0/pyed/elements/table_node.py`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/pyed/elements/uml_node.py` & `pyed-1.1.0/pyed/elements/uml_node.py`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/pyed/utils.py` & `pyed-1.1.0/pyed/utils.py`

 * *Files identical despite different names*

### Comparing `pyed-1.0.0/pyed.egg-info/SOURCES.txt` & `pyed-1.1.0/pyed.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.adoc
+pypi.md
 pyproject.toml
 setup.cfg
 setup.py
 pyed/__init__.py
 pyed/utils.py
 pyed/version.py
 pyed.egg-info/PKG-INFO
@@ -19,10 +20,12 @@
 pyed/core/xml_item.py
 pyed/elements/__init__.py
 pyed/elements/edge.py
 pyed/elements/generic_node.py
 pyed/elements/graph.py
 pyed/elements/group.py
 pyed/elements/label.py
+pyed/elements/resource.py
 pyed/elements/shape_node.py
+pyed/elements/svg_node.py
 pyed/elements/table_node.py
 pyed/elements/uml_node.py
```

