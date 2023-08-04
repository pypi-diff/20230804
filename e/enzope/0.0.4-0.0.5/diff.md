# Comparing `tmp/enzope-0.0.4.tar.gz` & `tmp/enzope-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enzope-0.0.4.tar", last modified: Thu Jul 20 15:14:54 2023, max compression
+gzip compressed data, was "enzope-0.0.5.tar", last modified: Fri Aug  4 14:30:15 2023, max compression
```

## Comparing `enzope-0.0.4.tar` & `enzope-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      593 2023-07-20 15:14:54.429321 enzope-0.0.4/PKG-INFO
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        4 2023-05-11 13:40:28.000000 enzope-0.0.4/README.md
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       78 2023-07-20 15:14:54.429321 enzope-0.0.4/setup.cfg
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1528 2023-07-20 15:14:35.000000 enzope-0.0.4/setup.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.425321 enzope-0.0.4/src/
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.425321 enzope-0.0.4/src/enzope/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      244 2023-07-17 16:53:44.000000 enzope-0.0.4/src/enzope/__init__.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/src/enzope/graphs/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-06-21 16:54:29.000000 enzope-0.0.4/src/enzope/graphs/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6768 2023-07-18 16:41:47.000000 enzope-0.0.4/src/enzope/graphs/custom_gtg.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     5185 2023-07-18 16:41:47.000000 enzope-0.0.4/src/enzope/graphs/graph_class.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/src/enzope/kernels/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-11 14:05:10.000000 enzope-0.0.4/src/enzope/kernels/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     2558 2023-07-18 16:41:47.000000 enzope-0.0.4/src/enzope/kernels/k_ys.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      430 2023-07-18 16:41:47.000000 enzope-0.0.4/src/enzope/kernels/locks.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/src/enzope/metrics/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-07-13 14:40:05.000000 enzope-0.0.4/src/enzope/metrics/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      465 2023-07-18 16:41:47.000000 enzope-0.0.4/src/enzope/metrics/gpu_measures.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      795 2023-07-20 15:13:09.000000 enzope-0.0.4/src/enzope/metrics/measures.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/src/enzope/models/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-07-13 14:40:02.000000 enzope-0.0.4/src/enzope/models/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)    10199 2023-07-20 15:13:10.000000 enzope-0.0.4/src/enzope/models/model.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.429321 enzope-0.0.4/src/enzope/trades/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:17.000000 enzope-0.0.4/src/enzope/trades/__init__.py
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       63 2023-06-01 14:02:21.000000 enzope-0.0.4/src/enzope/trades/ys.py
-drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-07-20 15:14:54.425321 enzope-0.0.4/src/enzope.egg-info/
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      593 2023-07-20 15:14:54.000000 enzope-0.0.4/src/enzope.egg-info/PKG-INFO
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      609 2023-07-20 15:14:54.000000 enzope-0.0.4/src/enzope.egg-info/SOURCES.txt
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        1 2023-07-20 15:14:54.000000 enzope-0.0.4/src/enzope.egg-info/dependency_links.txt
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       40 2023-07-20 15:14:54.000000 enzope-0.0.4/src/enzope.egg-info/requires.txt
--rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        7 2023-07-20 15:14:54.000000 enzope-0.0.4/src/enzope.egg-info/top_level.txt
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-08-04 14:30:15.628903 enzope-0.0.5/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      593 2023-08-04 14:30:15.628903 enzope-0.0.5/PKG-INFO
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        4 2023-05-11 13:40:28.000000 enzope-0.0.5/README.md
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       78 2023-08-04 14:30:15.632903 enzope-0.0.5/setup.cfg
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     1528 2023-08-04 14:29:55.000000 enzope-0.0.5/setup.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-08-04 14:30:15.628903 enzope-0.0.5/src/
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-08-04 14:30:15.628903 enzope-0.0.5/src/enzope/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      244 2023-07-31 12:50:17.000000 enzope-0.0.5/src/enzope/__init__.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-08-04 14:30:15.628903 enzope-0.0.5/src/enzope/graphs/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-06-21 16:54:29.000000 enzope-0.0.5/src/enzope/graphs/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     6768 2023-07-18 16:41:47.000000 enzope-0.0.5/src/enzope/graphs/custom_gtg.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     5264 2023-07-26 19:37:34.000000 enzope-0.0.5/src/enzope/graphs/graph_class.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-08-04 14:30:15.628903 enzope-0.0.5/src/enzope/kernels/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-11 14:05:10.000000 enzope-0.0.5/src/enzope/kernels/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)     2999 2023-07-31 12:46:30.000000 enzope-0.0.5/src/enzope/kernels/k_ys.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      430 2023-07-18 16:41:47.000000 enzope-0.0.5/src/enzope/kernels/locks.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-08-04 14:30:15.628903 enzope-0.0.5/src/enzope/metrics/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-07-13 14:40:05.000000 enzope-0.0.5/src/enzope/metrics/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      465 2023-07-18 16:41:47.000000 enzope-0.0.5/src/enzope/metrics/gpu_measures.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      795 2023-07-20 15:13:09.000000 enzope-0.0.5/src/enzope/metrics/measures.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-08-04 14:30:15.628903 enzope-0.0.5/src/enzope/models/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-07-13 14:40:02.000000 enzope-0.0.5/src/enzope/models/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)    10199 2023-07-20 15:13:10.000000 enzope-0.0.5/src/enzope/models/model.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-08-04 14:30:15.628903 enzope-0.0.5/src/enzope/trades/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        0 2023-05-15 13:37:17.000000 enzope-0.0.5/src/enzope/trades/__init__.py
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       63 2023-06-01 14:02:21.000000 enzope-0.0.5/src/enzope/trades/ys.py
+drwxrwxr-x   0 lautaro   (1000) lautaro   (1000)        0 2023-08-04 14:30:15.628903 enzope-0.0.5/src/enzope.egg-info/
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      593 2023-08-04 14:30:15.000000 enzope-0.0.5/src/enzope.egg-info/PKG-INFO
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)      609 2023-08-04 14:30:15.000000 enzope-0.0.5/src/enzope.egg-info/SOURCES.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        1 2023-08-04 14:30:15.000000 enzope-0.0.5/src/enzope.egg-info/dependency_links.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)       40 2023-08-04 14:30:15.000000 enzope-0.0.5/src/enzope.egg-info/requires.txt
+-rw-rw-r--   0 lautaro   (1000) lautaro   (1000)        7 2023-08-04 14:30:15.000000 enzope-0.0.5/src/enzope.egg-info/top_level.txt
```

### Comparing `enzope-0.0.4/PKG-INFO` & `enzope-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enzope
-Version: 0.0.4
+Version: 0.0.5
 Summary: Agent based modelling in complex networks
 Author: Lautaro Giordano
 Author-email: giordanolautaro@gmail.com
 Project-URL: Source, https://github.com/lautarogiordano/enzope/
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `enzope-0.0.4/setup.py` & `enzope-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
    name="enzope",  # Required
 
-   version="0.0.4",  # Required
+   version="0.0.5",  # Required
    
    description="Agent based modelling in complex networks",  # Optional
    
    long_description=long_description,  # Optional
    long_description_content_type="text/markdown",  # Optional (see note above)
    
    author="Lautaro Giordano",  # Optional
```

### Comparing `enzope-0.0.4/src/enzope/graphs/custom_gtg.py` & `enzope-0.0.5/src/enzope/graphs/custom_gtg.py`

 * *Files identical despite different names*

### Comparing `enzope-0.0.4/src/enzope/graphs/graph_class.py` & `enzope-0.0.5/src/enzope/graphs/graph_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,53 +45,64 @@
         pass
 
     def update_graph(self, *args, **kwargs):
         pass
 
     def get_opponents_cpu(self, *args, **kwargs):
         pass
-    
+
     def get_mean_connectivity(self):
         pass
-    
+
     def get_average_distance(self):
         pass
 
+
 class GTG(BaseGraph):
     def __init__(
-        self, n_nodes, theta, join="add", w0=None, posi=None, seed=None, **kwargs
+        self,
+        n_nodes,
+        theta,
+        join="add",
+        w0=None,
+        posi=None,
+        seed=None,
+        p_dist=None,
+        **kwargs,
     ):
         super().__init__(n_nodes, **kwargs)
         self.theta = theta
         self.posi = posi
         self.join = join
         self.seed = seed
 
         self.G = geographical_threshold_graph_custom(
             n_nodes,
             theta,
             dim=2,
             pos=posi,
             weight=w0,
             metric=None,
-            p_dist=None,
+            p_dist=p_dist,
             seed=seed,
             join=join,
         )
 
         if self.posi is None:
             self.posi = [self.G.nodes[i]["pos"] for i in range(n_nodes)]
 
         self.w = dict(enumerate(self.G.nodes[i]["weight"] for i in range(self.n_nodes)))
 
     def __call__(self, *args, **kwds):
         return self.G
 
     # Modificar la funcion para que o bien guarde en temp o bien muestre en pantalla
-    def plot_snapshot(self, w_min=1e-17, new_w=None, mcs=None, mode="show", *args, **kwargs):
+    def plot_snapshot(
+        self, w_min=1e-17, new_w=None, mcs=None, mode="show", *args, **kwargs
+    ):
         # Esto se tiene que escribir mejor
         if new_w is not None:
             self.update_weights(new_w)
 
         a = np.array(list(self.w.values()))
 
         dead_nodes = [node for node, weight in self.w.items() if weight < w_min]
@@ -155,19 +166,19 @@
         neighs = [(list(self.G.neighbors(i))) for i in range(self.n_nodes)]
         n_neighs = [0] + [len(x) for x in neighs]
         n_neighs = np.array(n_neighs, dtype=np.int32)
         # c_neighs has N+1 components, first is 0.
         c_neighs = np.cumsum(n_neighs)
         neighs = np.hstack(neighs).astype(np.int32)
         return c_neighs, neighs
-    
+
     # Some networkx functions for comfort
     def get_mean_connectivity(self):
         return np.mean(list(dict(nx.degree(self.G)).values()))
-    
+
     def get_average_distance(self):
         Gcc = sorted(nx.connected_components(self.G), key=len, reverse=True)
         G0 = self.G.subgraph(Gcc[0])
         return nx.average_shortest_path_length(G0)
 
 
 # Acá iría la clase del multigraph
```

### Comparing `enzope-0.0.4/src/enzope/metrics/measures.py` & `enzope-0.0.5/src/enzope/metrics/measures.py`

 * *Files identical despite different names*

### Comparing `enzope-0.0.4/src/enzope/models/model.py` & `enzope-0.0.5/src/enzope/models/model.py`

 * *Files identical despite different names*

### Comparing `enzope-0.0.4/src/enzope.egg-info/PKG-INFO` & `enzope-0.0.5/src/enzope.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enzope
-Version: 0.0.4
+Version: 0.0.5
 Summary: Agent based modelling in complex networks
 Author: Lautaro Giordano
 Author-email: giordanolautaro@gmail.com
 Project-URL: Source, https://github.com/lautarogiordano/enzope/
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `enzope-0.0.4/src/enzope.egg-info/SOURCES.txt` & `enzope-0.0.5/src/enzope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

