# Comparing `tmp/grewpy-0.4.1.tar.gz` & `tmp/grewpy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grewpy-0.4.1.tar", last modified: Tue Jun 13 13:32:17 2023, max compression
+gzip compressed data, was "grewpy-0.4.2.tar", last modified: Fri Aug  4 14:36:53 2023, max compression
```

## Comparing `grewpy-0.4.1.tar` & `grewpy-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-06-13 13:32:17.437492 grewpy-0.4.1/
--rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-06-13 13:32:17.437383 grewpy-0.4.1/PKG-INFO
--rw-r--r--   0 guillaum   (501) staff       (20)      113 2022-12-19 12:33:36.000000 grewpy-0.4.1/README.md
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-06-13 13:32:17.435468 grewpy-0.4.1/examples/
--rw-r--r--   0 guillaum   (501) staff       (20)     2057 2023-04-11 16:02:43.000000 grewpy-0.4.1/examples/allemand.py
--rw-r--r--   0 guillaum   (501) staff       (20)     4741 2023-06-13 12:46:05.000000 grewpy-0.4.1/examples/classifier.py
--rw-r--r--   0 guillaum   (501) staff       (20)     6822 2023-06-13 12:46:05.000000 grewpy-0.4.1/examples/learner.py
--rw-r--r--   0 guillaum   (501) staff       (20)     9359 2023-06-13 12:46:05.000000 grewpy-0.4.1/examples/rule_forgery.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2836 2023-05-02 13:38:29.000000 grewpy-0.4.1/examples/test_GRS.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2990 2023-06-13 13:00:03.000000 grewpy-0.4.1/examples/test_corpus.py
--rw-r--r--   0 guillaum   (501) staff       (20)      937 2023-01-16 14:38:31.000000 grewpy-0.4.1/examples/test_graph.py
--rw-r--r--   0 guillaum   (501) staff       (20)      736 2023-02-09 15:38:41.000000 grewpy-0.4.1/examples/test_grew_web.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1405 2023-01-09 12:56:06.000000 grewpy-0.4.1/examples/test_search.py
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-06-13 13:32:17.436728 grewpy-0.4.1/grewpy/
--rw-r--r--   0 guillaum   (501) staff       (20)      365 2023-06-13 12:46:05.000000 grewpy-0.4.1/grewpy/__init__.py
--rw-r--r--   0 guillaum   (501) staff       (20)     9167 2023-06-13 12:58:09.000000 grewpy-0.4.1/grewpy/corpus.py
--rw-r--r--   0 guillaum   (501) staff       (20)     9317 2023-06-13 13:30:36.000000 grewpy-0.4.1/grewpy/graph.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1109 2022-12-21 08:33:45.000000 grewpy-0.4.1/grewpy/grew.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2737 2023-06-13 12:46:05.000000 grewpy-0.4.1/grewpy/grew_web.py
--rw-r--r--   0 guillaum   (501) staff       (20)    13053 2023-06-13 12:46:05.000000 grewpy-0.4.1/grewpy/grs.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1752 2023-02-13 12:14:28.000000 grewpy-0.4.1/grewpy/matchings.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2938 2023-06-13 12:46:05.000000 grewpy-0.4.1/grewpy/network.py
--rw-r--r--   0 guillaum   (501) staff       (20)     2620 2023-02-21 09:38:54.000000 grewpy-0.4.1/grewpy/observation.py
--rw-r--r--   0 guillaum   (501) staff       (20)     1099 2023-06-13 12:46:05.000000 grewpy-0.4.1/grewpy/sketch.py
--rw-r--r--   0 guillaum   (501) staff       (20)      190 2022-12-19 17:10:04.000000 grewpy-0.4.1/grewpy/utils.py
-drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-06-13 13:32:17.437231 grewpy-0.4.1/grewpy.egg-info/
--rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-06-13 13:32:17.000000 grewpy-0.4.1/grewpy.egg-info/PKG-INFO
--rw-r--r--   0 guillaum   (501) staff       (20)      538 2023-06-13 13:32:17.000000 grewpy-0.4.1/grewpy.egg-info/SOURCES.txt
--rw-r--r--   0 guillaum   (501) staff       (20)        1 2023-06-13 13:32:17.000000 grewpy-0.4.1/grewpy.egg-info/dependency_links.txt
--rw-r--r--   0 guillaum   (501) staff       (20)       16 2023-06-13 13:32:17.000000 grewpy-0.4.1/grewpy.egg-info/top_level.txt
--rw-r--r--   0 guillaum   (501) staff       (20)       38 2023-06-13 13:32:17.437526 grewpy-0.4.1/setup.cfg
--rw-r--r--   0 guillaum   (501) staff       (20)      463 2023-06-13 13:31:39.000000 grewpy-0.4.1/setup.py
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-08-04 14:36:53.205511 grewpy-0.4.2/
+-rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-08-04 14:36:53.205394 grewpy-0.4.2/PKG-INFO
+-rw-r--r--   0 guillaum   (501) staff       (20)      113 2022-12-19 12:33:36.000000 grewpy-0.4.2/README.md
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-08-04 14:36:53.203348 grewpy-0.4.2/examples/
+-rw-r--r--   0 guillaum   (501) staff       (20)     2057 2023-04-11 16:02:43.000000 grewpy-0.4.2/examples/allemand.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     4741 2023-06-13 12:46:05.000000 grewpy-0.4.2/examples/classifier.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     6822 2023-06-13 12:46:05.000000 grewpy-0.4.2/examples/learner.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     9359 2023-06-13 12:46:05.000000 grewpy-0.4.2/examples/rule_forgery.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2836 2023-05-02 13:38:29.000000 grewpy-0.4.2/examples/test_GRS.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2727 2023-08-04 14:34:32.000000 grewpy-0.4.2/examples/test_corpus.py
+-rw-r--r--   0 guillaum   (501) staff       (20)      937 2023-01-16 14:38:31.000000 grewpy-0.4.2/examples/test_graph.py
+-rw-r--r--   0 guillaum   (501) staff       (20)      736 2023-02-09 15:38:41.000000 grewpy-0.4.2/examples/test_grew_web.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1529 2023-06-26 19:42:57.000000 grewpy-0.4.2/examples/test_search.py
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-08-04 14:36:53.204600 grewpy-0.4.2/grewpy/
+-rw-r--r--   0 guillaum   (501) staff       (20)      365 2023-06-13 12:46:05.000000 grewpy-0.4.2/grewpy/__init__.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     9167 2023-06-26 17:16:12.000000 grewpy-0.4.2/grewpy/corpus.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     9317 2023-06-26 17:16:12.000000 grewpy-0.4.2/grewpy/graph.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1109 2022-12-21 08:33:45.000000 grewpy-0.4.2/grewpy/grew.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2737 2023-06-13 12:46:05.000000 grewpy-0.4.2/grewpy/grew_web.py
+-rw-r--r--   0 guillaum   (501) staff       (20)    13057 2023-08-04 14:30:18.000000 grewpy-0.4.2/grewpy/grs.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1752 2023-02-13 12:14:28.000000 grewpy-0.4.2/grewpy/matchings.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2938 2023-06-13 12:46:05.000000 grewpy-0.4.2/grewpy/network.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     2620 2023-02-21 09:38:54.000000 grewpy-0.4.2/grewpy/observation.py
+-rw-r--r--   0 guillaum   (501) staff       (20)     1099 2023-06-13 12:46:05.000000 grewpy-0.4.2/grewpy/sketch.py
+-rw-r--r--   0 guillaum   (501) staff       (20)      190 2022-12-19 17:10:04.000000 grewpy-0.4.2/grewpy/utils.py
+drwxr-xr-x   0 guillaum   (501) staff       (20)        0 2023-08-04 14:36:53.205211 grewpy-0.4.2/grewpy.egg-info/
+-rw-r--r--   0 guillaum   (501) staff       (20)      386 2023-08-04 14:36:53.000000 grewpy-0.4.2/grewpy.egg-info/PKG-INFO
+-rw-r--r--   0 guillaum   (501) staff       (20)      538 2023-08-04 14:36:53.000000 grewpy-0.4.2/grewpy.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaum   (501) staff       (20)        1 2023-08-04 14:36:53.000000 grewpy-0.4.2/grewpy.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaum   (501) staff       (20)       16 2023-08-04 14:36:53.000000 grewpy-0.4.2/grewpy.egg-info/top_level.txt
+-rw-r--r--   0 guillaum   (501) staff       (20)       38 2023-08-04 14:36:53.205552 grewpy-0.4.2/setup.cfg
+-rw-r--r--   0 guillaum   (501) staff       (20)      463 2023-08-04 14:36:42.000000 grewpy-0.4.2/setup.py
```

### Comparing `grewpy-0.4.1/examples/allemand.py` & `grewpy-0.4.2/examples/allemand.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/examples/classifier.py` & `grewpy-0.4.2/examples/classifier.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/examples/learner.py` & `grewpy-0.4.2/examples/learner.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/examples/rule_forgery.py` & `grewpy-0.4.2/examples/rule_forgery.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/examples/test_GRS.py` & `grewpy-0.4.2/examples/test_GRS.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/examples/test_corpus.py` & `grewpy-0.4.2/examples/test_corpus.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 sys.path.insert(0, os.path.abspath(os.path.join( os.path.dirname(__file__), "../"))) # Use local grew lib
 
 from grewpy import Graph, CorpusDraft, Request, Corpus, request_counter
 
 pud_file = "examples/resources/pud_10.conllu"
 pud = Corpus(pud_file)
 
-print (pud.edge_diff(pud))
-exit (0)
 print ("\n=============== len ===============")
 print(f"nb of graph in {pud_file} = {len(pud)}")
 print (request_counter())
 
 print ("\n=============== Get one graph ===============")
 sent_id="n01003013"
 graph = pud[sent_id]
@@ -31,32 +29,26 @@
 for sent_id in pud.get_sent_ids():
   acc += len(pud[sent_id])
 print(f"nb of nodes in {pud_file} = ", acc)
 print (request_counter())
 
 print ("\n=============== Count request in a corpus ===============")
 upos="ADV"
-req1 = Request(f"X[upos={upos}]; Y -[advmod]-> X")
-req2 = Request(f"X[upos={upos}]", "Y -[advmod]-> X")
-req3 = Request.parse(f"pattern {{ X[upos={upos}]; Y -[advmod]-> X }}")
-print(" ----- basic count -----")
-print(f"nb of {upos} in {pud_file} = ", pud.count(req1))
-print(f"nb of {upos} in {pud_file} = ", pud.count(req2))
-print(f"nb of {upos} in {pud_file} = ", pud.count(req3))
-
+req = Request(f"X[upos={upos}]").global_('sent_id="n01001011"')
 
-exit(0)
+print(" ----- basic count -----")
+print(f"nb of {upos} in {pud_file} = ", pud.count(req))
 
+exit (0)
 print (" ----- count with clustering -----")
 print(f"nb of {upos} in {pud_file}, clustered by lemma:")
 print (json.dumps(pud.count(req, ["X.lemma"]), indent=2))
 print (request_counter())
 
 
-
 corpus = CorpusDraft(pud)
 print("\n=============== Iteration on graphs of a corpus ===============")
 acc = 0
 for sent_id in corpus:
   acc += len(corpus[sent_id])
 print(f"nb of nodes in {pud_file} = ", acc)
 print (request_counter())
```

### Comparing `grewpy-0.4.1/examples/test_graph.py` & `grewpy-0.4.2/examples/test_graph.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/examples/test_grew_web.py` & `grewpy-0.4.2/examples/test_grew_web.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/examples/test_search.py` & `grewpy-0.4.2/examples/test_search.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,34 +8,37 @@
 from grewpy import set_config
 set_config("sud")
 
 pud_file = "examples/resources/fr_pud-sud-test.conllu"
 pud = Corpus(pud_file)
 print(f"nb of graph in {pud_file} = {len(pud)}")
 
+r = Request.from_json([{'pattern': 'e: N -[1=subj]-> M'}])
+print (pud.count(r))
 
-# g = pud[9]
-# print(g)
-# print (g.edge('8', '4'))
+r = Request.from_json('pattern { e: N -[1=subj]-> M}')
+print (pud.count(r))
 
-r = Request('e: N -[1=subj]-> M;')
+r = Request.from_json(['pattern {',  'e: N -[1=subj]-> M', '}'])
 print (pud.count(r))
 
+
+
 x = Request('e: N -[subj]-> M;')
 print (pud.count(x))
 
-exit (0)
 
 r = Request('e: N -> M; M[form="a"]')
 print (r)
 
+
 matchings = pud.search(r, ['e.label'])
-print (json.dumps(matchings, indent=2)) 
-{'1': 'nsubj'}
+# print (json.dumps(matchings, indent=2)) 
 print ("------------------------------------------")
+exit(0)
 
 grs = GRS ("""
 rule r { pattern { N[upos=NOUN] } commands { N.upos=N} } 
 """)
 
 
 # grs = GRS ("""
```

### Comparing `grewpy-0.4.1/grewpy/corpus.py` & `grewpy-0.4.2/grewpy/corpus.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/grewpy/graph.py` & `grewpy-0.4.2/grewpy/graph.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/grewpy/grew.py` & `grewpy-0.4.2/grewpy/grew.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/grewpy/grew_web.py` & `grewpy-0.4.2/grewpy/grew_web.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/grewpy/grs.py` & `grewpy-0.4.2/grewpy/grs.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,21 +68,21 @@
                 except:
                     raise ValueError(f"{e} cannot be used to build a Request")
         self.items = elts
 
     def without(self, *L):
         self.items += tuple(RequestItem("without", e) for e in L)
         return self
+
     def with_(self, *L):
         self.items += tuple(RequestItem("with", e) for e in L)
         return self
 
-
-    def with_(self, *L):
-        self.items += tuple(RequestItem("with", e) for e in L)
+    def global_(self, *L):
+        self.items += tuple(RequestItem("global", e) for e in L)
         return self
 
     @classmethod
     def from_json(cls,json_data):
         elts = [RequestItem.from_json(c) for c in json_data]
         return cls(*elts)
```

### Comparing `grewpy-0.4.1/grewpy/matchings.py` & `grewpy-0.4.2/grewpy/matchings.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/grewpy/network.py` & `grewpy-0.4.2/grewpy/network.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/grewpy/observation.py` & `grewpy-0.4.2/grewpy/observation.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/grewpy/sketch.py` & `grewpy-0.4.2/grewpy/sketch.py`

 * *Files identical despite different names*

### Comparing `grewpy-0.4.1/grewpy.egg-info/SOURCES.txt` & `grewpy-0.4.2/grewpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

