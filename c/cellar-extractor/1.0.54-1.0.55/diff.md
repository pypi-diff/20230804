# Comparing `tmp/cellar_extractor-1.0.54.tar.gz` & `tmp/cellar_extractor-1.0.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellar_extractor-1.0.54.tar", last modified: Thu Aug  3 09:59:11 2023, max compression
+gzip compressed data, was "cellar_extractor-1.0.55.tar", last modified: Fri Aug  4 10:43:06 2023, max compression
```

## Comparing `cellar_extractor-1.0.54.tar` & `cellar_extractor-1.0.55.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 09:59:11.310483 cellar_extractor-1.0.54/
--rw-rw-rw-   0        0        0     7505 2023-08-03 09:59:11.309480 cellar_extractor-1.0.54/PKG-INFO
--rw-rw-rw-   0        0        0     7058 2023-08-03 09:57:16.000000 cellar_extractor-1.0.54/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 09:59:11.299971 cellar_extractor-1.0.54/cellar_extractor/
--rw-rw-rw-   0        0        0      709 2023-08-03 09:56:02.000000 cellar_extractor-1.0.54/cellar_extractor/Testing_file.py
--rw-rw-rw-   0        0        0      224 2023-08-03 09:50:44.000000 cellar_extractor-1.0.54/cellar_extractor/__init__.py
--rw-rw-rw-   0        0        0     3694 2023-08-03 09:58:14.000000 cellar_extractor-1.0.54/cellar_extractor/cellar.py
--rw-rw-rw-   0        0        0     1005 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/cellar_extra_extract.py
--rw-rw-rw-   0        0        0     5227 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/cellar_queries.py
--rw-rw-rw-   0        0        0    11308 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/citations_adder.py
--rw-rw-rw-   0        0        0     1355 2023-08-02 12:06:01.000000 cellar_extractor-1.0.54/cellar_extractor/csv_extractor.py
--rw-rw-rw-   0        0        0    16726 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/eurlex_scraping.py
--rw-rw-rw-   0        0        0     6477 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/fulltext_saving.py
--rw-rw-rw-   0        0        0     5411 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/json_to_csv.py
--rw-rw-rw-   0        0        0     1040 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/nodes_and_edges.py
--rw-rw-rw-   0        0        0     6834 2023-07-31 10:47:48.000000 cellar_extractor-1.0.54/cellar_extractor/sparql.py
-drwxrwxrwx   0        0        0        0 2023-08-03 09:59:11.308483 cellar_extractor-1.0.54/cellar_extractor.egg-info/
--rw-rw-rw-   0        0        0     7505 2023-08-03 09:59:11.000000 cellar_extractor-1.0.54/cellar_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-08-03 09:59:11.000000 cellar_extractor-1.0.54/cellar_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 09:59:11.000000 cellar_extractor-1.0.54/cellar_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-08-03 09:59:11.000000 cellar_extractor-1.0.54/cellar_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-03 09:59:11.000000 cellar_extractor-1.0.54/cellar_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 09:59:11.311480 cellar_extractor-1.0.54/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-08-03 09:58:14.000000 cellar_extractor-1.0.54/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 10:43:06.026636 cellar_extractor-1.0.55/
+-rw-rw-rw-   0        0        0     7765 2023-08-04 10:43:06.025636 cellar_extractor-1.0.55/PKG-INFO
+-rw-rw-rw-   0        0        0     7318 2023-08-04 10:40:54.000000 cellar_extractor-1.0.55/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 10:43:06.016636 cellar_extractor-1.0.55/cellar_extractor/
+-rw-rw-rw-   0        0        0      709 2023-08-03 09:56:02.000000 cellar_extractor-1.0.55/cellar_extractor/Testing_file.py
+-rw-rw-rw-   0        0        0      224 2023-08-03 09:50:44.000000 cellar_extractor-1.0.55/cellar_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3688 2023-08-04 10:37:49.000000 cellar_extractor-1.0.55/cellar_extractor/cellar.py
+-rw-rw-rw-   0        0        0     1005 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/cellar_extra_extract.py
+-rw-rw-rw-   0        0        0     5227 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/cellar_queries.py
+-rw-rw-rw-   0        0        0    11308 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/citations_adder.py
+-rw-rw-rw-   0        0        0     1355 2023-08-02 12:06:01.000000 cellar_extractor-1.0.55/cellar_extractor/csv_extractor.py
+-rw-rw-rw-   0        0        0    16726 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/eurlex_scraping.py
+-rw-rw-rw-   0        0        0     6477 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/fulltext_saving.py
+-rw-rw-rw-   0        0        0     5411 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/json_to_csv.py
+-rw-rw-rw-   0        0        0     1145 2023-08-04 10:37:49.000000 cellar_extractor-1.0.55/cellar_extractor/nodes_and_edges.py
+-rw-rw-rw-   0        0        0     6834 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/sparql.py
+drwxrwxrwx   0        0        0        0 2023-08-04 10:43:06.024637 cellar_extractor-1.0.55/cellar_extractor.egg-info/
+-rw-rw-rw-   0        0        0     7765 2023-08-04 10:43:05.000000 cellar_extractor-1.0.55/cellar_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-08-04 10:43:05.000000 cellar_extractor-1.0.55/cellar_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 10:43:05.000000 cellar_extractor-1.0.55/cellar_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-08-04 10:43:05.000000 cellar_extractor-1.0.55/cellar_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-04 10:43:05.000000 cellar_extractor-1.0.55/cellar_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 10:43:06.027635 cellar_extractor-1.0.55/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-08-04 10:41:46.000000 cellar_extractor-1.0.55/setup.py
```

### Comparing `cellar_extractor-1.0.54/PKG-INFO` & `cellar_extractor-1.0.55/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: cellar_extractor
-Version: 1.0.54
-Summary: Library for extracting cellar data
-Author: LawTech Lab
-Author-email: p.lewandowski@student.maastrichtuniversity.nl
-License: MIT
-Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
-Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
-Keywords: cellar,extractor
-Description-Content-Type: text/markdown
-
 ## Cellar extractor
 This library contains two functions to get cellar case law data from eurlex.
 
 ## Version
 Python 3.9
 
 ## Contributors
@@ -112,14 +100,17 @@
         <br>
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from the get_cellar_extra method with eurlex webservice credentials passed.
         This method will only work on dataframes with citations data.
+        <li><strong>only_local: boolean, optional, default False</strong></li>
+        Flag for nodes and edges generation. If set to True, the network created will only include nodes and edges between 
+        cases exclusively inside the given dataframe.
     </ul>
     <li><code>filter_subject_matter</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from any of the cellar extraction methods listed above.
         <li><strong>phrase: string, required, default None</strong></li>
         The phrase which has to be present in the subject matter of cases. Case insensitive.
```

#### html2text {}

```diff
@@ -1,15 +1,9 @@
-Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.54 Summary: Library
-for extracting cellar data Author: LawTech Lab Author-email:
-p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
-Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
-Build Source, https://github.com/maastrichtlawtech/extraction_libraries
-Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
-extractor This library contains two functions to get cellar case law data from
-eurlex. ## Version Python 3.9 ## Contributors
+## Cellar extractor This library contains two functions to get cellar case law
+data from eurlex. ## Version Python 3.9 ## Contributors
 [pranavnbapat]_    [Cloud956]_    [shashankmc]_ [gijsvd]_
  Pranav_Bapat   Piotr_Lewandowski  shashankmc    gijsvd
  ## How to install? pip install cellar-extractor ## What are the functions?
    1. get_cellar
    2. Gets all the ECLI data from the eurlex sparql endpoint and saves them in
       the CSV or JSON format, in-memory or as a saved file.
    3. get_cellar_extra
@@ -64,14 +58,18 @@
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
             method with eurlex webservice credentials passed. This method will
             only work on dataframes with citations data.
+          o only_local: boolean, optional, default False
+          o Flag for nodes and edges generation. If set to True, the network
+            created will only include nodes and edges between cases exclusively
+            inside the given dataframe.
    5. filter_subject_matter
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from any of the cellar
             extraction methods listed above.
           o phrase: string, required, default None
           o The phrase which has to be present in the subject matter of cases.
             Case insensitive.
```

### Comparing `cellar_extractor-1.0.54/README.md` & `cellar_extractor-1.0.55/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: cellar_extractor
+Version: 1.0.55
+Summary: Library for extracting cellar data
+Author: LawTech Lab
+Author-email: p.lewandowski@student.maastrichtuniversity.nl
+License: MIT
+Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
+Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
+Keywords: cellar,extractor
+Description-Content-Type: text/markdown
+
 ## Cellar extractor
 This library contains two functions to get cellar case law data from eurlex.
 
 ## Version
 Python 3.9
 
 ## Contributors
@@ -100,14 +112,17 @@
         <br>
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from the get_cellar_extra method with eurlex webservice credentials passed.
         This method will only work on dataframes with citations data.
+        <li><strong>only_local: boolean, optional, default False</strong></li>
+        Flag for nodes and edges generation. If set to True, the network created will only include nodes and edges between 
+        cases exclusively inside the given dataframe.
     </ul>
     <li><code>filter_subject_matter</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from any of the cellar extraction methods listed above.
         <li><strong>phrase: string, required, default None</strong></li>
         The phrase which has to be present in the subject matter of cases. Case insensitive.
```

#### html2text {}

```diff
@@ -1,9 +1,15 @@
-## Cellar extractor This library contains two functions to get cellar case law
-data from eurlex. ## Version Python 3.9 ## Contributors
+Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.55 Summary: Library
+for extracting cellar data Author: LawTech Lab Author-email:
+p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
+Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
+Build Source, https://github.com/maastrichtlawtech/extraction_libraries
+Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
+extractor This library contains two functions to get cellar case law data from
+eurlex. ## Version Python 3.9 ## Contributors
 [pranavnbapat]_    [Cloud956]_    [shashankmc]_ [gijsvd]_
  Pranav_Bapat   Piotr_Lewandowski  shashankmc    gijsvd
  ## How to install? pip install cellar-extractor ## What are the functions?
    1. get_cellar
    2. Gets all the ECLI data from the eurlex sparql endpoint and saves them in
       the CSV or JSON format, in-memory or as a saved file.
    3. get_cellar_extra
@@ -58,14 +64,18 @@
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
             method with eurlex webservice credentials passed. This method will
             only work on dataframes with citations data.
+          o only_local: boolean, optional, default False
+          o Flag for nodes and edges generation. If set to True, the network
+            created will only include nodes and edges between cases exclusively
+            inside the given dataframe.
    5. filter_subject_matter
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from any of the cellar
             extraction methods listed above.
           o phrase: string, required, default None
           o The phrase which has to be present in the subject matter of cases.
             Case insensitive.
```

### Comparing `cellar_extractor-1.0.54/cellar_extractor/Testing_file.py` & `cellar_extractor-1.0.55/cellar_extractor/Testing_file.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.54/cellar_extractor/cellar.py` & `cellar_extractor-1.0.55/cellar_extractor/cellar.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,25 +70,24 @@
     else:
         data, json = extra_cellar(data=data, threads=threads, username=username, password=password)
         print("\n--- DONE ---")
 
         return data, json
 
 
-def get_nodes_and_edges_lists(df=None):
+def get_nodes_and_edges_lists(df=None, only_local=False):
     if df is None:
         print("No dataframe passed!")
         return
-    else:
-        try:
-            nodes, edges = get_nodes_and_edges(df)
-        except:
-            print('Something went wrong. Nodes and edges creation unsuccessful.')
-            return False, False
-        return nodes, edges
+    try:
+        nodes, edges = get_nodes_and_edges(df,only_local)
+    except:
+        print('Something went wrong. Nodes and edges creation unsuccessful.')
+        return False, False
+    return nodes, edges
 
 
 def filter_subject_matter(df=None, phrase=None):
     if df is None or phrase is None:
         print("Incorrect input values! \n Returning... \n")
     else:
         try:
```

### Comparing `cellar_extractor-1.0.54/cellar_extractor/cellar_extra_extract.py` & `cellar_extractor-1.0.55/cellar_extractor/cellar_extra_extract.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.54/cellar_extractor/cellar_queries.py` & `cellar_extractor-1.0.55/cellar_extractor/cellar_queries.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.54/cellar_extractor/citations_adder.py` & `cellar_extractor-1.0.55/cellar_extractor/citations_adder.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.54/cellar_extractor/csv_extractor.py` & `cellar_extractor-1.0.55/cellar_extractor/csv_extractor.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.54/cellar_extractor/eurlex_scraping.py` & `cellar_extractor-1.0.55/cellar_extractor/eurlex_scraping.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.54/cellar_extractor/fulltext_saving.py` & `cellar_extractor-1.0.55/cellar_extractor/fulltext_saving.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.54/cellar_extractor/json_to_csv.py` & `cellar_extractor-1.0.55/cellar_extractor/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.54/cellar_extractor/nodes_and_edges.py` & `cellar_extractor-1.0.55/cellar_extractor/nodes_and_edges.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import pandas as pd
 def extract_containing_subject_matter(df,phrase):
     returner = df[df["LEGAL RESOURCE IS ABOUT SUBJECT MATTER"].str.contains(phrase, na=False)]
     return returner
 def get_df_with_celexes(df,celexes):
     returner = df[df['CELEX IDENTIFIER'].isin(celexes)]
     return returner
-def get_edges_list(df):
+def get_edges_list(df,only_local):
     extraction = df[['CELEX IDENTIFIER','citing']]
     extraction.reset_index(inplace=True)
     keys = extraction['CELEX IDENTIFIER']
     vals = extraction['citing']
     nodes = set()
     edges = list()
     for i in range(len(keys)):
         k = keys[i]
         val = vals[i]
-        if val == val:
-            nodes.add(str(k))
-            val_unpacked = val.split(";")
-            for val in val_unpacked:
-                nodes.add(str(val))
-                edges.append(str(k)+','+str(val))
-        else:
-            pass
+        if val != val:
+            continue
+        nodes.add(str(k))
+        val_unpacked = val.split(";")
+        for val in val_unpacked:
+            if only_local and val not in keys:
+                continue
+            nodes.add(str(val))
+            edges.append(str(k)+','+str(val))
+
+    nodes = list(nodes)
+
     return edges, list(nodes)
-def get_nodes_and_edges(df):
-    edges, nodes = get_edges_list(df)
+def get_nodes_and_edges(df,only_local):
+    edges, nodes = get_edges_list(df,only_local)
     #nodes = get_df_with_celexes(df,celexes)
     return nodes,edges
```

### Comparing `cellar_extractor-1.0.54/cellar_extractor/sparql.py` & `cellar_extractor-1.0.55/cellar_extractor/sparql.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.54/cellar_extractor.egg-info/PKG-INFO` & `cellar_extractor-1.0.55/cellar_extractor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar-extractor
-Version: 1.0.54
+Version: 1.0.55
 Summary: Library for extracting cellar data
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor
@@ -112,14 +112,17 @@
         <br>
     </ul>
     <li><code>get_nodes_and_edges_lists</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from the get_cellar_extra method with eurlex webservice credentials passed.
         This method will only work on dataframes with citations data.
+        <li><strong>only_local: boolean, optional, default False</strong></li>
+        Flag for nodes and edges generation. If set to True, the network created will only include nodes and edges between 
+        cases exclusively inside the given dataframe.
     </ul>
     <li><code>filter_subject_matter</code></li>
     <ul>
         <li><strong>df: DataFrame object, required, default None</strong></li>
         DataFrame of cellar metadata acquired from any of the cellar extraction methods listed above.
         <li><strong>phrase: string, required, default None</strong></li>
         The phrase which has to be present in the subject matter of cases. Case insensitive.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.54 Summary: Library
+Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.55 Summary: Library
 for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
 extractor This library contains two functions to get cellar case law data from
 eurlex. ## Version Python 3.9 ## Contributors
@@ -64,14 +64,18 @@
           o password: string, optional, default empty string
           o The password to the eurlex webservices.
    4. get_nodes_and_edges_lists
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from the get_cellar_extra
             method with eurlex webservice credentials passed. This method will
             only work on dataframes with citations data.
+          o only_local: boolean, optional, default False
+          o Flag for nodes and edges generation. If set to True, the network
+            created will only include nodes and edges between cases exclusively
+            inside the given dataframe.
    5. filter_subject_matter
           o df: DataFrame object, required, default None
           o DataFrame of cellar metadata acquired from any of the cellar
             extraction methods listed above.
           o phrase: string, required, default None
           o The phrase which has to be present in the subject matter of cases.
             Case insensitive.
```

### Comparing `cellar_extractor-1.0.54/cellar_extractor.egg-info/SOURCES.txt` & `cellar_extractor-1.0.55/cellar_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.54/setup.py` & `cellar_extractor-1.0.55/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='cellar_extractor',
     packages=find_packages(include=['cellar_extractor']),
-    version='1.0.54',
+    version='1.0.55',
     description='Library for extracting cellar data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4','SPARQLWrapper==2.0.0', 'requests==2.26.0', 'pandas','lxml==4.6.3','xmltodict==0.13.0','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['cellar', 'extractor'],
     long_description=long_descr,
```

