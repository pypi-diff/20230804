# Comparing `tmp/psychoanalyze-0.8.5.tar.gz` & `tmp/psychoanalyze-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.8.5.tar", max compression
+gzip compressed data, was "psychoanalyze-0.8.6.tar", max compression
```

## Comparing `psychoanalyze-0.8.5.tar` & `psychoanalyze-0.8.6.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.8.5/LICENSE
--rw-r--r--   0        0        0     1251 2023-07-31 00:45:44.501916 psychoanalyze-0.8.5/README.md
--rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.8.5/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.8.5/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.8.5/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.8.5/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.8.5/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.8.5/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1070 2023-07-10 06:31:40.686289 psychoanalyze-0.8.5/psychoanalyze/dashboard/__init__.py
--rw-r--r--   0        0        0    12468 2023-07-28 02:10:21.380217 psychoanalyze-0.8.5/psychoanalyze/dashboard/app.py
--rw-r--r--   0        0        0    10618 2023-07-11 07:34:32.872491 psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/PsychoAnalyze.svg
--rw-r--r--   0        0        0    33510 2023-07-11 07:34:42.444787 psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png
--rw-r--r--   0        0        0     6575 2023-07-20 04:43:03.897369 psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/favicon.ico
--rw-r--r--   0        0        0     6575 2023-07-20 04:41:06.090118 psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/logo_bgwhite.png
--rw-r--r--   0        0        0     5350 2023-07-11 09:34:15.577086 psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/logo_transparent_100x100.png
--rw-r--r--   0        0        0      551 2023-07-15 02:24:50.772266 psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/styles.css
--rw-r--r--   0        0        0     8915 2023-07-28 07:02:51.460865 psychoanalyze-0.8.5/psychoanalyze/dashboard/components.py
--rw-r--r--   0        0        0     9048 2023-07-31 00:45:44.521916 psychoanalyze-0.8.5/psychoanalyze/dashboard/layout.py
--rw-r--r--   0        0        0     1153 2023-07-20 09:25:55.060489 psychoanalyze-0.8.5/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     6031 2023-07-28 00:17:06.312544 psychoanalyze-0.8.5/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     6787 2023-07-28 00:17:06.312544 psychoanalyze-0.8.5/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.8.5/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.8.5/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.8.5/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     5225 2023-07-20 09:41:06.475106 psychoanalyze-0.8.5/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.8.5/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1135 2023-07-28 02:10:21.380217 psychoanalyze-0.8.5/psychoanalyze/main.py
--rw-r--r--   0        0        0     1239 2023-07-21 04:57:55.937376 psychoanalyze-0.8.5/psychoanalyze/params.py
--rw-r--r--   0        0        0     2116 2023-07-21 02:42:52.381174 psychoanalyze-0.8.5/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.8.5/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     3209 2023-07-31 01:06:36.840773 psychoanalyze-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 psychoanalyze-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-10-04 02:36:06.350931 psychoanalyze-0.8.6/LICENSE
+-rw-r--r--   0        0        0     1251 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/README.md
+-rw-r--r--   0        0        0     1357 2023-07-10 06:32:31.020291 psychoanalyze-0.8.6/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-10 06:35:55.935533 psychoanalyze-0.8.6/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-10 06:35:48.275360 psychoanalyze-0.8.6/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1120 2023-07-10 06:35:38.831225 psychoanalyze-0.8.6/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2302 2023-07-10 23:10:13.757714 psychoanalyze-0.8.6/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2373 2023-07-10 06:35:32.351775 psychoanalyze-0.8.6/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1070 2023-07-10 06:31:40.686289 psychoanalyze-0.8.6/psychoanalyze/dashboard/__init__.py
+-rw-r--r--   0        0        0    11725 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/dashboard/app.py
+-rw-r--r--   0        0        0    10618 2023-07-11 07:34:32.872491 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/PsychoAnalyze.svg
+-rw-r--r--   0        0        0    33510 2023-07-11 07:34:42.444787 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png
+-rw-r--r--   0        0        0     6575 2023-07-20 04:43:03.897369 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/favicon.ico
+-rw-r--r--   0        0        0     6575 2023-07-20 04:41:06.090118 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/logo_bgwhite.png
+-rw-r--r--   0        0        0     5350 2023-07-11 09:34:15.577086 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/logo_transparent_100x100.png
+-rw-r--r--   0        0        0      551 2023-07-15 02:24:50.772266 psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/styles.css
+-rw-r--r--   0        0        0     8915 2023-07-28 07:02:51.460865 psychoanalyze-0.8.6/psychoanalyze/dashboard/components.py
+-rw-r--r--   0        0        0     9048 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/dashboard/layout.py
+-rw-r--r--   0        0        0     1411 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/dashboard/utils.py
+-rw-r--r--   0        0        0     1153 2023-07-20 09:25:55.060489 psychoanalyze-0.8.6/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     6491 2023-08-04 02:43:16.389372 psychoanalyze-0.8.6/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     1876 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/data/logistic.py
+-rw-r--r--   0        0        0     6796 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2868 2023-07-10 06:35:10.993442 psychoanalyze-0.8.6/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      841 2023-07-10 06:35:04.783422 psychoanalyze-0.8.6/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1678 2023-07-10 06:34:48.603492 psychoanalyze-0.8.6/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     5507 2023-08-04 01:42:53.705383 psychoanalyze-0.8.6/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     3002 2023-07-16 02:29:21.297443 psychoanalyze-0.8.6/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1135 2023-07-28 02:10:21.380217 psychoanalyze-0.8.6/psychoanalyze/main.py
+-rw-r--r--   0        0        0     1239 2023-07-21 04:57:55.937376 psychoanalyze-0.8.6/psychoanalyze/params.py
+-rw-r--r--   0        0        0     1585 2023-08-04 02:43:16.389372 psychoanalyze-0.8.6/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1518 2023-07-10 06:34:24.801696 psychoanalyze-0.8.6/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     3260 2023-08-04 02:48:08.611110 psychoanalyze-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 psychoanalyze-0.8.6/PKG-INFO
```

### Comparing `psychoanalyze-0.8.5/LICENSE` & `psychoanalyze-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/README.md` & `psychoanalyze-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/__init__.py` & `psychoanalyze-0.8.6/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.8.6/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.8.6/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.8.6/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.8.6/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.8.6/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/dashboard/__init__.py` & `psychoanalyze-0.8.6/psychoanalyze/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/dashboard/app.py` & `psychoanalyze-0.8.6/psychoanalyze/dashboard/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-"""Main Dash app file.
-
-Contains callbacks.
-"""
-
 # Copyright 2023 Tyler Schlichenmeyer
 
 # This file is part of PsychoAnalyze.
 # PsychoAnalyze is free software: you can redistribute it and/or modify it under the
 # terms of the GNU General Public License as published by the Free Software Foundation,
 # either version 3 of the License, or (at your option) any later version.
 
 # PsychoAnalyze is distributed in the hope that it will be useful, but WITHOUT ANY
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
+"""Main Dash app file.
+
+Contains callbacks.
+"""
+
 import base64
 import io
-import random
 import zipfile
 from collections.abc import Hashable
 from datetime import datetime
 from pathlib import Path
 from typing import Any
 
 import duckdb
@@ -43,16 +42,20 @@
     callback_context,
     dcc,
 )
 from dash_bootstrap_components import icons, themes
 from scipy.special import expit, logit
 
 from psychoanalyze.dashboard.layout import layout
+from psychoanalyze.dashboard.utils import process_upload
 from psychoanalyze.data import blocks as pa_blocks
 from psychoanalyze.data import points as pa_points
+from psychoanalyze.data.logistic import to_intercept, to_slope
+from psychoanalyze.data.points import generate_index
+from psychoanalyze.data.trials import generate
 
 app = Dash(
     __name__,
     external_stylesheets=[
         themes.SUPERHERO,
         icons.BOOTSTRAP,
         "https://fonts.googleapis.com/css2?family=Comfortaa:wght@500&family=Glegoo:wght@700&display=swap",
@@ -70,65 +73,36 @@
     Output({"type": "x-param", "name": "min"}, "value"),
     Output({"type": "x-param", "name": "max"}, "value"),
     Input("upload", "contents"),
     State("upload", "filename"),
     Input({"type": "n-param", "name": ALL}, "value"),
     Input({"type": "param", "name": ALL}, "value"),
 )
-def update_data(
+def update_trials(
     contents: str,
     filename: str,
     n_param: list[int],
     param: list[float],
 ) -> tuple[Records, float, float]:
     """Update points table."""
-    n_param_values = [
-        "n_levels",
-        "n_trials",
-        "n_blocks",
-    ]
-    n_params = pd.Series(n_param, index=n_param_values)
-    param = [*param, 0.0, 0.0]
-    params = pd.Series(param, index=["x_0", "k", "gamma", "lambda"])
-    params["intercept"] = -params["x_0"] / params["k"]
-    params["slope"] = 1 / params["k"]
+    n_params = pd.Series(n_param, index=["n_levels", "n_trials", "n_blocks"])
+    params = pd.Series([*param, 0.0, 0.0], index=["x_0", "k", "gamma", "lambda"])
+    params["intercept"] = to_intercept(params["x_0"], params["k"])
+    params["slope"] = to_slope(params["k"])
     min_x = (logit(0.01) - params["intercept"]) / params["slope"]
     max_x = (logit(0.99) - params["intercept"]) / params["slope"]
     if callback_context.triggered_id == "upload":
-        _, content_string = contents.split(",")
-        decoded = base64.b64decode(content_string)
-        if "zip" in filename:
-            with zipfile.ZipFile(io.BytesIO(decoded)) as z:
-                trials = pd.read_csv(z.open("trials.csv"))
-        else:
-            trials = pd.read_csv(io.StringIO(decoded.decode("utf-8")))
+        trials = process_upload(contents, filename)
     else:
-        points_ix = pd.Index(
-            np.linspace(min_x, max_x, n_params["n_levels"]),
-            name="Intensity",
+        trials = generate(
+            n_trials=n_params["n_trials"],
+            options=generate_index(n_params["n_levels"], [min_x, max_x]),
+            params=params.to_dict(),
+            n_blocks=n_params["n_blocks"],
         )
-        all_trials = {}
-        for i in range(n_params["n_blocks"]):
-            execution_plan = pd.Index(
-                [random.choice(points_ix) for _ in range(n_params["n_trials"])],
-                name="Intensity",
-            )
-            trials_i = pd.Series(
-                [
-                    int(
-                        random.random()
-                        < expit(x * params["slope"] + params["intercept"]),
-                    )
-                    for x in execution_plan
-                ],
-                name="Result",
-                index=execution_plan,
-            )
-            all_trials[i] = trials_i
-        trials = pd.concat(all_trials, names=["Block"]).reset_index()
     return trials.to_dict("records"), min_x, max_x
 
 
 @callback(
     Output("points-store", "data"),
     Input("trials-store", "data"),
 )
```

### Comparing `psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/PsychoAnalyze.svg` & `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/PsychoAnalyze.svg`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png` & `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/PsychoAnalyze_350x350.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/favicon.ico` & `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/logo_bgwhite.png` & `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/logo_bgwhite.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/logo_transparent_100x100.png` & `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/logo_transparent_100x100.png`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/dashboard/assets/styles.css` & `psychoanalyze-0.8.6/psychoanalyze/dashboard/assets/styles.css`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/dashboard/components.py` & `psychoanalyze-0.8.6/psychoanalyze/dashboard/components.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/dashboard/layout.py` & `psychoanalyze-0.8.6/psychoanalyze/dashboard/layout.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/data/__init__.py` & `psychoanalyze-0.8.6/psychoanalyze/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/data/blocks.py` & `psychoanalyze-0.8.6/psychoanalyze/data/blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -180,7 +180,26 @@
 def logistic(location: float, scale: float) -> pd.Series:
     """Generate points for a line trace of a logistic function."""
     x_min = (location - 4) * scale
     x_max = (location + 4) * scale
     x = pd.Index(np.linspace(x_min, x_max, 100), name="Intensity")
     y = expit((x - location) / scale)
     return pd.Series(y, index=x, name="Ψ(x)")
+
+
+def plot_logistic(location: float, scale: float) -> go.Scatter:
+    """Plot a logistic function."""
+    return px.line(
+        logistic(location, scale),
+        y="Ψ(x)",
+        template="plotly_white",
+    )
+
+
+def plot_standard_logistic() -> go.Scatter:
+    """Plot a standard logistic function."""
+    return px.line(
+        standard_logistic(),
+        y="f(x)",
+        template="plotly_white",
+        title="$f(x) = \\frac{1}{1 + e^{-x}}$",
+    )
```

### Comparing `psychoanalyze-0.8.5/psychoanalyze/data/points.py` & `psychoanalyze-0.8.6/psychoanalyze/data/points.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,22 +153,22 @@
 
 
 def combine_plots(fig1: go.Figure, fig2: go.Figure) -> go.Figure:
     """Combine two points-level plots. Possible duplicate."""
     return go.Figure(data=fig1.data + fig2.data)
 
 
-def n(trials: pd.Series) -> pd.Series:
+def n(trials: pd.Index) -> pd.Index:
     """Count trials at each point."""
     return pd.Series(trials.value_counts(), name="n")
 
 
 def generate_n(n_trials: int, options: pd.Index) -> pd.Series:
     """Simulate how many trials were performed per intensity level."""
-    return n(pa_trials.generate_trial_index(n_trials, options))
+    return pd.Series(n(pa_trials.generate_trial_index(n_trials, options)))
 
 
 def to_block(points: pd.DataFrame) -> pd.DataFrame:
     """Aggregate to block-level measures from points-level data."""
     return points.groupby(level="Block").sum()
```

### Comparing `psychoanalyze-0.8.5/psychoanalyze/data/sessions.py` & `psychoanalyze-0.8.6/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.8.6/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/data/subjects.py` & `psychoanalyze-0.8.6/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/data/trials.py` & `psychoanalyze-0.8.6/psychoanalyze/data/trials.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,51 +16,63 @@
 import json
 import random
 from pathlib import Path
 from typing import TypedDict
 
 import numpy as np
 import pandas as pd
-from pandera import SeriesSchema, check_output
+from pandera import SeriesSchema
 from sklearn.linear_model import LogisticRegression
 
 from psychoanalyze.data import types
 
 schema = SeriesSchema(bool, name="Test Trials")
 
 data_path = Path("data/trials.csv")
 
 codes = {0: "Miss", 1: "Hit"}
 
 
 Trial = TypedDict("Trial", {"Result": bool, "Stimulus Magnitude": float})
 
 
-def generate_trial_index(n_trials: int, options: pd.Index) -> pd.Series:
+def generate_trial_index(n_trials: int, options: pd.Index) -> pd.Index:
     """Generate n trials (no outcomes)."""
-    return pd.Series(
+    return pd.Index(
         [random.choice(options) for _ in range(n_trials)],
         name="Intensity",
     )
 
 
-@check_output(types.trials)
+def sample_trials(trials_ix: pd.Index, params: dict[str, float]) -> pd.Series:
+    """Sample trials from a given index."""
+    return pd.Series(
+        [int(random.random() <= psi(x, params)) for x in trials_ix],
+        index=trials_ix,
+        name="Result",
+    )
+
+
 def generate(
     n_trials: int,
     options: pd.Index,
     params: dict[str, float],
+    n_blocks: int,
 ) -> pd.DataFrame:
     """Generate n trials with outcomes."""
-    x = generate_trial_index(n_trials, options)
-    return pd.DataFrame(
+    return pd.concat(
         {
-            "Result": [int(random.random() <= psi(x_val, params)) for x_val in x],
-            "Intensity": x,
+            i: sample_trials(
+                trials_ix=generate_trial_index(n_trials, options),
+                params=params,
+            )
+            for i in range(n_blocks)
         },
-    )
+        names=["Block"],
+    ).reset_index()
 
 
 def load(data_path: Path) -> pd.DataFrame:
     """Load trials data from csv."""
     return types.trials.validate(
         pd.read_csv(
             data_path,
@@ -125,18 +137,18 @@
 def labels(results: list[int]) -> list[str]:
     """Convert a list of outcome codes to their labels."""
     return [codes[result] for result in results]
 
 
 def psi(intensity: float, params: dict[str, float]) -> float:
     """Calculate the value of the psychometric function for a given intensity."""
-    gamma = params["Guess Rate"]
-    lambda_ = params["Lapse Rate"]
-    k = params["Slope"]
-    x_0 = params["Threshold"]
+    gamma = params["gamma"]
+    lambda_ = params["lambda"]
+    k = params["k"]
+    x_0 = params["x_0"]
     return gamma + (1 - gamma - lambda_) * (1 / (1 + np.exp(-k * (intensity - x_0))))
 
 
 def moc_sample(n_trials: int, model_params: dict[str, float]) -> pd.DataFrame:
     """Sample results from a method-of-constant-stimuli experiment."""
     x_0 = model_params["x_0"]
     k = model_params["k"]
```

### Comparing `psychoanalyze-0.8.5/psychoanalyze/data/types.py` & `psychoanalyze-0.8.6/psychoanalyze/data/types.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/main.py` & `psychoanalyze-0.8.6/psychoanalyze/main.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/params.py` & `psychoanalyze-0.8.6/psychoanalyze/params.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/psychoanalyze/plot.py` & `psychoanalyze-0.8.6/psychoanalyze/plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 # PARTICULAR PURPOSE. See the GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License along with
 # PsychoAnalyze. If not, see <https://www.gnu.org/licenses/>.
 
 """Global plot settings and generic plot utilities."""
 
-import plotly.express as px
 import plotly.graph_objects as go
 
-from psychoanalyze.data import blocks
-
 axis_settings = {
     "ticks": "outside",
     "showgrid": False,
     "showline": True,
     "zeroline": False,
     "title": {"font": {"size": 12, "family": "Arial"}},
 }
@@ -47,26 +44,7 @@
         "y": "Threshold Amplitude (μA)",
     },
     "Width": {
         "x": "Fixed Amplitude (μA)",
         "y": "Threshold Pulse Width (μs)",
     },
 }
-
-
-def standard_logistic() -> go.Scatter:
-    """Plot a standard logistic function."""
-    return px.line(
-        blocks.standard_logistic(),
-        y="f(x)",
-        template="plotly_white",
-        title="$f(x) = \\frac{1}{1 + e^{-x}}$",
-    )
-
-
-def logistic(location: float, scale: float) -> go.Scatter:
-    """Plot a logistic function."""
-    return px.line(
-        blocks.logistic(location, scale),
-        y="Ψ(x)",
-        template="plotly_white",
-    )
```

### Comparing `psychoanalyze-0.8.5/psychoanalyze/sigmoids.py` & `psychoanalyze-0.8.6/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.8.5/pyproject.toml` & `psychoanalyze-0.8.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.8.5"
+version = "0.8.6"
 description = "Interactive analysis and simulation of psychophysical data."
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://psychoanalyze.io"
 repository = "https://github.com/psychoanalyze/psychoanalyze"
 documentation = "https://docs.psychoanalyze.io"
@@ -59,14 +59,15 @@
 python-semantic-release = "^8.0.2"
 pytest = "^7.3.2"
 types-pytz = "^2023.3.0.0"
 types-setuptools = "^68.0.0.3"
 hypothesis = "^6.79.0"
 pandas-stubs = "^2.0.2.230605"
 datatest = "^0.11.1"
+dash = {extras = ["testing"], version = "^2.11.1"}
 
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1.21"
```

### Comparing `psychoanalyze-0.8.5/PKG-INFO` & `psychoanalyze-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.8.5
+Version: 0.8.6
 Summary: Interactive analysis and simulation of psychophysical data.
 Home-page: https://psychoanalyze.io
 License: GPL-3.0-or-later
 Keywords: psychophysics,neuroscience,psychology
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: >=3.9.0,<3.12.0
```

