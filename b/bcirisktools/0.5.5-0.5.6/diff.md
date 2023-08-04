# Comparing `tmp/bcirisktools-0.5.5.tar.gz` & `tmp/bcirisktools-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcirisktools-0.5.5.tar", last modified: Fri Aug  4 11:41:33 2023, max compression
+gzip compressed data, was "bcirisktools-0.5.6.tar", last modified: Fri Aug  4 11:50:24 2023, max compression
```

## Comparing `bcirisktools-0.5.5.tar` & `bcirisktools-0.5.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 11:41:33.812000 bcirisktools-0.5.5/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/LICENCE
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-04 11:41:33.806000 bcirisktools-0.5.5/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/README.md
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 11:41:33.696000 bcirisktools-0.5.5/bcirisktools/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      385 2023-08-03 23:14:09.000000 bcirisktools-0.5.5/bcirisktools/__init__.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/input_filters.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/metrics_bci.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/modeling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    18643 2023-08-04 11:39:21.000000 bcirisktools-0.5.5/bcirisktools/profiling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/shapley_report.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/stability.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/tree_crt.py
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 11:41:33.786000 bcirisktools-0.5.5/bcirisktools.egg-info/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-04 11:41:33.000000 bcirisktools-0.5.5/bcirisktools.egg-info/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-04 11:41:33.000000 bcirisktools-0.5.5/bcirisktools.egg-info/SOURCES.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-04 11:41:33.000000 bcirisktools-0.5.5/bcirisktools.egg-info/dependency_links.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       63 2023-08-04 11:41:33.000000 bcirisktools-0.5.5/bcirisktools.egg-info/requires.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-04 11:41:33.000000 bcirisktools-0.5.5/bcirisktools.egg-info/top_level.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/pyproject.toml
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-04 11:41:33.815000 bcirisktools-0.5.5/setup.cfg
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1019 2023-08-04 11:39:25.000000 bcirisktools-0.5.5/setup.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 11:50:24.658000 bcirisktools-0.5.6/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-07-27 13:56:43.000000 bcirisktools-0.5.6/LICENCE
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-04 11:50:24.651000 bcirisktools-0.5.6/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-07-27 13:56:43.000000 bcirisktools-0.5.6/README.md
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 11:50:24.552000 bcirisktools-0.5.6/bcirisktools/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      385 2023-08-03 23:14:09.000000 bcirisktools-0.5.6/bcirisktools/__init__.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-07-27 13:56:43.000000 bcirisktools-0.5.6/bcirisktools/input_filters.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-07-27 13:56:43.000000 bcirisktools-0.5.6/bcirisktools/metrics_bci.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-07-27 13:56:43.000000 bcirisktools-0.5.6/bcirisktools/modeling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    18528 2023-08-04 11:49:38.000000 bcirisktools-0.5.6/bcirisktools/profiling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-07-27 13:56:43.000000 bcirisktools-0.5.6/bcirisktools/shapley_report.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-07-27 13:56:43.000000 bcirisktools-0.5.6/bcirisktools/stability.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-07-27 13:56:43.000000 bcirisktools-0.5.6/bcirisktools/tree_crt.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 11:50:24.634000 bcirisktools-0.5.6/bcirisktools.egg-info/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-04 11:50:24.000000 bcirisktools-0.5.6/bcirisktools.egg-info/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-04 11:50:24.000000 bcirisktools-0.5.6/bcirisktools.egg-info/SOURCES.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-04 11:50:24.000000 bcirisktools-0.5.6/bcirisktools.egg-info/dependency_links.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       63 2023-08-04 11:50:24.000000 bcirisktools-0.5.6/bcirisktools.egg-info/requires.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-04 11:50:24.000000 bcirisktools-0.5.6/bcirisktools.egg-info/top_level.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-07-27 13:56:43.000000 bcirisktools-0.5.6/pyproject.toml
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-04 11:50:24.661000 bcirisktools-0.5.6/setup.cfg
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1019 2023-08-04 11:50:17.000000 bcirisktools-0.5.6/setup.py
```

### Comparing `bcirisktools-0.5.5/LICENCE` & `bcirisktools-0.5.6/LICENCE`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.5/PKG-INFO` & `bcirisktools-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.5.5
+Version: 0.5.6
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.5.5/README.md` & `bcirisktools-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.5/bcirisktools/input_filters.py` & `bcirisktools-0.5.6/bcirisktools/input_filters.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.5/bcirisktools/metrics_bci.py` & `bcirisktools-0.5.6/bcirisktools/metrics_bci.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.5/bcirisktools/modeling.py` & `bcirisktools-0.5.6/bcirisktools/modeling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.5/bcirisktools/profiling.py` & `bcirisktools-0.5.6/bcirisktools/profiling.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,15 +391,14 @@
                 df_modify, df_summary = concat_intervals(
                     df_modify, idx, idx + 1, model_target
                 )
                 df_summary = sortIntervals(df_summary)
 
     #############################################################################################
     # Concatenate KO profiles
-
     intervals_list = [-0.01]
     for row in df_summary.iloc[1:, :].iterrows():
         if KO > row[1]["BadRate %"]:
             intervals_list.append(row[1]["decile_rank"].left)
         else:
             intervals_list.append(row[1]["decile_rank"].left)
             break
@@ -430,18 +429,16 @@
     figs["steps_badrate"] = plot_steps(df_output_steps, "decile_rank", "BadRate %")
     # plot population steps
     figs["steps_population"] = plot_steps(df_output_steps, "decile_rank", "count")
 
     return df_summary, intervals_list, figs
 
 
-def refillProfiles_2(target, scores, expected_br, n_exploitation=100):
-    # TODO: ADD exploitation to the searching loop (testing in the version 2)
+def refillProfiles(target, scores, expected_br, n_exploitation=100):
     # TODO: Optimize the code, use pandas's paralellism to improve the execution time
-    # TODO: Fix in pipy the code.
     expected_br.append(100)
 
     # Prepare the data to sort the data
     df_pred = pd.DataFrame(columns=["yhat", "target"])
     df_pred["yhat"] = scores
     df_pred["target"] = target
     df_pred = df_pred.sort_values(["yhat", "target"], ascending=True).reset_index(
```

### Comparing `bcirisktools-0.5.5/bcirisktools/shapley_report.py` & `bcirisktools-0.5.6/bcirisktools/shapley_report.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.5/bcirisktools/stability.py` & `bcirisktools-0.5.6/bcirisktools/stability.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.5/bcirisktools/tree_crt.py` & `bcirisktools-0.5.6/bcirisktools/tree_crt.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.5/bcirisktools.egg-info/PKG-INFO` & `bcirisktools-0.5.6/bcirisktools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.5.5
+Version: 0.5.6
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.5.5/setup.py` & `bcirisktools-0.5.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.5.5"
+VERSION = "0.5.6"
 DESCRIPTION = "BCI risks tools"
 LONG_DESCRIPTION = "A package that compiles different risk tools used by BCI bank."
 
 # Setting up
 setup(
     name="bcirisktools",
     version=VERSION,
```

