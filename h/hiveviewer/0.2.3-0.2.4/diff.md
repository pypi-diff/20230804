# Comparing `tmp/hiveviewer-0.2.3.tar.gz` & `tmp/hiveviewer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiveviewer-0.2.3.tar", last modified: Thu Aug  3 06:11:20 2023, max compression
+gzip compressed data, was "hiveviewer-0.2.4.tar", last modified: Fri Aug  4 07:05:20 2023, max compression
```

## Comparing `hiveviewer-0.2.3.tar` & `hiveviewer-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.852433 hiveviewer-0.2.3/
--rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.2.3/LICENSE
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-03 06:11:20.852279 hiveviewer-0.2.3/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.2.3/README.md
--rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.2.3/pyproject.toml
--rw-r--r--   0 yin        (501) staff       (20)       38 2023-08-03 06:11:20.852491 hiveviewer-0.2.3/setup.cfg
--rw-r--r--   0 yin        (501) staff       (20)     1006 2023-08-03 06:10:45.000000 hiveviewer-0.2.3/setup.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.845913 hiveviewer-0.2.3/src/
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.847546 hiveviewer-0.2.3/src/hiveviewer/
--rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.2.3/src/hiveviewer/__init__.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.849123 hiveviewer-0.2.3/src/hiveviewer/dataloader/
--rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.2.3/src/hiveviewer/dataloader/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     3200 2023-08-03 06:08:44.000000 hiveviewer-0.2.3/src/hiveviewer/dataloader/base.py
--rw-r--r--   0 yin        (501) staff       (20)      885 2023-08-03 06:08:42.000000 hiveviewer-0.2.3/src/hiveviewer/dataloader/load_csv.py
--rw-r--r--   0 yin        (501) staff       (20)      862 2023-08-03 06:10:38.000000 hiveviewer-0.2.3/src/hiveviewer/dataloader/load_excel.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.849526 hiveviewer-0.2.3/src/hiveviewer/evaluation/
--rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.2.3/src/hiveviewer/evaluation/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     7362 2023-08-02 08:49:24.000000 hiveviewer-0.2.3/src/hiveviewer/evaluation/calculator.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.850110 hiveviewer-0.2.3/src/hiveviewer/optimization/
--rw-r--r--   0 yin        (501) staff       (20)      128 2023-08-01 02:03:43.000000 hiveviewer-0.2.3/src/hiveviewer/optimization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)      770 2023-08-02 03:43:12.000000 hiveviewer-0.2.3/src/hiveviewer/optimization/base.py
--rw-r--r--   0 yin        (501) staff       (20)     6582 2023-08-03 06:07:28.000000 hiveviewer-0.2.3/src/hiveviewer/optimization/multiple_objective.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.851050 hiveviewer-0.2.3/src/hiveviewer/sampling/
--rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.2.3/src/hiveviewer/sampling/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.2.3/src/hiveviewer/sampling/base.py
--rw-r--r--   0 yin        (501) staff       (20)     1394 2023-07-31 03:32:57.000000 hiveviewer-0.2.3/src/hiveviewer/sampling/frequency_sampler.py
--rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.2.3/src/hiveviewer/sampling/gini_sampler.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.852057 hiveviewer-0.2.3/src/hiveviewer/visualization/
--rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/__init__.py
--rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/lorenz_curve.py
--rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/plot_trisurf.py
--rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/venn2.py
--rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/venn3.py
--rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.2.3/src/hiveviewer/visualization/venn_base.py
-drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-03 06:11:20.848412 hiveviewer-0.2.3/src/hiveviewer.egg-info/
--rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-03 06:11:20.000000 hiveviewer-0.2.3/src/hiveviewer.egg-info/PKG-INFO
--rw-r--r--   0 yin        (501) staff       (20)     1013 2023-08-03 06:11:20.000000 hiveviewer-0.2.3/src/hiveviewer.egg-info/SOURCES.txt
--rw-r--r--   0 yin        (501) staff       (20)        1 2023-08-03 06:11:20.000000 hiveviewer-0.2.3/src/hiveviewer.egg-info/dependency_links.txt
--rw-r--r--   0 yin        (501) staff       (20)       82 2023-08-03 06:11:20.000000 hiveviewer-0.2.3/src/hiveviewer.egg-info/requires.txt
--rw-r--r--   0 yin        (501) staff       (20)       11 2023-08-03 06:11:20.000000 hiveviewer-0.2.3/src/hiveviewer.egg-info/top_level.txt
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.525215 hiveviewer-0.2.4/
+-rw-r--r--   0 yin        (501) staff       (20)     1066 2023-07-19 11:32:11.000000 hiveviewer-0.2.4/LICENSE
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-04 07:05:20.525065 hiveviewer-0.2.4/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)      735 2023-06-14 07:48:21.000000 hiveviewer-0.2.4/README.md
+-rw-r--r--   0 yin        (501) staff       (20)      327 2023-05-23 07:07:17.000000 hiveviewer-0.2.4/pyproject.toml
+-rw-r--r--   0 yin        (501) staff       (20)       38 2023-08-04 07:05:20.525260 hiveviewer-0.2.4/setup.cfg
+-rw-r--r--   0 yin        (501) staff       (20)     1006 2023-08-04 07:04:54.000000 hiveviewer-0.2.4/setup.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.518757 hiveviewer-0.2.4/src/
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.520251 hiveviewer-0.2.4/src/hiveviewer/
+-rw-r--r--   0 yin        (501) staff       (20)      133 2023-07-19 11:32:15.000000 hiveviewer-0.2.4/src/hiveviewer/__init__.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.521965 hiveviewer-0.2.4/src/hiveviewer/dataloader/
+-rw-r--r--   0 yin        (501) staff       (20)      159 2023-07-21 02:45:47.000000 hiveviewer-0.2.4/src/hiveviewer/dataloader/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     3200 2023-08-04 06:20:30.000000 hiveviewer-0.2.4/src/hiveviewer/dataloader/base.py
+-rw-r--r--   0 yin        (501) staff       (20)      885 2023-08-03 06:08:42.000000 hiveviewer-0.2.4/src/hiveviewer/dataloader/load_csv.py
+-rw-r--r--   0 yin        (501) staff       (20)      862 2023-08-03 06:10:38.000000 hiveviewer-0.2.4/src/hiveviewer/dataloader/load_excel.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.522414 hiveviewer-0.2.4/src/hiveviewer/evaluation/
+-rw-r--r--   0 yin        (501) staff       (20)       61 2023-07-26 06:20:36.000000 hiveviewer-0.2.4/src/hiveviewer/evaluation/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     7803 2023-08-04 07:04:12.000000 hiveviewer-0.2.4/src/hiveviewer/evaluation/calculator.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.523051 hiveviewer-0.2.4/src/hiveviewer/optimization/
+-rw-r--r--   0 yin        (501) staff       (20)      128 2023-08-01 02:03:43.000000 hiveviewer-0.2.4/src/hiveviewer/optimization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)      770 2023-08-02 03:43:12.000000 hiveviewer-0.2.4/src/hiveviewer/optimization/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     6703 2023-08-04 03:40:54.000000 hiveviewer-0.2.4/src/hiveviewer/optimization/multiple_objective.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.523797 hiveviewer-0.2.4/src/hiveviewer/sampling/
+-rw-r--r--   0 yin        (501) staff       (20)      174 2023-07-31 02:06:26.000000 hiveviewer-0.2.4/src/hiveviewer/sampling/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     1068 2023-07-31 03:32:36.000000 hiveviewer-0.2.4/src/hiveviewer/sampling/base.py
+-rw-r--r--   0 yin        (501) staff       (20)     1394 2023-08-04 06:40:00.000000 hiveviewer-0.2.4/src/hiveviewer/sampling/frequency_sampler.py
+-rw-r--r--   0 yin        (501) staff       (20)     2510 2023-07-30 03:20:30.000000 hiveviewer-0.2.4/src/hiveviewer/sampling/gini_sampler.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.524812 hiveviewer-0.2.4/src/hiveviewer/visualization/
+-rw-r--r--   0 yin        (501) staff       (20)      301 2023-06-08 08:44:36.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/__init__.py
+-rw-r--r--   0 yin        (501) staff       (20)     8779 2023-07-21 04:14:30.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/lorenz_curve.py
+-rw-r--r--   0 yin        (501) staff       (20)     3371 2023-06-07 12:51:20.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/plot_trisurf.py
+-rw-r--r--   0 yin        (501) staff       (20)     3929 2023-07-21 04:04:42.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/venn2.py
+-rw-r--r--   0 yin        (501) staff       (20)     6601 2023-07-21 03:59:13.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/venn3.py
+-rw-r--r--   0 yin        (501) staff       (20)     2758 2023-06-08 08:44:36.000000 hiveviewer-0.2.4/src/hiveviewer/visualization/venn_base.py
+drwxr-xr-x   0 yin        (501) staff       (20)        0 2023-08-04 07:05:20.521138 hiveviewer-0.2.4/src/hiveviewer.egg-info/
+-rw-r--r--   0 yin        (501) staff       (20)     1126 2023-08-04 07:05:20.000000 hiveviewer-0.2.4/src/hiveviewer.egg-info/PKG-INFO
+-rw-r--r--   0 yin        (501) staff       (20)     1013 2023-08-04 07:05:20.000000 hiveviewer-0.2.4/src/hiveviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 yin        (501) staff       (20)        1 2023-08-04 07:05:20.000000 hiveviewer-0.2.4/src/hiveviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 yin        (501) staff       (20)       82 2023-08-04 07:05:20.000000 hiveviewer-0.2.4/src/hiveviewer.egg-info/requires.txt
+-rw-r--r--   0 yin        (501) staff       (20)       11 2023-08-04 07:05:20.000000 hiveviewer-0.2.4/src/hiveviewer.egg-info/top_level.txt
```

### Comparing `hiveviewer-0.2.3/LICENSE` & `hiveviewer-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/PKG-INFO` & `hiveviewer-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.2.3
+Version: 0.2.4
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.2.3/README.md` & `hiveviewer-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/setup.py` & `hiveviewer-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "openpyxl",
         "optuna",
     ],
 )
 
 setup(
     name="hiveviewer",
-    version="0.2.3",
+    version="0.2.4",
     author="Yin Cheng",
     author_email="yin.sjtu@gmail.com",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/yinsn/hiveviewer",
     python_requires=">=3.6",
     description="Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.",
```

### Comparing `hiveviewer-0.2.3/src/hiveviewer/dataloader/base.py` & `hiveviewer-0.2.4/src/hiveviewer/dataloader/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/dataloader/load_csv.py` & `hiveviewer-0.2.4/src/hiveviewer/dataloader/load_csv.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/dataloader/load_excel.py` & `hiveviewer-0.2.4/src/hiveviewer/dataloader/load_excel.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/evaluation/calculator.py` & `hiveviewer-0.2.4/src/hiveviewer/evaluation/calculator.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,29 +124,42 @@
             laplace_smoothing=laplace_smoothing,
         )
         self.score_column = score_column
         self.create_score_columns(
             boundary_dict=self.sampler.sample(), score_column=score_column
         )
 
+        slice_from_condition = (
+            pd.Series(True, index=self.df.index)
+            if slice_from is None
+            else (self.df[score_column] >= slice_from)
+        )
+        slice_to_condition = (
+            pd.Series(True, index=self.df.index)
+            if slice_to is None
+            else (self.df[score_column] <= slice_to)
+        )
+        self.woauc_indices = self.df[slice_from_condition & slice_to_condition].index
+
     def calculate_woauc(
         self,
         weights_for_equation: List,
     ) -> List[float]:
         """Calculate weighted ordinal user AUC.
 
         :param weights_for_equation: weights for equation
         :param score_column: score column
         """
         self.get_overall_score(weights_for_equation)
         woauc = []
         for k, _ in self.sampler.boundary_dict.items():
             paritial_auc = float(
                 roc_auc_score(
-                    self.df[f"{self.score_column}_lt_{k}"], self.df["overall_score"]
+                    self.df.loc[self.woauc_indices][f"{self.score_column}_lt_{k}"],
+                    self.df.loc[self.woauc_indices]["overall_score"],
                 )
             )
             woauc.append(paritial_auc)
         return woauc
 
     def calculate_log_mse(self, target_column: str) -> float:
         """Calculate log mean squared error.
@@ -155,23 +168,21 @@
         """
         log_true = np.log(self.df[target_column] + 1)
         log_pred = np.log(self.df["overall_score"] + 1)
         mse = np.mean((log_true - log_pred) ** 2)
         return float(mse)
 
     def calculate_portfolio_concentration(
-        self, target_column: str, expected_return: Optional[float] = None
+        self, target_column: str, expected_return: Optional[float] = 0.95
     ) -> Tuple[float, float]:
         """Calculate portfolio concentration.
 
         :param target_column: target column
         :param expected_return: expected return
         """
-        if expected_return is None:
-            expected_return = 0.95
         df = self.df.sort_values("overall_score", ascending=False)
         sum_all = df[target_column].sum()
         df["cumulative_sum"] = df[target_column].cumsum()
         df["cumulative_ratio"] = df["cumulative_sum"] / sum_all
         threshold = df[df["cumulative_ratio"] > expected_return]["overall_score"].max()
         concentration = df[df["overall_score"] > threshold].shape[0] / self.df_len
         return threshold, concentration
```

### Comparing `hiveviewer-0.2.3/src/hiveviewer/optimization/base.py` & `hiveviewer-0.2.4/src/hiveviewer/optimization/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/optimization/multiple_objective.py` & `hiveviewer-0.2.4/src/hiveviewer/optimization/multiple_objective.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,21 +104,25 @@
                     )
                 power_weights.append(1 - sum(power_weights))
             else:
                 for i in range(self.weights_num):
                     power_weights.append(trial.suggest_float(f"w{i+1}", 0, 1))
 
         if self.first_order:
+            if self.first_order_lower_bound < 0:
+                log = False
+            else:
+                log = True
             for i in range(self.weights_num):
                 first_order_weights.append(
                     trial.suggest_float(
                         f"w_fo_{i+1}",
                         self.first_order_lower_bound,
                         self.first_order_upper_bound,
-                        log=True,
+                        log=log,
                     )
                 )
 
         targets: List[float] = []
         for calculator, flag, hyperparameter, groupby, target_column in zip(
             self.calculators,
             self.calculator_flags,
```

### Comparing `hiveviewer-0.2.3/src/hiveviewer/sampling/base.py` & `hiveviewer-0.2.4/src/hiveviewer/sampling/base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/sampling/frequency_sampler.py` & `hiveviewer-0.2.4/src/hiveviewer/sampling/frequency_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/sampling/gini_sampler.py` & `hiveviewer-0.2.4/src/hiveviewer/sampling/gini_sampler.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/visualization/lorenz_curve.py` & `hiveviewer-0.2.4/src/hiveviewer/visualization/lorenz_curve.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/visualization/plot_trisurf.py` & `hiveviewer-0.2.4/src/hiveviewer/visualization/plot_trisurf.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/visualization/venn2.py` & `hiveviewer-0.2.4/src/hiveviewer/visualization/venn2.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/visualization/venn3.py` & `hiveviewer-0.2.4/src/hiveviewer/visualization/venn3.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer/visualization/venn_base.py` & `hiveviewer-0.2.4/src/hiveviewer/visualization/venn_base.py`

 * *Files identical despite different names*

### Comparing `hiveviewer-0.2.3/src/hiveviewer.egg-info/PKG-INFO` & `hiveviewer-0.2.4/src/hiveviewer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiveviewer
-Version: 0.2.3
+Version: 0.2.4
 Summary: Offers a toolset for comprehensive, multi-faceted analysis of data exported from Hive, accompanied by powerful data visualization capabilities.
 Home-page: https://github.com/yinsn/hiveviewer
 Author: Yin Cheng
 Author-email: yin.sjtu@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hiveviewer-0.2.3/src/hiveviewer.egg-info/SOURCES.txt` & `hiveviewer-0.2.4/src/hiveviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

