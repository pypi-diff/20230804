# Comparing `tmp/coolpandas-0.4.5.tar.gz` & `tmp/coolpandas-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coolpandas-0.4.5.tar", last modified: Thu Jul 27 16:12:07 2023, max compression
+gzip compressed data, was "coolpandas-0.4.6.tar", last modified: Fri Aug  4 10:07:13 2023, max compression
```

## Comparing `coolpandas-0.4.5.tar` & `coolpandas-0.4.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.076561 coolpandas-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 16:11:46.000000 coolpandas-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-27 16:12:07.076561 coolpandas-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-27 16:11:46.000000 coolpandas-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.068561 coolpandas-0.4.5/coolpandas/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.068561 coolpandas-0.4.5/coolpandas/connect/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/connect/redshift.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.072561 coolpandas-0.4.5/coolpandas/eda/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/features_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/geo_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/random_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/eda/value_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.072561 coolpandas-0.4.5/coolpandas/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/evaluate/confusion_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.076561 coolpandas-0.4.5/coolpandas/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/distplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/geoplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/mapplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/plot/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.076561 coolpandas-0.4.5/coolpandas/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/stats/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/stats/ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.076561 coolpandas-0.4.5/coolpandas/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/transform/bin.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/transform/epoch.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/transform/missing_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/transform/outliers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.076561 coolpandas-0.4.5/coolpandas/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-27 16:11:46.000000 coolpandas-0.4.5/coolpandas/utils/random_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:12:07.068561 coolpandas-0.4.5/coolpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-27 16:12:07.000000 coolpandas-0.4.5/coolpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-27 16:12:07.000000 coolpandas-0.4.5/coolpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:12:07.000000 coolpandas-0.4.5/coolpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-27 16:12:07.000000 coolpandas-0.4.5/coolpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 16:12:07.000000 coolpandas-0.4.5/coolpandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-27 16:11:46.000000 coolpandas-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:12:07.076561 coolpandas-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:13.874711 coolpandas-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-04 10:06:46.000000 coolpandas-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-04 10:07:13.874711 coolpandas-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-08-04 10:06:46.000000 coolpandas-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:13.870711 coolpandas-0.4.6/coolpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:13.870711 coolpandas-0.4.6/coolpandas/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/connect/redshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:13.870711 coolpandas-0.4.6/coolpandas/eda/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/features_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/geo_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/random_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/eda/value_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:13.870711 coolpandas-0.4.6/coolpandas/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/evaluate/confusion_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:13.874711 coolpandas-0.4.6/coolpandas/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/plot/barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/plot/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/plot/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/plot/distplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/plot/geoplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/plot/lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/plot/mapplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/plot/scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/plot/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:13.874711 coolpandas-0.4.6/coolpandas/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/stats/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/stats/ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:13.874711 coolpandas-0.4.6/coolpandas/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/transform/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/transform/epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/transform/missing_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/transform/outliers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:13.874711 coolpandas-0.4.6/coolpandas/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-04 10:06:46.000000 coolpandas-0.4.6/coolpandas/utils/random_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:07:13.870711 coolpandas-0.4.6/coolpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-04 10:07:13.000000 coolpandas-0.4.6/coolpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-04 10:07:13.000000 coolpandas-0.4.6/coolpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:07:13.000000 coolpandas-0.4.6/coolpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-04 10:07:13.000000 coolpandas-0.4.6/coolpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 10:07:13.000000 coolpandas-0.4.6/coolpandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-08-04 10:06:46.000000 coolpandas-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:07:13.874711 coolpandas-0.4.6/setup.cfg
```

### Comparing `coolpandas-0.4.5/LICENSE` & `coolpandas-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/PKG-INFO` & `coolpandas-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.4.5/README.md` & `coolpandas-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/connect/redshift.py` & `coolpandas-0.4.6/coolpandas/connect/redshift.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/eda/__init__.py` & `coolpandas-0.4.6/coolpandas/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/eda/correlation.py` & `coolpandas-0.4.6/coolpandas/eda/correlation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import math
 
-import numpy as np
 import pandas as pd
+from plotly.graph_objs import Figure
 
 from coolpandas.plot import confusion_matrix
 
 
 def get_correlation(
     data_frame: pd.DataFrame, method: str = "pearson", plot: bool = True, **kwargs
-) -> pd.DataFrame:
+) -> tuple[pd.DataFrame, Figure | None]:
     """Get the correlations of a DataFrame.
 
     Args:
         data_frame (pd.DataFrame): DataFrame to get correlations from.
         method (str, optional): Correlation method. Defaults to "pearson".
         plot (bool, optional): Plot the correlation map. Defaults to True.
         **kwargs: Keyword arguments to pass to pandas.DataFrame.corr.
@@ -20,10 +20,11 @@
     Returns:
         pd.DataFrame: Correlations.
     """
     correlation_matrix: pd.DataFrame = data_frame.corr(method=method)
     truncate: callable = lambda x: math.trunc(100 * x) / 100
     correlation_matrix = correlation_matrix.applymap(truncate)
     if plot:
-        fig = confusion_matrix(data_frame, **kwargs)
+        fig: Figure = confusion_matrix(data_frame, **kwargs)
         fig.show()
-    return correlation_matrix
+        return correlation_matrix, fig
+    return correlation_matrix, None
```

### Comparing `coolpandas-0.4.5/coolpandas/eda/distribution.py` & `coolpandas-0.4.6/coolpandas/eda/distribution.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/eda/duplicates.py` & `coolpandas-0.4.6/coolpandas/eda/duplicates.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/eda/features_type.py` & `coolpandas-0.4.6/coolpandas/eda/features_type.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/eda/geo_distance.py` & `coolpandas-0.4.6/coolpandas/eda/geo_distance.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/eda/missing_values.py` & `coolpandas-0.4.6/coolpandas/eda/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/eda/shape.py` & `coolpandas-0.4.6/coolpandas/eda/shape.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/eda/summary.py` & `coolpandas-0.4.6/coolpandas/eda/summary.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/eda/value_counts.py` & `coolpandas-0.4.6/coolpandas/eda/value_counts.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/evaluate/confusion_matrix.py` & `coolpandas-0.4.6/coolpandas/evaluate/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/plot/barplot.py` & `coolpandas-0.4.6/coolpandas/plot/barplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/plot/boxplot.py` & `coolpandas-0.4.6/coolpandas/plot/boxplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/plot/confusion_matrix.py` & `coolpandas-0.4.6/coolpandas/plot/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/plot/distplot.py` & `coolpandas-0.4.6/coolpandas/plot/distplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/plot/geoplot.py` & `coolpandas-0.4.6/coolpandas/plot/geoplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/plot/lineplot.py` & `coolpandas-0.4.6/coolpandas/plot/lineplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/plot/mapplot.py` & `coolpandas-0.4.6/coolpandas/plot/mapplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/plot/scatterplot.py` & `coolpandas-0.4.6/coolpandas/plot/scatterplot.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/plot/style.py` & `coolpandas-0.4.6/coolpandas/plot/style.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/stats/effect.py` & `coolpandas-0.4.6/coolpandas/stats/effect.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/stats/ttest.py` & `coolpandas-0.4.6/coolpandas/stats/ttest.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/transform/bin.py` & `coolpandas-0.4.6/coolpandas/transform/bin.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/transform/missing_values.py` & `coolpandas-0.4.6/coolpandas/transform/missing_values.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas/transform/outliers.py` & `coolpandas-0.4.6/coolpandas/transform/outliers.py`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/coolpandas.egg-info/PKG-INFO` & `coolpandas-0.4.6/coolpandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coolpandas
-Version: 0.4.5
+Version: 0.4.6
 Summary: A Python package for Exploratory Data Analysis.
 Author-email: Avel Docquin <adocquin@outlook.com>
 Project-URL: Homepage, https://github.com/adocquin/coolpandas
 Project-URL: Bug Tracker, https://github.com/adocquin/coolpandas/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `coolpandas-0.4.5/coolpandas.egg-info/SOURCES.txt` & `coolpandas-0.4.6/coolpandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coolpandas-0.4.5/pyproject.toml` & `coolpandas-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coolpandas"
-version = "0.4.5"
+version = "0.4.6"
 authors = [
   { name="Avel Docquin", email="adocquin@outlook.com" },
   ]
 description = "A Python package for Exploratory Data Analysis."
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

