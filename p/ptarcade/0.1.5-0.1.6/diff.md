# Comparing `tmp/ptarcade-0.1.5.tar.gz` & `tmp/ptarcade-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptarcade-0.1.5.tar", max compression
+gzip compressed data, was "ptarcade-0.1.6.tar", max compression
```

## Comparing `ptarcade-0.1.5.tar` & `ptarcade-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-07-26 03:41:09.403224 ptarcade-0.1.5/LICENSE
--rw-r--r--   0        0        0      673 2023-07-26 03:41:09.403224 ptarcade-0.1.5/README.md
--rw-r--r--   0        0        0     3314 2023-07-26 03:41:09.435224 ptarcade-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      555 2023-07-26 03:41:09.435224 ptarcade-0.1.5/src/ptarcade/__init__.py
--rw-r--r--   0        0        0    32466 2023-07-26 03:41:09.435224 ptarcade-0.1.5/src/ptarcade/chains_utils.py
--rw-r--r--   0        0        0       23 2023-07-26 03:41:09.435224 ptarcade-0.1.5/src/ptarcade/data/__init__.py
--rw-r--r--   0        0        0     1026 2023-07-26 03:41:09.435224 ptarcade-0.1.5/src/ptarcade/data/default_config.py
--rw-r--r--   0        0        0    29964 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/data/g_star.dat
--rw-r--r--   0        0        0     4994 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/fast_interpolate.py
--rw-r--r--   0        0        0    15036 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/input_handler.py
--rw-r--r--   0        0        0    17354 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/models_utils.py
--rw-r--r--   0        0        0    30151 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/plot_utils.py
--rw-r--r--   0        0        0     6885 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/pta_importer.py
--rw-r--r--   0        0        0    12031 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/sampler.py
--rw-r--r--   0        0        0    18088 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/signal_builder.py
--rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 ptarcade-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-08-04 05:26:53.062848 ptarcade-0.1.6/LICENSE
+-rw-r--r--   0        0        0      673 2023-08-04 05:26:53.062848 ptarcade-0.1.6/README.md
+-rw-r--r--   0        0        0     3314 2023-08-04 05:26:53.090848 ptarcade-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-08-04 05:26:53.090848 ptarcade-0.1.6/src/ptarcade/__init__.py
+-rw-r--r--   0        0        0    32466 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/chains_utils.py
+-rw-r--r--   0        0        0       23 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/data/__init__.py
+-rw-r--r--   0        0        0     1026 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/data/default_config.py
+-rw-r--r--   0        0        0    29964 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/data/g_star.dat
+-rw-r--r--   0        0        0     4994 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/fast_interpolate.py
+-rw-r--r--   0        0        0    15036 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/input_handler.py
+-rw-r--r--   0        0        0    17354 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/models_utils.py
+-rw-r--r--   0        0        0    30178 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/plot_utils.py
+-rw-r--r--   0        0        0     6885 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/pta_importer.py
+-rw-r--r--   0        0        0    12031 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/sampler.py
+-rw-r--r--   0        0        0    18088 2023-08-04 05:26:53.094848 ptarcade-0.1.6/src/ptarcade/signal_builder.py
+-rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 ptarcade-0.1.6/PKG-INFO
```

### Comparing `ptarcade-0.1.5/LICENSE` & `ptarcade-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/README.md` & `ptarcade-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/pyproject.toml` & `ptarcade-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
   "doc/build/*.py",
   "doc/temp/*.py",
   ".eggs/*.py",
 ]
 
 [tool.poetry]
 name = "PTArcade"
-version = "0.1.5"
+version = "0.1.6"
 description = "PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data."
 readme = "README.md"
 authors = ["Andrea Mitridate <andrea.mitridate@nanograv.org>",]
 keywords = ["ptarcade"]
 repository = "https://github.com/andrea-mitridate/PTArcade"
 documentation = "https://andrea-mitridate.github.io/PTArcade/"
 classifiers = [
```

### Comparing `ptarcade-0.1.5/src/ptarcade/__init__.py` & `ptarcade-0.1.6/src/ptarcade/__init__.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/src/ptarcade/chains_utils.py` & `ptarcade-0.1.6/src/ptarcade/chains_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/src/ptarcade/data/default_config.py` & `ptarcade-0.1.6/src/ptarcade/data/default_config.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/src/ptarcade/data/g_star.dat` & `ptarcade-0.1.6/src/ptarcade/data/g_star.dat`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/src/ptarcade/fast_interpolate.py` & `ptarcade-0.1.6/src/ptarcade/fast_interpolate.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/src/ptarcade/input_handler.py` & `ptarcade-0.1.6/src/ptarcade/input_handler.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/src/ptarcade/models_utils.py` & `ptarcade-0.1.6/src/ptarcade/models_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/src/ptarcade/plot_utils.py` & `ptarcade-0.1.6/src/ptarcade/plot_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -847,15 +847,15 @@
     for idx, chain in enumerate(chains):
         filtered = utils.chain_filter(
             chain, params[idx], model_id[idx], par_to_plot[idx]
         )
         filtered_priors = {
             k.replace("_", "-"): v
             for k, v in priors[idx].items()
-            if k.replace("_", "-") in filtered[1] and v is not None
+            if k.replace("_", "-") in filtered[1] and (v is not None or not np.isnan(v).any())
         }
 
         samples.append(
             MCSamples(
                 samples=filtered[0],
                 names=filtered[1],
                 ranges=filtered_priors,
```

### Comparing `ptarcade-0.1.5/src/ptarcade/pta_importer.py` & `ptarcade-0.1.6/src/ptarcade/pta_importer.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/src/ptarcade/sampler.py` & `ptarcade-0.1.6/src/ptarcade/sampler.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/src/ptarcade/signal_builder.py` & `ptarcade-0.1.6/src/ptarcade/signal_builder.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.5/PKG-INFO` & `ptarcade-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptarcade
-Version: 0.1.5
+Version: 0.1.6
 Summary: PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data.
 Home-page: https://github.com/andrea-mitridate/PTArcade
 Keywords: ptarcade
 Author: Andrea Mitridate
 Author-email: andrea.mitridate@nanograv.org
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Developers
```

