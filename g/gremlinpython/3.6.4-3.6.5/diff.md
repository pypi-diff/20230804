# Comparing `tmp/gremlinpython-3.6.4.tar.gz` & `tmp/gremlinpython-3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gremlinpython-3.6.4.tar", last modified: Wed May 17 18:06:00 2023, max compression
+gzip compressed data, was "gremlinpython-3.6.5.tar", last modified: Fri Aug  4 19:25:19 2023, max compression
```

## Comparing `gremlinpython-3.6.4.tar` & `gremlinpython-3.6.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:06:00.711825 gremlinpython-3.6.4/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      814 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      170 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/NOTICE
--rw-r--r--   0 root         (0) root         (0)     6045 2023-05-17 18:06:00.714739 gremlinpython-3.6.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5543 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:05:59.875253 gremlinpython-3.6.4/gremlin_python/
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-05-17 18:05:59.000000 gremlinpython-3.6.4/gremlin_python/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:06:00.133024 gremlinpython-3.6.4/gremlin_python/driver/
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:06:00.211764 gremlinpython-3.6.4/gremlin_python/driver/aiohttp/
--rw-r--r--   0 root         (0) root         (0)      787 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/aiohttp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6228 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/aiohttp/transport.py
--rw-r--r--   0 root         (0) root         (0)     7321 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/client.py
--rw-r--r--   0 root         (0) root         (0)     3395 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/connection.py
--rw-r--r--   0 root         (0) root         (0)     8670 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/driver_remote_connection.py
--rw-r--r--   0 root         (0) root         (0)     8746 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/protocol.py
--rw-r--r--   0 root         (0) root         (0)     3014 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/remote_connection.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/request.py
--rw-r--r--   0 root         (0) root         (0)     2669 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/resultset.py
--rw-r--r--   0 root         (0) root         (0)    10009 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/serializer.py
--rw-r--r--   0 root         (0) root         (0)     1246 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/transport.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/driver/useragent.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:06:00.361778 gremlinpython-3.6.4/gremlin_python/process/
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/process/anonymous_traversal.py
--rw-r--r--   0 root         (0) root         (0)    61065 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/process/graph_traversal.py
--rw-r--r--   0 root         (0) root         (0)     9474 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/process/strategies.py
--rw-r--r--   0 root         (0) root         (0)     6078 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/process/translator.py
--rw-r--r--   0 root         (0) root         (0)    22450 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/process/traversal.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/statics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:06:00.415754 gremlinpython-3.6.4/gremlin_python/structure/
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/structure/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/structure/graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:06:00.569864 gremlinpython-3.6.4/gremlin_python/structure/io/
--rw-r--r--   0 root         (0) root         (0)      852 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/structure/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37104 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/structure/io/graphbinaryV1.py
--rw-r--r--   0 root         (0) root         (0)    20598 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/structure/io/graphsonV2d0.py
--rw-r--r--   0 root         (0) root         (0)    23918 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/structure/io/graphsonV3d0.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/gremlin_python/structure/io/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 18:06:00.684983 gremlinpython-3.6.4/gremlinpython.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6045 2023-05-17 18:05:59.000000 gremlinpython-3.6.4/gremlinpython.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1324 2023-05-17 18:05:59.000000 gremlinpython-3.6.4/gremlinpython.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 18:05:59.000000 gremlinpython-3.6.4/gremlinpython.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      153 2023-05-17 18:05:59.000000 gremlinpython-3.6.4/gremlinpython.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-17 18:05:59.000000 gremlinpython-3.6.4/gremlinpython.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-17 18:06:00.721108 gremlinpython-3.6.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3069 2023-05-17 17:17:10.000000 gremlinpython-3.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:25:19.087550 gremlinpython-3.6.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      814 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      170 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-08-04 19:25:19.087836 gremlinpython-3.6.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5553 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:25:19.024499 gremlinpython-3.6.5/gremlin_python/
+-rw-r--r--   0 root         (0) root         (0)      850 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      804 2023-08-04 19:25:18.000000 gremlinpython-3.6.5/gremlin_python/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:25:19.053407 gremlinpython-3.6.5/gremlin_python/driver/
+-rw-r--r--   0 root         (0) root         (0)      850 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:25:19.055901 gremlinpython-3.6.5/gremlin_python/driver/aiohttp/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/aiohttp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6228 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/aiohttp/transport.py
+-rw-r--r--   0 root         (0) root         (0)     7399 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/client.py
+-rw-r--r--   0 root         (0) root         (0)     3395 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/connection.py
+-rw-r--r--   0 root         (0) root         (0)     8670 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/driver_remote_connection.py
+-rw-r--r--   0 root         (0) root         (0)     8746 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/remote_connection.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/request.py
+-rw-r--r--   0 root         (0) root         (0)     2669 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/resultset.py
+-rw-r--r--   0 root         (0) root         (0)    10009 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/serializer.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/driver/transport.py
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-08-04 19:25:17.000000 gremlinpython-3.6.5/gremlin_python/driver/useragent.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:25:19.064350 gremlinpython-3.6.5/gremlin_python/process/
+-rw-r--r--   0 root         (0) root         (0)      850 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/process/anonymous_traversal.py
+-rw-r--r--   0 root         (0) root         (0)    61092 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/process/graph_traversal.py
+-rw-r--r--   0 root         (0) root         (0)     9474 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/process/strategies.py
+-rw-r--r--   0 root         (0) root         (0)     6159 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/process/translator.py
+-rw-r--r--   0 root         (0) root         (0)    22451 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/process/traversal.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/statics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:25:19.066998 gremlinpython-3.6.5/gremlin_python/structure/
+-rw-r--r--   0 root         (0) root         (0)      852 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/structure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/structure/graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:25:19.075048 gremlinpython-3.6.5/gremlin_python/structure/io/
+-rw-r--r--   0 root         (0) root         (0)      852 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/structure/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37104 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/structure/io/graphbinaryV1.py
+-rw-r--r--   0 root         (0) root         (0)    20598 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/structure/io/graphsonV2d0.py
+-rw-r--r--   0 root         (0) root         (0)    23918 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/structure/io/graphsonV3d0.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/gremlin_python/structure/io/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 19:25:19.086613 gremlinpython-3.6.5/gremlinpython.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-08-04 19:25:18.000000 gremlinpython-3.6.5/gremlinpython.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-08-04 19:25:18.000000 gremlinpython-3.6.5/gremlinpython.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 19:25:18.000000 gremlinpython-3.6.5/gremlinpython.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      153 2023-08-04 19:25:18.000000 gremlinpython-3.6.5/gremlinpython.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-04 19:25:18.000000 gremlinpython-3.6.5/gremlinpython.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      256 2023-08-04 19:25:19.088876 gremlinpython-3.6.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-08-04 19:06:25.000000 gremlinpython-3.6.5/setup.py
```

### Comparing `gremlinpython-3.6.4/LICENSE` & `gremlinpython-3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/MANIFEST.in` & `gremlinpython-3.6.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/PKG-INFO` & `gremlinpython-3.6.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlinpython
-Version: 3.6.4
+Version: 3.6.5
 Summary: Gremlin-Python for Apache TinkerPop
 Home-page: http://tinkerpop.apache.org
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -55,24 +55,24 @@
 protocols by which Gremlin-Python can connect.
 
 A typical connection to a server running on "localhost" that supports the Gremlin Server protocol using websockets
 from the Python shell looks like this:
 
     >>> from gremlin_python.process.anonymous_traversal import traversal
     >>> from gremlin_python.driver.driver_remote_connection import DriverRemoteConnection
-    >>> g = traversal().withRemote(DriverRemoteConnection('ws://localhost:8182/gremlin','g'))
+    >>> g = traversal().with_remote(DriverRemoteConnection('ws://localhost:8182/gremlin','g'))
 
 Once "g" has been created using a connection, it is then possible to start writing Gremlin traversals to query the
 remote graph:
 
-    >>> g.V().both()[1:3].toList()
+    >>> g.V().both()[1:3].to_list()
     [v[2], v[4]]
-    >>> g.V().both()[1].toList()
+    >>> g.V().both()[1].to_list()
     [v[2]]
-    >>> g.V().both().name.toList()
+    >>> g.V().both().name.to_list()
     [lop, vadas, josh, marko, marko, josh, peter, ripple, lop, marko, josh, lop]
 
 -----------------
 Sample Traversals
 -----------------
 
 The Gremlin language allows users to write highly expressive graph traversals and has a broad list of functions that
@@ -97,32 +97,32 @@
     from gremlin_python.process.traversal import Cardinality
 
     id = T.id
     single = Cardinality.single
 
     def create_vertex(self, vid, vlabel):
         # default database cardinality is used when Cardinality argument is not specified
-        g.addV(vlabel).property(id, vid). \
+        g.add_v(vlabel).property(id, vid). \
           property(single, 'name', 'Apache'). \
           property('lastname', 'Tinkerpop'). \
           next()
 
 Find Vertices
 ^^^^^^^^^^^^^
 
 .. code:: python
 
     def list_all(self, limit=500):
-        g.V().limit(limit).elementMap().toList()
+        g.V().limit(limit).element_map().to_list()
 
     def find_vertex(self, vid):
-        g.V(vid).elementMap().next()
+        g.V(vid).element_map().next()
 
     def list_by_label_name(self, vlabel, name):
-        g.V().has(vlabel, 'name', name).elementMap().toList()
+        g.V().has(vlabel, 'name', name).element_map().to_list()
 
 Update Vertex
 ^^^^^^^^^^^^^
 
 .. code:: python
 
     from gremlin_python.process.traversal import Cardinality
```

### Comparing `gremlinpython-3.6.4/README.rst` & `gremlinpython-3.6.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,24 +38,24 @@
 protocols by which Gremlin-Python can connect.
 
 A typical connection to a server running on "localhost" that supports the Gremlin Server protocol using websockets
 from the Python shell looks like this:
 
     >>> from gremlin_python.process.anonymous_traversal import traversal
     >>> from gremlin_python.driver.driver_remote_connection import DriverRemoteConnection
-    >>> g = traversal().withRemote(DriverRemoteConnection('ws://localhost:8182/gremlin','g'))
+    >>> g = traversal().with_remote(DriverRemoteConnection('ws://localhost:8182/gremlin','g'))
 
 Once "g" has been created using a connection, it is then possible to start writing Gremlin traversals to query the
 remote graph:
 
-    >>> g.V().both()[1:3].toList()
+    >>> g.V().both()[1:3].to_list()
     [v[2], v[4]]
-    >>> g.V().both()[1].toList()
+    >>> g.V().both()[1].to_list()
     [v[2]]
-    >>> g.V().both().name.toList()
+    >>> g.V().both().name.to_list()
     [lop, vadas, josh, marko, marko, josh, peter, ripple, lop, marko, josh, lop]
 
 -----------------
 Sample Traversals
 -----------------
 
 The Gremlin language allows users to write highly expressive graph traversals and has a broad list of functions that
@@ -80,32 +80,32 @@
     from gremlin_python.process.traversal import Cardinality
 
     id = T.id
     single = Cardinality.single
 
     def create_vertex(self, vid, vlabel):
         # default database cardinality is used when Cardinality argument is not specified
-        g.addV(vlabel).property(id, vid). \
+        g.add_v(vlabel).property(id, vid). \
           property(single, 'name', 'Apache'). \
           property('lastname', 'Tinkerpop'). \
           next()
 
 Find Vertices
 ^^^^^^^^^^^^^
 
 .. code:: python
 
     def list_all(self, limit=500):
-        g.V().limit(limit).elementMap().toList()
+        g.V().limit(limit).element_map().to_list()
 
     def find_vertex(self, vid):
-        g.V(vid).elementMap().next()
+        g.V(vid).element_map().next()
 
     def list_by_label_name(self, vlabel, name):
-        g.V().has(vlabel, 'name', name).elementMap().toList()
+        g.V().has(vlabel, 'name', name).element_map().to_list()
 
 Update Vertex
 ^^^^^^^^^^^^^
 
 .. code:: python
 
     from gremlin_python.process.traversal import Cardinality
```

### Comparing `gremlinpython-3.6.4/gremlin_python/__init__.py` & `gremlinpython-3.6.5/gremlin_python/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/__version__.py` & `gremlinpython-3.6.5/gremlin_python/__version__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 Unless required by applicable law or agreed to in writing,
 software distributed under the License is distributed on an
 "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 KIND, either express or implied.  See the License for the
 specific language governing permissions and limitations
 under the License.
 '''
-version   = '3.6.4'
-timestamp = 1684346759
+version   = '3.6.5'
+timestamp = 1691177118
```

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/__init__.py` & `gremlinpython-3.6.5/gremlin_python/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/aiohttp/__init__.py` & `gremlinpython-3.6.5/gremlin_python/driver/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/aiohttp/transport.py` & `gremlinpython-3.6.5/gremlin_python/driver/aiohttp/transport.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/client.py` & `gremlinpython-3.6.5/gremlin_python/driver/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,17 @@
         warnings.warn(
             "gremlin_python.driver.client.Client.submitAsync will be replaced by "
             "gremlin_python.driver.client.Client.submit_async.",
             DeprecationWarning)
         return self.submit_async(message, bindings, request_options)
 
     def submit_async(self, message, bindings=None, request_options=None):
+        if self.is_closed():
+            raise Exception("Client is closed")
+
         log.debug("message '%s'", str(message))
         args = {'gremlin': message, 'aliases': {'g': self._traversal_source}}
         processor = ''
         op = 'eval'
         if isinstance(message, traversal.Bytecode):
             op = 'bytecode'
             processor = 'traversal'
```

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/connection.py` & `gremlinpython-3.6.5/gremlin_python/driver/connection.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/driver_remote_connection.py` & `gremlinpython-3.6.5/gremlin_python/driver/driver_remote_connection.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/protocol.py` & `gremlinpython-3.6.5/gremlin_python/driver/protocol.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/remote_connection.py` & `gremlinpython-3.6.5/gremlin_python/driver/remote_connection.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/request.py` & `gremlinpython-3.6.5/gremlin_python/driver/request.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/resultset.py` & `gremlinpython-3.6.5/gremlin_python/driver/resultset.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/serializer.py` & `gremlinpython-3.6.5/gremlin_python/driver/serializer.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/transport.py` & `gremlinpython-3.6.5/gremlin_python/driver/transport.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/driver/useragent.py` & `gremlinpython-3.6.5/gremlin_python/driver/useragent.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,28 +14,24 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import platform
 
+gremlin_version = "3.6.5"  # DO NOT MODIFY - Configured automatically by Maven Replacer Plugin
 
 def _generate_user_agent():
     application_name = "NotAvailable"
-    try:
-        from gremlin_python import __version__
-        driver_version = __version__.version.replace(" ", "_")
-    except ImportError:
-        driver_version = "NotAvailable"
     runtime_version = platform.python_version().replace(" ", "_")
     os_name = platform.system().replace(" ", "_")
     os_version = platform.release().replace(" ", "_")
     architecture = platform.machine().replace(" ", "_")
     user_agent = "{appName} Gremlin-Python.{driverVersion} {runtimeVersion} {osName}.{osVersion} {cpuArch}".format(
-                    appName=application_name, driverVersion=driver_version, runtimeVersion=runtime_version,
+                    appName=application_name, driverVersion=gremlin_version, runtimeVersion=runtime_version,
                     osName=os_name, osVersion=os_version, cpuArch=architecture)
 
     return user_agent
 
 
 userAgent = _generate_user_agent()
 userAgentHeader = "User-Agent"
```

### Comparing `gremlinpython-3.6.4/gremlin_python/process/__init__.py` & `gremlinpython-3.6.5/gremlin_python/process/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/process/anonymous_traversal.py` & `gremlinpython-3.6.5/gremlin_python/process/anonymous_traversal.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/process/graph_traversal.py` & `gremlinpython-3.6.5/gremlin_python/process/graph_traversal.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         source = self.get_graph_traversal_source()
         options_strategy = next((x for x in source.bytecode.source_instructions
                                  if x[0] == "withStrategies" and type(x[1]) is OptionsStrategy), None)
 
         val = True if v is None else v
         if options_strategy is None:
             options_strategy = OptionsStrategy({k: val})
-            source = self.withStrategies(options_strategy)
+            source = self.with_strategies(options_strategy)
         else:
             options_strategy[1].configuration[k] = val
 
         return source
 
     def withRemote(self, remote_connection):
         warnings.warn(
@@ -1583,23 +1583,23 @@
 
 
 def V(*args):
     return __.V(*args)
 
 
 def addE(*args):
-    return __.addE(*args)
+    return __.add_e(*args)
 
 
 def add_e(*args):
     return __.add_e(*args)
 
 
 def addV(*args):
-    return __.addV(*args)
+    return __.add_v(*args)
 
 
 def add_v(*args):
     return __.add_v(*args)
 
 
 def aggregate(*args):
@@ -1619,23 +1619,23 @@
 
 
 def both(*args):
     return __.both(*args)
 
 
 def bothE(*args):
-    return __.bothE(*args)
+    return __.both_e(*args)
 
 
 def both_e(*args):
     return __.both_e(*args)
 
 
 def bothV(*args):
-    return __.bothV(*args)
+    return __.both_v(*args)
 
 
 def both_v(*args):
     return __.both_v(*args)
 
 
 def branch(*args):
@@ -1667,15 +1667,15 @@
 
 
 def count(*args):
     return __.count(*args)
 
 
 def cyclicPath(*args):
-    return __.cyclicPath(*args)
+    return __.cyclic_path(*args)
 
 
 def cyclic_path(*args):
     return __.cyclic_path(*args)
 
 
 def dedup(*args):
@@ -1687,15 +1687,15 @@
 
 
 def element(*args):
     return __.element(*args)
 
 
 def elementMap(*args):
-    return __.elementMap(*args)
+    return __.element_map(*args)
 
 
 def element_map(*args):
     return __.element_map(*args)
 
 
 def emit(*args):
@@ -1707,15 +1707,15 @@
 
 
 def filter_(*args):
     return __.filter_(*args)
 
 
 def flatMap(*args):
-    return __.flatMap(*args)
+    return __.flat_map(*args)
 
 
 def flat_map(*args):
     return __.flat_map(*args)
 
 
 def fold(*args):
@@ -1723,59 +1723,59 @@
 
 
 def group(*args):
     return __.group(*args)
 
 
 def groupCount(*args):
-    return __.groupCount(*args)
+    return __.group_count(*args)
 
 
 def group_count(*args):
     return __.group_count(*args)
 
 
 def has(*args):
     return __.has(*args)
 
 
 def hasId(*args):
-    return __.hasId(*args)
+    return __.has_id(*args)
 
 
 def has_id(*args):
     return __.has_id(*args)
 
 
 def hasKey(*args):
-    return __.hasKey(*args)
+    return __.has_key_(*args)
 
 
 def has_key_(*args):
     return __.has_key_(*args)
 
 
 def hasLabel(*args):
-    return __.hasLabel(*args)
+    return __.has_label(*args)
 
 
 def has_label(*args):
     return __.has_label(*args)
 
 
 def hasNot(*args):
-    return __.hasNot(*args)
+    return __.has_not(*args)
 
 
 def has_not(*args):
     return __.has_not(*args)
 
 
 def hasValue(*args):
-    return __.hasValue(*args)
+    return __.has_value(*args)
 
 
 def has_value(*args):
     return __.has_value(*args)
 
 
 def id_(*args):
@@ -1783,23 +1783,23 @@
 
 
 def identity(*args):
     return __.identity(*args)
 
 
 def inE(*args):
-    return __.inE(*args)
+    return __.in_e(*args)
 
 
 def in_e(*args):
     return __.in_e(*args)
 
 
 def inV(*args):
-    return __.inV(*args)
+    return __.in_v(*args)
 
 
 def in_v(*args):
     return __.in_v(*args)
 
 
 def in_(*args):
@@ -1883,35 +1883,35 @@
 
 
 def order(*args):
     return __.order(*args)
 
 
 def otherV(*args):
-    return __.otherV(*args)
+    return __.other_v(*args)
 
 
 def other_v(*args):
     return __.other_v(*args)
 
 
 def out(*args):
     return __.out(*args)
 
 
 def outE(*args):
-    return __.outE(*args)
+    return __.out_e(*args)
 
 
 def out_e(*args):
     return __.out_e(*args)
 
 
 def outV(*args):
-    return __.outV(*args)
+    return __.out_v(*args)
 
 
 def out_v(*args):
     return __.out_v(*args)
 
 
 def path(*args):
@@ -1927,15 +1927,15 @@
 
 
 def property(*args):
     return __.property(*args)
 
 
 def propertyMap(*args):
-    return __.propertyMap(*args)
+    return __.property_map(*args)
 
 
 def property_map(*args):
     return __.property_map(*args)
 
 
 def range_(*args):
@@ -1955,23 +1955,23 @@
 
 
 def select(*args):
     return __.select(*args)
 
 
 def sideEffect(*args):
-    return __.sideEffect(*args)
+    return __.side_effect(*args)
 
 
 def side_effect(*args):
     return __.side_effect(*args)
 
 
 def simplePath(*args):
-    return __.simplePath(*args)
+    return __.simple_path(*args)
 
 
 def simple_path(*args):
     return __.simple_path(*args)
 
 
 def skip(*args):
@@ -1991,15 +1991,15 @@
 
 
 def tail(*args):
     return __.tail(*args)
 
 
 def timeLimit(*args):
-    return __.timeLimit(*args)
+    return __.time_limit(*args)
 
 
 def time_limit(*args):
     return __.time_limit(*args)
 
 
 def times(*args):
@@ -2007,23 +2007,23 @@
 
 
 def to(*args):
     return __.to(*args)
 
 
 def toE(*args):
-    return __.toE(*args)
+    return __.to_e(*args)
 
 
 def to_e(*args):
     return __.to_e(*args)
 
 
 def toV(*args):
-    return __.toV(*args)
+    return __.to_v(*args)
 
 
 def to_v(*args):
     return __.to_v(*args)
 
 
 def tree(*args):
@@ -2043,15 +2043,15 @@
 
 
 def value(*args):
     return __.value(*args)
 
 
 def valueMap(*args):
-    return __.valueMap(*args)
+    return __.value_map(*args)
 
 
 def value_map(*args):
     return __.value_map(*args)
 
 
 def values(*args):
```

### Comparing `gremlinpython-3.6.4/gremlin_python/process/strategies.py` & `gremlinpython-3.6.5/gremlin_python/process/strategies.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/process/translator.py` & `gremlinpython-3.6.5/gremlin_python/process/translator.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     def of(self,traversal_source):
         self.traversal_source = traversal_source
         return self
 
     # Do any needed special processing for the representation
     # of strings and dates.
     def fixup(self, v):
-        if type(v) == str:
+        if isinstance(v, str):
             return f'\'{v}\''
         elif type(v) == datetime:
             return self.process_date(v)
         else:
             return str(v)
     
     # Turn a Python datetime into the equivalent new Date(...)
@@ -129,31 +129,33 @@
             with_opts = False
             for p in params:
                 script += ',' if c > 0 else ''
                 if with_opts:
                   script += f'WithOptions.{self.options[p]}'
                 elif type(p) == Bytecode:
                     script += self.translate(p, True)
-                elif type(p) == P:
+                elif isinstance(p, P):
                     script += self.process_predicate(p)
                 elif type(p) in [Cardinality, Pop, Operator]:
                     tmp = str(p)
                     script += tmp[0:-1] if tmp.endswith('_') else tmp 
                 elif type(p) in [ReadOnlyStrategy, SubgraphStrategy, VertexProgramStrategy,
                                  OptionsStrategy, PartitionStrategy]:
                     script += self.process_strategy(p)
                 elif type(p) == datetime:
                     script += self.process_date(p)
                 elif p == WithOptions.tokens:
                     script += 'WithOptions.tokens'
                     with_opts = True
-                elif type(p) == str:
+                elif isinstance(p, str):
                     script += f'\'{p}\''
                 elif type(p) == bool:
                     script += 'true' if p else 'false'
+                elif p is None:
+                    script += 'null'
                 else:
                     script += str(p)
                 c += 1
         script += ')'
         return script
 
     # Translation starts here. There are two main parts to a
```

### Comparing `gremlinpython-3.6.4/gremlin_python/process/traversal.py` & `gremlinpython-3.6.5/gremlin_python/process/traversal.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     def to_set(self):
         return set(iter(self))
 
     def iterate(self):
         self.bytecode.add_step("none")
         while True:
-            try: self.nextTraverser()
+            try: self.next_traverser()
             except StopIteration: return self
 
     def nextTraverser(self):
         warnings.warn(
             "gremlin_python.process.Traversal.nextTraverser will be replaced by "
             "gremlin_python.process.Traversal.next_traverser.",
             DeprecationWarning)
```

### Comparing `gremlinpython-3.6.4/gremlin_python/statics.py` & `gremlinpython-3.6.5/gremlin_python/statics.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/structure/__init__.py` & `gremlinpython-3.6.5/gremlin_python/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/structure/graph.py` & `gremlinpython-3.6.5/gremlin_python/structure/graph.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/structure/io/__init__.py` & `gremlinpython-3.6.5/gremlin_python/structure/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/structure/io/graphbinaryV1.py` & `gremlinpython-3.6.5/gremlin_python/structure/io/graphbinaryV1.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/structure/io/graphsonV2d0.py` & `gremlinpython-3.6.5/gremlin_python/structure/io/graphsonV2d0.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/structure/io/graphsonV3d0.py` & `gremlinpython-3.6.5/gremlin_python/structure/io/graphsonV3d0.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlin_python/structure/io/util.py` & `gremlinpython-3.6.5/gremlin_python/structure/io/util.py`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/gremlinpython.egg-info/PKG-INFO` & `gremlinpython-3.6.5/gremlinpython.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gremlinpython
-Version: 3.6.4
+Version: 3.6.5
 Summary: Gremlin-Python for Apache TinkerPop
 Home-page: http://tinkerpop.apache.org
 License: Apache 2
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -55,24 +55,24 @@
 protocols by which Gremlin-Python can connect.
 
 A typical connection to a server running on "localhost" that supports the Gremlin Server protocol using websockets
 from the Python shell looks like this:
 
     >>> from gremlin_python.process.anonymous_traversal import traversal
     >>> from gremlin_python.driver.driver_remote_connection import DriverRemoteConnection
-    >>> g = traversal().withRemote(DriverRemoteConnection('ws://localhost:8182/gremlin','g'))
+    >>> g = traversal().with_remote(DriverRemoteConnection('ws://localhost:8182/gremlin','g'))
 
 Once "g" has been created using a connection, it is then possible to start writing Gremlin traversals to query the
 remote graph:
 
-    >>> g.V().both()[1:3].toList()
+    >>> g.V().both()[1:3].to_list()
     [v[2], v[4]]
-    >>> g.V().both()[1].toList()
+    >>> g.V().both()[1].to_list()
     [v[2]]
-    >>> g.V().both().name.toList()
+    >>> g.V().both().name.to_list()
     [lop, vadas, josh, marko, marko, josh, peter, ripple, lop, marko, josh, lop]
 
 -----------------
 Sample Traversals
 -----------------
 
 The Gremlin language allows users to write highly expressive graph traversals and has a broad list of functions that
@@ -97,32 +97,32 @@
     from gremlin_python.process.traversal import Cardinality
 
     id = T.id
     single = Cardinality.single
 
     def create_vertex(self, vid, vlabel):
         # default database cardinality is used when Cardinality argument is not specified
-        g.addV(vlabel).property(id, vid). \
+        g.add_v(vlabel).property(id, vid). \
           property(single, 'name', 'Apache'). \
           property('lastname', 'Tinkerpop'). \
           next()
 
 Find Vertices
 ^^^^^^^^^^^^^
 
 .. code:: python
 
     def list_all(self, limit=500):
-        g.V().limit(limit).elementMap().toList()
+        g.V().limit(limit).element_map().to_list()
 
     def find_vertex(self, vid):
-        g.V(vid).elementMap().next()
+        g.V(vid).element_map().next()
 
     def list_by_label_name(self, vlabel, name):
-        g.V().has(vlabel, 'name', name).elementMap().toList()
+        g.V().has(vlabel, 'name', name).element_map().to_list()
 
 Update Vertex
 ^^^^^^^^^^^^^
 
 .. code:: python
 
     from gremlin_python.process.traversal import Cardinality
```

### Comparing `gremlinpython-3.6.4/gremlinpython.egg-info/SOURCES.txt` & `gremlinpython-3.6.5/gremlinpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gremlinpython-3.6.4/setup.py` & `gremlinpython-3.6.5/setup.py`

 * *Files identical despite different names*

