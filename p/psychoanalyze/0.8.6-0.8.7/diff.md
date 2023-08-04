# Comparing `tmp/psychoanalyze-0.8.6.tar.gz` & `tmp/psychoanalyze-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.8.6.tar", max compression
+gzip compressed data, was "psychoanalyze-0.8.7.tar", max compression
```

## Comparing `psychoanalyze-0.8.6.tar` & `psychoanalyze-0.8.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.8.6/LICENSE
--rw-r--r--   0        0        0     1251 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/README.md
--rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.8.6/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.8.6/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.8.6/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.8.6/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.8.6/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.8.6/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1070 2023-07-10 06:31:40.686289 psychoanalyze-0.8.6/psychoanalyze/dashboard/__init__.py
--rw-r--r--   0        0        0    11725 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/dashboard/app.py
--rw-r--r--   0        0        0    10618 2023-07-11 07:34:32.872491 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/PsychoAnalyze.svg
--rw-r--r--   0        0        0    33510 2023-07-11 07:34:42.444787 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png
--rw-r--r--   0        0        0     6575 2023-07-20 04:43:03.897369 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/favicon.ico
--rw-r--r--   0        0        0     6575 2023-07-20 04:41:06.090118 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/logo_bgwhite.png
--rw-r--r--   0        0        0     5350 2023-07-11 09:34:15.577086 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/logo_transparent_100x100.png
--rw-r--r--   0        0        0      551 2023-07-15 02:24:50.772266 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/styles.css
--rw-r--r--   0        0        0     8915 2023-07-28 07:02:51.460865 psychoanalyze-0.8.6/psychoanalyze/dashboard/components.py
--rw-r--r--   0        0        0     9048 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/dashboard/layout.py
--rw-r--r--   0        0        0     1411 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/dashboard/utils.py
--rw-r--r--   0        0        0     1153 2023-07-20 09:25:55.060489 psychoanalyze-0.8.6/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     6491 2023-08-04 02:43:16.389372 psychoanalyze-0.8.6/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     1876 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/data/logistic.py
--rw-r--r--   0        0        0     6796 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.8.6/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.8.6/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.8.6/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     5507 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.8.6/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1135 2023-07-28 02:10:21.380217 psychoanalyze-0.8.6/psychoanalyze/main.py
--rw-r--r--   0        0        0     1239 2023-07-21 04:57:55.937376 psychoanalyze-0.8.6/psychoanalyze/params.py
--rw-r--r--   0        0        0     1585 2023-08-04 02:43:16.389372 psychoanalyze-0.8.6/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.8.6/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     3260 2023-08-04 02:48:08.611110 psychoanalyze-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 psychoanalyze-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.8.7/LICENSE
+-rw-r--r--   0        0        0     1251 2023-08-04 01:42:53.705383 psychoanalyze-0.8.7/README.md
+-rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.8.7/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.8.7/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.8.7/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.8.7/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.8.7/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.8.7/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1070 2023-07-10 06:31:40.686289 psychoanalyze-0.8.7/psychoanalyze/dashboard/__init__.py
+-rw-r--r--   0        0        0    11725 2023-08-04 01:42:53.705383 psychoanalyze-0.8.7/psychoanalyze/dashboard/app.py
+-rw-r--r--   0        0        0    10618 2023-07-11 07:34:32.872491 psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/PsychoAnalyze.svg
+-rw-r--r--   0        0        0    33510 2023-07-11 07:34:42.444787 psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png
+-rw-r--r--   0        0        0     6575 2023-07-20 04:43:03.897369 psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/favicon.ico
+-rw-r--r--   0        0        0     6575 2023-07-20 04:41:06.090118 psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/logo_bgwhite.png
+-rw-r--r--   0        0        0     5350 2023-07-11 09:34:15.577086 psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/logo_transparent_100x100.png
+-rw-r--r--   0        0        0      551 2023-07-15 02:24:50.772266 psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/styles.css
+-rw-r--r--   0        0        0     8915 2023-07-28 07:02:51.460865 psychoanalyze-0.8.7/psychoanalyze/dashboard/components.py
+-rw-r--r--   0        0        0     9048 2023-08-04 01:42:53.705383 psychoanalyze-0.8.7/psychoanalyze/dashboard/layout.py
+-rw-r--r--   0        0        0     1411 2023-08-04 01:42:53.705383 psychoanalyze-0.8.7/psychoanalyze/dashboard/utils.py
+-rw-r--r--   0        0        0     1153 2023-07-20 09:25:55.060489 psychoanalyze-0.8.7/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     6775 2023-08-04 10:40:46.589412 psychoanalyze-0.8.7/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     1876 2023-08-04 01:42:53.705383 psychoanalyze-0.8.7/psychoanalyze/data/logistic.py
+-rw-r--r--   0        0        0     6796 2023-08-04 01:42:53.705383 psychoanalyze-0.8.7/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.8.7/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.8.7/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.8.7/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     5507 2023-08-04 01:42:53.705383 psychoanalyze-0.8.7/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.8.7/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1135 2023-07-28 02:10:21.380217 psychoanalyze-0.8.7/psychoanalyze/main.py
+-rw-r--r--   0        0        0     1239 2023-07-21 04:57:55.937376 psychoanalyze-0.8.7/psychoanalyze/params.py
+-rw-r--r--   0        0        0     1585 2023-08-04 02:43:16.389372 psychoanalyze-0.8.7/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.8.7/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     3272 2023-08-04 10:45:05.190720 psychoanalyze-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 psychoanalyze-0.8.7/PKG-INFO
```

### Comparing `psychoanalyze-0.8.6/LICENSE` & `psychoanalyze-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/README.md` & `psychoanalyze-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/__init__.py` & `psychoanalyze-0.8.7/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.8.7/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.8.7/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.8.7/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.8.7/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.8.7/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/__init__.py` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/app.py` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/app.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/PsychoAnalyze.svg` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/PsychoAnalyze.svg`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/favicon.ico` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/logo_bgwhite.png` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/logo_bgwhite.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/logo_transparent_100x100.png` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/logo_transparent_100x100.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/styles.css` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/assets/styles.css`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/components.py` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/components.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/layout.py` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/layout.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/dashboard/utils.py` & `psychoanalyze-0.8.7/psychoanalyze/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/data/__init__.py` & `psychoanalyze-0.8.7/psychoanalyze/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/data/blocks.py` & `psychoanalyze-0.8.7/psychoanalyze/data/blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,15 +183,23 @@
     x_max = (location + 4) * scale
     x = pd.Index(np.linspace(x_min, x_max, 100), name="Intensity")
     y = expit((x - location) / scale)
     return pd.Series(y, index=x, name="Ψ(x)")
 
 
 def plot_logistic(location: float, scale: float) -> go.Scatter:
-    """Plot a logistic function."""
+    """Plot a logistic function.
+
+    Parameters:
+        location: x₀ in the location-scale parameterization, corresponds to threshold.
+        scale: σ corresponds to the width of the curve (inverse of slope)
+
+    Returns:
+        A Plotly figure of the psychometric function with a logistic link function.
+    """
     return px.line(
         logistic(location, scale),
         y="Ψ(x)",
         template="plotly_white",
     )
```

### Comparing `psychoanalyze-0.8.6/psychoanalyze/data/logistic.py` & `psychoanalyze-0.8.7/psychoanalyze/data/logistic.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/data/points.py` & `psychoanalyze-0.8.7/psychoanalyze/data/points.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/data/sessions.py` & `psychoanalyze-0.8.7/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.8.7/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/data/subjects.py` & `psychoanalyze-0.8.7/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/data/trials.py` & `psychoanalyze-0.8.7/psychoanalyze/data/trials.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/data/types.py` & `psychoanalyze-0.8.7/psychoanalyze/data/types.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/main.py` & `psychoanalyze-0.8.7/psychoanalyze/main.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/params.py` & `psychoanalyze-0.8.7/psychoanalyze/params.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/plot.py` & `psychoanalyze-0.8.7/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/psychoanalyze/sigmoids.py` & `psychoanalyze-0.8.7/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.6/pyproject.toml` & `psychoanalyze-0.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.8.6"
+version = "0.8.7"
 description = "Interactive analysis and simulation of psychophysical data."
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://psychoanalyze.io"
 repository = "https://github.com/psychoanalyze/psychoanalyze"
 documentation = "https://docs.psychoanalyze.io"
@@ -59,15 +59,15 @@
 python-semantic-release = "^8.0.2"
 pytest = "^7.3.2"
 types-pytz = "^2023.3.0.0"
 types-setuptools = "^68.0.0.3"
 hypothesis = "^6.79.0"
 pandas-stubs = "^2.0.2.230605"
 datatest = "^0.11.1"
-dash = {extras = ["testing"], version = "^2.11.1"}
+dash = { extras = ["testing"], version = "^2.11.1" }
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1.21"
@@ -119,15 +119,15 @@
     'pytz',
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
 fix = true
 select = ["ALL", "CPY001"]
-ignore = ["S101", "S311", "D211", "D213"]
+ignore = ["S101", "S311", "D211", "D213", "RUF002"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = ["D100", "D103", "ANN201"]
```

### Comparing `psychoanalyze-0.8.6/PKG-INFO` & `psychoanalyze-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.8.6
+Version: 0.8.7
 Summary: Interactive analysis and simulation of psychophysical data.
 Home-page: https://psychoanalyze.io
 License: GPL-3.0-or-later
 Keywords: psychophysics,neuroscience,psychology
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: >=3.9.0,<3.12.0
```

