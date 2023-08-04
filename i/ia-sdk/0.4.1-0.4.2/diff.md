# Comparing `tmp/ia-sdk-0.4.1.tar.gz` & `tmp/ia-sdk-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia-sdk-0.4.1.tar", last modified: Wed Aug  2 12:28:06 2023, max compression
+gzip compressed data, was "ia-sdk-0.4.2.tar", last modified: Fri Aug  4 12:36:21 2023, max compression
```

## Comparing `ia-sdk-0.4.1.tar` & `ia-sdk-0.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1256 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/PKG-INFO
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      751 2023-02-02 14:25:09.000000 ia-sdk-0.4.1/README.md
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       22 2023-08-02 12:25:48.000000 ia-sdk-0.4.1/ia/__init__.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/gaius/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       79 2022-05-26 13:05:31.000000 ia-sdk-0.4.1/ia/gaius/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    75273 2023-08-01 15:18:51.000000 ia-sdk-0.4.1/ia/gaius/agent_client.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    22819 2023-05-08 22:12:27.000000 ia-sdk-0.4.1/ia/gaius/back_testing.py
--rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    12451 2023-07-25 14:50:28.000000 ia-sdk-0.4.1/ia/gaius/comcom_client.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      858 2023-04-14 14:57:27.000000 ia-sdk-0.4.1/ia/gaius/data_language.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     9361 2023-08-01 19:37:22.000000 ia-sdk-0.4.1/ia/gaius/data_ops.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    17348 2023-07-19 12:51:12.000000 ia-sdk-0.4.1/ia/gaius/data_structures.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/gaius/experimental/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2023-07-14 15:07:29.000000 ia-sdk-0.4.1/ia/gaius/experimental/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    11085 2023-07-14 15:07:29.000000 ia-sdk-0.4.1/ia/gaius/experimental/genome_optimizer.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     3217 2023-06-08 15:56:58.000000 ia-sdk-0.4.1/ia/gaius/genome_info.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    27195 2023-08-01 15:18:51.000000 ia-sdk-0.4.1/ia/gaius/kb_ops.py
--rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    36330 2023-07-25 14:03:17.000000 ia-sdk-0.4.1/ia/gaius/manager.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     8771 2023-06-08 15:56:58.000000 ia-sdk-0.4.1/ia/gaius/prediction_models.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/gaius/pvt/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    76162 2023-08-01 20:44:52.000000 ia-sdk-0.4.1/ia/gaius/pvt/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    26516 2023-08-01 19:14:20.000000 ia-sdk-0.4.1/ia/gaius/pvt/mongo_interface.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    10707 2023-08-01 15:18:46.000000 ia-sdk-0.4.1/ia/gaius/pvt/offline_sio.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    17775 2023-08-01 21:14:21.000000 ia-sdk-0.4.1/ia/gaius/pvt/pvt_utils.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/gaius/tests/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2022-05-26 13:05:31.000000 ia-sdk-0.4.1/ia/gaius/tests/__init__.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2786 2023-06-08 15:56:58.000000 ia-sdk-0.4.1/ia/gaius/tests/classification.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2679 2023-06-08 15:56:58.000000 ia-sdk-0.4.1/ia/gaius/tests/utility.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    11002 2023-06-08 15:56:58.000000 ia-sdk-0.4.1/ia/gaius/utils.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia/scripts/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2023-03-24 19:12:06.000000 ia-sdk-0.4.1/ia/scripts/__init__.py
--rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    40560 2023-08-01 17:33:50.000000 ia-sdk-0.4.1/ia/scripts/spawn_agent.py
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2762 2023-07-25 13:21:37.000000 ia-sdk-0.4.1/ia/scripts/spawn_general.py
-drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/ia_sdk.egg-info/
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1256 2023-08-02 12:28:06.000000 ia-sdk-0.4.1/ia_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      825 2023-08-02 12:28:06.000000 ia-sdk-0.4.1/ia_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        1 2023-08-02 12:28:06.000000 ia-sdk-0.4.1/ia_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      139 2023-08-02 12:28:06.000000 ia-sdk-0.4.1/ia_sdk.egg-info/requires.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        3 2023-08-02 12:28:06.000000 ia-sdk-0.4.1/ia_sdk.egg-info/top_level.txt
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      110 2023-08-02 12:28:06.852782 ia-sdk-0.4.1/setup.cfg
--rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1176 2023-07-18 13:37:42.000000 ia-sdk-0.4.1/setup.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-04 12:36:21.217730 ia-sdk-0.4.2/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1256 2023-08-04 12:36:21.217730 ia-sdk-0.4.2/PKG-INFO
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      751 2023-02-02 14:25:09.000000 ia-sdk-0.4.2/README.md
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-04 12:36:21.217730 ia-sdk-0.4.2/ia/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       22 2023-08-02 15:47:14.000000 ia-sdk-0.4.2/ia/__init__.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-04 12:36:21.217730 ia-sdk-0.4.2/ia/gaius/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)       79 2022-05-26 13:05:31.000000 ia-sdk-0.4.2/ia/gaius/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    75273 2023-08-02 14:52:24.000000 ia-sdk-0.4.2/ia/gaius/agent_client.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    22819 2023-05-08 22:12:27.000000 ia-sdk-0.4.2/ia/gaius/back_testing.py
+-rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    12451 2023-08-02 14:52:24.000000 ia-sdk-0.4.2/ia/gaius/comcom_client.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      858 2023-04-14 14:57:27.000000 ia-sdk-0.4.2/ia/gaius/data_language.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     9361 2023-08-02 14:52:24.000000 ia-sdk-0.4.2/ia/gaius/data_ops.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    17348 2023-08-02 14:52:24.000000 ia-sdk-0.4.2/ia/gaius/data_structures.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-04 12:36:21.217730 ia-sdk-0.4.2/ia/gaius/experimental/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-02 14:52:24.000000 ia-sdk-0.4.2/ia/gaius/experimental/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    11148 2023-08-03 20:40:47.000000 ia-sdk-0.4.2/ia/gaius/experimental/genome_optimizer.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     4306 2023-08-03 21:25:15.000000 ia-sdk-0.4.2/ia/gaius/genome_info.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    27195 2023-08-01 15:18:51.000000 ia-sdk-0.4.2/ia/gaius/kb_ops.py
+-rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    38911 2023-08-03 18:56:17.000000 ia-sdk-0.4.2/ia/gaius/manager.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     8771 2023-06-08 15:56:58.000000 ia-sdk-0.4.2/ia/gaius/prediction_models.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-04 12:36:21.217730 ia-sdk-0.4.2/ia/gaius/pvt/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    75372 2023-08-02 15:37:17.000000 ia-sdk-0.4.2/ia/gaius/pvt/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    26516 2023-08-02 14:52:24.000000 ia-sdk-0.4.2/ia/gaius/pvt/mongo_interface.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    10707 2023-08-01 15:18:46.000000 ia-sdk-0.4.2/ia/gaius/pvt/offline_sio.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    17775 2023-08-02 14:52:24.000000 ia-sdk-0.4.2/ia/gaius/pvt/pvt_utils.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-04 12:36:21.217730 ia-sdk-0.4.2/ia/gaius/tests/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2022-05-26 13:05:31.000000 ia-sdk-0.4.2/ia/gaius/tests/__init__.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2786 2023-06-08 15:56:58.000000 ia-sdk-0.4.2/ia/gaius/tests/classification.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2679 2023-06-08 15:56:58.000000 ia-sdk-0.4.2/ia/gaius/tests/utility.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)    11002 2023-06-08 15:56:58.000000 ia-sdk-0.4.2/ia/gaius/utils.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-04 12:36:21.217730 ia-sdk-0.4.2/ia/scripts/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        0 2023-03-24 19:12:06.000000 ia-sdk-0.4.2/ia/scripts/__init__.py
+-rwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)    40670 2023-08-03 20:39:02.000000 ia-sdk-0.4.2/ia/scripts/spawn_agent.py
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     2762 2023-08-02 14:52:24.000000 ia-sdk-0.4.2/ia/scripts/spawn_general.py
+drwxrwxr-x   0 alexlukens  (1000) alexlukens  (1000)        0 2023-08-04 12:36:21.217730 ia-sdk-0.4.2/ia_sdk.egg-info/
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1256 2023-08-04 12:36:21.000000 ia-sdk-0.4.2/ia_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      825 2023-08-04 12:36:21.000000 ia-sdk-0.4.2/ia_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        1 2023-08-04 12:36:21.000000 ia-sdk-0.4.2/ia_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      152 2023-08-04 12:36:21.000000 ia-sdk-0.4.2/ia_sdk.egg-info/requires.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)        3 2023-08-04 12:36:21.000000 ia-sdk-0.4.2/ia_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)      110 2023-08-04 12:36:21.217730 ia-sdk-0.4.2/setup.cfg
+-rw-rw-r--   0 alexlukens  (1000) alexlukens  (1000)     1225 2023-08-03 21:29:16.000000 ia-sdk-0.4.2/setup.py
```

### Comparing `ia-sdk-0.4.1/PKG-INFO` & `ia-sdk-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-sdk
-Version: 0.4.1
+Version: 0.4.2
 Summary: SDK for Intelligent Artifact's GAIuS agents.
 Home-page: https://intelligent-artifacts.com
 Author: Intelligent Artifacts
 Author-email: support@intelligent-artifacts.com
 Project-URL: Documentation, https://intelligent-artifacts.bitbucket.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ia-sdk-0.4.1/README.md` & `ia-sdk-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/agent_client.py` & `ia-sdk-0.4.2/ia/gaius/agent_client.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/back_testing.py` & `ia-sdk-0.4.2/ia/gaius/back_testing.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/comcom_client.py` & `ia-sdk-0.4.2/ia/gaius/comcom_client.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/data_language.py` & `ia-sdk-0.4.2/ia/gaius/data_language.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/data_ops.py` & `ia-sdk-0.4.2/ia/gaius/data_ops.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/data_structures.py` & `ia-sdk-0.4.2/ia/gaius/data_structures.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/experimental/genome_optimizer.py` & `ia-sdk-0.4.2/ia/gaius/experimental/genome_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                  pvt_config: dict,
                  evolutionary_params: dict,
                  agent_constructor=AgentClient,
                  agent_kwargs: dict = None,
                  pvt_constructor=PerformanceValidationTest,
                  weights: dict = {"accuracy": 1.0, "precision": 1.0},
                  ):
-        self.am = AgentManager(local=True)
+        self.am = AgentManager(local=False)
         self.genome_path = path_to_original_genome
         self.nodes_to_optimize = nodes_to_optimize
         self.agent_constructor = agent_constructor
         self.agent_kwargs = agent_kwargs
         self.pvt_config = pvt_config
         self.pvt_constructor = pvt_constructor
         self._results = None  # internal variable to hold copy of results
@@ -95,15 +95,15 @@
         params = deepcopy(self.evolutionary_params)
         population = self.toolbox.population(params.pop("npop"))
 
         self._results = algorithms.eaSimple(
             population=population, toolbox=self.toolbox, stats=self.stats, **params)
         return deepcopy(self._results)
 
-    def multiprocessed_evolve(self, n_proc: int = None) -> Tuple[Any, Logbook]:
+    def multiprocessed_evolve(self, n_proc: int = None, start_hoster: bool=True) -> Tuple[Any, Logbook]:
         """Driver function to run genetic optimization using multithreading.
         Utilizes AgentManager to spawn and manage multiple agents
 
         Args:
             n_proc (int, optional): Number of processing cores to use. Defaults to minimum of (core_count, population_size).
 
         Returns:
@@ -121,15 +121,16 @@
         try:
             SPAWN_AGENT_LOCK.release() # ensure lock is released before starting multiprocessing pool
         except:
             pass
 
         try:
             with multiprocessing.Pool(processes=n_proc) as pool:
-                self.am.start_hoster()
+                if start_hoster:
+                    self.am.start_hoster()
                 pop = self.evolve(pool=pool)
         except Exception as e:
             traceback.print_exc()
             logger.exception("Exception during multiprocessed_evolve")
             logger.info("Killing started agents")
             self.am.kill_all_agents()
             pass
```

### Comparing `ia-sdk-0.4.1/ia/gaius/genome_info.py` & `ia-sdk-0.4.2/ia/gaius/genome_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+import json
+import logging
+
+logger = logging.getLogger(__file__)
+
+
 class Genome:
     """Wrapper class for a Genome topology, loaded from a dict
 
     :ivar topology: the data representing a Genome
     :ivar agent: agent data parsed from topology
     :ivar description: Genome description field
     :ivar primitive_map: dict of "node name" to "node id" pairings
     """
+
     def __init__(self, topology: dict):
         """Initialize a genome from a GAIuS agent topology (dict)
 
         Args:
             topology (dict, required): GAIuS agent topology
         """
         self.topology = topology
@@ -27,17 +34,20 @@
         self.actions_manifests = {}
         for node in self.topology['elements']['nodes']:
             if node['data']['type'] == 'primitive':
                 self.primitives[node['data']['id']] = node['data']
             elif node['data']['type'] == 'manipulative':
                 self.manipulatives[node['data']['id']] = node['data']
 
-        self.agent_genome = {'primitives': self.primitives, 'manipulatives': self.manipulatives}
-        self.primitive_map = {x['name']: _id for _id, x in self.primitives.items()}
-        self.manipulative_map = {_id: x['name'] for _id, x in self.manipulatives.items()}
+        self.agent_genome = {'primitives': self.primitives,
+                             'manipulatives': self.manipulatives}
+        self.primitive_map = {x['name']: _id for _id,
+                              x in self.primitives.items()}
+        self.manipulative_map = {_id: x['name']
+                                 for _id, x in self.manipulatives.items()}
 
         return
 
     def get_nodes(self):
         """Return a tuple of :samp:`primitive node names`, :samp:`manipulative node names` from the topology"""
         return self.agent_genome['primitives'], self.agent_genome['manipulatives']
 
@@ -69,15 +79,46 @@
             p_id (str): primitive id of the node to edit
             gene_data (dict): dictionary of genes to update in the Genome's cache
         """
         for key, value in gene_data.items():
             self.agent_genome['primitives'][p_id][key] = value
         return
 
-    def display(self): # pragma: no cover
+    def display(self):  # pragma: no cover
         """Display the Genome topology in Cytoscape
         """
-        from cyjupyter import Cytoscape
-        return Cytoscape(data=self.topology,
-                         visual_style=self.style_obj,
-                         layout={'height': '500px'},
-                         background='white')
+        try:
+            from ipycytoscape import CytoscapeWidget
+            from IPython.display import display, clear_output
+            from ipywidgets import Output
+        except ImportError as e:
+            logger.exception(
+                "Failed to import dependencies for displaying Cytoscape graph")
+            raise
+
+        cyto = CytoscapeWidget()
+        cyto.graph.add_graph_from_json(self.topology['elements'])
+        cyto.set_style(self.style_obj)
+        clear_output()
+
+        out = Output(layout={'border': '1px solid black'})
+
+        def display_node_data(node):
+            with out:
+                out.clear_output()
+                print(
+                    f'Node {node["data"]["id"]} details:\n{json.dumps(node, indent=2)}')
+            pass
+
+        def display_edge_data(edge):
+            with out:
+                out.clear_output()
+                print(
+                    f'Edge {edge["data"]["id"]} details:\n{json.dumps(edge, indent=2)}')
+            pass
+
+        cyto.on('node', 'click', display_node_data)
+        cyto.on('edge', 'click', display_edge_data)
+        display(cyto)
+        display(out)
+
+        return
```

### Comparing `ia-sdk-0.4.1/ia/gaius/kb_ops.py` & `ia-sdk-0.4.2/ia/gaius/kb_ops.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/manager.py` & `ia-sdk-0.4.2/ia/gaius/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,14 @@
     def check_running(self):
         """Check if we can access the agent
 
         Returns:
             bool: True for success, False for failure
         """
         if self.location == 'local':
-            print(f'{self.toJSON()}')
             agent = AgentClient(bottle_info=self.agent_config)
             try:
                 agent.set_timeout(10)
                 agent.connect()
             except Exception:
                 return False
 
@@ -457,34 +456,41 @@
                            docker_image=self.docker_image):
 
             self.save_config_file()
 
         return True
 
     def kill(self):
+        """Kill Comcom and delete container
+        """
         kill_container(self.container_name)
         return self.delete_config_file()
 
     def delete_config_file(self):
-        """delete config information from agents directory
+        """delete config file information
         """
         if os.path.exists(f'{self.save_dir}/{self.name}'):
             os.remove(f'{self.save_dir}/{self.name}')
         return f"deleted {self.save_dir}/{self.name}"
 
     def save_config_file(self):
-        """Store config information for agent in agents directory, based on agent name
+        """Store config information, based on comcom name
         """
         with open(f'{self.save_dir}/{self.name}', 'w') as f:
             json.dump(obj=self.toJSON(), fp=f)
 
         logger.debug(f'saved to {self.save_dir}/{self.name}')
         return f'{self.save_dir}/{self.name}'
 
     def connect_agents(self, agents: List[AgentInfo]):
+        """Connect agents to Comcom docker network
+
+        Args:
+            agents (List[AgentInfo]): list of AgentInfo objects to connect to network
+        """
         nets = set()
         for agent in agents:
             nets.update(agent.get_docker_networks())
 
         logger.debug(f'{nets=}')
         if not connect_networks_container(networks=list(nets), container_name=self.container_name):
             return False
@@ -566,15 +572,15 @@
         self.config_file = f'{self.data_dir}/config.json'
         self.local = local
         if not os.path.exists(self.data_dir):
             os.makedirs(self.data_dir, exist_ok=True)
         logger.info(f'   agents dir: {self.agents_dir}')
         logger.info(f'   genome dir: {self.genome_dir}')
         logger.info(f'thinkflux dir: {self.thinkflux_dir}')
-        logger.info(f'comcom_dir: {self.comcom_dir}')
+        logger.info(f'   comcom_dir: {self.comcom_dir}')
 
         if not os.path.exists(self.genome_dir):
             os.makedirs(self.genome_dir, exist_ok=True)
 
         if not os.path.exists(self.agents_dir):
             os.makedirs(self.agents_dir, exist_ok=True)
 
@@ -587,14 +593,16 @@
         self.current_agents: Dict[str, AgentInfo] = {}
         self.current_tfs: Dict[str, TFInfo] = {}
         self.current_comcoms: Dict[str, ComcomInfo] = {}
 
         self.update_current_agents()
 
     def start_hoster(self):
+        """Start `dvdarias/docker-hoster <https://github.com/dvddarias/docker-hoster>`_ docker container to resolve
+        container hostnames into IP addresses. More friendly for AgentManager usage"""
         START_COMMAND = """
         if [ ! "$(docker ps -a -q -f name=docker-hoster)" ]; then
             if [ "$(docker ps -aq -f status=exited -f name=docker-hoster)" ]; then
                 # cleanup
                 docker rm docker-hoster
             fi
             # run your container
@@ -609,14 +617,15 @@
         output = subprocess.run(START_COMMAND, capture_output=True, shell=True)
         if output.returncode != 0:
             raise Exception(
                 f'Starting hoster failed with exitcode {output.returncode}')
         return
 
     def stop_hoster(self):
+        """Stop `dvdarias/docker-hoster <https://github.com/dvddarias/docker-hoster>`_ docker container"""
         STOP_COMMAND = """
         if [ "$(docker ps -a -q -f name=docker-hoster)" ]; then
             docker rm --force docker-hoster;
         fi
         
         """
         output = subprocess.run(STOP_COMMAND,
@@ -636,48 +645,58 @@
                  tf_id: str = '1',
                  environment: dict = None,
                  privileged: bool = None,
                  volumes: dict = None,
                  agents_to_connect: list = None) -> TFInfo:
         """Spawn a Thinkflux container using provided config. Store config in AgentManager
 
+        Container name is defined as:
+            "tf-{user_id}-{tf_id}"
+        
         Args:
-            tf_name (str): _description_
-            api_key (str): _description_
-            docker_image (str): _description_
+            tf_name (str): descriptive name "alias" for Thinkflux
+            api_key (str): Passed as API_KEY env variable to container
+            docker_image (str): Container image to spawn. E.g. "registry.digitalocean.com/intelligent-artifacts/thinkflux:develop"
             port (int, optional): _description_. Defaults to 8090.
-            user_id (str, optional): _description_. Defaults to 'tf'.
-            tf_id (str, optional): _description_. Defaults to '1'.
-            environment (dict, optional): _description_. Defaults to None.
-            privileged (bool, optional): _description_. Defaults to None.
-            volumes (dict, optional): _description_. Defaults to None.
-            agents_to_connect (list, optional): _description_. Defaults to None.
+            user_id (str, optional): user_id portion of container extension. Defaults to 'tf'.
+            tf_id (str, optional): tf_id portion of container extension. Defaults to '1'.
+            environment (dict, optional): additional environment variables to provide to container, as key-value pairs. Defaults to None.
+            privileged (bool, optional): run container in privileged mode. Defaults to None.
+            volumes (dict, optional): volumes to mount in container as key-value pairs. Defaults to None.
+            agents_to_connect (list, optional): list of agents to connect to Thinkflux. Defaults to None.
 
         Raises:
-            Exception: _description_
-            Exception: _description_
-            Exception: _description_
+            Exception: If invalid agents passed in agents_to_connect
+            Exception: If tf_name already exists in AgentManager
+            Exception: If a thinkflux with user_id and tf_id already exists in AgentManager
 
         Returns:
-            TFInfo: _description_
+            TFInfo: Object corresponding to spawned Thinkflux
         """
 
         self.update_current_agents()
 
         agents = []
 
         if agents_to_connect is None:
             agents_to_connect = []
 
         for agent_name in agents_to_connect:
-            if agent_name not in self.current_agents:
-                raise KeyError(
-                    f'Agent {agent_name} not found in current agents')
+            if isinstance(agent_name, AgentInfo):
+                pass
+            elif isinstance(agent_name, str):
+                
+                agents.append(self.current_agents[agent_name])
+                if agent_name not in self.current_agents:
+                    raise KeyError(
+                        f'Agent {agent_name} not found in current agents')
+                    
+            else:
+                raise Exception(f"Invalid agent found in agents_to_connect: {agent_name}")
 
-            agents.append(self.current_agents[agent_name])
 
         if tf_name in self.current_tfs:
             raise Exception(f'Thinkflux({tf_name}) already exists')
             pass
 
         for name, tf in self.current_tfs.items():
             if tf.tf_id == tf_id and tf.user_id == user_id:
@@ -700,15 +719,23 @@
         self.update_current_agents()  # update agents after spawn, before linking networks
         logger.debug(f'{agents=}')
         tf.connect_agents(agents=agents)
 
         return tf
 
     def delete_tf(self,
-                  tf_name):
+                  tf_name: str):
+        """Kill a Thinkflux container using it's tf_name attribute
+
+        Args:
+            tf_name (str): attribute passed when spawning Thinkflux
+
+        Raises:
+            Exception: When config not found
+        """
         if tf_name not in self.current_tfs:
             raise Exception(f'Thinkflux({tf_name}) not found in current_tfs')
 
         tf: TFInfo = self.current_tfs[tf_name]
         tf.kill()
 
         self.update_current_agents()
@@ -901,15 +928,15 @@
         if genome_name not in self.list_genomes():
             raise Exception(
                 f'{genome_name} not in genome dir: {self.list_genomes()}')
         with open(genome_path, 'r') as f:
             return json.load(f)
 
     def update_current_agents(self):
-        """Update the current_agents_dict
+        """Update AgentManager's list of configured agents, thinkflux, comcom, genomes
         """
 
         # retrieve all agent files
         self.current_agents = [Path(p) for p in os.listdir(
             self.agents_dir) if not os.path.isdir(os.path.realpath(p))]
         self.current_tfs = [Path(p) for p in os.listdir(
             self.thinkflux_dir) if not os.path.isdir(os.path.realpath(p))]
@@ -956,28 +983,52 @@
                 self.delete_agent(agent_name)
                 killed_agents.append(agent_name)
 
         logger.debug(f'{killed_agents=}')
 
     def kill_all_agents(self, update=True):
         """Kill all agents known to AgentManager
+
+        Args:
+            update (bool, optional): Whether to update AgentManager information before killing containers. Defaults to True.
         """
 
         if update:
             self.update_current_agents()
 
         for agent_name in list(self.current_agents.keys()):
             logger.info(f"Killing agent {agent_name}")
             self.delete_agent(agent_name=agent_name)
 
         for tf_name in list(self.current_tfs.keys()):
             self.delete_tf(tf_name=tf_name)
 
     @contextmanager
-    def agent_context(self, genome_file=None, genome_name=None, user_id: str = 'jia', agent_id: str = '1', agent_name=None, connect_jia=True, api_key='ABCD-1234'):
+    def agent_context(self,
+                      genome_file: str = None,
+                      genome_name: str = None,
+                      user_id: str = 'jia',
+                      agent_id: str = '1',
+                      agent_name: str = None,
+                      connect_jia=True,
+                      api_key='ABCD-1234'):
+        """Provide ability to use Agent as a context manager. Internally calls start_agent and stop_agent.
+
+        Args:
+            genome_file (_type_, optional): _description_. Defaults to None.
+            genome_name (_type_, optional): _description_. Defaults to None.
+            user_id (str, optional): _description_. Defaults to 'jia'.
+            agent_id (str, optional): _description_. Defaults to '1'.
+            agent_name (_type_, optional): _description_. Defaults to None.
+            connect_jia (bool, optional): _description_. Defaults to True.
+            api_key (str, optional): _description_. Defaults to 'ABCD-1234'.
+
+        Yields:
+            _type_: _description_
+        """
         try:
             agent = self.start_agent(genome_file=genome_file,
                                      genome_name=genome_name,
                                      user_id=user_id,
                                      agent_id=agent_id,
                                      agent_name=agent_name,
                                      connect_jia=connect_jia,
```

### Comparing `ia-sdk-0.4.1/ia/gaius/prediction_models.py` & `ia-sdk-0.4.2/ia/gaius/prediction_models.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/pvt/__init__.py` & `ia-sdk-0.4.2/ia/gaius/pvt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -304,15 +304,15 @@
                                          user_id=self.user_id,
                                          test_type=self.test_type).toJSON(),
                               to=self.user_id)
             try:
 
                 self.train_agent()
 
-                if self.training_percentage == 100:
+                if len(self.dataset.test_sequences) == 0:
                     logger.debug(f'Complete!')
                     continue
 
                 self.test_agent()
 
                 for k, labels in self.labels_set.items():
                     self.labels_set[k] = set(
@@ -390,26 +390,26 @@
                                          test_id=self.test_id,
                                          user_id=self.user_id,
                                          test_type=self.test_type).toJSON(),
                               to=self.user_id)
 
             self.train_agent()
 
-            if self.training_percentage == 100:
+            if len(self.dataset.test_sequences) == 0:
+                logger.debug(f'Complete!')
                 return
 
             self.test_agent()
 
             self.emotive_value_results = get_emotives_value_metrics(
                 emotives_set=self.emotives_set, this_test_log=self.testing_log[self.test_num], overall=False)
             self.overall_results = get_emotives_value_metrics(
                 emotives_set=self.emotives_set, this_test_log=list(chain(*self.testing_log)), overall=True)
             self.pvt_results.append(deepcopy(self.emotive_value_results))
-            if not self.QUIET:  # pragma: no cover
-                logger.debug('Plotting Results...')
+            logger.debug('Plotting Results...')
 
             # don't try to plot emotive values if we're working to save in a mongo database
             # (its probably running without a jupyter GUI)
             if self.PLOT:
                 plot_emotives_value_charts(test_num=self.test_num,
                                            emotive_value_results=self.emotive_value_results,
                                            QUIET=self.QUIET,
@@ -439,17 +439,16 @@
             self.mongo_results.saveResults(final_msg)
         return
 
     def run_emotive_polarity_pvt(self):
         self.pvt_results = []
         for test_num in range(0, self.test_count):
             self.test_num = test_num
-            if not self.QUIET:  # pragma: no cover
-                logger.debug(f'Conducting Test # {test_num}')
-                logger.debug('\n---------------------\n')
+            logger.debug(f'Conducting Test # {test_num}')
+
             self.prepare_datasets()
 
             if self.sio:  # pragma: no cover
                 self.sio.emit(self.socket_channel,
                               PVTMessage(status='training',
                                          current_record=0,
                                          total_record_count=len(
@@ -459,29 +458,26 @@
                                          cur_test_num=self.test_num,
                                          total_test_num=self.test_count-1,
                                          test_id=self.test_id,
                                          user_id=self.user_id,
                                          test_type=self.test_type).toJSON(),
                               to=self.user_id)
 
-            if not self.QUIET:  # pragma: no cover
-                logger.debug("Training Agent...")
+            logger.debug("Training Agent...")
             self.train_agent()
 
-            if self.training_percentage == 100:
+            if len(self.dataset.test_sequences) == 0:
+                logger.debug(f'Complete!')
                 return
 
-            if not self.QUIET:  # pragma: no cover
-                logger.debug("Testing Agent...")
+            logger.debug("Testing Agent...")
             self.test_agent()
 
-            if not self.QUIET:  # pragma: no cover
-                logger.debug('Getting Emotives Polarity Metrics...')
-            if not self.QUIET:  # pragma: no cover
-                logger.debug('Saving results to pvt_results...')
+            logger.debug('Getting Emotives Polarity Metrics...')
+            logger.debug('Saving results to pvt_results...')
             self.pvt_results.append(
                 deepcopy(get_emotives_polarity_metrics(emotives_set=self.emotives_set,
                                                        this_test_log=self.testing_log[self.test_num],
                                                        overall=False)))
             self.overall_results = get_emotives_polarity_metrics(
                 emotives_set=self.emotives_set,
                 this_test_log=list(chain(*self.testing_log)),
@@ -561,26 +557,23 @@
                 self.overall_metrics['negative'] = defaultdict(
                     lambda: defaultdict(lambda: defaultdict(float)))
                 self.overall_metrics['overall'] = defaultdict(
                     lambda: defaultdict(lambda: defaultdict(float)))
 
             # Validate Test Type
             if self.test_type == 'classification':
-                if not self.QUIET:  # pragma: no cover
-                    logger.debug("Conducting Classification PVT...\n")
+                logger.debug("Conducting Classification PVT...\n")
                 self.run_classification_pvt()
 
             elif self.test_type == 'emotives_value':
-                if not self.QUIET:  # pragma: no cover
-                    logger.debug("Conducting Emotives Value PVT...\n")
+                logger.debug("Conducting Emotives Value PVT...\n")
                 self.run_emotive_value_pvt()
 
             elif self.test_type == 'emotives_polarity':
-                if not self.QUIET:  # pragma: no cover
-                    logger.debug("Conducting Emotives Polarity PVT...\n")
+                logger.debug("Conducting Emotives Polarity PVT...\n")
                 self.run_emotive_polarity_pvt()
 
             else:
                 raise Exception(
                     """
                     Please choose one of the test type:
                     - classification
@@ -590,17 +583,16 @@
                     ex.
                     --> pvt.test_type='emotives_value'
                     then, retry
                     --> pvt.conduct_pvt()
                     """
                 )
         except Exception as e:
-            if not self.QUIET:  # pragma: no cover
-                logger.exception(
-                    f'failed to conduct PVT test, test_type={self.test_type}: {str(e)}')
+            logger.exception(
+                f'failed to conduct PVT test, test_type={self.test_type}: {str(e)}')
             raise e
 
         # convert defaultdict to normal dict by dumping and loading pvt results
         self.pvt_results = json.loads(json.dumps(self.pvt_results))
         self.overall_metrics = json.loads(json.dumps(self.overall_metrics))
 
     def train_agent(self):
@@ -674,16 +666,15 @@
                                       user_id=self.user_id,
                                       test_type=self.test_type)
 
             self.store_train_record(
                 test_num=self.test_num, record=training_msg)
 
         train_progress_bar.reset()
-        if not self.QUIET:  # pragma: no cover
-            logger.debug('Finished training agent!')
+        logger.debug('Finished training agent!')
 
     def _apply_learning_strategy(self, sequence, current_labels, record_emotive_set):
 
         if self.learning_strategy == 'on_error':
 
             predictions = self.agent.get_predictions()
             self.agent.observe(data=sequence[-1], nodes=self.ingress_nodes)
@@ -796,16 +787,15 @@
         self.predictions = []
         self.actuals = []
 
         self.testing_log.append([])
 
         test_seq_len = len(self.dataset.test_sequences)
         if test_seq_len == 0:
-            if not self.QUIET:  # pragma: no cover
-                logger.debug('length of testing sequences is 0... returning\n')
+            logger.debug('length of testing sequences is 0... returning\n')
             return
 
         test_step_info, test_progress_bar = self._setup_testing()
 
         for k, _ in enumerate(test_progress_bar):
 
             if k % 10 == 0:
@@ -1103,35 +1093,32 @@
         Sums all emotive values
         """
         emotives_seq = [event['emotives']
                         for event in sequence if event['emotives']]
         return dict(functools.reduce(operator.add, map(Counter, emotives_seq)))
 
     def abort_test_remediation(self, current_record, record_count):  # pragma: no cover (testing disabled for Celery code (used by Lab))
-        if not self.QUIET:  # pragma: no cover
-            logger.info(
-                f'about to abort {self.task.request.id =}, {self.test_id=}')
+        logger.info(
+            f'about to abort {self.task.request.id =}, {self.test_id=}')
         if self.sio:  # pragma: no cover
-            if not self.QUIET:  # pragma: no cover
-                logger.info('Sending abort message')
+            logger.info('Sending abort message')
             abort_msg = PVTMessage(status='aborted',
                                    current_record=current_record + 1,
                                    total_record_count=record_count,
                                    metrics={},
                                    overall_metrics={},
                                    cur_test_num=self.test_num,
                                    total_test_num=self.test_count-1,
                                    test_id=self.test_id,
                                    user_id=self.user_id,
                                    test_type=self.test_type)
             self.sio.emit(self.socket_channel,
                           abort_msg.toJSON(), to=self.user_id)
         if self.mongo_results:
-            if not self.QUIET:  # pragma: no cover
-                logger.info('cleaning up MongoDB')
+            logger.info('cleaning up MongoDB')
             self.mongo_results.deleteResults()
 
         raise PVTAbortError(
             f"Aborting Test, at record {current_record} of {record_count}")
 
     def store_train_record(self, test_num, record: PVTMessage):
```

### Comparing `ia-sdk-0.4.1/ia/gaius/pvt/mongo_interface.py` & `ia-sdk-0.4.2/ia/gaius/pvt/mongo_interface.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/pvt/offline_sio.py` & `ia-sdk-0.4.2/ia/gaius/pvt/offline_sio.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/pvt/pvt_utils.py` & `ia-sdk-0.4.2/ia/gaius/pvt/pvt_utils.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/tests/classification.py` & `ia-sdk-0.4.2/ia/gaius/tests/classification.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/tests/utility.py` & `ia-sdk-0.4.2/ia/gaius/tests/utility.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/gaius/utils.py` & `ia-sdk-0.4.2/ia/gaius/utils.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia/scripts/spawn_agent.py` & `ia-sdk-0.4.2/ia/scripts/spawn_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -779,15 +779,18 @@
         network: Network = docker_client.networks.get(network_name)
         network.reload()
         container_list = network.containers
 
         # remove all remaining containers from docker network (forcefully)
         container: Container
         for container in container_list:
-            network.disconnect(container=container, force=True)
+            try:
+                network.disconnect(container=container, force=True)
+            except de.APIError:
+                pass # if container already disconnected
         network.remove()
     except de.NotFound:
         logger.debug("Network %s was not found", network_name)
         pass
 
     except de.APIError:
         logger.exception(
```

### Comparing `ia-sdk-0.4.1/ia/scripts/spawn_general.py` & `ia-sdk-0.4.2/ia/scripts/spawn_general.py`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/ia_sdk.egg-info/PKG-INFO` & `ia-sdk-0.4.2/ia_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-sdk
-Version: 0.4.1
+Version: 0.4.2
 Summary: SDK for Intelligent Artifact's GAIuS agents.
 Home-page: https://intelligent-artifacts.com
 Author: Intelligent Artifacts
 Author-email: support@intelligent-artifacts.com
 Project-URL: Documentation, https://intelligent-artifacts.bitbucket.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ia-sdk-0.4.1/ia_sdk.egg-info/SOURCES.txt` & `ia-sdk-0.4.2/ia_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ia-sdk-0.4.1/setup.py` & `ia-sdk-0.4.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,10 +34,12 @@
                 'plotly',
                 'scikit-learn',
                 'matplotlib',
                 'ipywidgets',
                 'ipython',
                 'tqdm',
                 'kaleido',
-                'networkx']
+                'networkx',
+                'ipycytoscape'
+                ]
     },
 )
```

