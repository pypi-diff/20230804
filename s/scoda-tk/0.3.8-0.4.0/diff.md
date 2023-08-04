# Comparing `tmp/scoda-tk-0.3.8.tar.gz` & `tmp/scoda-tk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.3.8.tar", last modified: Wed Aug  2 17:22:54 2023, max compression
+gzip compressed data, was "scoda-tk-0.4.0.tar", last modified: Fri Aug  4 16:39:58 2023, max compression
```

## Comparing `scoda-tk-0.3.8.tar` & `scoda-tk-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:22:54.769088 scoda-tk-0.3.8/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-02 12:34:47.000000 scoda-tk-0.3.8/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-02 12:34:47.000000 scoda-tk-0.3.8/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 17:22:54.769088 scoda-tk-0.3.8/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-02 12:34:48.000000 scoda-tk-0.3.8/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-02 17:21:22.000000 scoda-tk-0.3.8/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-02 17:22:54.769088 scoda-tk-0.3.8/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-02 12:34:47.000000 scoda-tk-0.3.8/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:22:54.745088 scoda-tk-0.3.8/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:22:54.749088 scoda-tk-0.3.8/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-02 12:34:52.000000 scoda-tk-0.3.8/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-08-02 12:34:49.000000 scoda-tk-0.3.8/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:22:54.769088 scoda-tk-0.3.8/src/scoda/default_optional_files/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-02 12:34:49.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/analysis_config.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-02 12:34:50.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/cpdb.zip
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-02 12:34:51.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/hg38_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-02 13:29:18.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/kegg_human.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-02 13:29:18.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/kegg_mouse.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-02 12:34:49.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/markers_hs.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-02 12:34:49.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/markers_mm.tsv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-02 12:34:52.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/mm10_gene_only.gtf
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-02 13:30:21.000000 scoda-tk-0.3.8/src/scoda/default_optional_files/msig.gmt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 12:34:52.000000 scoda-tk-0.3.8/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    13947 2023-08-02 14:40:32.000000 scoda-tk-0.3.8/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-02 12:34:48.000000 scoda-tk-0.3.8/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    33986 2023-08-02 12:34:51.000000 scoda-tk-0.3.8/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-08-02 12:34:52.000000 scoda-tk-0.3.8/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    23980 2023-08-02 17:22:35.000000 scoda-tk-0.3.8/src/scoda/pipeline.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    64916 2023-08-02 16:11:38.000000 scoda-tk-0.3.8/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-02 17:22:54.769088 scoda-tk-0.3.8/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-02 17:22:54.000000 scoda-tk-0.3.8/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-04 16:39:58.743104 scoda-tk-0.4.0/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-08-02 17:43:12.000000 scoda-tk-0.4.0/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      128 2023-08-02 17:43:13.000000 scoda-tk-0.4.0/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-04 16:39:58.743104 scoda-tk-0.4.0/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-08-02 17:43:21.000000 scoda-tk-0.4.0/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-08-04 16:38:31.000000 scoda-tk-0.4.0/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-08-04 16:39:58.743104 scoda-tk-0.4.0/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-08-02 17:43:12.000000 scoda-tk-0.4.0/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-04 16:39:58.407112 scoda-tk-0.4.0/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-04 16:39:58.447111 scoda-tk-0.4.0/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-08-02 17:43:20.000000 scoda-tk-0.4.0/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-08-02 17:43:18.000000 scoda-tk-0.4.0/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-04 16:39:58.735104 scoda-tk-0.4.0/src/scoda/default_optional_files/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      291 2023-08-02 17:43:18.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/analysis_config.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   110525 2023-08-02 17:43:19.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/cpdb.zip
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  9812023 2023-08-02 17:43:19.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/hg38_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   216264 2023-08-02 17:43:19.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/kegg_human.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   200990 2023-08-02 17:43:19.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/kegg_mouse.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     9771 2023-08-02 17:43:18.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/markers_hs.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    10054 2023-08-02 17:43:18.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/markers_mm.tsv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)  6641898 2023-08-02 17:43:20.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/mm10_gene_only.gtf
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    98551 2023-08-02 17:43:19.000000 scoda-tk-0.4.0/src/scoda/default_optional_files/msig.gmt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    18849 2023-08-02 17:43:20.000000 scoda-tk-0.4.0/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    13947 2023-08-02 17:43:17.000000 scoda-tk-0.4.0/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157974 2023-08-02 17:43:17.000000 scoda-tk-0.4.0/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37683 2023-08-04 16:36:57.000000 scoda-tk-0.4.0/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    31368 2023-08-02 17:43:20.000000 scoda-tk-0.4.0/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    24791 2023-08-04 16:38:16.000000 scoda-tk-0.4.0/src/scoda/pipeline.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    64946 2023-08-03 10:06:50.000000 scoda-tk-0.4.0/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-08-04 16:39:58.743104 scoda-tk-0.4.0/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      872 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-08-04 16:39:58.000000 scoda-tk-0.4.0/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.3.8/LICENSE` & `scoda-tk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/PKG-INFO` & `scoda-tk-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.8
+Version: 0.4.0
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.8/src/scoda/cpdb.py` & `scoda-tk-0.4.0/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/default_optional_files/cpdb.zip` & `scoda-tk-0.4.0/src/scoda/default_optional_files/cpdb.zip`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/default_optional_files/hg38_gene_only.gtf` & `scoda-tk-0.4.0/src/scoda/default_optional_files/hg38_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/default_optional_files/kegg_human.gmt` & `scoda-tk-0.4.0/src/scoda/default_optional_files/kegg_human.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/default_optional_files/kegg_mouse.gmt` & `scoda-tk-0.4.0/src/scoda/default_optional_files/kegg_mouse.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/default_optional_files/markers_hs.tsv` & `scoda-tk-0.4.0/src/scoda/default_optional_files/markers_hs.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/default_optional_files/markers_mm.tsv` & `scoda-tk-0.4.0/src/scoda/default_optional_files/markers_mm.tsv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/default_optional_files/mm10_gene_only.gtf` & `scoda-tk-0.4.0/src/scoda/default_optional_files/mm10_gene_only.gtf`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/default_optional_files/msig.gmt` & `scoda-tk-0.4.0/src/scoda/default_optional_files/msig.gmt`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/deg.py` & `scoda-tk-0.4.0/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/gsea.py` & `scoda-tk-0.4.0/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/hicat.py` & `scoda-tk-0.4.0/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/icnv.py` & `scoda-tk-0.4.0/src/scoda/icnv.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,17 +85,18 @@
     b = (xs < mu0)
     pr[b] = MIN_ABS_VALUE
     
     return pr
 
 
 def get_cnv_threshold_bimodal( obs, ref_ind, score_key = 'cnv_score', 
-                               cluster_key = 'cnv_leiden', th_min = 0, refp_min = 0.9, 
+                               cluster_key = 'cnv_leiden', th_max = 0, refp_min = 0.9, 
                                ucr = 0.1, plot_stat = True, suffix = '', Data = None ):
     
+    th_min = -th_max
     ## obs must contain columns 'cnv_cluster', 'cnv_score'
     
     df = obs.groupby([cluster_key])[score_key].agg(**{'cmean':'mean'})
     idx_lst = list(df.index.values)
     
     ps = bimodal_fit( df['cmean'] )
     w0, m0, v0, w1, m1, v1 = tuple(ps)
@@ -124,14 +125,15 @@
             
     s = obs[score_key]
     tpr = get_malignancy_prob( s, list(ps) )
     obs['tumor_score'+ suffix] = tpr
     
     # print('threshold: ', th )
     th = max(th, th_min)
+    th = min(th, th_max)
     
     dec = pd.Series(['Normal']*len(s), index = obs.index)
     
     lt = th - (th - m0)*ucr # p_exc 
     ut = th + (m1 - th)*ucr #p_exc
     
     bs = (s > th)
@@ -184,18 +186,20 @@
                     legend_loc = 'upper left', bbox_to_anchor = (1, 1),
                     figsize = (4,3), log = False, alpha = 0.8 )
         
     return obs[['tumor_dec'+ suffix, 'tumor_score'+ suffix]], params
 
 
 def get_cnv_threshold_useref( obs, ref_ind, score_key = 'tumor_score', 
-                              cluster_key = 'cnv_leiden', th_min = 0, refp_min = 0.9, 
+                              cluster_key = 'cnv_leiden', th_max = 0, refp_min = 0.9, 
                               p_exc = 0.1, ucr = 0.1, plot_stat = True, 
                               suffix = '', Data = None ):
     
+    th_min = -th_max
+    
     ## obs must contain columns 'cnv_cluster', 'cnv_score'
     start_time = time.time()
     
     # df = obs.groupby([cluster_key])[score_key].agg(**{'cmean':'median'})
     df = obs.groupby([cluster_key])[score_key].agg(**{'cmean':'mean'})
     idx_lst = list(df.index.values)
     
@@ -326,14 +330,15 @@
     if ss_div_dm > 1:
         print('\nINFO: Std_sum/Mean_diff: %f > 1' % (ss_div_dm))
         print('INFO: indicating that no tumor cells might be present in this sample.' % (ss_div_dm))
         # th = m0 + np.sqrt(v0)
         
     # print('threshold: ', th )
     th = max(th, th_min)
+    th = min(th, th_max)
             
     s = obs[score_key]
     tpr = get_malignancy_prob( s, [w0, m0, v0, w1, m1, v1] )
     
     obs['tumor_prob'+ suffix] = tpr
     
     dec = pd.Series(['Normal']*len(s), index = obs.index)
@@ -570,83 +575,133 @@
         else:
             break
             
     return seed_clusters
 
 
 def extend_major_clusters( adj_agg_mat, seed_clusters, 
-                           cluster_size, alpha = 1, 
-                           pv_cutoff = None, verbose = False ):
+                           cluster_size, n_neighbors, alpha = 0.08, 
+                           pv_cutoff = None, mode = 'max', 
+                           verbose = False ):
 
+    selected_clusters = copy.deepcopy(seed_clusters)
     maj_clusters = copy.deepcopy(seed_clusters)
-    selected_clusters = copy.deepcopy(maj_clusters)
+    pair_clusters = list(np.zeros(len(seed_clusters)))
+    metrics = list(np.zeros(len(seed_clusters)))
+    thresholds = list(np.zeros(len(seed_clusters)))
     
     adj_agg_mat = np.array(adj_agg_mat)
     adj_agg_mat = adj_agg_mat - np.diag(np.diag(adj_agg_mat))
     adj_agg_mat = adj_agg_mat + adj_agg_mat.transpose()
+
+    csz_lst = [cluster_size[n] for n in maj_clusters]
+    odr = (-np.array(csz_lst)).argsort()
+    maj_clusters = [maj_clusters[o] for o in odr]
+    
+    core_mat = adj_agg_mat[maj_clusters, :][:,maj_clusters]
+
+    for j, n in enumerate(maj_clusters):
+        cnt_n = adj_agg_mat[maj_clusters,n]                
+        odr = np.array(cnt_n).argsort()
+        p = maj_clusters[int(odr[-1])]
+        if mode == 'max':
+            met = (adj_agg_mat[p,n]/n_neighbors)
+        else:
+            met = (np.sum(cnt_n)/n_neighbors)
+        pair_clusters[j] = p
+        metrics[j] = met
+        thresholds[j] = met/min(cluster_size[n], cluster_size[p])
+    
     
     flag = True
     for a in range(adj_agg_mat.shape[0] - len(seed_clusters)):
         
         core_mat = adj_agg_mat[maj_clusters, :][:,maj_clusters]
-        core_mxs = core_mat.max(axis = 1)
-        
-        # odr = (-core_mxs).argsort()
-        # core_mxs = core_mxs[odr]
-        # maj_clusters = list(np.array(maj_clusters)[odr])
+        if mode == 'max':
+            core_mxs = core_mat.max(axis = 1)
+        else:
+            core_mxs = core_mat.sum(axis = 1)
         
         core_dm = np.mean(core_mxs)
         core_ds = np.std(core_mxs)
         
-        dvs = []
+        met = []
         nodes = []
         pair = []
+        csz_lst = []
         for n in range(adj_agg_mat.shape[0]):
 
             if n not in maj_clusters:
-                cnt_n = adj_agg_mat[maj_clusters,n]
+                cnt_n = adj_agg_mat[maj_clusters,n]                
                 odr = np.array(cnt_n).argsort()
                 nodes.append(n)
                 p = maj_clusters[int(odr[-1])]
                 pair.append(p)
-                dvs.append(adj_agg_mat[p,n])
-                    
-        if len(dvs) == 1:
-            md = dvs[0]
-            cn = nodes[0]
-        else:
-            odr = np.array(dvs).argsort()
-
-            md = dvs[odr[-1]]
-            cn = nodes[odr[-1]]
-            pp = pair[odr[-1]]
+                csz_lst.append(cluster_size[n])
+                if mode == 'max':
+                    met.append(adj_agg_mat[p,n]/n_neighbors)
+                else:
+                    met.append(np.sum(cnt_n)/n_neighbors)
+              
+        cnt = 0
+        med_cluster_size = 0 # np.median(csz_lst)
+        for md, cn, pp, cs in zip(met, nodes, pair, csz_lst):
 
-        if alpha is not None:
-            condition = md >= cluster_size[cn]*alpha
-        else:
-            st = np.abs(core_dm - md)/(core_ds)
-            pv = stats.t.sf(st*np.sqrt(2), df = 1)*2
-            condition = pv >= pv_cutoff
-            
-        if flag & condition:
-            maj_clusters.append(cn)
-            selected_clusters = copy.deepcopy(maj_clusters)
-            if verbose: print(cn, pp, md, cluster_size[cn]) 
-        else:
+            if cs >= med_cluster_size:
+                if alpha is not None:
+                    csz = md/min(cluster_size[cn], cluster_size[pp])
+                    condition = (csz >= (alpha))
+                else:
+                    st = np.abs(core_dm - md)/(core_ds)
+                    pv = stats.t.sf(st*np.sqrt(2), df = 1)*2
+                    condition = pv >= pv_cutoff
+                    csz = pv
+
+                if flag & condition:
+                    maj_clusters.append(cn)
+                    pair_clusters.append(pp)
+                    metrics.append(md)
+                    thresholds.append(csz)
+                    selected_clusters = copy.deepcopy(maj_clusters)
+                    cnt += 1
+                    if verbose: print('A', cn, pp, '%4i' % int(md), cluster_size[cn]) 
+                    
+        if len(selected_clusters) == len(cluster_size): break
+        
+        if cnt == 0:
             flag = False
-            if verbose: print(cn, pp, md, cluster_size[cn]) 
-            # break
-            maj_clusters.append(cn)
-            pass
+            for md, cn, pp, cs in zip(met, nodes, pair, csz_lst):
+
+                if alpha is not None:
+                    csz = md/min(cluster_size[cn], cluster_size[pp])
+                    condition = (csz >= (alpha))
+                else:
+                    st = np.abs(core_dm - md)/(core_ds)
+                    pv = stats.t.sf(st*np.sqrt(2), df = 1)*2
+                    condition = pv >= pv_cutoff
+                    csz = pv
+
+                if verbose: print('B', cn, pp, '%4i' % int(md), cluster_size[cn], selected_clusters) 
+                # break
+                maj_clusters.append(cn)
+                pair_clusters.append(pp)
+                metrics.append(md)
+                thresholds.append(csz)
+                pass
                     
+        if len(maj_clusters) >= len(cluster_size): break
+        
     core_mat = adj_agg_mat[maj_clusters, :][:,maj_clusters]
-    core_mxs = core_mat.max(axis = 1)
+    if mode == 'max':
+        core_mxs = core_mat.max(axis = 1)
+    else:
+        core_mxs = core_mat.sum(axis = 1)
     
-    return np.array(selected_clusters), np.array(maj_clusters), core_mxs
-
+    return (np.array(selected_clusters), 
+           np.array(maj_clusters), np.array(pair_clusters), metrics, thresholds)
 
 
 import warnings
 
 def run_icnv(adata, ref_key, ref_types, gtf_file, cluster_key = 'cnv_leiden', 
              resolution = 2, N_pca = 15, n_neighbors = 10, umap = True, pca = True, n_cores = 4 ):
     
@@ -715,15 +770,15 @@
         km = cluster.KMeans(n_clusters = int(N_clusters), random_state = 0)
         km.fit(X_pca)
         cluster_label = km.labels_
         return cluster_label, km, adj
     else:
         adj = kneighbors_graph(X_pca, int(N_neighbors), mode=mode, include_self=True, 
                                n_jobs = n_cores)
-        louvain = Louvain(resolution = resolution)
+        louvain = Louvain(resolution = resolution, random_state = 0)
         if hasattr(louvain, 'fit_predict'):
             cluster_label = louvain.fit_predict(adj)        
         else:
             cluster_label = louvain.fit_transform(adj)        
         return cluster_label, louvain, adj
     '''
     elif clust_algo[:2] == 'ld':
@@ -765,21 +820,27 @@
 
     df['b_inc'] = b_inc
     b = np.array(b_inc)
     # print(df)
     return df
 
 
-def identify_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, 
-                       clust = None, Clustering_resolution = 1, N_clusters = 30,
-                       # cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
-                       gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
-                       dec_margin = 0.05, n_neighbors = 10, cmd_cutoff = 0.03, 
-                       gcm = 0.05, plot_stat = False, use_ref = False, 
-                       n_cores = 4, cd_alpha = 1, suffix = '', Data = None):
+def identify_tumor_cells(X_cnv, ref_ind, pca = False, use_cnv_score = False, clust = None, 
+                         Clustering_algo = 'lv', Clustering_resolution = 1, N_clusters = 30,
+                         # cluster_key = 'cnv_leiden', score_key = 'tumor_score', 
+                         gmm_N_comp = 20, th_max = 0.1, refp_min = 0.9, p_exc = 0.1, 
+                         dec_margin = 0.05, n_neighbors = 10, cmd_cutoff = 0.03, 
+                         gcm = 0.05, plot_stat = False, use_ref = False, 
+                         n_cores = 4, connectivity_thresh = 0.08, net_search_mode = 'sum', 
+                         suffix = '', Data = None, verbose = False):
+    
+    N_clusters = int(np.log2(X_cnv.shape[0])*2*np.sqrt(Clustering_resolution))
+    gmm_N_comp = int(N_clusters/2)
+    if Clustering_algo != 'lv':
+        print('Clustering using %s with N_clusters = %i, %i. ' % (Clustering_algo.upper(), N_clusters, gmm_N_comp))
     
     ## Remove all zero X_cnv
     X_cnv_mean = np.array(X_cnv.sum(axis = 1))
     b = X_cnv_mean == 0
     if np.sum(b) > 0:
         # print(np.sum(b))
         odr = np.array(X_cnv_mean).argsort()
@@ -802,28 +863,28 @@
         df = pd.DataFrame(index = X_cnv.index.values)
     else:
         df = pd.DataFrame()
         X_cnv = pd.DataFrame(X_cnv)
     
     N_components_pca = 15
     # pca_obj = PCA(n_components = int(N_components_pca), copy = True, random_state = 0)
-    pca_obj = TruncatedSVD(n_components = int(N_components_pca)) # , algorithm = 'arpack')
+    pca_obj = TruncatedSVD(n_components = int(N_components_pca), random_state = 0) # , algorithm = 'arpack')
     
     if not pca: 
         X_pca = pca_obj.fit_transform(X_cnv)
         
         etime = round(time.time() - start_time) 
         print('P(%i) .. ' % etime, end = '', flush = True)
         start_time = time.time()           
     else: 
         X_pca = np.array(X_cnv.copy(deep = True)) #.copy(deep = True)
             
-    y_clust, cobj, adj = clustering_alg(X_pca, clust_algo = CLUSTERING_AGO, N_clusters = N_clusters, 
-                                   resolution = Clustering_resolution, N_neighbors = n_neighbors, 
-                                   n_cores = n_cores)
+    y_clust, cobj, adj = clustering_alg( X_pca, clust_algo = Clustering_algo, N_clusters = N_clusters, 
+                                         resolution = Clustering_resolution, N_neighbors = n_neighbors, 
+                                         mode = 'connectivity', n_cores = n_cores)
 
     if adj is None:
         adj = kneighbors_graph(X_pca, int(n_neighbors), mode = 'connectivity', 
                                include_self=True, n_jobs = n_cores)
     
     etime = round(time.time() - start_time) 
     print('C(%i) .. ' % etime, end = '', flush = True)
@@ -879,39 +940,48 @@
             adj_agg_mat[y_clust[r],y_clust[c]] += 1
 
     cluster_size = [] 
     for c in cnv_clust_lst:
         b = y_clust == c
         cluster_size.append(np.sum(b))
     
-    cluster_sel, cluster_odr, strength_odr = extend_major_clusters(adj_agg_mat, 
-                                               cluster_sel, cluster_size, 
-                                               alpha = cd_alpha, pv_cutoff = None)
+    cluster_sel, cluster_odr, pair_cluster, strength_odr, threshold_odr = \
+            extend_major_clusters(adj_agg_mat, cluster_sel, cluster_size, 
+                                  n_neighbors = n_neighbors, 
+                                  alpha = connectivity_thresh, pv_cutoff = None, 
+                                  mode = net_search_mode, verbose = verbose )
     
     b = y_clust == cluster_sel[0]
     if len(cluster_sel) > 1:
         for c in cluster_sel[1:]:
             b = b | (y_clust == c)
     ref_ind2 = b
     
-    print('N_ref: %i -> %i .. ' % \
-          (np.sum(ref_ind), np.sum(ref_ind2)), end = '')
+    etime = round(time.time() - start_time) 
+    print('NS(%i) N_ref: %i -> %i .. ' % \
+          (etime, np.sum(ref_ind), np.sum(ref_ind2)), end = '')
+    start_time = time.time()
 
+    y_conf = np.sqrt((X_cnv**2).mean(axis = 1))*100  
     #'''
     X_pca_sel = X_pca[ref_ind2,:]
     
     gmm = mixture.GaussianMixture(n_components = int(gmm_N_comp), random_state = 0)
     gmm.fit(X_pca_sel)
     y_conf_gmm = -gmm.score_samples(X_pca)
     #'''
-    y_conf = np.sqrt((X_cnv**2).mean(axis = 1))*100  
 
     # df[score_key] = y_conf*(1/(1+np.exp(-y_conf_gmm)))
     MIN_VAL = 1e-10
     df[score_key] = np.log((y_conf)*(1/(1+np.exp(-y_conf_gmm*gcm))) + MIN_VAL) 
+    df['y_conf'] = y_conf
+    df['tumor_prob'] = (1/(1+np.exp(-y_conf_gmm*gcm)))
+    df['tumor_dec'] = 'Normal'
+    b = df[score_key] > 0
+    df.loc[b, 'tumor_dec'] = 'Tumor'
     # df[score_key] = np.log(y_conf + 1e-10)
 
     '''
     yc = np.array(df[score_key])
     odr = yc.argsort()
     n1 = int(len(yc)*0.01)
     n2 = int(len(yc)*0.99)
@@ -923,39 +993,51 @@
     df.loc[b, score_key] = mnv
     #'''
     
     etime = round(time.time() - start_time) 
     print('G(%i) .. ' % etime, end = '', flush = True)
     start_time = time.time()
     
+    #'''
     dft, td_params = get_cnv_threshold_useref( df, ref_ind2, 
                                        score_key = score_key, cluster_key = cluster_key,
-                                       th_min = th_min, refp_min = refp_min, p_exc = p_exc, 
+                                       th_max = th_max, refp_min = refp_min, p_exc = p_exc, 
                                        ucr = dec_margin, plot_stat = plot_stat, 
                                        suffix = suffix, Data = Data )
+    #'''
     
     summary = {}
     summary['tumor_dec_params'] = td_params
     summary['adj_mat'] = adj
     summary['agg_adj_mat'] = adj_agg_mat
     # summary['cluster_sizes'] = cluster_size
     # summary['normal_clusters'] = cluster_sel
     # summary['cluster_selection_order'] = cluster_odr
     # summary['connection_strengths'] = strength_odr
-    summary['alpha_for_cluster_discovery'] = cd_alpha
+    summary['connectivity_threshold'] = connectivity_thresh
     
-    df_res = td_params['df']
+    td_params['df'].rename(columns = {'dec': 'tumor_dec'}, inplace = True)
+    df_res = td_params['df'].copy(deep = True)
+    # df_res = get_cluster_stat( df, ref_ind2, cluster_key = 'cnv_cluster', 
+    #                            score_key = 'tumor_score', refp_min = 0.9)
     # df_res['Normal'] = False
     # for c in cluster_sel: df_res.loc[c, 'Normal'] = True
     df_res['cluster_size'] = cluster_size
+    df_res['selected'] = 0
+    df_res.loc[cluster_sel, 'selected'] = 1
     df_res['selection_order'] = 0
-    for j, (c, v) in enumerate(zip(cluster_odr, strength_odr)): 
+    df_res['paired_cluster'] = 0
+    df_res['edge_wgt'] = 0
+    df_res['threshold'] = 0
+    for j, (c, p, v, u) in enumerate(zip(cluster_odr, pair_cluster, strength_odr, threshold_odr)): 
         df_res.loc[c, 'selection_order'] = j
+        df_res.loc[c, 'paired_cluster'] = p
         df_res.loc[c, 'edge_wgt'] = v
-    df_res.rename(columns = {'dec': 'tumor_dec'}, inplace = True)
+        df_res.loc[c, 'threshold'] = u
+    # df_res.rename(columns = {'dec': 'tumor_dec'}, inplace = True)
     df_res.drop(columns = 'b_inc', inplace = True)
     summary['cnv_cluster_info'] = df_res    
     
     etime = round(time.time() - start_time_a) 
     print('done (%i) ' % etime) #, end = '', flush = True)
     
     return df, summary, cobj, X_pca
```

### Comparing `scoda-tk-0.3.8/src/scoda/misc.py` & `scoda-tk-0.4.0/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.3.8/src/scoda/pipeline.py` & `scoda-tk-0.4.0/src/scoda/pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,45 +80,48 @@
     mkr_info['subset_to_minor_map'] = minor_dict
     adata.uns['Celltype_marker_DB'] = mkr_info
     
     return # adata
 
 
 def scoda_icnv_addon( adata_t, gtf_file, ref_types = None, 
-                      ref_key = "celltype_major", n_cores = 4,
-                      use_ref_only = False, cmd_cutoff = 0.03, 
-                      gcm = 0.05, tumor_dec_margin = 0.05, cd_alpha = 1 ):
+                      ref_key = "celltype_major", use_ref_only = False, 
+                      clustering_algo = 'lv', clustering_resolution = 1, 
+                      connectivity_thresh = 0.08, n_cores = 4, verbose = False,
+                      tumor_dec_margin = 0.05, tumor_dec_th_max = 0.1,  
+                      net_search_mode = 'max', cmd_cutoff = 0.03, gcm = 0.05 ):
     
     adata = adata_t[:,:]
 
     ref_types2 = ref_types
     ref_ind = None
 
     if ref_types is not None:
         if isinstance(ref_types, list):
             if len(ref_types) > 0:
                 ref_types2 = list(set(ref_types).intersection(adata.obs[ref_key].unique()))
                 ref_ind = adata.obs[ref_key].isin(ref_types)
     #'''
     adata = run_icnv(adata, ref_key, ref_types2, gtf_file, 
-                     resolution = 2, N_pca = 15, n_neighbors = 10,
+                     resolution = 1, N_pca = 15, n_neighbors = 15,
                      cluster_key = 'cnv_leiden', umap = False, pca = False,
                      n_cores = n_cores )
 
     #'''
     X_cnv = np.array(adata.obsm['X_cnv'].todense())
     pca = False
 
-    df_res, summary, cobj, X_pca = identify_tumor_cells(X_cnv, ref_ind, pca = pca, 
-                           use_cnv_score = False, clust = None, 
-                           Clustering_resolution = 1, N_clusters = 30,
-                           gmm_N_comp = 20, th_min = 0, refp_min = 0.9, p_exc = 0.1, 
+    df_res, summary, cobj, X_pca = identify_tumor_cells(X_cnv, ref_ind, pca = pca, clust = None, 
+                           use_cnv_score = False, Clustering_algo = clustering_algo, 
+                           Clustering_resolution = clustering_resolution, N_clusters = 30,
+                           gmm_N_comp = 20, th_max = tumor_dec_th_max, refp_min = 0.9, p_exc = 0.1, 
                            dec_margin = tumor_dec_margin, n_neighbors = 15, cmd_cutoff = cmd_cutoff, 
                            gcm = gcm, plot_stat = False, use_ref = use_ref_only, 
-                           cd_alpha = cd_alpha, suffix = '', Data = None, n_cores = n_cores)
+                           connectivity_thresh = connectivity_thresh, net_search_mode = net_search_mode,
+                           suffix = '', Data = None, n_cores = n_cores, verbose = verbose)
 
     if not pca: adata.obsm['X_cnv_pca'] = X_pca
         
     adata_t.obsm['X_cnv'] = adata.obsm['X_cnv']
     adata_t.obsm['X_cnv_pca'] = adata.obsm['X_cnv_pca']
     adata_t.uns['cnv'] = adata.uns['cnv']
 
@@ -143,16 +146,17 @@
     if ref_types is not None:
         b = b & (~adata_t.obs['celltype_major'].isin(ref_types))
     adata_t.obs.loc[b, 'celltype_minor_rev'] = 'Tumor cell'
     #'''
     return df_res
 
 
+
 def scoda_cci( adata_t, cpdb_path, cond_col = 'condition', sample_col = 'sample', 
-               cci_base = 'celltype_minor_rev', unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, 
+               cci_base = 'celltype_minor', unit_of_cci_run = 'sample', min_n_cells_for_cci = 40, 
                data_dir = '.', pval_max = 0.1, mean_min = 0, Rth = 0.5, n_cores = 4,
                print_prefix = ''):
     
     if cci_base in list(adata_t.obs.columns.values):
         celltype_col = cci_base
     else:
         celltype_col = 'celltype_minor'
@@ -484,21 +488,22 @@
         adata_t.uns['GSA_down'] = df_dct_dct_enr_dn
         adata_t.uns['GSEA'] = df_dct_dct_pr
     
     return
 
 
 def scoda_all_in_one( adata_t, mkr_db, cpdb_path, gsea_pw_db, cnv_gtf = None, 
-                      cond_col = 'condition', sample_col = 'sample', cci_deg_base = 'celltype_minor',
+                      cond_col = 'condition', sample_col = 'sample', 
                       cnv_ref_list = None, cnv_cmd_cutoff = 0.03, cnv_use_ref_only = False,
-                      cnv_gcm = 0.05, cnv_tdec_margin = 0.05, cnv_cd_alpha = 1, 
-                      cci_run_unit = 'sample', cci_n_cells_min = 40, 
+                      cnv_gcm = 0.05, cnv_tdec_margin = 0.05, cnv_connectivity_thresh = 0.08, 
+                      cnv_clustering_algo = 'lv', cnv_clustering_resolution = 1,
+                      cci_run_unit = 'sample', cci_n_cells_min = 40, cci_base = 'celltype_minor',
                       cci_pval_cutoff = 0.1, cci_mean_cutoff = 0, cci_rth = 0.5, 
                       deg_ref_group = None, deg_pval_cutoff = 0.01, deg_n_cells_min = 100, 
-                      gsea_pval_cutoff = 0.1, n_cores = 4, jump = 0,
+                      deg_base = 'celltype_minor', gsea_pval_cutoff = 0.1, n_cores = 4, jump_to = 0,
                       data_dir = '.', verbose = True, print_prefix = ''):
 
     df_mkr_db = mkr_db
     gtf_file = cnv_gtf 
     # cpdb_path = , 
     pw_db_for_gsea = gsea_pw_db 
     # cond_col = 'condition' 
@@ -515,15 +520,15 @@
     n_cores_to_use = n_cores 
     # data_dir = '.', 
     # verbose = True, 
     # prefix = ''
     
     ################################
     ### Cell-type identification ###
-    if jump < 1:
+    if jump_to < 1:
         if verbose: print('%sCelltype annotation running .. ' % print_prefix)
 
         scoda_hicat(adata_t, df_mkr_db, verbose = False)
 
         if verbose: print('%sCelltype annotation done.' % print_prefix)
 
         # adata_t.write(file_h5ad)
@@ -542,55 +547,59 @@
         if verbose: 
             print('%s  %i major type, %i minor type, %i subset identified.' 
                    % (print_prefix, len(ct_lst_maj), len(ct_lst_min), len(ct_lst_sub)))
             print('%s  Major types: %s' % (print_prefix, s))
         
     #################################
     ### tumor cell identification ###
-    if jump <= 1:
+    if jump_to <= 1:
         if cnv_gtf is not None:
 
             ## Test without Reference 
             if verbose: print('%sIdentifying tumor cells .. ' % print_prefix)
 
             ref_types = tumor_id_ref_celltypes
 
             df = scoda_icnv_addon( adata_t, gtf_file, ref_types = ref_types, 
-                                   ref_key = "celltype_major", n_cores = n_cores_to_use,
-                                   use_ref_only = False, cmd_cutoff = 0.03, gcm = 0.05, 
-                                   tumor_dec_margin = 0.01, cd_alpha = cnv_cd_alpha )
-
+                                   ref_key = "celltype_major", use_ref_only = False, 
+                                   clustering_algo = cnv_clustering_algo, 
+                                   clustering_resolution = cnv_clustering_resolution, 
+                                   connectivity_thresh = cnv_connectivity_thresh, 
+                                   n_cores = n_cores_to_use, verbose = False, 
+                                   tumor_dec_th_max = 0.1, tumor_dec_margin = 0.05, 
+                                   net_search_mode = 'max', cmd_cutoff = 0.03, gcm = 0.05 )
+            
             if verbose: print('%sTumor cells identification done. ' % print_prefix)
             # adata_t.write(file_h5ad)
            
     #############################
     ### Cell-cell interaction ###
-    if jump <= 2:
+    if jump_to <= 2:
         if verbose: print('%sInfering cell-cell interactions .. ' % print_prefix)
 
         scoda_cci( adata_t, cpdb_path, cond_col = cond_col, sample_col = sample_col, 
-                   cci_base = cci_deg_base, unit_of_cci_run = unit_of_cci_run, n_cores = n_cores_to_use, 
+                   cci_base = cci_base, unit_of_cci_run = unit_of_cci_run, n_cores = n_cores_to_use, 
                    min_n_cells_for_cci = min_n_cells_for_cci, Rth = Rth,
                    pval_max = cci_pval_max, mean_min = cci_mean_min, data_dir = data_dir)
 
         if verbose: print('%sInfering cell-cell interactions done. ' % print_prefix)    
         # adata_t.write(file_h5ad)
         
     ####################
     ### DEG analysis ###
     
-    if jump <= 3:
+    if jump_to <= 3:
         if verbose: print('%sDEG/GSEA analysis ..       ' % print_prefix)
         scoda_deg_gsea( adata_t, pw_db = pw_db_for_gsea, 
                         cond_col = cond_col, sample_col = sample_col, 
-                        deg_base = cci_deg_base, ref_group = deg_ref_group, 
+                        deg_base = deg_base, ref_group = deg_ref_group, 
                         deg_pval_cutoff = deg_pval_cutoff, 
                         gsea_pval_cutoff = gsea_pval_cutoff,
                         N_cells_min_per_sample = min_n_cells_for_deg, 
                         N_cells_min_per_condition = min_n_cells_for_deg, 
                         n_cores = n_cores_to_use, print_prefix = print_prefix)
 
         ## Overwrite 
         # adata_t.write(file_h5ad)        
         if verbose: print('%sDEG/GSEA analysis done.       ' % print_prefix)
         
-    return
+    return
```

### Comparing `scoda-tk-0.3.8/src/scoda/viz.py` & `scoda-tk-0.4.0/src/scoda/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -1765,49 +1765,49 @@
 
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 
 def plot_gsea_all( df_qv, df_es, title = 'Test', title_fs = 14, 
                    tick_fs = 10, tick_rot = 90, tick_ha = 'center',
                    label_fs = 10, legend_fs = 10, fig_size_sf = 1,
-                   mx_pnt_size = 80, swap_ax = True ):
+                   dot_size = 14, mx_pnt_size = 80, swap_ax = True ):
                  
     df1 = df_qv
     df2 = df_es
     alabel = 'Cases'
     n = df1.shape[0]
 
-    fig_size_sf = fig_size_sf*3
-    mx_pnt_size = 20*fig_size_sf
+    mx_pnt_size = dot_size
+    mx_pv = np.ceil(df1.max().max())
+    ssf = mx_pnt_size/mx_pv
     
     mn, mx = 0, 1
     if df2 is not None:
         mn, mx = np.floor(df2.min().min()), np.ceil(df2.max().max())
         cbar_title = 'NES'
     else:
         mn, mx = np.floor(df1.min().min()), np.ceil(df1.max().max())
         cbar_title = '-log10(P)'
-
-    mx_pv = np.ceil(df1.max().max())
-    ssf = mx_pnt_size/mx_pv
         
+    norm = mpl.colors.Normalize(vmin=mn, vmax=mx)
+
     # plt.figure(figsize = (2+1, 2*df1.shape[0]/df1.shape[1]))
 
     if swap_ax:
-        sf = fig_size_sf/df1.shape[1]
-        xs = (df1.shape[0] + 6)
+        fig_size = fig_size_sf*df1.shape[1]/6
+        sf = fig_size/df1.shape[1]
+        xs = (df1.shape[0]) 
         ys = df1.shape[1]
         fig, ax = plt.subplots(figsize = (sf*xs, sf*ys)) 
     else:
-        sf = fig_size_sf/df1.shape[1]
+        fig_size = fig_size_sf*df1.shape[1]/6
+        sf = fig_size/df1.shape[1]
         xs = df1.shape[1]
-        ys = (df1.shape[0] + 6)
-        fig, ax = plt.subplots(figsize = (sf*df1.shape[1], sf*(df1.shape[0] + 6))) 
-
-    norm = mpl.colors.Normalize(vmin=mn, vmax=mx)
+        ys = (df1.shape[0]) 
+        fig, ax = plt.subplots(figsize = (sf*xs, sf*ys)) 
 
     x = []
     y = []
     ss = []
     cc = []
     for j, c in enumerate(list(df1.columns.values)):
         if swap_ax:
@@ -1852,21 +1852,21 @@
     y_ticks_labels = list(yt_label)
     a = ax.set_yticklabels(y_ticks_labels, rotation=0, fontsize=tick_fs)
 
     # Adding the colorbar
     cmap = p.cmap
     if swap_ax:
         lgap = 0.01
-        frac = 0.08
+        frac = 0.05
         # cbaxes = fig.add_axes([0.91, 0.6, 0.1*df1.shape[1]/df1.shape[0], 0.25]) 
         cbar = plt.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap),ax=ax, 
                         fraction = frac, location = 'top', anchor = (1,1)) #, cax = cbaxes)
     else:
         lgap = 0.02 # 0.005
-        frac = 0.08
+        frac = 0.05
         r = df1.shape[1]/df1.shape[0]
         # cbaxes = fig.add_axes([1, 1, 0.1*(1-df1.shape[1]/30), 0.1]) 
         cbar = plt.colorbar(mpl.cm.ScalarMappable(norm=norm, cmap=cmap),ax=ax, 
                         fraction = frac, location = 'right', anchor = (0,0)) #, cax = cbaxes)
         
     # if df2 is not None:
     cbar.set_label(cbar_title, fontsize = label_fs)
```

### Comparing `scoda-tk-0.3.8/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.4.0/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.3.8
+Version: 0.4.0
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.3.8/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.4.0/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

