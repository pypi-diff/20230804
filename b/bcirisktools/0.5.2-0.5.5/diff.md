# Comparing `tmp/bcirisktools-0.5.2.tar.gz` & `tmp/bcirisktools-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcirisktools-0.5.2.tar", last modified: Thu Aug  3 15:57:43 2023, max compression
+gzip compressed data, was "bcirisktools-0.5.5.tar", last modified: Fri Aug  4 11:41:33 2023, max compression
```

## Comparing `bcirisktools-0.5.2.tar` & `bcirisktools-0.5.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-03 15:57:43.462000 bcirisktools-0.5.2/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-07-27 13:56:43.000000 bcirisktools-0.5.2/LICENCE
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-03 15:57:43.456000 bcirisktools-0.5.2/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-07-27 13:56:43.000000 bcirisktools-0.5.2/README.md
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-03 15:57:43.337000 bcirisktools-0.5.2/bcirisktools/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      385 2023-08-02 19:08:07.000000 bcirisktools-0.5.2/bcirisktools/__init__.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-07-27 13:56:43.000000 bcirisktools-0.5.2/bcirisktools/input_filters.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-07-27 13:56:43.000000 bcirisktools-0.5.2/bcirisktools/metrics_bci.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-07-27 13:56:43.000000 bcirisktools-0.5.2/bcirisktools/modeling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    16951 2023-08-02 19:27:19.000000 bcirisktools-0.5.2/bcirisktools/profiling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-07-27 13:56:43.000000 bcirisktools-0.5.2/bcirisktools/shapley_report.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-07-27 13:56:43.000000 bcirisktools-0.5.2/bcirisktools/stability.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-07-27 13:56:43.000000 bcirisktools-0.5.2/bcirisktools/tree_crt.py
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-03 15:57:43.438000 bcirisktools-0.5.2/bcirisktools.egg-info/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-03 15:57:42.000000 bcirisktools-0.5.2/bcirisktools.egg-info/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-03 15:57:42.000000 bcirisktools-0.5.2/bcirisktools.egg-info/SOURCES.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-03 15:57:42.000000 bcirisktools-0.5.2/bcirisktools.egg-info/dependency_links.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       63 2023-08-03 15:57:42.000000 bcirisktools-0.5.2/bcirisktools.egg-info/requires.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-03 15:57:42.000000 bcirisktools-0.5.2/bcirisktools.egg-info/top_level.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-07-27 13:56:43.000000 bcirisktools-0.5.2/pyproject.toml
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-03 15:57:43.465000 bcirisktools-0.5.2/setup.cfg
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1019 2023-08-03 15:57:22.000000 bcirisktools-0.5.2/setup.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 11:41:33.812000 bcirisktools-0.5.5/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/LICENCE
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-04 11:41:33.806000 bcirisktools-0.5.5/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/README.md
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 11:41:33.696000 bcirisktools-0.5.5/bcirisktools/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      385 2023-08-03 23:14:09.000000 bcirisktools-0.5.5/bcirisktools/__init__.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/input_filters.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/metrics_bci.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/modeling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    18643 2023-08-04 11:39:21.000000 bcirisktools-0.5.5/bcirisktools/profiling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/shapley_report.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/stability.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/bcirisktools/tree_crt.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 11:41:33.786000 bcirisktools-0.5.5/bcirisktools.egg-info/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-04 11:41:33.000000 bcirisktools-0.5.5/bcirisktools.egg-info/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-04 11:41:33.000000 bcirisktools-0.5.5/bcirisktools.egg-info/SOURCES.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-04 11:41:33.000000 bcirisktools-0.5.5/bcirisktools.egg-info/dependency_links.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       63 2023-08-04 11:41:33.000000 bcirisktools-0.5.5/bcirisktools.egg-info/requires.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-04 11:41:33.000000 bcirisktools-0.5.5/bcirisktools.egg-info/top_level.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-07-27 13:56:43.000000 bcirisktools-0.5.5/pyproject.toml
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-04 11:41:33.815000 bcirisktools-0.5.5/setup.cfg
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1019 2023-08-04 11:39:25.000000 bcirisktools-0.5.5/setup.py
```

### Comparing `bcirisktools-0.5.2/LICENCE` & `bcirisktools-0.5.5/LICENCE`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.2/PKG-INFO` & `bcirisktools-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.5.2
+Version: 0.5.5
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.5.2/README.md` & `bcirisktools-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.2/bcirisktools/input_filters.py` & `bcirisktools-0.5.5/bcirisktools/input_filters.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.2/bcirisktools/metrics_bci.py` & `bcirisktools-0.5.5/bcirisktools/metrics_bci.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.2/bcirisktools/modeling.py` & `bcirisktools-0.5.5/bcirisktools/modeling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.2/bcirisktools/profiling.py` & `bcirisktools-0.5.5/bcirisktools/profiling.py`

 * *Files 3% similar despite different names*

```diff
@@ -430,36 +430,74 @@
     figs["steps_badrate"] = plot_steps(df_output_steps, "decile_rank", "BadRate %")
     # plot population steps
     figs["steps_population"] = plot_steps(df_output_steps, "decile_rank", "count")
 
     return df_summary, intervals_list, figs
 
 
-def refillProfiles(target, scores, expected_br):
-    # TODO: ADD exploitation to the searching loop
-    # TODO: PLOTS
+def refillProfiles_2(target, scores, expected_br, n_exploitation=100):
+    # TODO: ADD exploitation to the searching loop (testing in the version 2)
+    # TODO: Optimize the code, use pandas's paralellism to improve the execution time
+    # TODO: Fix in pipy the code.
     expected_br.append(100)
 
     # Prepare the data to sort the data
     df_pred = pd.DataFrame(columns=["yhat", "target"])
     df_pred["yhat"] = scores
     df_pred["target"] = target
     df_pred = df_pred.sort_values(["yhat", "target"], ascending=True).reset_index(
         drop=True
     )
 
     # Generate variables to search the badrate
     df_temp = pd.DataFrame(columns=["yhat", "target"])
-    br_idx = 0
+    br_idx, idx = 0, 0
     br_output = pd.DataFrame(columns=["decile_rank", "BadRate %", "count"])
-    for idx, row in df_pred.iterrows():
-        df_temp = pd.concat([df_temp, pd.DataFrame(row).T], axis=0)
+    # Don't try this loop at home please, put a True is a really bad practice
+    while True:
+        # comprobate if the len
+        if br_idx > len(expected_br) or idx == df_pred.shape[0]:
+            break
+
+        # Generate de dataframe to compare the badrate
+        df_temp = pd.concat([df_temp, pd.DataFrame(df_pred.iloc[idx, :]).T], axis=0)
         crr_br = df_temp["target"].mean() * 100
-        # If the current badrate is bigger than the expected badrate
-        if crr_br >= expected_br[br_idx]:
+
+        # If the current badrate is bigger than the expected badrate enter here
+        if crr_br >= expected_br[br_idx] and crr_br < 100 and crr_br > 0:
+            # Exploitation over N values
+            # The idea here is explore more option, sometimes we have a fake high rate and
+            # we need to see beyond.
+            df_exploit = df_temp.copy()
+            exploited = False
+            for it_exploit in range(1, n_exploitation):
+                if idx + it_exploit <= df_pred.shape[0]:
+                    df_exploit = pd.concat(
+                        [df_exploit, pd.DataFrame(df_pred.iloc[idx + it_exploit, :]).T],
+                        axis=0,
+                    )
+                    crr_br_exploit = df_exploit["target"].mean() * 100
+                    if (
+                        crr_br_exploit < crr_br
+                        and crr_br_exploit >= expected_br[br_idx]
+                        and crr_br < 100
+                        and crr_br > 0
+                    ):
+                        df_temp = df_exploit.copy()
+                        idx = idx + it_exploit
+                        exploited = True
+                        break
+                else:
+                    break
+
+            if exploited:
+                continue
+
+            # If we can't find a good fit, we choose the previous value
+            # so we prepare this info
             df_temp_2 = df_temp.iloc[:-1, :]
             save_br = df_temp_2["target"].mean() * 100
             n_pop = df_temp_2["target"].count()
             br_idx += 1
             # If the badrate is more than zero, we save the value in the dict
             if save_br > 0:
                 df = pd.DataFrame(
@@ -467,27 +505,30 @@
                         "decile_rank": df_temp["yhat"].max(),
                         "BadRate %": crr_br,
                         "count": n_pop,
                     },
                     index=[0],
                 )
                 br_output = pd.concat([br_output, df], axis=0)
-            # Else, choose the previous value
+            # Else, choose
             else:
                 n_pop = df_temp["target"].count()
                 df = pd.DataFrame(
                     {
                         "decile_rank": df_temp["yhat"].max(),
                         "BadRate %": crr_br,
                         "count": n_pop,
                     },
                     index=[0],
                 )
                 br_output = pd.concat([br_output, df], axis=0)
             df_temp = pd.DataFrame(columns=["yhat", "target"])
+        # loop
+        idx += 1
+
     br_output["KO"] = False
     # Add the KO profile to the output
     n_pop = df_temp["target"].count()
     df = pd.DataFrame(
         {
             "decile_rank": df_temp["yhat"].max(),
             "BadRate %": crr_br,
```

### Comparing `bcirisktools-0.5.2/bcirisktools/shapley_report.py` & `bcirisktools-0.5.5/bcirisktools/shapley_report.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.2/bcirisktools/stability.py` & `bcirisktools-0.5.5/bcirisktools/stability.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.2/bcirisktools/tree_crt.py` & `bcirisktools-0.5.5/bcirisktools/tree_crt.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.2/bcirisktools.egg-info/PKG-INFO` & `bcirisktools-0.5.5/bcirisktools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.5.2
+Version: 0.5.5
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.5.2/setup.py` & `bcirisktools-0.5.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.5.2"
+VERSION = "0.5.5"
 DESCRIPTION = "BCI risks tools"
 LONG_DESCRIPTION = "A package that compiles different risk tools used by BCI bank."
 
 # Setting up
 setup(
     name="bcirisktools",
     version=VERSION,
```

