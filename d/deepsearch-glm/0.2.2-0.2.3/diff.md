# Comparing `tmp/deepsearch_glm-0.2.2.tar.gz` & `tmp/deepsearch_glm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsearch_glm-0.2.2.tar", max compression
+gzip compressed data, was "deepsearch_glm-0.2.3.tar", max compression
```

## Comparing `deepsearch_glm-0.2.2.tar` & `deepsearch_glm-0.2.3.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0     1088 2023-07-08 03:50:49.893964 deepsearch_glm-0.2.2/LICENSE
--rw-r--r--   0        0        0     2984 2023-07-14 09:21:46.015603 deepsearch_glm-0.2.2/README.md
--rw-r--r--   0        0        0     1981 2023-07-28 09:11:03.283385 deepsearch_glm-0.2.2/build.py
--rw-r--r--   0        0        0        0 2023-07-08 03:50:49.913495 deepsearch_glm-0.2.2/deepsearch_glm/__init__.py
--rw-r--r--   0        0        0     3022 2023-07-23 04:35:49.855789 deepsearch_glm-0.2.2/deepsearch_glm/glm_create_from_docs.py
--rw-r--r--   0        0        0     4988 2023-07-14 09:21:46.051654 deepsearch_glm-0.2.2/deepsearch_glm/glm_docqa.py
--rw-r--r--   0        0        0     3152 2023-07-23 04:36:41.893381 deepsearch_glm-0.2.2/deepsearch_glm/glm_explore.py
--rw-r--r--   0        0        0     2974 2023-07-23 04:36:37.575434 deepsearch_glm-0.2.2/deepsearch_glm/glm_utils.py
--rw-r--r--   0        0        0     6508 2023-07-27 12:59:58.320686 deepsearch_glm-0.2.2/deepsearch_glm/nlp_analyse_docs.py
--rw-r--r--   0        0        0     4004 2023-07-28 03:55:33.481106 deepsearch_glm-0.2.2/deepsearch_glm/nlp_apply_on_docs.py
--rw-r--r--   0        0        0     2827 2023-07-23 05:26:44.746779 deepsearch_glm-0.2.2/deepsearch_glm/nlp_apply_on_text.py
--rw-r--r--   0        0        0    19285 2023-07-22 05:49:57.517610 deepsearch_glm-0.2.2/deepsearch_glm/nlp_train_reference.py
--rw-r--r--   0        0        0    12115 2023-07-25 05:52:14.456260 deepsearch_glm-0.2.2/deepsearch_glm/nlp_train_semantic.py
--rw-r--r--   0        0        0     2367 2023-07-23 04:14:53.204506 deepsearch_glm-0.2.2/deepsearch_glm/nlp_utils.py
--rw-r--r--   0        0        0     8534 2023-07-14 09:21:46.056334 deepsearch_glm-0.2.2/deepsearch_glm/resources/confusables/confusablesRestricted.txt
--rw-r--r--   0        0        0   599388 2023-07-14 09:21:46.058795 deepsearch_glm-0.2.2/deepsearch_glm/resources/confusables/confusablesSummary.txt
--rw-r--r--   0        0        0       82 2023-07-14 09:21:46.059061 deepsearch_glm-0.2.2/deepsearch_glm/resources/confusables/note.txt
--rw-r--r--   0        0        0      679 2023-07-14 09:21:46.059828 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/crf/part-of-speech/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.059928 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/crf/reference/note.md
--rw-r--r--   0        0        0      188 2023-07-14 09:21:46.060169 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/fasttext/language/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060269 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/fasttext/person-name/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060409 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/fasttext/semantic/note.md
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060599 deepsearch_glm-0.2.2/deepsearch_glm/resources/models/fasttext/topic/note.md
--rw-r--r--   0        0        0      801 2023-07-14 09:21:46.059514 deepsearch_glm-0.2.2/deepsearch_glm/resources/models.json
--rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060732 deepsearch_glm-0.2.2/deepsearch_glm/utils/__init__.py
--rw-r--r--   0        0        0     1822 2023-07-24 14:23:30.124083 deepsearch_glm-0.2.2/deepsearch_glm/utils/ds_query.py
--rw-r--r--   0        0        0     7973 2023-07-28 04:05:17.418171 deepsearch_glm-0.2.2/deepsearch_glm/utils/ds_utils.py
--rw-r--r--   0        0        0     1293 2023-07-21 13:46:59.409978 deepsearch_glm-0.2.2/deepsearch_glm/utils/load_pretrained_models.py
--rw-r--r--   0        0        0      729 2023-07-28 09:13:41.626532 deepsearch_glm-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3957 1970-01-01 00:00:00.000000 deepsearch_glm-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-08 03:50:49.893964 deepsearch_glm-0.2.3/LICENSE
+-rw-r--r--   0        0        0     8677 2023-08-04 06:02:23.034548 deepsearch_glm-0.2.3/README.md
+-rw-r--r--   0        0        0     2493 2023-08-04 06:02:38.615104 deepsearch_glm-0.2.3/build.py
+-rw-r--r--   0        0        0        0 2023-07-08 03:50:49.913495 deepsearch_glm-0.2.3/deepsearch_glm/__init__.py
+-rw-r--r--   0        0        0     3023 2023-08-04 06:02:23.036070 deepsearch_glm-0.2.3/deepsearch_glm/glm_create_from_docs.py
+-rw-r--r--   0        0        0     4988 2023-07-14 09:21:46.051654 deepsearch_glm-0.2.3/deepsearch_glm/glm_docqa.py
+-rw-r--r--   0        0        0     3292 2023-08-04 06:02:23.036939 deepsearch_glm-0.2.3/deepsearch_glm/glm_explore.py
+-rw-r--r--   0        0        0     3073 2023-08-04 06:02:23.038055 deepsearch_glm-0.2.3/deepsearch_glm/glm_utils.py
+-rw-r--r--   0        0        0     6731 2023-08-04 06:02:23.038765 deepsearch_glm-0.2.3/deepsearch_glm/nlp_analyse_docs.py
+-rw-r--r--   0        0        0     4136 2023-08-04 06:02:23.040047 deepsearch_glm-0.2.3/deepsearch_glm/nlp_apply_on_docs.py
+-rw-r--r--   0        0        0     2827 2023-07-28 12:49:20.419427 deepsearch_glm-0.2.3/deepsearch_glm/nlp_apply_on_text.py
+-rw-r--r--   0        0        0    19410 2023-08-04 06:02:23.041019 deepsearch_glm-0.2.3/deepsearch_glm/nlp_train_reference.py
+-rw-r--r--   0        0        0    12193 2023-08-04 06:02:23.041768 deepsearch_glm-0.2.3/deepsearch_glm/nlp_train_semantic.py
+-rw-r--r--   0        0        0     2424 2023-08-04 06:02:23.042401 deepsearch_glm-0.2.3/deepsearch_glm/nlp_utils.py
+-rw-r--r--   0        0        0     8534 2023-07-14 09:21:46.056334 deepsearch_glm-0.2.3/deepsearch_glm/resources/confusables/confusablesRestricted.txt
+-rw-r--r--   0        0        0   599388 2023-07-14 09:21:46.058795 deepsearch_glm-0.2.3/deepsearch_glm/resources/confusables/confusablesSummary.txt
+-rw-r--r--   0        0        0       82 2023-07-14 09:21:46.059061 deepsearch_glm-0.2.3/deepsearch_glm/resources/confusables/note.txt
+-rw-r--r--   0        0        0       32 2023-08-04 06:02:23.043954 deepsearch_glm-0.2.3/deepsearch_glm/resources/models/crf/geoloc/note.md
+-rw-r--r--   0        0        0      679 2023-07-14 09:21:46.059828 deepsearch_glm-0.2.3/deepsearch_glm/resources/models/crf/part-of-speech/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.059928 deepsearch_glm-0.2.3/deepsearch_glm/resources/models/crf/reference/note.md
+-rw-r--r--   0        0        0      188 2023-07-14 09:21:46.060169 deepsearch_glm-0.2.3/deepsearch_glm/resources/models/fasttext/language/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060269 deepsearch_glm-0.2.3/deepsearch_glm/resources/models/fasttext/person-name/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060409 deepsearch_glm-0.2.3/deepsearch_glm/resources/models/fasttext/semantic/note.md
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060599 deepsearch_glm-0.2.3/deepsearch_glm/resources/models/fasttext/topic/note.md
+-rw-r--r--   0        0        0       32 2023-08-04 06:02:23.044301 deepsearch_glm-0.2.3/deepsearch_glm/resources/models/rgx/geoloc/note.md
+-rw-r--r--   0        0        0      875 2023-08-04 06:02:23.043215 deepsearch_glm-0.2.3/deepsearch_glm/resources/models.json
+-rw-r--r--   0        0        0        0 2023-07-14 09:21:46.060732 deepsearch_glm-0.2.3/deepsearch_glm/utils/__init__.py
+-rw-r--r--   0        0        0     1822 2023-07-28 12:49:20.423097 deepsearch_glm-0.2.3/deepsearch_glm/utils/ds_query.py
+-rw-r--r--   0        0        0     7973 2023-08-03 12:29:12.345476 deepsearch_glm-0.2.3/deepsearch_glm/utils/ds_utils.py
+-rw-r--r--   0        0        0     1344 2023-08-04 06:02:23.045124 deepsearch_glm-0.2.3/deepsearch_glm/utils/load_pretrained_models.py
+-rw-r--r--   0        0        0      729 2023-08-04 06:02:23.045923 deepsearch_glm-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     9650 1970-01-01 00:00:00.000000 deepsearch_glm-0.2.3/PKG-INFO
```

### Comparing `deepsearch_glm-0.2.2/LICENSE` & `deepsearch_glm-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/glm_create_from_docs.py` & `deepsearch_glm-0.2.3/deepsearch_glm/glm_create_from_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import textwrap
 import datetime
 
 from tabulate import tabulate
 
 from deepsearch_glm.glm_utils import create_glm_dir, create_glm_from_docs
 
-import andromeda_glm
+#import andromeda_glm
 
 def parse_arguments():
 
     parser = argparse.ArgumentParser(
         prog = 'create_glm_from_docs',
         description = 'Create GLM from Deep Search documents',
         epilog =
```

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/glm_docqa.py` & `deepsearch_glm-0.2.3/deepsearch_glm/glm_docqa.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/glm_explore.py` & `deepsearch_glm-0.2.3/deepsearch_glm/glm_explore.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 import textwrap
 import datetime
 
 from tabulate import tabulate
 
 from deepsearch_glm.glm_utils import load_glm
 
-import andromeda_nlp
-import andromeda_glm
+from deepsearch_glm.andromeda_nlp import nlp_model
+from deepsearch_glm.andromeda_glm import glm_model, glm_query
+
+#import andromeda_nlp
+#import andromeda_glm
 
 def parse_arguments():
 
     parser = argparse.ArgumentParser(
         prog = 'explore_glm',
         description = 'Explore GLM from Deep Search documents',
         epilog =
@@ -57,20 +60,22 @@
             text = row[headers.index("text")]
             #print("text: ", text)
             
             data[j][headers.index("text")] = "\n".join(wrapper.wrap(text))
                     
         print(f"operation {i}: \n", tabulate(data[0:max_nodes], headers=headers), "\n")
 
-def expand_terms(terms, glm_model):
+def expand_terms(terms, glm):
 
     for term in terms:
         print(term)
         
-        qry = andromeda_glm.glm_query()
+        #qry = andromeda_glm.glm_query()
+        qry = glm_query()
+        
         qry.select({"nodes":[[term]]})
         qry.filter_by({"mode": "node-flavor", "node-flavors":["token"]})
         #qry.filter_by({"mode": "node-flavor", "node-flavors":["term"]})
 
         #flid = qry.get_last_flid()
         qry.traverse({"name": "roots", "edge":"to-root"})
         qry.traverse({"name": "tax-up", "edge":"tax-up"})
@@ -82,15 +87,15 @@
         #qry.traverse({"edge":"to-sent"})
 
         qry.filter_by({"mode": "node-regex", "node-regex":[f".*{term}.*"]})
         
         config = qry.to_config()    
         #print("query: ", json.dumps(config, indent=2))    
         
-        res = glm_model.query(config)
+        res = glm.query(config)
         if "status" in res and res["status"]=="success":
             show_query_result(res)
         else:
             print(res)
             #print(res["status"], ": ", res["message"])
 
 def explore(glm_model):
```

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/glm_utils.py` & `deepsearch_glm-0.2.3/deepsearch_glm/glm_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 import textwrap
 import datetime
 
 from tabulate import tabulate
 
 from deepsearch_glm.utils.ds_utils import get_scratch_dir
 
+from deepsearch_glm.andromeda_glm import glm_model
+
 #import andromeda_nlp
-import andromeda_glm
+#import andromeda_glm
 
 def create_glm_dir():
 
     tdir = get_scratch_dir()
 
     now = datetime.datetime.now()
     glmdir = now.strftime("GLM-model-%Y-%m-%d_%H-%M-%S")
@@ -38,15 +40,16 @@
 
     return config
 
 def load_glm(idir:str):
 
     config = load_glm_config(idir)
     
-    glm = andromeda_glm.glm_model()
+    #glm = andromeda_glm.glm_model()
+    glm = glm_model()
     glm.load(config)
 
     return glm
 
 def create_glm_config_from_docs(odir:str, json_files:list[str],
                                 nlp_models:str="conn;verb;term;abbreviation"):
 
@@ -122,14 +125,15 @@
     return config
 
 def create_glm_from_docs(odir:str, json_files:list[str],
                          nlp_models:str="conn;verb;term;abbreviation"):
     
     config = create_glm_config_from_docs(odir, json_files, nlp_models)
     
-    glm = andromeda_glm.glm_model()
+    #glm = andromeda_glm.glm_model()
+    glm = glm_model()
     glm.create(config)
 
     return odir, glm
```

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/nlp_analyse_docs.py` & `deepsearch_glm-0.2.3/deepsearch_glm/nlp_analyse_docs.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 import numpy as np
 import pandas as pd
 
 from tabulate import tabulate
 from PIL import Image, ImageDraw
 
-import andromeda_nlp
+#import andromeda_nlp
+from deepsearch_glm.andromeda_nlp import nlp_model
 
 def parse_arguments():
 
     parser = argparse.ArgumentParser(
         prog = 'nlp_analyse_docs',
         description = 'Analyse NLP on `Deep Search` documents ()',
         epilog =
@@ -62,16 +63,21 @@
 
     # FIXME: ineffecient but works ...
     df = pd.read_json(json.dumps(page_items), orient='records')
     print(df)
 
     df_page = df[df["page"]==page_num]
 
-    ph = int(df_dims[df_dims["page"]==page_num]["height"][0])
-    pw = int(df_dims[df_dims["page"]==page_num]["width"][0])
+    print(df_dims[df_dims["page"]==page_num])
+
+    ph = int(df_dims[df_dims["page"]==page_num]["height"])
+    pw = int(df_dims[df_dims["page"]==page_num]["width"])
+    
+    #ph = int(df_dims[df_dims["page"]==page_num]["height"][0])
+    #pw = int(df_dims[df_dims["page"]==page_num]["width"][0])
 
     print("height: ", ph)
     print("width: ", pw)
     
     df_page["bbox"] = df_page["bbox"].apply(lambda bbox: [bbox[0], ph-bbox[3], bbox[2], ph-bbox[1]])
     #df_page = df_page.apply(lambda row: [row["bbox"][0], ph-row["bbox"][3], row["bbox"][2], ph-row["bbox"][1]], axis=1)
     
@@ -222,15 +228,15 @@
     for json_file in json_files:
 
         print(f" --> reading {json_file}")
         with open(json_file, "r") as fr:
             doc = json.load(fr)
 
         if "page" in mode or mode=="all":
-            show_page(doc, page_num=1)
+            show_page(doc, page_num=8)
 
         if "text" in mode or mode=="all":
             extract_text(doc)
 
         if "sentence" in mode or mode=="all":            
             extract_sentences(doc)
```

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/nlp_apply_on_docs.py` & `deepsearch_glm-0.2.3/deepsearch_glm/nlp_apply_on_docs.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import glob
 import argparse
 
 import pandas as pd
 
 from utils.ds_utils import convert_pdffiles
 
-import andromeda_nlp
+#import andromeda_nlp
+from deepsearch_glm.andromeda_nlp import nlp_model
 
 def parse_arguments():
 
     parser = argparse.ArgumentParser(
         prog = 'apply_nlp_on_doc',
         description = 'Apply NLP on `Deep Search` documents',
         epilog =
@@ -73,18 +74,20 @@
     if json!=None:
         json_files=sorted(glob.glob(json))
     else:
         json_files=[]
         
     return pdf_files, json_files, args.models, args.force_convert
 
+# FIXME: to be replaced with function in nlp_utils
 def init_nlp_model(models:str):
     
-    model = andromeda_nlp.nlp_model()
-
+    #model = andromeda_nlp.nlp_model()
+    model = nlp_model()
+    
     config = model.get_apply_configs()[0]
     config["models"] = models
     
     model.initialise(config)
 
     return model
```

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/nlp_apply_on_text.py` & `deepsearch_glm-0.2.3/deepsearch_glm/nlp_apply_on_text.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/nlp_train_reference.py` & `deepsearch_glm-0.2.3/deepsearch_glm/nlp_train_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,20 @@
 
 #import fasttext
 import textColor as tc
 
 #import deepsearch as ds
 #from tabulate import tabulate
 
-import andromeda_nlp
+#import andromeda_nlp
+from deepsearch_glm.andromeda_nlp import nlp_model
 
 from deepsearch_glm.utils.ds_utils import convert_pdffiles
 from deepsearch_glm.nlp_utils import create_nlp_dir
 
-
-
 def parse_arguments():
 
     parser = argparse.ArgumentParser(
         prog = "nlp_train_reference",
         description = 'Prepare CRF data for CRF-reference parser',
         epilog =
 """
@@ -103,15 +102,16 @@
     
     config = {
         "mode" : "apply",
         "order" : True,
         "models": "numval,link"
     }
     
-    model = andromeda_nlp.nlp_model()
+    #model = andromeda_nlp.nlp_model()
+    model = nlp_model()
     model.initialise(config)
     
     MINLEN = 5
 
     fws = open(sfile, "w")
     fwr = open(rfile, "w")
     
@@ -520,15 +520,16 @@
         fw.write(json.dumps(ref)+"\n")
     fw.close()
 
     print(tc.green(f"training file has been written to {afile}"))
 
 def train_crf(train_file, model_file, metrics_file):
 
-    model = andromeda_nlp.nlp_model()
+    #model = andromeda_nlp.nlp_model()
+    model = nlp_model()
                 
     configs = model.get_train_configs()
 
     for config in configs:
         if config["mode"]=="train" and \
            config["model"]=="reference":
 
@@ -545,15 +546,16 @@
 #
 #  => the parameters can be found via
 #
 # `./fasttext dump model_cooking.bin args`
 #
 def train_fst(train_file, model_file, metrics_file):
 
-    model = andromeda_nlp.nlp_model()
+    #model = andromeda_nlp.nlp_model()
+    model = nlp_model()
                 
     configs = model.get_train_configs()    
     print(configs)
     
     for config in configs:
         if config["mode"]=="train" and \
            config["model"]=="semantic":
```

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/nlp_train_semantic.py` & `deepsearch_glm-0.2.3/deepsearch_glm/nlp_train_semantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 import glob
 
 import random
 import argparse
 
 import textColor as tc
 
+from deepsearch_glm.andromeda_nlp import nlp_model
+
 from deepsearch_glm.utils.ds_utils import convert_pdffiles, ds_index_query
 from deepsearch_glm.nlp_utils import create_nlp_dir, init_nlp_model, print_on_shell
 
-import andromeda_nlp
+#import andromeda_nlp
 
 def parse_arguments():
 
     parser = argparse.ArgumentParser(
         prog = "nlp_train_semantic",
         description = 'train classifier for semantic text classifier',
         epilog =
@@ -319,15 +321,16 @@
 #
 #  => the parameters can be found via
 #
 # `./fasttext dump model_cooking.bin args`
 #
 def train_fst(train_file, model_file, metrics_file):
 
-    model = andromeda_nlp.nlp_model()
+    #model = andromeda_nlp.nlp_model()
+    model = nlp_model()
                 
     configs = model.get_train_configs()    
     print(json.dumps(configs, indent=2))
 
     for config in configs:
         if config["mode"]=="train" and \
            config["model"]=="semantic":
```

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/nlp_utils.py` & `deepsearch_glm-0.2.3/deepsearch_glm/nlp_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 import textColor as tc
 import pandas as pd
 
 from tabulate import tabulate
 
 from deepsearch_glm.utils.ds_utils import get_scratch_dir
 
-import andromeda_nlp
+from deepsearch_glm.andromeda_nlp import nlp_model
+#import andromeda_nlp
 
 def create_nlp_dir(tdir=None):
 
     if tdir==None:
         tdir = get_scratch_dir()
 
     now = datetime.datetime.now()
@@ -37,25 +38,26 @@
     configs += nlp_model.get_apply_configs()
     configs += nlp_model.get_train_configs()
 
     return configs
 
 def init_nlp_model(model_names:str="language;term"):
 
-    nlp_model = andromeda_nlp.nlp_model()
+    #model = andromeda_nlp.nlp_model()
+    model = nlp_model()
 
-    configs = nlp_model.get_apply_configs()
+    configs = model.get_apply_configs()
     #print(json.dumps(configs, indent=2))
     
-    config = nlp_model.get_apply_configs()[0]
+    config = model.get_apply_configs()[0]
     config["models"] = model_names
 
-    nlp_model.initialise(config)
+    model.initialise(config)
     
-    return nlp_model
+    return model
 
 def print_key_on_shell(key, items):
 
     df = pd.DataFrame(items["data"],
                       columns=items["headers"])
     
     if key in ["instances", "entities"]:
```

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/resources/confusables/confusablesRestricted.txt` & `deepsearch_glm-0.2.3/deepsearch_glm/resources/confusables/confusablesRestricted.txt`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/resources/confusables/confusablesSummary.txt` & `deepsearch_glm-0.2.3/deepsearch_glm/resources/confusables/confusablesSummary.txt`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/resources/models/crf/part-of-speech/note.md` & `deepsearch_glm-0.2.3/deepsearch_glm/resources/models/crf/part-of-speech/note.md`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/resources/models.json` & `deepsearch_glm-0.2.3/deepsearch_glm/resources/models.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953703703703703%*

 * *Differences: {"'nlp'": "{'trained-models': {'geoloc': ['rgx_geoloc.json', "*

 * *          "'models/rgx/geoloc/rgx_geoloc.json']}}"}*

```diff
@@ -4,14 +4,18 @@
         "prefix": "deepsearch_glm/v1/glm",
         "trained-models": {}
     },
     "nlp": {
         "bucket": "ds4sd-public-artifacts",
         "prefix": "deepsearch_glm/v1/nlp",
         "trained-models": {
+            "geoloc": [
+                "rgx_geoloc.json",
+                "models/rgx/geoloc/rgx_geoloc.json"
+            ],
             "language": [
                 "fst_language.bin",
                 "models/fasttext/language/fst_language.bin"
             ],
             "name": [
                 "fst_person_name.bin",
                 "models/fasttext/person-name/fst_person_name.bin"
```

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/utils/ds_query.py` & `deepsearch_glm-0.2.3/deepsearch_glm/utils/ds_query.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/utils/ds_utils.py` & `deepsearch_glm-0.2.3/deepsearch_glm/utils/ds_utils.py`

 * *Files identical despite different names*

### Comparing `deepsearch_glm-0.2.2/deepsearch_glm/utils/load_pretrained_models.py` & `deepsearch_glm-0.2.3/deepsearch_glm/utils/load_pretrained_models.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 
 import os
 import json
 import subprocess
 
-def load_pretrained_nlp_models(force:bool=False):
+def load_pretrained_nlp_models(force:bool=False, verbose:bool=False):
 
     if "DEEPSEARCH_GLM_RESOURCES_DIR" in os.environ:
         RESOURCES_DIR = os.getenv("DEEPSEARCH_GLM_RESOURCES_DIR")
     else:
-        # FIXME: not sure about this ...
-        ROOT_DIR=os.path.abspath("./deepsearch_glm")
-        RESOURCES_DIR=os.path.join(ROOT_DIR, "resources")
+        from deepsearch_glm.andromeda_nlp import nlp_model
+
+        model = nlp_model()
+        RESOURCES_DIR = model.get_resources_path()
     
     with open(f"{RESOURCES_DIR}/models.json") as fr:
         models = json.load(fr)
         
     COS_URL = models["object-store"]
     COS_PRFX = models["nlp"]["prefix"]
     COS_PATH = os.path.join(COS_URL, COS_PRFX)
     
     cmds=[]
     for name,files in models["nlp"]["trained-models"].items():
         source = os.path.join(COS_PATH, files[0])
         target = os.path.join(RESOURCES_DIR, files[1])
 
         cmd = ["curl", source, "-o", target, "-s"]
-        #print(" ".join(cmd))        
         cmds.append(cmd)
         
     for cmd in cmds:
-        if force or (not os.path.exists(cmd[3])):
-            #print(f"downloading {cmd[3]} ... ", end="")
-            print(f"downloading {os.path.basename(cmd[3])} ... ", end="")            
+
+        model_weights = cmd[3]
+        
+        if force or (not os.path.exists(model_weights)):
+
+            if verbose:
+                print(f"downloading {os.path.basename(model_weights)} ... ", end="")            
+
             message = subprocess.run(cmd)#, cwd=ROOT_DIR)    
-            print("done!")
-        else:
+
+            if verbose:
+                print("done!")
+                
+        elif verbose:
             print(f" -> already downloaded {os.path.basename(cmd[3])}")
```

### Comparing `deepsearch_glm-0.2.2/pyproject.toml` & `deepsearch_glm-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsearch-glm"
-version = "0.2.2"
+version = "0.2.3"
 description = "Graph Language Models"
 authors = ["Peter Staar <taa@zurich.ibm.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "deepsearch_glm"}]
 include = [
     {path = "deepsearch_glm/*.so", format = "wheel"}
```

