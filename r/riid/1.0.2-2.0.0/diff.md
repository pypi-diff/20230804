# Comparing `tmp/riid-1.0.2.tar.gz` & `tmp/riid-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PyRIID/PyRIID/dist/tmpmc591_j3/riid-1.0.2.tar", last modified: Tue Nov 23 18:15:15 2021, max compression
+gzip compressed data, was "riid-2.0.0.tar", last modified: Thu Aug  3 23:37:09 2023, max compression
```

## Comparing `riid-1.0.2.tar` & `riid-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-23 18:15:15.000000 riid-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1452 2021-11-23 18:15:04.000000 riid-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (116)     2923 2021-11-23 18:15:15.000000 riid-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1802 2021-11-23 18:15:04.000000 riid-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       90 2021-11-23 18:15:04.000000 riid-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-23 18:15:15.000000 riid-1.0.2/riid/
--rw-r--r--   0 runner    (1001) docker     (116)     1295 2021-11-23 18:15:04.000000 riid-1.0.2/riid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8442 2021-11-23 18:15:04.000000 riid-1.0.2/riid/data.py
--rw-r--r--   0 runner    (1001) docker     (116)    18464 2021-11-23 18:15:04.000000 riid-1.0.2/riid/gadras.py
--rw-r--r--   0 runner    (1001) docker     (116)     8062 2021-11-23 18:15:04.000000 riid-1.0.2/riid/list_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-23 18:15:15.000000 riid-1.0.2/riid/models/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-23 18:15:04.000000 riid-1.0.2/riid/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10206 2021-11-23 18:15:04.000000 riid-1.0.2/riid/models/bayes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1603 2021-11-23 18:15:04.000000 riid-1.0.2/riid/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (116)     2127 2021-11-23 18:15:04.000000 riid-1.0.2/riid/models/metrics.py
--rw-r--r--   0 runner    (1001) docker     (116)    11568 2021-11-23 18:15:04.000000 riid-1.0.2/riid/models/neural_nets.py
--rw-r--r--   0 runner    (1001) docker     (116)    30411 2021-11-23 18:15:04.000000 riid-1.0.2/riid/sampleset.py
--rw-r--r--   0 runner    (1001) docker     (116)    32201 2021-11-23 18:15:04.000000 riid-1.0.2/riid/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (116)    25646 2021-11-23 18:15:04.000000 riid-1.0.2/riid/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-23 18:15:15.000000 riid-1.0.2/riid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2923 2021-11-23 18:15:15.000000 riid-1.0.2/riid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      417 2021-11-23 18:15:15.000000 riid-1.0.2/riid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-11-23 18:15:15.000000 riid-1.0.2/riid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      166 2021-11-23 18:15:15.000000 riid-1.0.2/riid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2021-11-23 18:15:15.000000 riid-1.0.2/riid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-11-23 18:15:15.000000 riid-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1969 2021-11-23 18:15:04.000000 riid-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:37:09.052814 riid-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-08-03 23:37:00.000000 riid-2.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-03 23:37:00.000000 riid-2.0.0/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-08-03 23:37:09.052814 riid-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-08-03 23:37:00.000000 riid-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-03 23:37:00.000000 riid-2.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:37:09.052814 riid-2.0.0/riid/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 23:37:00.000000 riid-2.0.0/riid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20931 2023-08-03 23:37:00.000000 riid-2.0.0/riid/anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-08-03 23:37:00.000000 riid-2.0.0/riid/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:37:09.052814 riid-2.0.0/riid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-08-03 23:37:09.000000 riid-2.0.0/riid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-08-03 23:37:09.000000 riid-2.0.0/riid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:37:09.000000 riid-2.0.0/riid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 23:37:09.000000 riid-2.0.0/riid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 23:37:09.000000 riid-2.0.0/riid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 23:37:09.052814 riid-2.0.0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `riid-1.0.2/LICENSE.md` & `riid-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `riid-1.0.2/riid/visualize.py` & `riid-2.0.0/riid/visualize.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,101 @@
 # Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
-# Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
+# Under the terms of Contract DE-NA0003525 with NTESS,
+# the U.S. Government retains certain rights in this software.
 """This module provides visualization functions primarily for visualizing SampleSets."""
+import hashlib
+
 import matplotlib
 import matplotlib.pyplot as plt  # noqa: E402
 import numpy as np
 import pandas as pd
 from matplotlib import cm, rcParams  # noqa: E402
 from matplotlib.colors import ListedColormap
-from numpy.random import choice
-from scipy.special import comb
 from seaborn import heatmap
 from sklearn.metrics import confusion_matrix as confusion_matrix_sklearn
-from sklearn.metrics import f1_score
 
-from riid.sampleset import SampleSet
+from riid.data import SampleSet
 
 # DO NOT TOUCH what is set below, nor should you override them inside a function.
 plt.style.use("default")
 rcParams["font.family"] = "serif"
-CM = cm.tab10
+CM = cm.tab20
 MARKER = "."
 
 
 def save_or_show_plot(func):
     """Function decorator providing standardized handling of
     saving and/or showing matplotlib plots.
 
     Args:
-        func: the function to call that builds the plot and
+        func: Defines the function to call that builds the plot and
             returns a tuple of (Figure, Axes).
+
     """
     def save_or_show_plot_wrapper(*args, save_file_path=None, show=True,
                                   return_bytes=False, **kwargs):
         if return_bytes:
             matplotlib.use("Agg")
         fig, ax = func(*args, **kwargs)
+        plt.tight_layout()
         if save_file_path:
             fig.savefig(save_file_path)
         if show:
             plt.show()
         if save_file_path:
             plt.close(fig)
         if return_bytes:
             import io
             buf = io.BytesIO()
-            fig.savefig(buf, format='png')
+            fig.savefig(buf, format="png")
             buf.seek(0)
             plt.close(fig)
             return buf
         return fig, ax
 
     return save_or_show_plot_wrapper
 
 
 @save_or_show_plot
 def confusion_matrix(ss: SampleSet, as_percentage: bool = False, cmap: str = "binary",
                      title: str = None, value_format: str = None, value_fontsize: int = None,
-                     figsize: str = None, alpha: float = None):
-    """Generates a confusion matrix for a SampleSet.
-
-    Prediction and label information is used to distinguish between correct
-    and incorrect classifications using color (green for correct, red for incorrect).
-
-    Args:
-        ss: a SampleSet of events to plot.
-        as_percentage: scales existing confusion matrix values to the range 0 to 100.
-        cmap: the colormap to use for seaborn colormap function.
-        title: the plot title.
-        value_format: the format string controlling how values are displayed in the matrix cells.
-        value_fontsize: the font size of the values displayed in the matrix cells.
-        figsize: the figure size passed to the matplotlib subplots call.
-        alpha: the degree of opacity.
+                     figsize=(10, 10), alpha: float = None, target_level="Isotope"):
+    """Generates a confusion matrix for a SampleSet. Prediction and label information is
+    used to distinguish between correct and incorrect classifications using color
+    (green for correct, red for incorrect).
+
+    Args:
+        ss: Defines a SampleSet of events to plot.
+        as_percentage: Scales existing confusion matrix values to the range 0 to 100.
+        cmap: Defines the colormap to use for seaborn colormap function.
+        title: Defines the plot title.
+        value_format: Defines the format string controlling how values are displayed in the matrix
+            cells.
+        value_fontsize: Defines the font size of the values displayed in the matrix cells.
+        figsize: Width, height of figure in inches.
+        alpha: Defines the degree of opacity.
+        target_level: sources level to plot.
 
     Returns:
         A tuple (Figure, Axes) of matplotlib objects.
 
     Raises:
-        EmptyPredictionsArrayError: raised when the sampleset does not contain any predictions
+        EmptyPredictionsArrayError: Raised when the sampleset does not contain any predictions.
+
     """
-    y_true = ss.labels
-    y_pred = ss.predictions
+    y_true = ss.get_labels(target_level=target_level)
+    y_pred = ss.get_predictions(target_level=target_level)
     labels = sorted(set(list(y_true) + list(y_pred)))
 
     if y_pred.size == 0:
         msg = "Predictions array was empty.  Have you called `model.predict(ss)`?"
         raise EmptyPredictionsArrayError(msg)
 
     if not cmap:
-        cmap = ListedColormap(['white'])
+        cmap = ListedColormap(["white"])
 
     cm_values = confusion_matrix_sklearn(y_true, y_pred, labels=labels)
     if as_percentage:
         cm_values = np.array(cm_values)
         cm_values = cm_values / cm_values.sum(axis=1)
         if not value_format:
             value_format = ".1%"
@@ -103,256 +107,177 @@
     if alpha:
         heatmap_kwargs.update({"alpha": alpha})
     if value_format:
         heatmap_kwargs.update({"fmt": value_format})
     if cmap:
         heatmap_kwargs.update({"cmap": cmap})
 
-    fig, ax = plt.subplots(**{"figsize": figsize})
+    fig, ax = plt.subplots(figsize=figsize)
     mask = cm_values == 0
     ax = heatmap(cm_values, annot=True, linewidths=0.25, linecolor="grey", cbar=False,
                  mask=mask, **heatmap_kwargs)
 
     tick_locs = np.arange(len(labels)) + 0.5
     ax.set_ylabel("Truth")
     ax.set_yticks(tick_locs)
     ax.set_yticklabels(labels, rotation=0)
-
     ax.set_xlabel("Prediction")
     ax.set_xticks(tick_locs)
     ax.set_xticklabels(labels, rotation=90)
-
     ax.set_title(title)
-    plt.tight_layout()
+
     return fig, ax
 
 
 @save_or_show_plot
 def plot_live_time_vs_snr(ss: SampleSet, overlay_ss: SampleSet = None, alpha: float = 0.5,
                           xscale: str = "linear", yscale: str = "log",
                           xlim: tuple = None, ylim: tuple = None,
-                          title: str = "Live Time vs. SNR", sigma_line_value: float = None):
+                          title: str = "Live Time vs. SNR", snr_line_value: float = None,
+                          figsize=(6.4, 4.8), target_level: str = "Isotope"):
     """Plots SNR against live time for all samples in a SampleSet.
 
-    Prediction and label information is used to distinguish between correct
-    and incorrect classifications using color (green for correct, red for incorrect).
+    Prediction and label information is used to distinguish between correct and incorrect
+    classifications using color (green for correct, red for incorrect).
 
     Args:
-        ss: a SampleSet of events to plot.
-        overlay_ss: another SampleSet to color as black.
-        alpha: the degree of opacity (not applied to overlay_ss scatterplot if used).
-        xscale: the X-axis scale.
-        yscale: the Y-axis scale.
-        xlim: a tuple containing the X-axis min and max values.
-        ylim: a tuple containing the Y-axis min and max values.
-        title: the plot title.
-        sigma_line_value: plots a sigma line representing the `value` number of
-            standard deviations from background.
+        ss: Defines a SampleSet of events to plot.
+        overlay_ss: Defines another SampleSet to color as black.
+        alpha: Defines the degree of opacity (not applied to overlay_ss scatterplot if used).
+        xscale: Defines the x-axis scale.
+        yscale: Defines the y-axis scale.
+        xlim: tuple containing the x-axis min and max values.
+        ylim: tuple containing the y-axis min and max values.
+        title: Defines the plot title.
+        snr_line_value: Plots a vertical line for contextualizing data to threshold
+        figsize: Width, height of figure in inches.
 
     Returns:
         A tuple (Figure, Axes) of matplotlib objects.
 
-    Raises:
-        None
     """
-    correct_ss = ss.get_indices(ss.labels == ss.predictions)
-    incorrect_ss = ss.get_indices(ss.labels != ss.predictions)
+    labels = ss.get_labels(target_level=target_level)
+    predictions = ss.get_predictions(target_level=target_level)
+    correct_ss = ss[labels == predictions]
+    incorrect_ss = ss[labels != predictions]
     if not xlim:
-        xlim = (ss.live_time.min(), ss.live_time.max())
+        xlim = (ss.info.live_time.min(), ss.info.live_time.max())
     if not ylim:
         if yscale == "log":
-            ylim = (ss.snr_estimate.clip(1e-3).min(), ss.snr_estimate.max())
+            ylim = (ss.info.snr.clip(1e-3).min(), ss.info.snr.max())
         else:
-            ylim = (ss.snr_estimate.clip(0).min(), ss.snr_estimate.max())
-    fig, ax = plt.subplots()
+            ylim = (ss.info.snr.clip(0).min(), ss.info.snr.max())
 
+    fig, ax = plt.subplots(figsize=figsize)
     ax.scatter(
-        correct_ss.live_time,
-        correct_ss.snr_estimate,
-        c="green", alpha=alpha, marker=MARKER, label="Correct"
+        correct_ss.info.live_time,
+        correct_ss.info.snr,
+        c="blue", alpha=alpha, marker=MARKER, label="Correct"
     )
     ax.scatter(
-        incorrect_ss.live_time,
-        incorrect_ss.snr_estimate,
+        incorrect_ss.info.live_time,
+        incorrect_ss.info.snr,
         c="red", alpha=alpha, marker=MARKER, label="Incorrect"
     )
     if overlay_ss:
         plt.scatter(
-            overlay_ss.live_time,
-            overlay_ss.snr_estimate,
+            overlay_ss.info.live_time,
+            overlay_ss.info.snr,
             c="black", marker="+", label="Event" + ("" if overlay_ss.n_samples == 1 else "s"),
             s=75
         )
-    if sigma_line_value:
+    if snr_line_value:
         live_times = np.linspace(xlim[0], xlim[1])
-        background_cps = ss.collection_information["bg_counts_expected"][0] / ss.live_time[0]
-        snrs = sigma_line_value / np.sqrt(live_times * background_cps)
         plt.plot(
             live_times,
-            snrs,
-            c="blue",
+            snr_line_value,
+            c="black",
             alpha=alpha,
-            label="{}-sigma".format(sigma_line_value),
+            label=f"SNR={snr_line_value}",
             ls="dashed"
         )
 
     ax.set_xscale(xscale)
     ax.set_yscale(yscale)
     ax.set_xlim(xlim)
     ax.set_ylim(ylim)
     ax.set_xlabel("Live Time (s)")
     ax.set_ylabel("Signal-to-Noise Ratio (SNR)")
     ax.set_title(title)
-    fig.legend(loc="lower right")
-    return fig, ax
-
-
-@save_or_show_plot
-def plot_strength_vs_score(ss: SampleSet, overlay_ss: SampleSet = None, alpha: float = 0.5,
-                           marker_size=75, xscale: str = "log", yscale: str = "linear",
-                           xlim: tuple = (None, None), ylim: tuple = (0, 1.05),
-                           title: str = "Signal Strength vs. Score", sigma_line_value: float = None):
-    """Plots strength against prediction score for all samples in a SampleSet.
-
-    Prediction and label information is used to distinguish between correct
-    and incorrect classifications using color (green for correct, red for incorrect).
-
-    Args:
-        ss: a SampleSet of events to plot.
-        overlay_ss: another SampleSet to color as blue (correct) and/or black (incorrect).
-        alpha: the degree of opacity (not applied to overlay_ss scatterplot if used).
-        xscale: the X-axis scale.
-        yscale: the Y-axis scale.
-        xlim: a tuple containing the X-axis min and max values.
-        ylim: a tuple containing the Y-axis min and max values.
-        title: the plot title.
-        sigma_line_value: plots a sigma line representing the `value` number of
-            standard deviations from background.
-
-    Returns:
-        A tuple (Figure, Axes) of matplotlib objects.
-
-    Raises:
-        None
-    """
-    correct_ss = ss.get_indices(ss.labels == ss.predictions)
-    incorrect_ss = ss.get_indices(ss.labels != ss.predictions)
-    if not xlim:
-        if xscale == "log":
-            xlim = (ss.sigma.clip(1e-3).min(), ss.sigma.max())
-        else:
-            xlim = (ss.sigma.clip(0).min(), ss.sigma.max())
-    fig, ax = plt.subplots()
-
-    ax.scatter(
-        correct_ss.sigma,
-        correct_ss.prediction_probas.max(axis=1),
-        c="green", alpha=alpha, marker=MARKER, label="Correct", s=marker_size
-    )
-    ax.scatter(
-        incorrect_ss.sigma,
-        incorrect_ss.prediction_probas.max(axis=1),
-        c="red", alpha=alpha, marker=MARKER, label="Incorrect", s=marker_size
-    )
-    if overlay_ss:
-        overlay_correct_ss = overlay_ss.get_indices(overlay_ss.labels == overlay_ss.predictions)
-        overlay_incorrect_ss = overlay_ss.get_indices(overlay_ss.labels != overlay_ss.predictions)
-        ax.scatter(
-            overlay_correct_ss.sigma,
-            overlay_correct_ss.prediction_probas.max(axis=1),
-            c="blue", marker="*", label="Correct Event" + ("" if overlay_incorrect_ss.n_samples == 1 else "s"),
-            s=marker_size*1.25
-        )
-        ax.scatter(
-            overlay_incorrect_ss.sigma,
-            overlay_incorrect_ss.prediction_probas.max(axis=1),
-            c="black", marker="+", label="Incorrect Event" + ("" if overlay_incorrect_ss.n_samples == 1 else "s"),
-            s=marker_size*1.25
-        )
-    if sigma_line_value:
-        ax.vlines(
-            sigma_line_value,
-            0,
-            1,
-            colors="blue",
-            alpha=alpha,
-            label="{}-sigma".format(sigma_line_value),
-            linestyles="dashed"
-        )
-
-    ax.set_xscale(xscale)
-    ax.set_yscale(yscale)
-    ax.set_xlim(xlim)
-    ax.set_ylim(ylim)
-    ax.set_xlabel("Sigma (net / sqrt(background))")
-    ax.set_ylabel("Score")
-    ax.set_title(title)
-    ax.legend()
+    ax.legend(loc="lower right")
 
     return fig, ax
 
 
 @save_or_show_plot
 def plot_snr_vs_score(ss: SampleSet, overlay_ss: SampleSet = None, alpha: float = 0.5,
                       marker_size=75, xscale: str = "log", yscale: str = "linear",
                       xlim: tuple = (None, None), ylim: tuple = (0, 1.05),
-                      title: str = "SNR vs. Score"):
+                      title: str = "SNR vs. Score", figsize=(6.4, 4.8), target_level="Isotope"):
     """Plots SNR against prediction score for all samples in a SampleSet.
 
-    Prediction and label information is used to distinguish between correct
-    and incorrect classifications using color (green for correct, red for incorrect).
+    Prediction and label information is used to distinguish between correct and incorrect
+    classifications using color (green for correct, red for incorrect).
 
     Args:
-        ss: a SampleSet of events to plot.
-        overlay_ss: another SampleSet to color as blue (correct) and/or black (incorrect).
-        alpha: the degree of opacity (not applied to overlay_ss scatterplot if used).
-        xscale: the X-axis scale.
-        yscale: the Y-axis scale.
-        xlim: a tuple containing the X-axis min and max values.
-        ylim: a tuple containing the Y-axis min and max values.
-        title: the plot title.
+        ss: Defines a SampleSet of events to plot.
+        overlay_ss: Defines another SampleSet to color as blue (correct) and/or black (incorrect).
+        alpha: Defines the degree of opacity (not applied to overlay_ss scatterplot if used).
+        xscale: Defines the x-axis scale.
+        yscale: Defines the y-axis scale.
+        xlim: Defines a tuple containing the x-axis min and max values.
+        ylim: Defines a tuple containing the y-axis min and max values.
+        title: Defines the plot title.
+        figsize: Width, height of figure in inches.
+        target_level: The level of the sources multi index to use for comparing correctness.
 
     Returns:
         A tuple (Figure, Axes) of matplotlib objects.
 
-    Raises:
-        None
     """
-    correct_ss = ss.get_indices(ss.labels == ss.predictions)
-    incorrect_ss = ss.get_indices(ss.labels != ss.predictions)
+    labels = ss.get_labels(target_level=target_level)
+    predictions = ss.get_predictions(target_level=target_level, level_aggregation=None)
+    correct_ss = ss[labels == predictions]
+    incorrect_ss = ss[labels != predictions]
     if not xlim:
         if xscale == "log":
-            xlim = (ss.snr_estimate.clip(1e-3).min(), ss.snr_estimate.max())
+            xlim = (ss.info.snr.clip(1e-3).min(), ss.info.snr.max())
         else:
-            xlim = (ss.snr_estimate.clip(0).min(), ss.snr_estimate.max())
-    fig, ax = plt.subplots()
+            xlim = (ss.info.snr.clip(0).min(), ss.info.snr.max())
 
+    fig, ax = plt.subplots(figsize=figsize)
     ax.scatter(
-        correct_ss.snr_estimate,
+        correct_ss.info.snr,
         correct_ss.prediction_probas.max(axis=1),
         c="green", alpha=alpha, marker=MARKER, label="Correct", s=marker_size
     )
     ax.scatter(
-        incorrect_ss.snr_estimate,
+        incorrect_ss.info.snr,
         incorrect_ss.prediction_probas.max(axis=1),
         c="red", alpha=alpha, marker=MARKER, label="Incorrect", s=marker_size
     )
     if overlay_ss:
-        overlay_correct_ss = overlay_ss.get_indices(overlay_ss.labels == overlay_ss.predictions)
-        overlay_incorrect_ss = overlay_ss.get_indices(overlay_ss.labels != overlay_ss.predictions)
+        overlay_labels = overlay_ss.get_labels()
+        overlay_predictions = overlay_ss.get_predictions()
+        overlay_correct_ss = overlay_ss[overlay_labels == overlay_predictions]
+        overlay_incorrect_ss = overlay_ss[overlay_labels != overlay_predictions]
         ax.scatter(
-            overlay_correct_ss.snr_estimate,
+            overlay_correct_ss.info.snr,
             overlay_correct_ss.prediction_probas.max(axis=1),
-            c="blue", marker="*", label="Correct Event" + ("" if overlay_correct_ss.n_samples == 1 else "s"),
+            c="blue",
+            marker="*",
+            label="Correct Event" + ("" if overlay_correct_ss.n_samples == 1 else "s"),
             s=marker_size*1.25
         )
         ax.scatter(
-            overlay_incorrect_ss.snr_estimate,
+            overlay_incorrect_ss.info.snr,
             overlay_incorrect_ss.prediction_probas.max(axis=1),
-            c="black", marker="+", label="Incorrect Event" + ("" if overlay_incorrect_ss.n_samples == 1 else "s"),
+            c="black",
+            marker="+",
+            label="Incorrect Event" + ("" if overlay_incorrect_ss.n_samples == 1 else "s"),
             s=marker_size*1.25
         )
 
     ax.set_xscale(xscale)
     ax.set_yscale(yscale)
     ax.set_xlim(xlim)
     ax.set_ylim(ylim)
@@ -361,69 +286,67 @@
     ax.set_title(title)
     ax.legend()
 
     return fig, ax
 
 
 @save_or_show_plot
-def plot_spectra(ss: SampleSet, is_in_energy: bool = False, limit: int = None,
-                 figsize: tuple = None, xscale: str = "linear", yscale: str = "log",
-                 xlim: tuple = (0, None), ylim: tuple = (1e-1, None),
-                 ylabel: str = None, title: str = None, legend_loc: str = None) -> tuple:
+def plot_spectra(ss: SampleSet, in_energy: bool = False,
+                 figsize: tuple = (12.8, 7.2), xscale: str = "linear", yscale: str = "log",
+                 xlim: tuple = (None, None), ylim: tuple = (None, None),
+                 ylabel: str = None, title: str = None, legend_loc: str = None,
+                 target_level="Isotope") -> tuple:
     """Plots the spectra contained with a SampleSet.
 
     Args:
-        ss: spectra to plot.
-        is_in_energy: whether or not to try and use each spectrum's
-            energy bin values to convert the spectrum from bins to energy.
-        limit: the number of spectra to plot; None will plot all.
-        figsize: the figure size passed to the matplotlib subplots call.
-        xscale: the X-axis scale.
-        yscale: the Y-axis scale.
-        xlim: a tuple containing the X-axis min and max values.
-        ylim: a tuple containing the Y-axis min and max values.
-        ylabel: the Y-axis label.
-        title: the plot title.
-        legend_loc: the location in which to place the legend. Defaults to None.
+        ss: Defines spectra to plot.
+        in_energy: Determines whether or not to try and use each spectrum's
+            energy calibration to interpet bins in terms of energy.
+        figsize: Width, height of figure in inches.
+        xscale: Defines the x-axis scale.
+        yscale: Defines the y-axis scale.
+        xlim: Defines a tuple containing the x-axis min and max values.
+        ylim: Defines a tuple containing the y-axis min and max values.
+        ylabel: Defines the y-axis label.
+        title: Defines the plot title.
+        legend_loc: Defines the location in which to place the legend. Defaults to None.
+        target_level: The level of the sources multi index to use for legend labels.
 
     Returns:
         A tuple (Figure, Axes) of matplotlib objects.
 
     Raises:
-        ValueError: is_in_energy=True but energy bin centers are missing for any spectra.
-        ValueError: limit is not None and less than 1.
-    """
-    if is_in_energy and pd.isnull(ss.energy_bin_centers.reshape(-1)).any():
-        msg = "When using 'is_in_energy' a valid energy calibration is required."
-        raise ValueError(msg)
-    if limit and limit < 1:
-        raise ValueError("'limit' argument can not be less than 1.")
+        ValueError: Raised if is_in_energy=True but energy bin centers are missing for any spectra.
+        ValueError: Raised if limit is not None and less than 1.
 
-    if limit:
-        ss = ss.get_indices(range(limit))
+    """
     fig, ax = plt.subplots(figsize=figsize)
-    for i in range(len(ss.spectra.index)):
-        label = ss.labels[i]
+    if ss.sources.empty:
+        labels = list(range(ss.n_samples))
+    else:
+        labels = ss.get_labels(target_level=target_level)
 
-        if is_in_energy:
-            xvals = ss.energy_bin_centers[i, :]
+    for i in range(ss.n_samples):
+        label = labels[i]
+        if in_energy:
+            xvals = ss.get_channel_energies(i)
         else:
             xvals = np.arange(ss.n_channels)
         ax.plot(
             xvals,
             ss.spectra.iloc[i],
             label=label,
-            color=CM(i),
+            color=CM(i % CM.N),
         )
 
     ax.set_xscale(xscale)
     ax.set_yscale(yscale)
     ax.set_xlim(xlim)
     ax.set_ylim(ylim)
-    if is_in_energy:
+    if in_energy:
         if xscale == "log":
             ax.set_xlabel("log(Energy (keV))")
         else:
             ax.set_xlabel("Energy (keV)")
     else:
         if xscale == "log":
             ax.set_xlabel("log(Channel)")
@@ -448,33 +371,34 @@
 
 
 @save_or_show_plot
 def plot_learning_curve(train_loss: list, validation_loss: list,
                         xscale: str = "linear", yscale: str = "linear",
                         xlim: tuple = (0, None), ylim: tuple = (0, None),
                         ylabel: str = "Loss", legend_loc: str = "upper right",
-                        smooth: bool = False, title: str = None) -> tuple:
+                        smooth: bool = False, title: str = None, figsize=(6.4, 4.8)) -> tuple:
     """Plots training and validation loss curves.
 
     Args:
-        train_loss: list of training loss values.
-        validation_loss: list of validation loss values.
-        xscale: the X-axis scale.
-        yscale: the Y-axis scale.
-        xlim: a tuple containing the X-axis min and max values.
-        ylim: a tuple containing the Y-axis min and max values.
-        smooth: whether or not to apply smoothing to the loss curves.
-        title: the plot title.
+        train_loss: Defines a list of training loss values.
+        validation_loss: Defines a list of validation loss values.
+        xscale: Defines the x-axis scale.
+        yscale: Defines the y-axis scale.
+        xlim: Defines a tuple containing the x-axis min and max values.
+        ylim: Defines a tuple containing the y-axis min and max values.
+        smooth: Determines whether or not to apply smoothing to the loss curves.
+        title: Defines the plot title.
+        figsize: Width, height of figure in inches.
 
     Returns:
         A tuple (Figure, Axes) of matplotlib objects.
 
     Raises:
-        ValueError:
-            - if either list of values is empty
+        ValueError: Raised if either list of values is empty.
+
     """
     train_loss = np.array(train_loss)
     validation_loss = np.array(validation_loss)
     if train_loss.size == 0:
         raise ValueError("List of training loss values was not provided.")
     if validation_loss.size == 0:
         raise ValueError("List of validation loss values was not provided.")
@@ -489,15 +413,15 @@
     if isinstance(validation_loss[0], (list, tuple)):
         val_x = np.array([ep for ep, _ in validation_loss])
         val_y = np.array([lv for _, lv in validation_loss])
     else:
         val_x = np.arange(len(validation_loss))
         val_y = np.array([lv for lv in validation_loss])
 
-    fig, ax = plt.subplots()
+    fig, ax = plt.subplots(figsize=figsize)
     if smooth:
         from scipy.interpolate import make_interp_spline
 
         # The 300 one the next line is the number of points to make between min and max
         train_xnew = np.linspace(train_x.min(), train_x.max(), 50)
         spl = make_interp_spline(train_x, train_y, k=3)
         train_ps = spl(train_xnew)
@@ -529,34 +453,33 @@
 
     return fig, ax
 
 
 @save_or_show_plot
 def plot_count_rate_history(cr_history: list, sample_interval: float,
                             event_duration: float, pre_event_duration: float,
-                            ylim: tuple = (0, None), title: str = None):
+                            ylim: tuple = (0, None), title: str = None, figsize=(6.4, 4.8)):
     """Plots a count rate history.
 
     Args:
-        cr_history: list of count rate values.
-        sample_interval: the time in seconds for which each count rate values was collected.
-        event_duration: the time in seconds during which an anomalous source was present.
-        pre_event_duration: the time in seconds at which the anomalous source appears
+        cr_history: Defines a list of count rate values.
+        sample_interval: Defines the time in seconds for which each count rate values was collected.
+        event_duration: Defines the time in seconds during which an anomalous source was present.
+        pre_event_duration: Defines the time in seconds at which the anomalous source appears
             (i.e., the start of the event).
-        validation_loss: list of validation loss values.
-        ylim: a tuple containing the Y-axis min and max values.
-        title: the plot title.
+        validation_loss: Defines a list of validation loss values.
+        ylim: Defines a tuple containing the y-axis min and max values.
+        title: Defines the plot title.
+        figsize: Width, height of figure in inches.
 
     Returns:
         A tuple (Figure, Axes) of matplotlib objects.
 
-    Raises:
-        None
     """
-    fig, ax = plt.subplots()
+    fig, ax = plt.subplots(figsize=figsize)
 
     time_steps = np.arange(
         start=-pre_event_duration,
         stop=len(cr_history) * sample_interval - pre_event_duration,
         step=sample_interval
     )
     ax.plot(
@@ -578,149 +501,340 @@
     else:
         ax.set_title("Count Rate History")
 
     return fig, ax
 
 
 @save_or_show_plot
-def plot_score_histogram(ss: SampleSet, yscale="log", ylim=(1e-1, None),
-                         title="Score Distribution"):
+def plot_score_distribution(ss: SampleSet, bin_width=None, n_bins=100,
+                            xscale="linear", min_bin=0.0, max_bin=1.0,
+                            yscale="log", ylim=(1e-1, None),
+                            title="Score Distribution", figsize=(6.4, 4.8)):
     """Plots a histogram of all of the model prediction scores.
 
     Args:
         ss: SampleSet containing prediction_probas values.
-        yscale: the Y-axis scale.
-        ylim: a tuple containing the Y-axis min and max values.
+        bin_width: width of each bin
+        n_bins: number of bins into which to bin scores.
+        xscale: the x-axis scale.
+        min_bin: min value of the bin range; also sets x-axis min.
+        max_bin: max value of the bin range; also sets x-axis max.
+        yscale: the y-axis scale.
+        ylim: a tuple containing the y-axis min and max values.
         title: the plot title.
+        figsize: Width, height of figure in inches.
 
     Returns:
         A tuple (Figure, Axes) of matplotlib objects.
 
-    Raises:
-        None
     """
-    fig, ax = plt.subplots()
+    fig, ax = plt.subplots(figsize=figsize)
 
-    indices1 = ss.collection_information.index[ss.collection_information["sigma"] <= 5]
-    values1 = ss.prediction_probas.loc[indices1].values.flatten()
-    values1 = np.where(values1 > 0.0, values1, values1)
-    indices2 = ss.collection_information.index[(ss.collection_information["sigma"] > 5) &
-                                               (ss.collection_information["sigma"] <= 50)]
-    values2 = ss.prediction_probas.loc[indices2].values.flatten()
-    values2 = np.where(values2 > 0.0, values2, values2)
-    indices3 = ss.collection_information.index[ss.collection_information["sigma"] > 50]
-    values3 = ss.prediction_probas.loc[indices3].values.flatten()
-    values3 = np.where(values3 > 0.0, values3, values3)
-
-    width = 0.35
-    bins = np.linspace(0.0, 1.0, 100)
-    ax.bar(
-        values3,
-        bins,
-        width,
-        color="green"
-    )
-    ax.bar(
-        values2,
-        bins,
-        width,
-        color="yellow"
-    )
-    ax.bar(
-        values1,
-        bins,
-        width,
-        color="red"
-    )
+    scores = ss.prediction_probas.values.flatten()
+
+    BINS = np.linspace(min_bin, max_bin, n_bins)
+    ax.hist(scores, bins=BINS, rwidth=bin_width)
 
+    ax.set_xscale(xscale)
+    ax.set_xlim((min_bin, max_bin))
     ax.set_yscale(yscale)
     ax.set_ylim(ylim)
     ax.set_xlabel("Scores")
     ax.set_ylabel("Occurrences")
     ax.set_title(title)
+    fig.tight_layout()
 
     return fig, ax
 
 
+def _bin_df_values_and_plot(data: pd.Series, fig, ax):
+    binned_labels = data.value_counts()
+    binned_labels.sort_index(inplace=True)
+    binned_labels.plot(kind="bar", subplots=True, fig=fig, ax=ax)
+
+
 @save_or_show_plot
-def plot_n_isotopes_vs_f1_bayes(ss: SampleSet, seeds: SampleSet, title="Number of Isotopes vs. F1 Score"):
-    """Plots the F1 score for different numbers of isotopes under consideration,
-    specifically for a PoissonBayes model.
+def plot_label_distribution(ss: SampleSet, ylim: tuple = (1, None),
+                            yscale: str = "log", figsize: tuple = (12.8, 7.2),
+                            title: str = "Label Distribution",
+                            target_level: str = "Isotope"):
+    """Plots a histogram of number of ooccurences for each prediction.
 
     Args:
-        ss: SampleSet containing prediction_probas values.
-        seeds: the same seeds that were used by the PoissonBayes model.
-        title: the plot title.
+        ss: a SampleSet with prediction information filled in.
+        ylim: tuple containing the y-axis min and max values.
+        yscale: scale of y-axis.
+        figsize: width, height of figure in inches.
+        target_level: level of the multi index to use for x-axis labels.
 
     Returns:
         A tuple (Figure, Axes) of matplotlib objects.
 
-    Raises:
-        None
     """
-    n_to_sample = 20
-    isotopes = np.array(list(set(seeds.labels)))
-    isotope_to_index = {isotope: [] for isotope in isotopes}
-
-    for i in range(seeds.labels.shape[0]):
-        isotope_to_index[seeds.labels[i]].append(i)
-
-    f1_scores = np.zeros((isotopes.shape[0] - 1,))
-    for n in range(1, isotopes.shape[0]):
-        inds = [choice(isotopes.shape[0], n + 1, replace=False) for _ in
-                range(min(n_to_sample, comb(isotopes.shape[0], n, exact=True)))]
-        for j in inds:
-            # the isotopes we are considering this iteration
-            curr_isotopes = isotopes[j]
-            assert len(j) == n + 1
-            proba_indicies = []
-            for iso in curr_isotopes:
-                proba_indicies += isotope_to_index[iso]
-            proba_indicies.sort()
-
-            # get the isotopes, whose correct label is in the set of isotopes we are considering
-            i_labels = range(ss.labels.shape[0])
-            all_proba_indicies = [i for i in i_labels if ss.labels[i] in curr_isotopes]
-            # get probas that we need
-            curr_probas = ss.prediction_probas.values[all_proba_indicies]
-            curr_probas = curr_probas[:, proba_indicies]
-            max_indicies = curr_probas.argmax(axis=1)
-            predictions = [seeds.labels[proba_indicies[i]] for i in max_indicies]
-            labels = ss.labels[all_proba_indicies]
-            f1_scores[n - 1] += (f1_score(labels, predictions, average="micro"))
+    fig, ax = plt.subplots(figsize=figsize)
 
-        f1_scores[n - 1] /= len(inds)
+    labels = ss.get_labels(target_level=target_level)
+    _bin_df_values_and_plot(labels, fig, ax)
 
-    fig, ax = plt.subplots()
-    plt.plot(np.arange(2, f1_scores.shape[0] + 2), f1_scores)
-    ax.set_ylim((0, 1.1))
-    ax.set_xlabel("Number of Isotopes")
-    ax.set_ylabel("F1-Score")
+    ax.set_ylim(ylim)
+    ax.set_yscale(yscale)
     ax.set_title(title)
+
     return fig, ax
 
 
 @save_or_show_plot
-def plot_n_isotopes_vs_f1(f1_scores: list, title: str = "Number of Isotopes vs. F1 Score"):
-    """Plots the pre-computed F1 score for different numbers of isotopes under consideration.
+def plot_prediction_distribution(ss: SampleSet, ylim: tuple = (1, None),
+                                 yscale: str = "log", figsize: tuple = (12.8, 7.2),
+                                 title: str = "Prediction Distribution",
+                                 target_level: str = "Isotope"):
+    """Plots a histogram of number of ooccurences for each prediction.
 
     Args:
-        f1_scores: list of pre-computed F1 scores.
-        title: the plot title.
+        ss: a SampleSet with prediction information filled in.
+        ylim: tuple containing the y-axis min and max values.
+        yscale: scale of y-axis.
+        figsize: width, height of figure in inches.
+        target_level: level of the multi index to use for x-axis labels.
 
     Returns:
         A tuple (Figure, Axes) of matplotlib objects.
 
-    Raises:
-        None
     """
-    fig, ax = plt.subplots()
-    ax.plot([x for x in range(1, len(f1_scores)+1)], f1_scores)
-    ax.set_ylim((0, 1.1))
-    ax.set_xlabel("Number of Isotopes")
-    ax.set_ylabel("F1-Score")
+    fig, ax = plt.subplots(figsize=figsize)
+
+    labels = ss.get_predictions(target_level=target_level)
+    _bin_df_values_and_plot(labels, fig, ax)
+
+    ax.set_ylim(ylim)
+    ax.set_yscale(yscale)
     ax.set_title(title)
+
+    return fig, ax
+
+
+@save_or_show_plot
+def plot_label_and_prediction_distributions(ss: SampleSet, ylim: tuple = (1, None),
+                                            yscale: str = "log", figsize: tuple = (12.8, 7.2),
+                                            title: str = "Label and Prediction Distribution",
+                                            target_level: str = "Isotope"):
+    """Plots a histogram of number of ooccurences for each label and prediction.
+
+    Args:
+        ss: a SampleSet with label and prediction information filled in.
+        ylim: tuple containing the y-axis min and max values.
+        yscale: scale of y-axis.
+        figsize: width, height of figure in inches.
+        target_level: level of the multi index to use for x-axis labels.
+
+    Returns:
+        A tuple (Figure, Axes) of matplotlib objects.
+
+    """
+    fig, ax = plt.subplots(figsize=figsize)
+
+    labels = ss.get_labels(target_level=target_level)
+    binned_labels = labels.value_counts()
+    predictions = ss.get_predictions(target_level=target_level)
+    binned_predictions = predictions.value_counts()
+
+    binned_labels_and_predictions = pd.DataFrame(
+        [binned_labels, binned_predictions],
+        index=["Labels", "Predictions"]).T.fillna(0.0)
+    binned_labels_and_predictions.sort_index(inplace=True)
+
+    binned_labels.plot(kind="bar", subplots=True, fig=fig, ax=ax)
+
+    ax.set_ylim(ylim)
+    ax.set_yscale(yscale)
+    ax.set_title(title)
+    ax.set_xlabel(target_level)
+    ax.set_ylabel("Occurences")
+    fig.tight_layout()
+
+    return fig, ax
+
+
+@save_or_show_plot
+def plot_correlation_between_all_labels(ss: SampleSet, mean: bool = False,
+                                        figsize=(6.4, 4.8), target_level: str = "Isotope"):
+    """Plots a correlation matrix of each label against each other label.
+
+    Args:
+        ss: a SampleSet
+        mean: if true, plot the mean correlation of all enumerations of seeds, otherwise plot the
+            max correlation
+        figsize: Width, height of figure in inches.
+        target_level: The level of the sources multi index to use for legend labels.
+
+    Returns:
+        A tuple (Figure, Axes) of matplotlib objects.
+
+    """
+    labels = ss.get_labels(target_level=target_level)
+    X = np.zeros((len(labels), len(labels)))
+    for i, label1 in enumerate(labels):
+        spectra1 = ss[labels == label1].spectra
+        for j, label2 in enumerate(labels):
+            spectra2 = ss[labels == label2].spectra
+            cur_corr = spectra1.dot(spectra2.T).values
+            if mean:
+                X[i, j] = np.mean(cur_corr)
+            else:
+                X[i, j] = np.max(cur_corr)
+    X = pd.DataFrame(X, index=labels, columns=labels)
+
+    fig, ax = plt.subplots(figsize=figsize)
+    ax = heatmap(X, annot=False)
+    ax.set_title(f"{'Mean' if mean else 'Max'} Correlation for Seeds")
+    return fig, ax
+
+
+@save_or_show_plot
+def plot_precision_recall(precision, recall, marker="D", lw=2, show_legend=True, fig_ax=None,
+                          title="Precision VS Recall", cmap="gist_ncar",
+                          label_plot_kwargs_map=None, figsize=(6.4, 4.8)):
+    """Plots the multi-class or multi-label Precision-Recall curve and marks the optimal
+    F1 score for each class.
+
+    Per-class average precision (AP) and mean average precision (mAP) are annotated on
+    the plot.
+
+    Args:
+        precision: precision dict output of utils.precision_recall_curve()
+        recall: precision dict output of utils.precision_recall_curve()
+        marker: the marker to use to mark the optimal F1 score point
+        lw: the plot line width
+        show_legend: whether or not to display a legend
+        fig_ax: optional tuple of (fig, ax) to plot on, if provided decreasing precision function
+        title: the plot title
+        cmap: the colormap to choose line colors (per label) from
+        label_plot_kwargs_map: optional dictionary of (label, plot kwargs) mappings
+            that will override the plot kwargs for the given label
+        figsize: Width, height of figure in inches.
+
+    """
+    from riid.models.metrics import average_precision_score, harmonic_mean
+
+    fig, ax = fig_ax if fig_ax else plt.subplots(figsize=figsize)
+
+    labels = [label for label in recall if label != "micro"]
+    micro = ["micro"] if "micro" in recall else []
+
+    average_precision = average_precision_score(precision, recall)
+    mAP = np.mean([average_precision[label] for label in labels])
+
+    # create F-score reference lines
+    f_scores = np.linspace(0.2, 0.8, num=4)
+    for f_score in f_scores:
+        x = np.linspace(0.01, 1)
+        y = f_score * x / (2 * x - f_score)
+        ax.plot(x[y >= 0], y[y >= 0], color="gray", alpha=0.2)
+        ax.annotate(f"f1={f_score:0.1f}", xy=(0.85, y[45] + 0.02))
+
+    # plot each label
+    for label in labels + micro:
+        f1_score = harmonic_mean(recall[label], precision[label])
+        optimal_f1_idx = np.argmax(f1_score)
+        optimal_f1 = f1_score[optimal_f1_idx]
+
+        plot_kwargs = dict(lw=lw, marker=marker)
+
+        if label == "micro":
+            plot_kwargs.update(
+                dict(
+                    color="k",
+                    linestyle=":",
+                    label=f"micro-average (AP:{average_precision[label]:0.2f} "
+                          f"F1*:{optimal_f1:.2f})",
+                )
+            )
+        else:
+            plot_kwargs.update(
+                dict(
+                    label=f"{label} (AP:{average_precision[label]:0.2f} "
+                          f"F1*:{optimal_f1:.2f})",
+                    color=_choose_color(label, cmap=cmap)
+                )
+            )
+
+        if label_plot_kwargs_map and label in label_plot_kwargs_map:
+            plot_kwargs.update(label_plot_kwargs_map[label])
+
+        ax.plot(
+            recall[label],
+            precision[label],
+            markevery=[optimal_f1_idx],
+            **plot_kwargs,
+        )
+
+    ax.set_xlim([0.0, 1.0])
+    ax.set_ylim([0.0, 1.05])
+    ax.set_xlabel("Recall")
+    ax.set_ylabel("Precision")
+    ax.set_title(f"{title} (mAP: {mAP:.3f})")
+    if show_legend:
+        ax.legend(loc="lower left", prop=dict(size=8))
+
+    return fig, ax
+
+
+@save_or_show_plot
+def plot_ss_comparison(info_stats1: dict, info_stats2: dict, col_comparisons: dict,
+                       target_col: str = None, title: str = None, x_label: str = None,
+                       distance_precision: int = 3):
+    """Creates a plot for output from SampleSet.compare_to().
+    Args:
+        info_stats1: stats for first SampleSet
+        info_stats2: stats for second SampleSet
+        col_comparisons: Jensen-Shannon distance for each info column histogram
+        target_col: the SampleSet.info column that will be plotted
+        title: the plot title
+        distance_precision: number of decimals to include for distance metric value
+
+    Returns:
+        A tuple (Figure, Axes) of matplotlib objects.
+    """
+    fig, ax = plt.subplots()
+
+    if info_stats1[target_col]["density"]:
+        ax.set_ylabel("Density")
+    else:
+        ax.set_ylabel("Count")
+
+    if x_label:
+        ax.set_xlabel(x_label)
+        xlbl = x_label
+    else:
+        ax.set_xlabel(target_col)
+        xlbl = target_col
+
+    dist_value = col_comparisons[target_col]
+    if title:
+        ax.set_title(f"{title}\nJ-S Distance: {round(dist_value, distance_precision)}")
+    else:
+        ax.set_title(f"Histogram of {xlbl} Occurrences"
+                     f"\nJ-S Distance: {round(dist_value, distance_precision)}")
+
+    stats1 = info_stats1[target_col]
+    bin_width = stats1["bins"][1] - stats1["bins"][0]
+    ax.bar(stats1["bins"][:-1], stats1["hist"], label="hist. 1", width=bin_width)
+
+    stats2 = info_stats2[target_col]
+    bin_width = stats2["bins"][1] - stats2["bins"][0]
+    ax.bar(stats2["bins"][:-1], stats2["hist"], label="hist. 2", width=bin_width)
+
+    ax.legend()
+
     return fig, ax
 
 
 class EmptyPredictionsArrayError(Exception):
     pass
+
+
+def _choose_color(label, cmap="gist_ncar", hashfunc=hashlib.md5):
+    """Chooses a random color based by hashing the label, such that the same color is
+    always chosen for that label."""
+    colormap = plt.get_cmap(cmap)
+    hash_val = int(hashfunc(str(label).encode()).hexdigest(), 16)
+    return colormap(hash_val % colormap.N)
```

### Comparing `riid-1.0.2/setup.py` & `riid-2.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,79 @@
-# Copyright 2021 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
-# Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
-"""Simple setup script for installing the core package.
-"""
-from os import path
-from setuptools import find_packages, setup
+[build-system]
+requires = ["setuptools >= 66", "wheel"]
+build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+packages = ["riid"]
 
-p = path.abspath(path.dirname(__file__))
-with open(path.join(p, './README.md')) as f:
-    README = f.read()
+[project]
+name = "riid"
+description = "Machine learning-based models and utilities for radioisotope identification"
+version = "2.0.0"
+maintainers = [
+    {name="Tyler Morrow", email="tmorro@sandia.gov"},
+]
+authors = [
+    {name="Tyler Morrow"},
+    {name="Nathan Price"},
+    {name="Travis McGuire"},
+    {name="Tyler Ganter"},
+    {name="Aislinn Handley"},
+    {name="Paul Thelen"},
+    {name="Alan Van Omen"},
+    {name="Leon Ross"},
+    {name="Alyshia Bustos"},
+]
+readme = "README.md"
+license = {file = "LICENSE.md"}
+classifiers = [
+    'Development Status :: 5 - Production/Stable',
+    'Intended Audience :: Developers',
+    'Intended Audience :: Education',
+    'Intended Audience :: Science/Research',
+    'License :: OSI Approved :: BSD License',
+    'Topic :: Scientific/Engineering',
+    'Topic :: Scientific/Engineering :: Mathematics',
+    'Topic :: Scientific/Engineering :: Artificial Intelligence',
+    'Topic :: Software Development',
+    'Topic :: Software Development :: Libraries',
+    'Topic :: Software Development :: Libraries :: Python Modules',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3 :: Only',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+]
+keywords = ["pyriid", "riid", "machine learning", "radioisotope identification", "gamma spectrum"]
 
-setup(
-    name="riid",
-    version="1.0.2",
-    description="Machine learning-based models and utilities for radioisotope identification",
-    long_description=README,
-    long_description_content_type='text/markdown',
-    author="Tyler Morrow,Nathan Price",
-    author_email="tmorro@sandia.gov,njprice@sandia.gov",
-    url="https://github.com/sandialabs/PyRIID",
-    packages=find_packages(),
-    python_requires=">=3.7, <3.8",
-    install_requires=[
-        "tensorflow==2.0.0",
-        "tensorflow-model-optimization==0.1.3",
-        "numpy==1.17.4",
-        "pandas==1.0.5",
-        "matplotlib==3.1.2",
-        "scikit-learn==0.22",
-        "tables==3.6.1",
-        "tqdm",
-        "seaborn==0.10.1",
-        "h5py<3.0.0",
-    ],
-    # PyPI package information.
-    classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Education',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: BSD License',
-        'Topic :: Scientific/Engineering',
-        'Topic :: Scientific/Engineering :: Mathematics',
-        'Topic :: Scientific/Engineering :: Artificial Intelligence',
-        'Topic :: Software Development',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7'
-    ],
-    license='BSD-3',
-    keywords='pyriid riid machine learning',
-)
+requires-python = ">=3.8,<3.11"
+dependencies = [
+    "jsonschema                     ==4.17.*",
+    "matplotlib                     ==3.7.*",
+    "pyyaml                         ==6.0.*",
+    "seaborn                        ==0.12.*",
+    "tf2onnx                        ==1.14.*",
+    "tqdm                           ==4.65.*",
+    "numpy                          ==1.23.*",
+    "onnxruntime                    ==1.15.*",
+    "pandas                         ==2.0.*",
+    "pythonnet                      ==3.0.*; platform_system == 'Windows'",
+    "tables                         ==3.8.*",
+    "tensorflow                     ==2.12.*",
+    "tensorflow-io                  ==0.27.*",
+    "tensorflow-model-optimization  ==0.7.*",
+    "tensorflow-probability         ==0.20.*",
+    "typeguard                      ==2.7.*",
+    "scikit-learn                   ==1.2.*",
+]
+
+[project.optional-dependencies]
+dev = [
+    "flake8",
+    "flake8-quotes",
+    "coverage",
+    "ipykernel",
+    "tabulate",
+]
+
+[project.urls]
+repository = "https://github.com/sandialabs/PyRIID"
```

