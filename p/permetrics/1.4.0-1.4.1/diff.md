# Comparing `tmp/permetrics-1.4.0.tar.gz` & `tmp/permetrics-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\permetrics-1.4.0.tar", last modified: Thu Jul 27 02:16:17 2023, max compression
+gzip compressed data, was "permetrics-1.4.1.tar", last modified: Fri Aug  4 04:25:06 2023, max compression
```

## Comparing `permetrics-1.4.0.tar` & `permetrics-1.4.1.tar`

### file list

```diff
@@ -1,39 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.638870 permetrics-1.4.0/
--rw-rw-rw-   0        0        0     7065 2023-07-27 02:15:50.000000 permetrics-1.4.0/ChangeLog.md
--rw-rw-rw-   0        0        0    11346 2019-12-06 02:04:06.000000 permetrics-1.4.0/LICENSE
--rw-rw-rw-   0        0        0       38 2023-07-27 02:15:50.000000 permetrics-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0    17802 2023-07-27 02:16:17.638870 permetrics-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    14077 2023-07-27 02:15:50.000000 permetrics-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.550759 permetrics-1.4.0/assets/
--rw-rw-rw-   0        0        0      399 2022-05-23 03:13:19.000000 permetrics-1.4.0/assets/__init__.py
--rw-rw-rw-   0        0        0     1445 2022-04-02 11:00:24.000000 permetrics-1.4.0/assets/check_kld.py
-drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.574753 permetrics-1.4.0/assets/class/
--rw-rw-rw-   0        0        0     7472 2022-05-18 14:02:24.000000 permetrics-1.4.0/assets/class/BC_01_breast_cancer.py
--rw-rw-rw-   0        0        0      953 2022-05-18 08:35:29.000000 permetrics-1.4.0/assets/class/BC_01_coronary_heart_disease.py
--rw-rw-rw-   0        0        0      399 2022-05-23 03:13:09.000000 permetrics-1.4.0/assets/class/__init__.py
--rw-rw-rw-   0        0        0     2609 2022-05-19 15:28:37.000000 permetrics-1.4.0/assets/class/example.py
--rw-rw-rw-   0        0        0     1019 2022-05-18 01:19:52.000000 permetrics-1.4.0/assets/class/fruits_lover_edition.py
--rw-rw-rw-   0        0        0     2960 2022-04-08 11:46:49.000000 permetrics-1.4.0/assets/example.py
--rw-rw-rw-   0        0        0     1280 2022-03-03 13:18:19.000000 permetrics-1.4.0/assets/ga_exam.py
--rw-rw-rw-   0        0        0     1854 2022-03-25 11:44:18.000000 permetrics-1.4.0/assets/test.py
-drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.602968 permetrics-1.4.0/permetrics/
--rw-rw-rw-   0        0        0     1987 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/__init__.py
--rw-rw-rw-   0        0        0    35187 2023-07-25 04:34:31.000000 permetrics-1.4.0/permetrics/classification.py
--rw-rw-rw-   0        0        0    48718 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/clustering.py
--rw-rw-rw-   0        0        0     5095 2022-10-02 08:46:37.000000 permetrics-1.4.0/permetrics/evaluator.py
--rw-rw-rw-   0        0        0    93856 2023-07-25 04:34:31.000000 permetrics-1.4.0/permetrics/regression.py
-drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.637875 permetrics-1.4.0/permetrics/utils/
--rw-rw-rw-   0        0        0      399 2022-05-23 04:40:57.000000 permetrics-1.4.0/permetrics/utils/__init__.py
--rw-rw-rw-   0        0        0    10317 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/utils/classifier_util.py
--rw-rw-rw-   0        0        0     6186 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/utils/cluster_util.py
--rw-rw-rw-   0        0        0     9460 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/utils/data_util.py
--rw-rw-rw-   0        0        0      959 2023-07-27 02:15:50.000000 permetrics-1.4.0/permetrics/utils/encoder.py
--rw-rw-rw-   0        0        0     3025 2023-07-25 04:34:31.000000 permetrics-1.4.0/permetrics/utils/regressor_util.py
-drwxrwxrwx   0        0        0        0 2023-07-27 02:16:17.623911 permetrics-1.4.0/permetrics.egg-info/
--rw-rw-rw-   0        0        0    17802 2023-07-27 02:16:17.000000 permetrics-1.4.0/permetrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      794 2023-07-27 02:16:17.000000 permetrics-1.4.0/permetrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 02:16:17.000000 permetrics-1.4.0/permetrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-27 02:16:17.000000 permetrics-1.4.0/permetrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-27 02:16:17.000000 permetrics-1.4.0/permetrics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 02:16:17.639867 permetrics-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2117 2023-07-27 02:15:50.000000 permetrics-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:25:06.795924 permetrics-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-08-04 04:24:44.000000 permetrics-1.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-08-04 04:24:44.000000 permetrics-1.4.1/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 04:24:44.000000 permetrics-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-04 04:24:44.000000 permetrics-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-08-04 04:25:06.795924 permetrics-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   340278 2023-08-04 04:24:44.000000 permetrics-1.4.1/R-R2-Rsquared.docx
+-rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-08-04 04:24:44.000000 permetrics-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:25:06.791924 permetrics-1.4.1/permetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37300 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72219 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97099 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:25:06.795924 permetrics-1.4.1/permetrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/classifier_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/cluster_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/data_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-04 04:24:44.000000 permetrics-1.4.1/permetrics/utils/regressor_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:25:06.791924 permetrics-1.4.1/permetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-08-04 04:25:06.000000 permetrics-1.4.1/permetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-08-04 04:25:06.000000 permetrics-1.4.1/permetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 04:25:06.000000 permetrics-1.4.1/permetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-04 04:25:06.000000 permetrics-1.4.1/permetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 04:25:06.000000 permetrics-1.4.1/permetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 04:25:06.795924 permetrics-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-04 04:24:44.000000 permetrics-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:25:06.795924 permetrics-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-04 04:24:44.000000 permetrics-1.4.1/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-08-04 04:24:44.000000 permetrics-1.4.1/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-08-04 04:24:44.000000 permetrics-1.4.1/tests/test_regression.py
```

### Comparing `permetrics-1.4.0/permetrics/classification.py` & `permetrics-1.4.1/permetrics/classification.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,651 +1,707 @@
-# !/usr/bin/env python
-# Created by "Thieu" at 09:29, 23/09/2020 ----------%
-#       Email: nguyenthieu2102@gmail.com            %
-#       Github: https://github.com/thieu1995        %
-# --------------------------------------------------%
-
-from permetrics.evaluator import Evaluator
-from permetrics.utils.data_util import *
-from permetrics.utils.classifier_util import *
-import numpy as np
-
-
-class ClassificationMetric(Evaluator):
-    """
-    This is class contains all classification metrics (for both binary and multiple classification problem)
-
-    Notes
-    ~~~~~
-    + Extension of: https://scikit-learn.org/stable/modules/model_evaluation.html#classification-metrics
-    """
-
-    def __init__(self, y_true=None, y_pred=None, decimal=5, **kwargs):
-        """
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            decimal (int): The number of fractional parts after the decimal point
-            **kwargs ():
-        """
-        super().__init__(y_true, y_pred, decimal, **kwargs)
-        if kwargs is None: kwargs = {}
-        self.set_keyword_arguments(kwargs)
-        self.binary = True
-        self.representor = "number"     # "number" or "string"
-        self.le = None  # LabelEncoder
-
-    def get_processed_data(self, y_true=None, y_pred=None, decimal=None):
-        """
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            clean (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred)
-            decimal (int, None): The number of fractional parts after the decimal point
-
-        Returns:
-            y_true_final: y_true used in evaluation process.
-            y_pred_final: y_pred used in evaluation process
-            one_dim: is y_true has 1 dimensions or not
-            decimal: The number of fractional parts after the decimal point
-        """
-        decimal = self.decimal if decimal is None else decimal
-        if (y_true is not None) and (y_pred is not None):
-            y_true, y_pred, binary, representor = format_classification_data(y_true, y_pred)
-        else:
-            if (self.y_true is not None) and (self.y_pred is not None):
-                y_true, y_pred, binary, representor = format_classification_data(self.y_true, self.y_pred)
-            else:
-                raise ValueError("y_true or y_pred is None. You need to pass y_true and y_pred to object creation or function called.")
-        return y_true, y_pred, binary, representor, decimal
-
-    def confusion_matrix(self, y_true=None, y_pred=None, labels=None, normalize=None):
-        """
-        Generate confusion matrix and useful information
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            normalize ('true', 'pred', 'all', None): Normalizes confusion matrix over the true (rows), predicted (columns) conditions or all the population.
-
-        Returns:
-            matrix (np.ndarray): a 2-dimensional list of pairwise counts
-            imap (dict): a map between label and index of confusion matrix
-            imap_count (dict): a map between label and number of true label in y_true
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal=None)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize)
-        return matrix, imap, imap_count
-
-    def precision_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate precision score for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-                If None, the scores for each class are returned. Otherwise, this determines the type of averaging performed on the data:
-
-                ``'micro'``:
-                    Calculate metrics globally by considering each element of the label indicator matrix as a label.
-                ``'macro'``:
-                    Calculate metrics for each label, and find their unweighted mean.  This does not take label imbalance into account.
-                ``'weighted'``:
-                    Calculate metrics for each label, and find their average, weighted by support (the number of true instances for each label).
-
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            precision (float, dict): the precision score
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_precision = np.array([item["precision"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp_global = np.sum(np.diag(matrix))
-            fp_global = fn_global = np.sum(matrix) - tp_global
-            precision = np.round(tp_global / (tp_global + fp_global), decimal)
-        elif average == "macro":
-            precision = np.mean(list_precision)
-        elif average == "weighted":
-            precision = np.dot(list_weights, list_precision) / np.sum(list_weights)
-        else:
-            precision = dict([(label, np.round(item["precision"], decimal)) for label, item in metrics.items()])
-        return precision if type(precision) == dict else np.round(precision, decimal)
-
-    def negative_predictive_value(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate negative predictive value for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            npv (float, dict): the negative predictive value
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_npv = np.array([item["negative_predictive_value"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp_global = tn_global = np.sum(np.diag(matrix))
-            fp_global = fn_global = np.sum(matrix) - tp_global
-            npv = tn_global / (tn_global + fn_global)
-        elif average == "macro":
-            npv = np.mean(list_npv)
-        elif average == "weighted":
-            npv = np.dot(list_weights, list_npv) / np.sum(list_weights)
-        else:
-            npv = dict([(label, np.round(item["negative_predictive_value"], decimal)) for label, item in metrics.items()])
-        return npv if type(npv) == dict else np.round(npv, decimal)
-
-    def specificity_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate specificity score for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            ss (float, dict): the specificity score
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_ss = np.array([item["specificity"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp_global = tn_global = np.sum(np.diag(matrix))
-            fp_global = fn_global = np.sum(matrix) - tp_global
-            ss = tn_global / (tn_global + fp_global)
-        elif average == "macro":
-            ss = np.mean(list_ss)
-        elif average == "weighted":
-            ss = np.dot(list_weights, list_ss) / np.sum(list_weights)
-        else:
-            ss = dict([(label, np.round(item["specificity"], decimal)) for label, item in metrics.items()])
-        return ss if type(ss) == dict else np.round(ss, decimal)
-
-    def recall_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate recall score for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            recall (float, dict): the recall score
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_recall = np.array([item["recall"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp_global = np.sum(np.diag(matrix))
-            fp_global = fn_global = np.sum(matrix) - tp_global
-            recall = tp_global / (tp_global + fn_global)
-        elif average == "macro":
-            recall = np.mean(list_recall)
-        elif average == "weighted":
-            recall = np.dot(list_weights, list_recall) / np.sum(list_weights)
-        else:
-            recall = dict([(label, np.round(item["recall"], decimal)) for label, item in metrics.items()])
-        return recall if type(recall) == dict else np.round(recall, decimal)
-
-    def accuracy_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate accuracy score for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            accuracy (float, dict): the accuracy score
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_accuracy = np.array([item["accuracy"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-        list_tp = np.array([item['tp'] for item in metrics.values()])
-
-        if average == "micro":
-            accuracy = np.sum(list_tp) / np.sum(list_weights)
-        elif average == "macro":
-            accuracy = np.mean(list_accuracy)
-        elif average == "weighted":
-            accuracy = np.dot(list_weights, list_accuracy) / np.sum(list_weights)
-        else:
-            accuracy = dict([(label, np.round(item["precision"], decimal)) for label, item in metrics.items()])
-        return accuracy if type(accuracy) == dict else np.round(accuracy, decimal)
-
-    def f1_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate f1 score for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            f1 (float, dict): the f1 score
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_f1 = np.array([item["f1"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp_global = np.sum(np.diag(matrix))
-            fp_global = fn_global = np.sum(matrix) - tp_global
-            precision = np.round(tp_global / (tp_global + fp_global), decimal)
-            recall = tp_global / (tp_global + fn_global)
-            f1 = (2 * precision * recall) / (precision + recall)
-        elif average == "macro":
-            f1 = np.mean(list_f1)
-        elif average == "weighted":
-            f1 = np.dot(list_weights, list_f1) / np.sum(list_weights)
-        else:
-            f1 = dict([(label, item["f1"]) for label, item in metrics.items()])
-        return f1 if type(f1) == dict else np.round(f1, decimal)
-
-    def f2_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate f2 score for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            f2 (float, dict): the f2 score
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_f2 = np.array([item["f1"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp_global = np.sum(np.diag(matrix))
-            fp_global = fn_global = np.sum(matrix) - tp_global
-            precision = np.round(tp_global / (tp_global + fp_global), decimal)
-            recall = tp_global / (tp_global + fn_global)
-            f2 = (5 * precision * recall) / (4 * precision + recall)
-        elif average == "macro":
-            f2 = np.mean(list_f2)
-        elif average == "weighted":
-            f2 = np.dot(list_weights, list_f2) / np.sum(list_weights)
-        else:
-            f2 = dict([(label, item["f2"]) for label, item in metrics.items()])
-        return f2 if type(f2) == dict else np.round(f2, decimal)
-
-    def fbeta_score(self, y_true=None, y_pred=None, beta=1.0, labels=None, average="macro", decimal=None):
-        """
-        The beta parameter determines the weight of recall in the combined score.
-        beta < 1 lends more weight to precision, while beta > 1 favors recall
-        (beta -> 0 considers only precision, beta -> +inf only recall).
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            beta (float): the weight of recall in the combined score, default = 1.0
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            fbeta (float, dict): the fbeta score
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count, beta=beta)
-
-        list_fbeta = np.array([item["f1"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp_global = np.sum(np.diag(matrix))
-            fp_global = fn_global = np.sum(matrix) - tp_global
-            precision = np.round(tp_global / (tp_global + fp_global), decimal)
-            recall = tp_global / (tp_global + fn_global)
-            fbeta = ((1 + beta ** 2) * precision * recall) / (beta ** 2 * precision + recall)
-        elif average == "macro":
-            fbeta = np.mean(list_fbeta)
-        elif average == "weighted":
-            fbeta = np.dot(list_weights, list_fbeta) / np.sum(list_weights)
-        else:
-            fbeta = dict([(label, item["fbeta"]) for label, item in metrics.items()])
-        return fbeta if type(fbeta) == dict else np.round(fbeta, decimal)
-
-    def matthews_correlation_coefficient(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            mcc (float, dict): the Matthews correlation coefficient
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_mcc = np.array([item["mcc"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp = tn = np.sum(np.diag(matrix))
-            fp = fn = np.sum(matrix) - tp
-            mcc = (tp * tn - fp * fn) / np.sqrt(((tp + fp) * (tp + fn) * (tn + fp) * (tn + fn)))
-        elif average == "macro":
-            mcc = np.mean(list_mcc)
-        elif average == "weighted":
-            mcc = np.dot(list_weights, list_mcc) / np.sum(list_weights)
-        else:
-            mcc = dict([(label, item["mcc"]) for label, item in metrics.items()])
-        return mcc if type(mcc) == dict else np.round(mcc, decimal)
-
-    def hamming_loss(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate hamming loss for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            hl (float, dict): the hamming loss
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_accuracy = np.array([item["accuracy"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-        list_tp = np.array([item['tp'] for item in metrics.values()])
-
-        if average == "micro":
-            hl = 1.0 - np.sum(list_tp) / np.sum(list_weights)
-        elif average == "macro":
-            hl = np.mean(list_accuracy)
-        elif average == "weighted":
-            hl = np.dot(list_weights, list_accuracy) / np.sum(list_weights)
-        else:
-            hl = dict([(label, np.round(item["hamming_loss"], decimal)) for label, item in metrics.items()])
-        return hl if type(hl) == dict else np.round(hl, decimal)
-
-    def lift_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate lift score for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            ls (float, dict): the lift score
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_ls = np.array([item["lift_score"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp = tn = np.sum(np.diag(matrix))
-            fp = fn = np.sum(matrix) - tp
-            ls = (tp/(tp + fp)) / ((tp + fn) / (tp + tn + fp + fn))
-        elif average == "macro":
-            ls = np.mean(list_ls)
-        elif average == "weighted":
-            ls = np.dot(list_weights, list_ls) / np.sum(list_weights)
-        else:
-            ls = dict([(label, np.round(item["lift_score"], decimal)) for label, item in metrics.items()])
-        return ls if type(ls) == dict else np.round(ls, decimal)
-
-    def cohen_kappa_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate Cohen Kappa score for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            cks (float, dict): the Cohen Kappa score
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_kp = np.array([item["kappa_score"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == 'weighted':
-            kappa = np.dot(list_weights, list_kp) / np.sum(list_weights)
-        elif average == 'macro':
-            kappa = np.mean(list_kp)
-        elif average == 'micro':
-            kappa = np.average(list_kp)
-        else:
-            kappa = dict([(label, np.round(item["kappa_score"], decimal)) for label, item in metrics.items()])
-        return kappa if type(kappa) == dict else np.round(kappa, decimal)
-
-    def jaccard_similarity_index(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Generate Jaccard similarity index for multiple classification problem
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            jsi (float, dict): the Jaccard similarity index
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_js = np.array([item["jaccard_similarities"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp = tn = np.sum(np.diag(matrix))
-            fp = fn = np.sum(matrix) - tp
-            js = tp / (tp + fp + fn)
-        elif average == "macro":
-            js = np.mean(list_js)
-        elif average == "weighted":
-            js = np.dot(list_weights, list_js) / np.sum(list_weights)
-        else:
-            js = dict([(label, np.round(item["jaccard_similarities"], decimal)) for label, item in metrics.items()])
-        return js if type(js) == dict else np.round(js, decimal)
-
-    def g_mean_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None):
-        """
-        Calculates the G-mean score between y_true and y_pred.
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
-            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            float, dict: The G-mean score.
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
-        metrics = calculate_single_label_metric(matrix, imap, imap_count)
-
-        list_gm = np.array([item["g_mean"] for item in metrics.values()])
-        list_weights = np.array([item["n_true"] for item in metrics.values()])
-
-        if average == "micro":
-            tp = tn = np.sum(np.diag(matrix))
-            fp = fn = np.sum(matrix) - tp
-            gm = np.sqrt((tp / (tp + fn)) * (tn / (tn + fp)))
-        elif average == "macro":
-            gm = np.mean(list_gm)
-        elif average == "weighted":
-            gm = np.dot(list_weights, list_gm) / np.sum(list_weights)
-        else:
-            gm = dict([(label, np.round(item["g_mean"], decimal)) for label, item in metrics.items()])
-        return gm if type(gm) == dict else np.round(gm, decimal)
-
-    def gini_index(self, y_true=None, y_pred=None, average="macro", decimal=None):
-        """
-        Calculates the Gini index between y_true and y_pred. Higher is better. Range [0, 1]
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
-            average (str, None): {'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            float, dict: The Gini index
-        """
-        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if binary:
-            return calculate_gini(y_true, y_pred)
-        else:
-            # Compute the number of classes and examples
-            num_classes = len(np.unique(y_true))
-            num_examples = len(y_true)
-            # Initialize arrays to store class weights and Gini indices
-            class_weights = np.zeros(num_classes)
-            class_ginis = np.zeros(num_classes)
-            # Compute the Gini index for each class
-            for i in range(num_classes):
-                # Create a binary array indicating whether the example belongs to the current class
-                y_true_binary = np.where(y_true == i, 1, 0)
-                # Compute the Gini index for the current class using the binary array and predicted scores
-                class_ginis[i] = calculate_gini(y_true_binary, y_pred)
-                # Compute the class weight based on the number of examples
-                class_weights[i] = np.sum(y_true_binary) / num_examples
-
-            if average == "macro":
-                result = np.mean(class_ginis)
-            elif average == "weighted":
-                result = np.dot(class_weights, class_ginis) / np.sum(class_weights)
-            else:
-                result = dict([(idx, np.round(class_ginis[idx], decimal)) for idx in range(num_classes)])
-            return result if type(result) == dict else np.round(result, decimal)
-
-    def roc_auc_score(self, y_true=None, y_score=None, average="macro", decimal=5):
-        """
-        Calculates the ROC-AUC score between y_true and y_score.
-
-        Args:
-            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
-            y_score (tuple, list, np.ndarray): a list of predicted scores.
-            average (str, None): {'macro', 'weighted'} or None, default="macro"
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            float, dict: The AUC score.
-        """
-        y_true, y_score, binary, representor = format_y_score(y_true, y_score)
-        if binary:
-            tpr, fpr, thresholds = calculate_roc_curve(y_true, y_score)
-            # Calculate the area under the curve (AUC) using the trapezoidal rule
-            return np.trapz(tpr, fpr)
-        else:
-            list_weights = calculate_class_weights(y_true, y_pred=None, y_score=y_score)
-            # one-vs-all (rest) approach
-            tpr = dict()
-            fpr = dict()
-            thresholds = dict()
-            auc = []
-            n_classes = len(np.unique(y_true))
-            for i in range(n_classes):
-                y_true_i = np.array([1 if y == i else 0 for y in y_true])
-                y_score_i = y_score[:, i]
-                tpr[i], fpr[i], thresholds[i] = calculate_roc_curve(y_true_i, y_score_i)
-                # Calculate the area under the curve (AUC) using the trapezoidal rule
-                auc.append(np.trapz(tpr[i], fpr[i]))
-            if average == "macro":
-                result = np.mean(auc)
-            elif average == "weighted":
-                result = np.dot(list_weights, auc) / np.sum(list_weights)
-            else:
-                result = dict([(idx, np.round(auc[idx], decimal)) for idx in range(n_classes)])
-            return result if type(result) == dict else np.round(result, decimal)
-
-
-    CM = cm = confusion_matrix
-    PS = ps = precision_score
-    NPV = npv = negative_predictive_value
-    RS = rs = recall_score
-    AS = accuracy_score
-    F1S = f1s = f1_score
-    F2S = f2s = f2_score
-    FBS = fbs = fbeta_score
-    SS = ss = specificity_score
-    MCC = mcc = matthews_correlation_coefficient
-    HL = hl = hamming_loss
-    LS = ls = lift_score
-    CKS = cks = cohen_kappa_score
-    JSI = jsi = JSC = jsc = jaccard_similarity_coefficient = jaccard_similarity_index
-    GMS = gms = g_mean_score
-    GINI = gini = gini_index
-    ROC = AUC = RAS = roc = auc = ras = roc_auc_score
+# !/usr/bin/env python
+# Created by "Thieu" at 09:29, 23/09/2020 ----------%
+#       Email: nguyenthieu2102@gmail.com            %
+#       Github: https://github.com/thieu1995        %
+# --------------------------------------------------%
+
+from permetrics.evaluator import Evaluator
+from permetrics.utils.data_util import *
+from permetrics.utils.classifier_util import *
+import numpy as np
+
+
+class ClassificationMetric(Evaluator):
+    """
+    Defines a ClassificationMetric class that hold all classification metrics (for both binary and multiple classification problem)
+
+    + An extension of scikit-learn metrics section, with the addition of many more classification metrics.
+    + https://scikit-learn.org/stable/modules/model_evaluation.html#classification-metrics
+
+    Parameters
+    ----------
+    y_true: tuple, list, np.ndarray, default = None
+        The ground truth values.
+
+    y_pred: tuple, list, np.ndarray, default = None
+        The prediction values.
+
+    decimal: int, default = 5
+        The number of fractional parts after the decimal point
+
+    labels: tuple, list, np.ndarray, default = None
+        List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+
+    average: (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+        If None, the scores for each class are returned. Otherwise, this determines the type of averaging performed on the data:
+
+        ``'micro'``:
+            Calculate metrics globally by considering each element of the label indicator matrix as a label.
+        ``'macro'``:
+            Calculate metrics for each label, and find their unweighted mean.  This does not take label imbalance into account.
+        ``'weighted'``:
+            Calculate metrics for each label, and find their average, weighted by support (the number of true instances for each label).
+    """
+
+    SUPPORT = {
+        "PS": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "NPV": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "RS": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "AS": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "F1S": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "F2S": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "FBS": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "SS": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "MCC": {"type": "max", "range": "[-1, +1]", "best": "1"},
+        "HS": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "CKS": {"type": "max", "range": "[-1, +1]", "best": "1"},
+        "JSI": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "GMS": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "ROC-AUC": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "LS": {"type": "max", "range": "[0, +inf)", "best": "no best"},
+        "GINI": {"type": "min", "range": "[0, 1]", "best": "0"},
+    }
+
+    def __init__(self, y_true=None, y_pred=None, decimal=5, **kwargs):
+        super().__init__(y_true, y_pred, decimal, **kwargs)
+        if kwargs is None: kwargs = {}
+        self.set_keyword_arguments(kwargs)
+        self.binary = True
+        self.representor = "number"     # "number" or "string"
+        self.le = None  # LabelEncoder
+
+    @staticmethod
+    def get_support(name=None, verbose=True):
+        if name == "all":
+            if verbose:
+                for key, value in ClassificationMetric.SUPPORT.items():
+                    print(f"Metric {key} : {value}")
+                return ClassificationMetric.SUPPORT
+        if name not in list(ClassificationMetric.SUPPORT.keys()):
+            raise ValueError(f"ClassificationMetric doesn't support metric named: {name}")
+        else:
+            if verbose:
+                print(f"Metric {name}: {ClassificationMetric.SUPPORT[name]}")
+            return ClassificationMetric.SUPPORT[name]
+
+    def get_processed_data(self, y_true=None, y_pred=None, decimal=None):
+        """
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            clean (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred)
+            decimal (int, None): The number of fractional parts after the decimal point
+
+        Returns:
+            y_true_final: y_true used in evaluation process.
+            y_pred_final: y_pred used in evaluation process
+            one_dim: is y_true has 1 dimensions or not
+            decimal: The number of fractional parts after the decimal point
+        """
+        decimal = self.decimal if decimal is None else decimal
+        if (y_true is not None) and (y_pred is not None):
+            y_true, y_pred, binary, representor = format_classification_data(y_true, y_pred)
+        else:
+            if (self.y_true is not None) and (self.y_pred is not None):
+                y_true, y_pred, binary, representor = format_classification_data(self.y_true, self.y_pred)
+            else:
+                raise ValueError("y_true or y_pred is None. You need to pass y_true and y_pred to object creation or function called.")
+        return y_true, y_pred, binary, representor, decimal
+
+    def confusion_matrix(self, y_true=None, y_pred=None, labels=None, normalize=None, **kwargs):
+        """
+        Generate confusion matrix and useful information
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            normalize ('true', 'pred', 'all', None): Normalizes confusion matrix over the true (rows), predicted (columns) conditions or all the population.
+
+        Returns:
+            matrix (np.ndarray): a 2-dimensional list of pairwise counts
+            imap (dict): a map between label and index of confusion matrix
+            imap_count (dict): a map between label and number of true label in y_true
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal=None)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize)
+        return matrix, imap, imap_count
+
+    def precision_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate precision score for multiple classification problem
+        Higher is better (Best = 1), Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+                If None, the scores for each class are returned. Otherwise, this determines the type of averaging performed on the data:
+
+                ``'micro'``:
+                    Calculate metrics globally by considering each element of the label indicator matrix as a label.
+                ``'macro'``:
+                    Calculate metrics for each label, and find their unweighted mean.  This does not take label imbalance into account.
+                ``'weighted'``:
+                    Calculate metrics for each label, and find their average, weighted by support (the number of true instances for each label).
+
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            precision (float, dict): the precision score
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_precision = np.array([item["precision"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp_global = np.sum(np.diag(matrix))
+            fp_global = fn_global = np.sum(matrix) - tp_global
+            precision = np.round(tp_global / (tp_global + fp_global), decimal)
+        elif average == "macro":
+            precision = np.mean(list_precision)
+        elif average == "weighted":
+            precision = np.dot(list_weights, list_precision) / np.sum(list_weights)
+        else:
+            precision = dict([(label, np.round(item["precision"], decimal)) for label, item in metrics.items()])
+        return precision if type(precision) == dict else np.round(precision, decimal)
+
+    def negative_predictive_value(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate negative predictive value for multiple classification problem
+        Higher is better (Best = 1), Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            npv (float, dict): the negative predictive value
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_npv = np.array([item["negative_predictive_value"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp_global = tn_global = np.sum(np.diag(matrix))
+            fp_global = fn_global = np.sum(matrix) - tp_global
+            npv = tn_global / (tn_global + fn_global)
+        elif average == "macro":
+            npv = np.mean(list_npv)
+        elif average == "weighted":
+            npv = np.dot(list_weights, list_npv) / np.sum(list_weights)
+        else:
+            npv = dict([(label, np.round(item["negative_predictive_value"], decimal)) for label, item in metrics.items()])
+        return npv if type(npv) == dict else np.round(npv, decimal)
+
+    def specificity_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate specificity score for multiple classification problem
+        Higher is better (Best = 1), Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            ss (float, dict): the specificity score
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_ss = np.array([item["specificity"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp_global = tn_global = np.sum(np.diag(matrix))
+            fp_global = fn_global = np.sum(matrix) - tp_global
+            ss = tn_global / (tn_global + fp_global)
+        elif average == "macro":
+            ss = np.mean(list_ss)
+        elif average == "weighted":
+            ss = np.dot(list_weights, list_ss) / np.sum(list_weights)
+        else:
+            ss = dict([(label, np.round(item["specificity"], decimal)) for label, item in metrics.items()])
+        return ss if type(ss) == dict else np.round(ss, decimal)
+
+    def recall_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate recall score for multiple classification problem
+        Higher is better (Best = 1), Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            recall (float, dict): the recall score
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_recall = np.array([item["recall"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp_global = np.sum(np.diag(matrix))
+            fp_global = fn_global = np.sum(matrix) - tp_global
+            recall = tp_global / (tp_global + fn_global)
+        elif average == "macro":
+            recall = np.mean(list_recall)
+        elif average == "weighted":
+            recall = np.dot(list_weights, list_recall) / np.sum(list_weights)
+        else:
+            recall = dict([(label, np.round(item["recall"], decimal)) for label, item in metrics.items()])
+        return recall if type(recall) == dict else np.round(recall, decimal)
+
+    def accuracy_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate accuracy score for multiple classification problem
+        Higher is better (Best = 1), Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            accuracy (float, dict): the accuracy score
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_accuracy = np.array([item["accuracy"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+        list_tp = np.array([item['tp'] for item in metrics.values()])
+
+        if average == "micro":
+            accuracy = np.sum(list_tp) / np.sum(list_weights)
+        elif average == "macro":
+            accuracy = np.mean(list_accuracy)
+        elif average == "weighted":
+            accuracy = np.dot(list_weights, list_accuracy) / np.sum(list_weights)
+        else:
+            accuracy = dict([(label, np.round(item["precision"], decimal)) for label, item in metrics.items()])
+        return accuracy if type(accuracy) == dict else np.round(accuracy, decimal)
+
+    def f1_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate f1 score for multiple classification problem
+        Higher is better (Best = 1), Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            f1 (float, dict): the f1 score
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_f1 = np.array([item["f1"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp_global = np.sum(np.diag(matrix))
+            fp_global = fn_global = np.sum(matrix) - tp_global
+            precision = np.round(tp_global / (tp_global + fp_global), decimal)
+            recall = tp_global / (tp_global + fn_global)
+            f1 = (2 * precision * recall) / (precision + recall)
+        elif average == "macro":
+            f1 = np.mean(list_f1)
+        elif average == "weighted":
+            f1 = np.dot(list_weights, list_f1) / np.sum(list_weights)
+        else:
+            f1 = dict([(label, item["f1"]) for label, item in metrics.items()])
+        return f1 if type(f1) == dict else np.round(f1, decimal)
+
+    def f2_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate f2 score for multiple classification problem
+        Higher is better (Best = 1), Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            f2 (float, dict): the f2 score
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_f2 = np.array([item["f1"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp_global = np.sum(np.diag(matrix))
+            fp_global = fn_global = np.sum(matrix) - tp_global
+            precision = np.round(tp_global / (tp_global + fp_global), decimal)
+            recall = tp_global / (tp_global + fn_global)
+            f2 = (5 * precision * recall) / (4 * precision + recall)
+        elif average == "macro":
+            f2 = np.mean(list_f2)
+        elif average == "weighted":
+            f2 = np.dot(list_weights, list_f2) / np.sum(list_weights)
+        else:
+            f2 = dict([(label, item["f2"]) for label, item in metrics.items()])
+        return f2 if type(f2) == dict else np.round(f2, decimal)
+
+    def fbeta_score(self, y_true=None, y_pred=None, beta=1.0, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        The beta parameter determines the weight of recall in the combined score.
+        beta < 1 lends more weight to precision, while beta > 1 favors recall
+        (beta -> 0 considers only precision, beta -> +inf only recall).
+        Higher is better (Best = 1), Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            beta (float): the weight of recall in the combined score, default = 1.0
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            fbeta (float, dict): the fbeta score
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count, beta=beta)
+
+        list_fbeta = np.array([item["f1"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp_global = np.sum(np.diag(matrix))
+            fp_global = fn_global = np.sum(matrix) - tp_global
+            precision = np.round(tp_global / (tp_global + fp_global), decimal)
+            recall = tp_global / (tp_global + fn_global)
+            fbeta = ((1 + beta ** 2) * precision * recall) / (beta ** 2 * precision + recall)
+        elif average == "macro":
+            fbeta = np.mean(list_fbeta)
+        elif average == "weighted":
+            fbeta = np.dot(list_weights, list_fbeta) / np.sum(list_weights)
+        else:
+            fbeta = dict([(label, item["fbeta"]) for label, item in metrics.items()])
+        return fbeta if type(fbeta) == dict else np.round(fbeta, decimal)
+
+    def matthews_correlation_coefficient(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate Matthews Correlation Coefficient
+        Higher is better (Best = 1), Range = [-1, +1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            mcc (float, dict): the Matthews correlation coefficient
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_mcc = np.array([item["mcc"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp = tn = np.sum(np.diag(matrix))
+            fp = fn = np.sum(matrix) - tp
+            mcc = (tp * tn - fp * fn) / np.sqrt(((tp + fp) * (tp + fn) * (tn + fp) * (tn + fn)))
+        elif average == "macro":
+            mcc = np.mean(list_mcc)
+        elif average == "weighted":
+            mcc = np.dot(list_weights, list_mcc) / np.sum(list_weights)
+        else:
+            mcc = dict([(label, item["mcc"]) for label, item in metrics.items()])
+        return mcc if type(mcc) == dict else np.round(mcc, decimal)
+
+    def hamming_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate hamming score for multiple classification problem
+        Higher is better (Best = 1), Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            hl (float, dict): the hamming score
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_accuracy = np.array([item["accuracy"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+        list_tp = np.array([item['tp'] for item in metrics.values()])
+
+        if average == "micro":
+            hl = 1.0 - np.sum(list_tp) / np.sum(list_weights)
+        elif average == "macro":
+            hl = np.mean(list_accuracy)
+        elif average == "weighted":
+            hl = np.dot(list_weights, list_accuracy) / np.sum(list_weights)
+        else:
+            hl = dict([(label, np.round(item["hamming_score"], decimal)) for label, item in metrics.items()])
+        return hl if type(hl) == dict else np.round(hl, decimal)
+
+    def lift_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate lift score for multiple classification problem
+        Higher is better (Best = +1), Range = [0, +1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            ls (float, dict): the lift score
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_ls = np.array([item["lift_score"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp = tn = np.sum(np.diag(matrix))
+            fp = fn = np.sum(matrix) - tp
+            ls = (tp/(tp + fp)) / ((tp + fn) / (tp + tn + fp + fn))
+        elif average == "macro":
+            ls = np.mean(list_ls)
+        elif average == "weighted":
+            ls = np.dot(list_weights, list_ls) / np.sum(list_weights)
+        else:
+            ls = dict([(label, np.round(item["lift_score"], decimal)) for label, item in metrics.items()])
+        return ls if type(ls) == dict else np.round(ls, decimal)
+
+    def cohen_kappa_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate Cohen Kappa score for multiple classification problem
+        Higher is better (Best = +1), Range = [-1, +1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            cks (float, dict): the Cohen Kappa score
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_kp = np.array([item["kappa_score"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == 'weighted':
+            kappa = np.dot(list_weights, list_kp) / np.sum(list_weights)
+        elif average == 'macro':
+            kappa = np.mean(list_kp)
+        elif average == 'micro':
+            kappa = np.average(list_kp)
+        else:
+            kappa = dict([(label, np.round(item["kappa_score"], decimal)) for label, item in metrics.items()])
+        return kappa if type(kappa) == dict else np.round(kappa, decimal)
+
+    def jaccard_similarity_index(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Generate Jaccard similarity index for multiple classification problem
+        Higher is better (Best = +1), Range = [0, +1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            jsi (float, dict): the Jaccard similarity index
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_js = np.array([item["jaccard_similarities"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp = tn = np.sum(np.diag(matrix))
+            fp = fn = np.sum(matrix) - tp
+            js = tp / (tp + fp + fn)
+        elif average == "macro":
+            js = np.mean(list_js)
+        elif average == "weighted":
+            js = np.dot(list_weights, list_js) / np.sum(list_weights)
+        else:
+            js = dict([(label, np.round(item["jaccard_similarities"], decimal)) for label, item in metrics.items()])
+        return js if type(js) == dict else np.round(js, decimal)
+
+    def g_mean_score(self, y_true=None, y_pred=None, labels=None, average="macro", decimal=None, **kwargs):
+        """
+        Calculates the G-mean (Geometric mean) score between y_true and y_pred.
+        Higher is better (Best = +1), Range = [0, +1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            labels (tuple, list, np.ndarray): List of labels to index the matrix. This may be used to reorder or select a subset of labels.
+            average (str, None): {'micro', 'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            float, dict: The G-mean score.
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        matrix, imap, imap_count = calculate_confusion_matrix(y_true, y_pred, labels, normalize=None)
+        metrics = calculate_single_label_metric(matrix, imap, imap_count)
+
+        list_gm = np.array([item["g_mean"] for item in metrics.values()])
+        list_weights = np.array([item["n_true"] for item in metrics.values()])
+
+        if average == "micro":
+            tp = tn = np.sum(np.diag(matrix))
+            fp = fn = np.sum(matrix) - tp
+            gm = np.sqrt((tp / (tp + fn)) * (tn / (tn + fp)))
+        elif average == "macro":
+            gm = np.mean(list_gm)
+        elif average == "weighted":
+            gm = np.dot(list_weights, list_gm) / np.sum(list_weights)
+        else:
+            gm = dict([(label, np.round(item["g_mean"], decimal)) for label, item in metrics.items()])
+        return gm if type(gm) == dict else np.round(gm, decimal)
+
+    def gini_index(self, y_true=None, y_pred=None, decimal=None, **kwargs):
+        """
+        Calculates the Gini index between y_true and y_pred.
+        Smaller is better (Best = 0), Range = [0, +1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_pred (tuple, list, np.ndarray): a list of integers or strings for y_pred classes
+            average (str, None): {'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            float, dict: The Gini index
+        """
+        y_true, y_pred, binary, representor, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        # Calculate class probabilities
+        total_samples = len(y_true)
+        y_prob = np.zeros(total_samples)
+        for idx in range(0, total_samples):
+            if y_true[idx] == y_pred[idx]:
+                y_prob[idx] = 1
+            else:
+                y_prob[idx] = 0
+        positive_samples = np.sum(y_prob)
+        negative_samples = total_samples - positive_samples
+        p_positive = positive_samples / total_samples
+        p_negative = negative_samples / total_samples
+        # Calculate Gini index
+        result = 1 - (p_positive ** 2 + p_negative ** 2)
+        return np.round(result, decimal)
+
+    def roc_auc_score(self, y_true=None, y_score=None, average="macro", decimal=5, **kwargs):
+        """
+        Calculates the ROC-AUC score between y_true and y_score.
+        Higher is better (Best = +1), Range = [0, +1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): a list of integers or strings for known classes
+            y_score (tuple, list, np.ndarray): a list of predicted scores.
+            average (str, None): {'macro', 'weighted'} or None, default="macro"
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            float, dict: The AUC score.
+        """
+        y_true, y_score, binary, representor = format_y_score(y_true, y_score)
+        if binary:
+            tpr, fpr, thresholds = calculate_roc_curve(y_true, y_score)
+            # Calculate the area under the curve (AUC) using the trapezoidal rule
+            return np.trapz(tpr, fpr)
+        else:
+            list_weights = calculate_class_weights(y_true, y_pred=None, y_score=y_score)
+            # one-vs-all (rest) approach
+            tpr = dict()
+            fpr = dict()
+            thresholds = dict()
+            auc = []
+            n_classes = len(np.unique(y_true))
+            for i in range(n_classes):
+                y_true_i = np.array([1 if y == i else 0 for y in y_true])
+                y_score_i = y_score[:, i]
+                tpr[i], fpr[i], thresholds[i] = calculate_roc_curve(y_true_i, y_score_i)
+                # Calculate the area under the curve (AUC) using the trapezoidal rule
+                auc.append(np.trapz(tpr[i], fpr[i]))
+            if average == "macro":
+                result = np.mean(auc)
+            elif average == "weighted":
+                result = np.dot(list_weights, auc) / np.sum(list_weights)
+            else:
+                result = dict([(idx, np.round(auc[idx], decimal)) for idx in range(n_classes)])
+            return result if type(result) == dict else np.round(result, decimal)
+
+    CM = confusion_matrix
+    PS = precision_score
+    NPV = negative_predictive_value
+    RS = recall_score
+    AS = accuracy_score
+    F1S = f1_score
+    F2S = f2_score
+    FBS = fbeta_score
+    SS = specificity_score
+    MCC = matthews_correlation_coefficient
+    HS = hamming_score
+    LS = lift_score
+    CKS = cohen_kappa_score
+    JSI = JSC = jaccard_similarity_coefficient = jaccard_similarity_index
+    GMS = g_mean_score
+    GINI = gini_index
+    ROC = AUC = RAS = roc_auc_score
```

### Comparing `permetrics-1.4.0/permetrics/evaluator.py` & `permetrics-1.4.1/permetrics/evaluator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,123 +1,124 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 10:48, 25/03/2022 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import numpy as np
-import copy as cp
-
-
-class Evaluator:
-    """
-    This is base class for all performance metrics
-    """
-
-    EPSILON = 1e-10
-
-    def __init__(self, y_true=None, y_pred=None, decimal=5, **kwargs):
-        """
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            decimal (int): The number of fractional parts after the decimal point
-        """
-        if kwargs is None: kwargs = {}
-        self.set_keyword_arguments(kwargs)
-        self.y_true_original = cp.deepcopy(y_true)
-        self.y_pred_original = cp.deepcopy(y_pred)
-        self.y_true = cp.deepcopy(y_true)
-        self.y_pred = cp.deepcopy(y_pred)
-        self.decimal = decimal
-
-    def set_keyword_arguments(self, kwargs):
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-
-    def get_processed_data(self, y_true=None, y_pred=None, decimal=None):
-        pass
-
-    def get_multi_output_result(self, result=None, multi_output=None, decimal=None):
-        """
-        Get multiple output results based on selected parameter
-
-        Args:
-            result: The raw result from metric
-            multi_output: "raw_values" - return multi-output, [weights] - return single output based on weights, else - return mean result
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            final_result: Multiple outputs results based on selected parameter
-        """
-        if isinstance(multi_output, (tuple, list, set, np.ndarray)):
-            weights = np.array(multi_output)
-            if self.y_true.shape[1] != len(weights):
-                raise ValueError("Multi-output weights must have the same length with y_true or y_pred!")
-            return np.round(np.dot(result, multi_output), decimal)
-        elif multi_output == "raw_values":  # Default: raw_values
-            return np.round(result, decimal)
-        else:
-            return np.round(np.mean(result), decimal)
-
-    def get_metric_by_name(self, metric_name=str, paras=None) -> dict:
-        """
-        Get single metric by name, specific parameter of metric by dictionary
-
-        Args:
-            metric_name (str): Select name of metric
-            paras (dict): Dictionary of hyper-parameter for that metric
-
-        Returns:
-            result (dict): { metric_name: value }
-        """
-        result = {}
-        obj = getattr(self, metric_name)
-        result[metric_name] = obj() if paras is None else obj(**paras)
-        return result
-
-    def get_metrics_by_list_names(self, list_metric_names=list, list_paras=None) -> dict:
-        """
-        Get results of list metrics by its name and parameters
-
-        Args:
-            list_metric_names (list): e.g, ["RMSE", "MAE", "MAPE"]
-            list_paras (list): e.g, [ {"decimal": 5, None}, {"decimal": 4, "multi_output": "raw_values"}, {"decimal":6, "multi_output": [2, 3]} ]
-
-        Returns:
-            results (dict): e.g, { "RMSE": 0.25, "MAE": [0.3, 0.6], "MAPE": 0.15 }
-        """
-        results = {}
-        for idx, metric_name in enumerate(list_metric_names):
-            obj = getattr(self, metric_name)
-            if list_paras is None:
-                results[metric_name] = obj()
-            else:
-                if len(list_metric_names) != len(list_paras):
-                    raise ValueError("list_metric_names and list_paras must have the same length!")
-                if list_paras[idx] is None:
-                    results[metric_name] = obj()
-                else:
-                    results[metric_name] = obj(**list_paras[idx])
-        return results
-
-    def get_metrics_by_dict(self, metrics_dict:dict) -> dict:
-        """
-        Get results of list metrics by its name and parameters wrapped by dictionary
-
-        For example:
-            {"RMSE": { "multi_output": multi_output, "decimal": 4 }, "MAE": { "non_zero": True, "multi_output": multi_output, "decimal": 6}}
-
-        Args:
-            metrics_dict (dict): key is metric name and value is dict of parameters
-
-        Returns:
-            results (dict): e.g, { "RMSE": 0.3524, "MAE": 0.445263 }
-        """
-        results = {}
-        for metric_name, paras_dict in metrics_dict.items():
-            obj = getattr(self, metric_name)
-            if paras_dict is None:
-                results[metric_name] = obj()
-            else:
-                results[metric_name] = obj(**paras_dict)     # Unpacking a dictionary and passing it to function
-        return results
+#!/usr/bin/env python
+# Created by "Thieu" at 10:48, 25/03/2022 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import numpy as np
+import copy as cp
+
+
+class Evaluator:
+    """
+    This is base class for all performance metrics
+    """
+
+    EPSILON = 1e-10
+    SUPPORT = {}
+
+    def __init__(self, y_true=None, y_pred=None, decimal=5, **kwargs):
+        """
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            decimal (int): The number of fractional parts after the decimal point
+        """
+        if kwargs is None: kwargs = {}
+        self.set_keyword_arguments(kwargs)
+        self.y_true_original = cp.deepcopy(y_true)
+        self.y_pred_original = cp.deepcopy(y_pred)
+        self.y_true = cp.deepcopy(y_true)
+        self.y_pred = cp.deepcopy(y_pred)
+        self.decimal = decimal
+
+    def set_keyword_arguments(self, kwargs):
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+    def get_processed_data(self, y_true=None, y_pred=None, decimal=None):
+        pass
+
+    def get_multi_output_result(self, result=None, multi_output=None, decimal=None):
+        """
+        Get multiple output results based on selected parameter
+
+        Args:
+            result: The raw result from metric
+            multi_output: "raw_values" - return multi-output, [weights] - return single output based on weights, else - return mean result
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            final_result: Multiple outputs results based on selected parameter
+        """
+        if isinstance(multi_output, (tuple, list, set, np.ndarray)):
+            weights = np.array(multi_output)
+            if self.y_true.shape[1] != len(weights):
+                raise ValueError("Multi-output weights must have the same length with y_true or y_pred!")
+            return np.round(np.dot(result, multi_output), decimal)
+        elif multi_output == "raw_values":  # Default: raw_values
+            return np.round(result, decimal)
+        else:
+            return np.round(np.mean(result), decimal)
+
+    def get_metric_by_name(self, metric_name=str, paras=None) -> dict:
+        """
+        Get single metric by name, specific parameter of metric by dictionary
+
+        Args:
+            metric_name (str): Select name of metric
+            paras (dict): Dictionary of hyper-parameter for that metric
+
+        Returns:
+            result (dict): { metric_name: value }
+        """
+        result = {}
+        obj = getattr(self, metric_name)
+        result[metric_name] = obj() if paras is None else obj(**paras)
+        return result
+
+    def get_metrics_by_list_names(self, list_metric_names=list, list_paras=None) -> dict:
+        """
+        Get results of list metrics by its name and parameters
+
+        Args:
+            list_metric_names (list): e.g, ["RMSE", "MAE", "MAPE"]
+            list_paras (list): e.g, [ {"decimal": 5, None}, {"decimal": 4, "multi_output": "raw_values"}, {"decimal":6, "multi_output": [2, 3]} ]
+
+        Returns:
+            results (dict): e.g, { "RMSE": 0.25, "MAE": [0.3, 0.6], "MAPE": 0.15 }
+        """
+        results = {}
+        for idx, metric_name in enumerate(list_metric_names):
+            obj = getattr(self, metric_name)
+            if list_paras is None:
+                results[metric_name] = obj()
+            else:
+                if len(list_metric_names) != len(list_paras):
+                    raise ValueError("list_metric_names and list_paras must have the same length!")
+                if list_paras[idx] is None:
+                    results[metric_name] = obj()
+                else:
+                    results[metric_name] = obj(**list_paras[idx])
+        return results
+
+    def get_metrics_by_dict(self, metrics_dict:dict) -> dict:
+        """
+        Get results of list metrics by its name and parameters wrapped by dictionary
+
+        For example:
+            {"RMSE": { "multi_output": multi_output, "decimal": 4 }, "MAE": { "non_zero": True, "multi_output": multi_output, "decimal": 6}}
+
+        Args:
+            metrics_dict (dict): key is metric name and value is dict of parameters
+
+        Returns:
+            results (dict): e.g, { "RMSE": 0.3524, "MAE": 0.445263 }
+        """
+        results = {}
+        for metric_name, paras_dict in metrics_dict.items():
+            obj = getattr(self, metric_name)
+            if paras_dict is None:
+                results[metric_name] = obj()
+            else:
+                results[metric_name] = obj(**paras_dict)     # Unpacking a dictionary and passing it to function
+        return results
```

### Comparing `permetrics-1.4.0/permetrics/regression.py` & `permetrics-1.4.1/permetrics/regression.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1544 +1,1625 @@
-# !/usr/bin/env python
-# Created by "Thieu" at 18:07, 18/07/2020 ----------%
-#       Email: nguyenthieu2102@gmail.com            %
-#       Github: https://github.com/thieu1995        %
-# --------------------------------------------------%
-
-from permetrics.evaluator import Evaluator
-from permetrics.utils.regressor_util import *
-from permetrics.utils.data_util import *
-import numpy as np
-
-
-class RegressionMetric(Evaluator):
-    """
-    This is class contains all regression metrics (for both regression and time-series problem)
-
-    Notes
-    ~~~~~
-    + An extension of scikit-learn metrics section, besides so many new metrics
-    + Some methods in scikit-learn can't generate the multi-output metrics, we re-implement all of them and allow multi-output metrics
-    + Therefore, this class can calculate the multi-output metrics for all methods
-    + https://scikit-learn.org/stable/modules/model_evaluation.html#regression-metrics
-    """
-
-    def __init__(self, y_true=None, y_pred=None, decimal=5, **kwargs):
-        """
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            decimal (int): The number of fractional parts after the decimal point
-            **kwargs ():
-        """
-        super().__init__(y_true, y_pred, decimal, **kwargs)
-        if kwargs is None: kwargs = {}
-        self.set_keyword_arguments(kwargs)
-        self.one_dim = False
-
-    def get_processed_data(self, y_true=None, y_pred=None, decimal=None):
-        """
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            clean (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred)
-            decimal (int): The number of fractional parts after the decimal point
-
-        Returns:
-            y_true_final: y_true used in evaluation process.
-            y_pred_final: y_pred used in evaluation process
-            one_dim: is y_true has 1 dimensions or not
-            decimal: The number of fractional parts after the decimal point
-        """
-        decimal = self.decimal if decimal is None else decimal
-        if (y_true is not None) and (y_pred is not None):
-            y_true, y_pred = format_regression_data_type(y_true, y_pred)
-            y_true, y_pred, one_dim = format_regression_data(y_true, y_pred)
-        else:
-            if (self.y_true is not None) and (self.y_pred is not None):
-                y_true, y_pred = format_regression_data_type(self.y_true, self.y_pred)
-                y_true, y_pred, one_dim = format_regression_data(y_true, y_pred)
-            else:
-                raise ValueError("y_true or y_pred is None. You need to pass y_true and y_pred to object creation or function called.")
-        return y_true, y_pred, one_dim, decimal
-
-    def explained_variance_score(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Explained Variance Score (EVS). Best possible score is 1.0, greater value is better. Range = (-inf, 1.0]
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in denominator (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): EVS metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(1 - np.var(y_true - y_pred) / np.var(y_true), decimal)
-        else:
-            result = 1 - np.var(y_true - y_pred, axis=0) / np.var(y_true, axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def max_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Max Error (ME): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): ME metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.max(np.abs(y_true - y_pred)), decimal)
-        else:
-            result = np.max(np.abs(y_true - y_pred), axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def mean_bias_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Mean Bias Error (MBE): Best possible score is 0.0. Range = (-inf, +inf)
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): MBE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.mean(y_pred - y_true), decimal)
-        else:
-            result = np.mean(y_pred - y_true, axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def mean_absolute_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Mean Absolute Error (MAE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): MAE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.sum(np.abs(y_pred - y_true)) / len(y_true), decimal)
-        else:
-            result = np.sum(np.abs(y_pred - y_true), axis=0) / len(y_true)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def mean_squared_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Mean Squared Error (MSE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): MSE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        score = calculate_mse(y_true, y_pred, one_dim)
-        return np.round(score, decimal) if one_dim else self.get_multi_output_result(score, multi_output, decimal)
-
-    def root_mean_squared_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Root Mean Squared Error (RMSE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): RMSE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        score = np.sqrt(calculate_mse(y_true, y_pred, one_dim))
-        return np.round(score, decimal) if one_dim else self.get_multi_output_result(score, multi_output, decimal)
-
-    def mean_squared_log_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=True):
-        """
-        Mean Squared Log Error (MSLE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-        Link: https://peltarion.com/knowledge-center/documentation/modeling-view/build-an-ai-model/loss-functions/mean-squared-logarithmic-error-(msle)
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = True)
-
-        Returns:
-            result (float, int, np.ndarray): MSLE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.sum(np.log((y_true + 1) / (y_pred+1)) ** 2) / len(y_true), decimal)
-        else:
-            result = np.sum(np.log((y_true + 1) / (y_pred + 1)) ** 2, axis=0) / len(y_true)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def median_absolute_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Median Absolute Error (MedAE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): MedAE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.median(np.abs(y_true - y_pred)), decimal)
-        else:
-            result = np.median(np.abs(y_true - y_pred), axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def mean_relative_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False):
-        """
-        Mean Relative Error (MRE) - Mean Relative Bias (MRB): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): MRE (MRB) metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 0)
-        else:
-            y_true[y_true == 0] = self.EPSILON
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.mean(np.abs((y_pred - y_true) / y_true)), decimal)
-        else:
-            result = np.mean(np.abs((y_pred - y_true) / y_true), axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def mean_percentage_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False):
-        """
-        Mean Percentage Error (MPE): Best possible score is 0.0. Range = (-inf, +inf)
-        Link: https://www.dataquest.io/blog/understanding-regression-error-metrics/
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): MPE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 0)
-        else:
-            y_true[y_true == 0] = self.EPSILON
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.mean((y_true - y_pred) / y_true), decimal)
-        else:
-            result = np.mean((y_true - y_pred) / y_true, axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def mean_absolute_percentage_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False):
-        """
-        Mean Absolute Percentage Error (MAPE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): MAPE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 0)
-        else:
-            y_true[y_true == 0] = self.EPSILON
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.mean(np.abs(y_true - y_pred) / np.abs(y_true)), decimal)
-        else:
-            result = np.mean(np.abs(y_true - y_pred) / np.abs(y_true), axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def symmetric_mean_absolute_percentage_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Symmetric Mean Absolute Percentage Error (SMAPE): Best possible score is 0.0, smaller value is better. Range = [0, 1]
-        If you want percentage then multiply with 100%
-
-        Link: https://en.wikipedia.org/wiki/Symmetric_mean_absolute_percentage_error
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): SMAPE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.mean(np.abs(y_pred - y_true) / (np.abs(y_true) + np.abs(y_pred))), decimal)
-        else:
-            result = np.mean(np.abs(y_pred - y_true) / (np.abs(y_true) + np.abs(y_pred)), axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def mean_arctangent_absolute_percentage_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Mean Arctangent Absolute Percentage Error (MAAPE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Link: https://support.numxl.com/hc/en-us/articles/115001223463-MAAPE-Mean-Arctangent-Absolute-Percentage-Error
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): MAAPE metric for single column or multiple columns (radian values)
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.mean(np.arctan(np.abs((y_true - y_pred)/y_true))), decimal)
-        else:
-            result = np.mean(np.arctan(np.abs((y_true - y_pred)/y_true)), axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def mean_absolute_scaled_error(self, y_true=None, y_pred=None, m=1, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Mean Absolute Scaled Error (MASE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Link: https://en.wikipedia.org/wiki/Mean_absolute_scaled_error
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            m (int): m = 1 for non-seasonal data, m > 1 for seasonal data
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): MASE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.mean(np.abs(y_true - y_pred)) / np.mean(np.abs(y_true[m:] - y_true[:-m])), decimal)
-        else:
-            result = np.mean(np.abs(y_true - y_pred), axis=0) / np.mean(np.abs(y_true[m:] - y_true[:-m]), axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def nash_sutcliffe_efficiency(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Nash-Sutcliffe Efficiency (NSE): Best possible score is 1.0, bigger value is better. Range = (-inf, 1]
-
-        Link: https://agrimetsoft.com/calculators/Nash%20Sutcliffe%20model%20Efficiency%20coefficient
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): NSE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        nse = calculate_nse(y_true, y_pred, one_dim)
-        return np.round(nse, decimal) if one_dim else self.get_multi_output_result(nse, multi_output, decimal)
-
-    def normalized_nash_sutcliffe_efficiency(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Normalize Nash-Sutcliffe Efficiency (NNSE): Best possible score is 1.0, bigger value is better. Range = [0, 1]
-
-        Link: https://agrimetsoft.com/calculators/Nash%20Sutcliffe%20model%20Efficiency%20coefficient
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): NSE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        nse = calculate_nse(y_true, y_pred, one_dim)
-        nnse = 1 / (2 - nse)
-        return np.round(nnse, decimal) if one_dim else self.get_multi_output_result(nnse, multi_output, decimal)
-
-    def willmott_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Willmott Index (WI): Best possible score is 1.0, bigger value is better. Range = [0, 1]
-
-        Notes
-        ~~~~~
-        + Reference evapotranspiration for Londrina, Paraná, Brazil: performance of different estimation methods
-        + https://www.researchgate.net/publication/319699360_Reference_evapotranspiration_for_Londrina_Parana_Brazil_performance_of_different_estimation_methods
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): WI metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        wi = calculate_wi(y_true, y_pred, one_dim)
-        return np.round(wi, decimal) if one_dim else self.get_multi_output_result(wi, multi_output, decimal)
-
-    def coefficient_of_determination(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Coefficient of Determination (COD/R2): Best possible score is 1.0, bigger value is better. Range = (-inf, 1]
-
-        Notes
-        ~~~~~
-            + https://scikit-learn.org/stable/modules/model_evaluation.html#r2-score
-            + Scikit-learn and other websites denoted COD as R^2 (or R squared), it leads to the misunderstanding of R^2 in which R is PCC.
-            + We should denote it as COD or R2 only.
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): R2 metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(1 - np.sum((y_true - y_pred) ** 2) / np.sum((y_true - np.mean(y_true)) ** 2), decimal)
-        else:
-            result = 1 - np.sum((y_true - y_pred) ** 2, axis=0) / np.sum((y_true - np.mean(y_true, axis=0)) ** 2, axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def adjusted_coefficient_of_determination(self, y_true=None, y_pred=None, X_shape=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Adjusted Coefficient of Determination (ACOD/AR2): Best possible score is 1.0, bigger value is better. Range = (-inf, 1]
-
-        Notes
-        ~~~~~
-            + https://dziganto.github.io/data%20science/linear%20regression/machine%20learning/python/Linear-Regression-101-Metrics/
-            + Scikit-learn and other websites denoted COD as R^2 (or R squared), it leads to the misunderstanding of R^2 in which R is PCC.
-            + We should denote it as COD or R2 only.
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            X_shape (tuple, list, np.ndarray): The shape of X_train dataset
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): AR2 metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if X_shape is None:
-            raise ValueError("You need to pass the shape of X_train dataset to calculate Adjusted R2.")
-        if len(X_shape) != 2 or X_shape[0] < 4 or X_shape[1] < 1:
-            raise ValueError("You need to pass the real shape of X_train dataset to calculate Adjusted R2.")
-        dft = X_shape[0] - 1.0
-        dfe = X_shape[0] - X_shape[1] - 1.0
-        df_final = dft/dfe
-        if one_dim:
-            return np.round(1 - df_final * np.sum((y_true - y_pred) ** 2) / np.sum((y_true - np.mean(y_true)) ** 2), decimal)
-        else:
-            result = 1 - df_final * np.sum((y_true - y_pred) ** 2, axis=0) / np.sum((y_true - np.mean(y_true, axis=0)) ** 2, axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def pearson_correlation_coefficient(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Pearson’s Correlation Coefficient (PCC or R): Best possible score is 1.0, bigger value is better. Range = [-1, 1]
-        Notes
-        ~~~~~
-            + Reference evapotranspiration for Londrina, Paraná, Brazil: performance of different estimation methods
-            + Remember no absolute in the equations
-            + https://en.wikipedia.org/wiki/Pearson_correlation_coefficient
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): R metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        pcc = calculate_pcc(y_true, y_pred, one_dim)
-        return np.round(pcc, decimal) if one_dim else self.get_multi_output_result(pcc, multi_output, decimal)
-
-    def absolute_pearson_correlation_coefficient(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Absolute Pearson’s Correlation Coefficient (APCC or AR): Best possible score is 1.0, bigger value is better. Range = [0, 1]
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): AR metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        pcc = calculate_absolute_pcc(y_true, y_pred, one_dim)
-        return np.round(pcc, decimal) if one_dim else self.get_multi_output_result(pcc, multi_output, decimal)
-
-    def pearson_correlation_coefficient_square(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        (Pearson’s Correlation Index)^2 = R^2 = R2s (R square): Best possible score is 1.0, bigger value is better. Range = [0, 1]
-        Notes
-        ~~~~~
-            + Do not misunderstand between R2s and R2 (Coefficient of Determination), they are different
-            + Most of online tutorials (article, wikipedia,...) or even scikit-learn library are denoted the wrong R2s and R2.
-            + R^2 = R2s = R squared should be (Pearson’s Correlation Index)^2
-            + Meanwhile, R2 = Coefficient of Determination
-            + https://en.wikipedia.org/wiki/Pearson_correlation_coefficient
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): R2s metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        pcc = calculate_pcc(y_true, y_pred, one_dim)
-        return np.round(pcc**2, decimal) if one_dim else self.get_multi_output_result(pcc**2, multi_output, decimal)
-
-    def confidence_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Confidence Index (or Performance Index): CI (PI): Best possible score is 1.0, bigger value is better. Range = (-inf, 1]
-
-        Notes
-        ~~~~~
-        - Reference evapotranspiration for Londrina, Paraná, Brazil: performance of different estimation methods
-        - > 0.85,          Excellent
-        - 0.76-0.85,       Very good
-        - 0.66-0.75,       Good
-        - 0.61-0.65,       Satisfactory
-        - 0.51-0.60,       Poor
-        - 0.41-0.50,       Bad
-        - ≤ 0.40,          Very bad
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): CI (PI) metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        r = calculate_pcc(y_true, y_pred, one_dim)
-        d = calculate_wi(y_true, y_pred, one_dim)
-        return np.round(r*d, decimal) if one_dim else self.get_multi_output_result(r*d, multi_output, decimal)
-
-    def deviation_of_runoff_volume(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Deviation of Runoff Volume (DRV): Best possible score is 1.0, smaller value is better. Range = [1, +inf)
-        Link: https://rstudio-pubs-static.s3.amazonaws.com/433152_56d00c1e29724829bad5fc4fd8c8ebff.html
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): DRV metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.sum(y_pred) / np.sum(y_true), decimal)
-        else:
-            result = np.sum(y_pred, axis=0) / np.sum(y_true, axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def kling_gupta_efficiency(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Kling-Gupta Efficiency (KGE): Best possible score is 1, bigger value is better. Range = (-inf, 1]
-        Link: https://rstudio-pubs-static.s3.amazonaws.com/433152_56d00c1e29724829bad5fc4fd8c8ebff.html
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): KGE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            m1, m2 = np.mean(y_true), np.mean(y_pred)
-            r = np.sum((y_true - m1) * (y_pred - m2)) / (np.sqrt(np.sum((y_true - m1) ** 2)) * np.sqrt(np.sum((y_pred - m2) ** 2)))
-            beta = m2 / m1
-            gamma = (np.std(y_pred) / m2) / (np.std(y_true) / m1)
-            return np.round(1 - np.sqrt((r - 1) ** 2 + (beta - 1) ** 2 + (gamma - 1) ** 2), decimal)
-        else:
-            m1, m2 = np.mean(y_true, axis=0), np.mean(y_pred, axis=0)
-            num_r = np.sum((y_true - m1) * (y_pred - m2), axis=0)
-            den_r = np.sqrt(np.sum((y_true - m1) ** 2, axis=0)) * np.sqrt(np.sum((y_pred - m2) ** 2, axis=0))
-            r = num_r / den_r
-            beta = m2 / m1
-            gamma = (np.std(y_pred, axis=0) / m2) / (np.std(y_true, axis=0) / m1)
-            result = 1 - np.sqrt((r - 1) ** 2 + (beta - 1) ** 2 + (gamma - 1) ** 2)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def prediction_of_change_in_direction(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Prediction of Change in Direction (PCD): Best possible score is 1.0, bigger value is better. Range = [0, 1]
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): PCD metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            d = np.diff(y_true)
-            dp = np.diff(y_pred)
-            return np.round(np.mean(np.sign(d) == np.sign(dp)), decimal)
-        else:
-            d = np.diff(y_true, axis=0)
-            dp = np.diff(y_pred, axis=0)
-            result = np.mean(np.sign(d) == np.sign(dp), axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def cross_entropy(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=True):
-        """
-        Cross Entropy (CE) or Entropy (E): Range = (-inf, 0]. Can't give comment about this one
-
-        Notes
-        ~~~~~
-            + Greater value of Entropy, the greater the uncertainty for probability distribution and smaller the value the less the uncertainty
-            + https://datascience.stackexchange.com/questions/20296/cross-entropy-loss-explanation
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = True)
-
-        Returns:
-            result (float, int, np.ndarray): CE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        else:
-            y_pred[y_pred == 0] = self.EPSILON
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        entropy = calculate_entropy(y_true, y_pred, one_dim)
-        return np.round(entropy, decimal) if one_dim else self.get_multi_output_result(entropy, multi_output, decimal)
-
-    def kullback_leibler_divergence(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=True):
-        """
-        Kullback-Leibler Divergence (KLD): Best possible score is 0.0 . Range = (-inf, +inf)
-        Link: https://machinelearningmastery.com/divergence-between-probability-distributions/
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = True)
-
-        Returns:
-            result (float, int, np.ndarray): KLD metric (bits) for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        else:
-            y_pred[y_pred == 0] = self.EPSILON
-        y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round(np.sum(y_true * np.log2(y_true / y_pred)), decimal)
-        else:
-            score = np.sum(y_true * np.log2(y_true / y_pred), axis=0)
-            return self.get_multi_output_result(score, multi_output, decimal)
-
-    def jensen_shannon_divergence(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=True):
-        """
-        Jensen-Shannon Divergence (JSD): Best possible score is 0.0 (identical), smaller value is better . Range = [0, +inf)
-        Link: https://machinelearningmastery.com/divergence-between-probability-distributions/
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = True)
-
-        Returns:
-            result (float, int, np.ndarray): JSD metric (bits) for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            m = 0.5 * (y_true + y_pred)
-            score = 0.5 * np.sum(y_true * np.log2(y_true / m)) + 0.5 * np.sum(y_pred * np.log2(y_pred / m))
-            return np.round(score, decimal)
-        else:
-            m = 0.5 * (y_true + y_pred)
-            score = 0.5 * np.sum(y_true * np.log2(y_true / m), axis=0) + 0.5 * np.sum(y_pred * np.log2(y_pred / m), axis=0)
-            return self.get_multi_output_result(score, multi_output, decimal)
-
-    def variance_accounted_for(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Variance Accounted For between 2 signals (VAF): Best possible score is 100% (identical signal), bigger value is better. Range = (-inf, 100%]
-
-        Link: https://www.dcsc.tudelft.nl/~jwvanwingerden/lti/doc/html/vaf.html
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): VAF metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 0)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-
-        if one_dim:
-            return np.round((1 - np.var(y_true - y_pred) / np.var(y_true)) * 100, decimal)
-        else:
-            result = (1 - np.var(y_true - y_pred, axis=0) / np.var(y_true, axis=0)) * 100
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def relative_absolute_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Relative Absolute Error (RAE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Notes
-        ~~~~~
-            + https://stackoverflow.com/questions/59499222/how-to-make-a-function-of-mae-and-rae-without-using-librarymetrics
-            + https://www.statisticshowto.com/relative-absolute-error
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): RAE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            numerator = np.power(np.sum((y_pred - y_true)**2), 1/2)
-            denominator = np.power(np.sum(y_true**2), 1/2)
-            return np.round(numerator/denominator, decimal)
-        else:
-            numerator = np.power(np.sum((y_pred - y_true) ** 2, axis=0), 1 / 2)
-            denominator = np.power(np.sum(y_true ** 2, axis=0), 1 / 2)
-            return self.get_multi_output_result(numerator/denominator, multi_output, decimal)
-
-    def a10_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False):
-        """
-        A10 index (A10): Best possible score is 1.0, bigger value is better. Range = [0, 1]
-
-        Notes
-        ~~~~~
-            + a10-index is engineering index for evaluating artificial intelligence models by showing the number of samples
-            + that fit the prediction values with a deviation of ±10% compared to experimental values
-            + https://www.mdpi.com/2076-3417/9/18/3715/htm
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): A10 metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        else:
-            y_pred[y_pred == 0] = self.EPSILON
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-
-        if one_dim:
-            div = y_true / y_pred
-            div = np.where(np.logical_and(div >= 0.9, div <= 1.1), 1, 0)
-            return np.round(np.mean(div), decimal)
-        else:
-            div = y_true / y_pred
-            div = np.where(np.logical_and(div >= 0.9, div <= 1.1), 1, 0)
-            return self.get_multi_output_result(np.mean(div, axis=0), multi_output, decimal)
-
-    def a20_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False):
-        """
-        A20 index (A20): Best possible score is 1.0, bigger value is better. Range = [0, 1]
-
-        Notes
-        ~~~~~
-            + a20-index evaluated metric by showing the number of samples that fit the prediction values with a deviation of ±20% compared to experimental values
-            + https://www.mdpi.com/2076-3417/9/18/3715/htm
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): A20 metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        else:
-            y_pred[y_pred == 0] = self.EPSILON
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            div = y_true / y_pred
-            div = np.where(np.logical_and(div >= 0.8, div <= 1.2), 1, 0)
-            return np.round(np.mean(div), decimal)
-        else:
-            div = y_true / y_pred
-            div = np.where(np.logical_and(div >= 0.8, div <= 1.2), 1, 0)
-            return self.get_multi_output_result(np.mean(div, axis=0), multi_output, decimal)
-
-    def a30_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False):
-        """
-        A30 index (A30): Best possible score is 1.0, bigger value is better. Range = [0, 1]
-
-        Note: a30-index evaluated metric by showing the number of samples that fit the prediction values with a deviation of ±30% compared to experimental values
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): A30 metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        else:
-            y_pred[y_pred == 0] = self.EPSILON
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            div = y_true / y_pred
-            div = np.where(np.logical_and(div >= 0.7, div <= 1.3), 1, 0)
-            return np.round(np.mean(div), decimal)
-        else:
-            div = y_true / y_pred
-            div = np.where(np.logical_and(div >= 0.7, div <= 1.3), 1, 0)
-            return self.get_multi_output_result(np.mean(div, axis=0), multi_output, decimal)
-
-    def normalized_root_mean_square_error(self, y_true=None, y_pred=None, model=0, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Normalized Root Mean Square Error (NRMSE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Link: https://medium.com/microsoftazure/how-to-better-evaluate-the-goodness-of-fit-of-regressions-990dbf1c0091
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            model (int): Normalize RMSE by different ways, (Optional, default = 0, valid values = [0, 1, 2, 3]
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): NRMSE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            rmse = np.sqrt(np.mean((y_pred - y_true) ** 2))
-            if model == 1:
-                result = rmse / np.mean(y_pred)
-            elif model == 2:
-                result = rmse / (np.max(y_true) - np.min(y_true))
-            elif model == 3:
-                result = np.sqrt(np.sum(np.log((y_pred + 1) / (y_true + 1)) ** 2) / len(y_true))
-            else:
-                result = rmse / y_pred.std()
-            return np.round(result, decimal)
-        else:
-            rmse = np.sqrt(np.sum((y_pred - y_true) ** 2, axis=0) / len(y_true))
-            if model == 1:
-                result = rmse / np.mean(y_pred, axis=0)
-            elif model == 2:
-                result = rmse / (np.max(y_true, axis=0) - np.min(y_true, axis=0))
-            elif model == 3:
-                result = np.sqrt(np.sum(np.log((y_pred + 1) / (y_true + 1)) ** 2, axis=0) / len(y_true))
-            else:
-                result = rmse / y_pred.std(axis=0)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def residual_standard_error(self, y_true=None, y_pred=None, n_paras=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Residual Standard Error (RSE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Links:
-            + https://www.statology.org/residual-standard-error-r/
-            + https://machinelearningmastery.com/degrees-of-freedom-in-machine-learning/
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            n_paras (int): The number of model's parameters
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): RSE metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if n_paras is None:
-            n_paras = len(y_true) / 2
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            ss_residuals = np.sum((y_true - y_pred)**2)
-            df_residuals = len(y_true) - n_paras - 1
-            return np.round(np.sqrt(ss_residuals / df_residuals), decimal)
-        else:
-            ss_residuals = np.sum((y_true - y_pred) ** 2, axis=0)
-            df_residuals = len(y_true) - n_paras - 1
-            score = np.sqrt(ss_residuals / df_residuals)
-            return self.get_multi_output_result(score, multi_output, decimal)
-
-    def covariance(self, y_true=None, y_pred=None, sample=False, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Covariance (COV): There is no best value, bigger value is better. Range = [-inf, +inf)
-            + is a measure of the relationship between two random variables
-            + evaluates how much – to what extent – the variables change together
-            + does not assess the dependency between variables
-            + Positive covariance: Indicates that two variables tend to move in the same direction.
-            + Negative covariance: Reveals that two variables tend to move in inverse directions.
-
-        Links:
-            + https://corporatefinanceinstitute.com/resources/data-science/covariance/
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            sample (bool): sample covariance or population covariance. See the website above for more details
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): COV metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        denominator = len(y_true) - 1 if sample else len(y_true)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            s1 = y_true - np.mean(y_true)
-            s2 = y_pred - np.mean(y_pred)
-            return np.round(np.dot(s1, s2) / denominator, decimal)
-        else:
-            s1 = y_true - np.mean(y_true, axis=0)
-            s2 = y_pred - np.mean(y_pred, axis=0)
-            return self.get_multi_output_result(np.sum(s1 * s2, axis=0) / denominator, multi_output, decimal)
-
-    def correlation(self, y_true=None, y_pred=None, sample=False, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Correlation (COR): Best possible value = 1, bigger value is better. Range = [-1, +1]
-            + measures the strength of the relationship between variables
-            + is the scaled measure of covariance. It is dimensionless.
-            + the correlation coefficient is always a pure value and not measured in any units.
-
-        Links:
-            + https://corporatefinanceinstitute.com/resources/data-science/covariance/
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            sample (bool): sample covariance or population covariance. See the website above for more details
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): COR metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        denominator = len(y_true) - 1 if sample else len(y_true)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            s1 = y_true - np.mean(y_true)
-            s2 = y_pred - np.mean(y_pred)
-            return np.round((np.dot(s1, s2) / denominator) / (np.std(y_true) * np.std(y_pred)), decimal)
-        else:
-            s1 = y_true - np.mean(y_true, axis=0)
-            s2 = y_pred - np.mean(y_pred, axis=0)
-            cov = np.sum(s1 * s2, axis=0) / denominator
-            den = np.std(y_true, axis=0) * np.std(y_pred, axis=0)
-            return self.get_multi_output_result(cov / den, multi_output, decimal)
-
-    def efficiency_coefficient(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Efficiency Coefficient (EC): Best possible value = 1, bigger value is better. Range = [-inf, +1]
-
-        Links:
-            + https://doi.org/10.1016/j.solener.2019.01.037
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): EC metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        score = calculate_ec(y_true, y_pred, one_dim)
-        return np.round(score, decimal) if one_dim else self.get_multi_output_result(score, multi_output, decimal)
-
-    def overall_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Overall Index (OI): Best possible value = 1, bigger value is better. Range = [-inf, +1]
-
-        Links:
-            + https://doi.org/10.1016/j.solener.2019.01.037
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): OI metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        ec = calculate_ec(y_true, y_pred, one_dim)
-        rmse = np.sqrt(calculate_mse(y_true, y_pred, one_dim))
-        if one_dim:
-            score = (1 - rmse / (np.max(y_true) - np.min(y_true)) + ec) / 2.0
-            return np.round(score, decimal)
-        else:
-            score = (1 - rmse / (np.max(y_true, axis=0) - np.min(y_true, axis=0)) + ec) / 2.0
-            return self.get_multi_output_result(score, multi_output, decimal)
-
-    def coefficient_of_residual_mass(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Coefficient of Residual Mass (CRM): Best possible value = 0.0, smaller value is better. Range = [-inf, +inf]
-
-        Links:
-            + https://doi.org/10.1016/j.csite.2022.101797
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): CRM metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            return np.round((np.sum(y_pred) - np.sum(y_true)) / np.sum(y_true), decimal)
-        else:
-            score = (np.sum(y_pred, axis=0) - np.sum(y_true, axis=0)) / np.sum(y_true, axis=0)
-            return self.get_multi_output_result(score, multi_output, decimal)
-
-    def gini_coefficient(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Gini coefficient (Gini): Best possible score is 1, bigger value is better. Range = [0, 1]
-
-        Notes
-        ~~~~~
-            + This version is based on below repository matlab code.
-            + https://github.com/benhamner/Metrics/blob/master/MATLAB/metrics/gini.m
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): Gini metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            idx_sort = np.argsort(-y_pred)
-            population_delta = 1.0 / len(y_true)
-            accumulated_population_percentage_sum, accumulated_loss_percentage_sum, score = 0, 0, 0
-            total_losses = np.sum(y_true)
-            for i in range(0, len(y_true)):
-                accumulated_loss_percentage_sum += y_true[idx_sort[i]] / total_losses
-                accumulated_population_percentage_sum += population_delta
-                score += accumulated_loss_percentage_sum - accumulated_population_percentage_sum
-            score = score / len(y_true)
-            return np.round(score, decimal)
-        else:
-            col = y_true.shape[1]
-            idx_sort = np.argsort(-y_pred, axis=0)
-            population_delta = 1.0 / len(y_true)
-            accumulated_population_percentage_sum, accumulated_loss_percentage_sum, score = np.zeros(col), np.zeros(col), np.zeros(col)
-            total_losses = np.sum(y_true, axis=0)
-            for i in range(0, col):
-                for j in range(0, len(y_true)):
-                    accumulated_loss_percentage_sum[i] += y_true[idx_sort[j, i], i] / total_losses[i]
-                    accumulated_population_percentage_sum[i] += population_delta
-                    score[i] += accumulated_loss_percentage_sum[i] - accumulated_population_percentage_sum[i]
-            result = score / len(y_true)
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def gini_coefficient_wiki(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False):
-        """
-        Gini coefficient (Gini): Best possible score is 1, bigger value is better. Range = [0, 1]
-
-        Notes
-        ~~~~~
-            + This version is based on wiki page, may be is the true version
-            + https://en.wikipedia.org/wiki/Gini_coefficient
-            + Gini coefficient can theoretically range from 0 (complete equality) to 1 (complete inequality)
-            + It is sometimes expressed as a percentage ranging between 0 and 100.
-            + If negative values are possible, then the Gini coefficient could theoretically be more than 1.
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (float, int, np.ndarray): Gini metric for single column or multiple columns
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        if one_dim:
-            y = np.concatenate((y_true, y_pred), axis=0)
-            score = 0
-            for i in range(0, len(y)):
-                score += np.sum(np.abs(y[i] - y))
-            score = score / (2 * len(y) * np.sum(y))
-            return np.round(score, decimal)
-        else:
-            y = np.concatenate((y_true, y_pred), axis=0)
-            col = y.shape[1]
-            d = len(y)
-            score = np.zeros(col)
-            for k in range(0, col):
-                for i in range(0, d):
-                    for j in range(0, d):
-                        score[k] += np.abs(y[i, k] - y[j, k])
-            result = score / (2 * len(y) ** 2 * np.mean(y, axis=0))
-            return self.get_multi_output_result(result, multi_output, decimal)
-
-    def single_relative_error(self, y_true=None, y_pred=None, decimal=None, non_zero=True, positive=False):
-        """
-        Relative Error (RE): Best possible score is 0.0, smaller value is better. Range = (-inf, +inf)
-
-        Note: Computes the relative error between two numbers, or for element between a pair of list, tuple or numpy arrays.
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (np.ndarray): RE metric
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 0)
-        else:
-            y_true[y_true == 0] = self.EPSILON
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        return np.round(y_pred / y_true - 1, decimal)
-
-    def single_absolute_error(self, y_true=None, y_pred=None, decimal=None, non_zero=False, positive=False):
-        """
-        Absolute Error (AE): Best possible score is 0.0, smaller value is better. Range = (-inf, +inf)
-
-        Note: Computes the absolute error between two numbers, or for element between a pair of list, tuple or numpy arrays.
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (np.ndarray): AE metric
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        return np.round(np.abs(y_true) - np.abs(y_pred), decimal)
-
-    def single_squared_error(self, y_true=None, y_pred=None, decimal=None, non_zero=False, positive=False):
-        """
-        Squared Error (SE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Note: Computes the squared error between two numbers, or for element between a pair of list, tuple or numpy arrays.
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
-
-        Returns:
-            result (np.ndarray): SE metric
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        return np.round((y_true - y_pred) ** 2, decimal)
-
-    def single_squared_log_error(self, y_true=None, y_pred=None, decimal=None, non_zero=True, positive=True):
-        """
-        Squared Log Error (SLE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
-
-        Note: Computes the squared log error between two numbers, or for element between a pair of list, tuple or numpy arrays.
-
-        Args:
-            y_true (tuple, list, np.ndarray): The ground truth values
-            y_pred (tuple, list, np.ndarray): The prediction values
-            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
-            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
-            positive (bool): Calculate metric based on positive values only or not (Optional, default = True)
-
-        Returns:
-            result (np.ndarray): SLE metric
-        """
-        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
-        if non_zero:
-            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
-        else:
-            y_pred[y_pred == 0] = self.EPSILON
-        if positive:
-            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
-        return np.round((np.log(y_true) - np.log(y_pred)) ** 2, decimal)
-
-    EVS = evs = explained_variance_score
-    ME = me = max_error
-    MBE = mbe = mean_bias_error
-    MAE = mae = mean_absolute_error
-    MSE = mse = mean_squared_error
-    RMSE = rmse = root_mean_squared_error
-    MSLE = msle = mean_squared_log_error
-    MedAE = medae = median_absolute_error
-    MRE = mre = MRB = mrb = mean_relative_bias = mean_relative_error
-    MPE = mpe = mean_percentage_error
-    MAPE = mape = mean_absolute_percentage_error
-    SMAPE = smape = symmetric_mean_absolute_percentage_error
-    MAAPE = maape = mean_arctangent_absolute_percentage_error
-    MASE = mase = mean_absolute_scaled_error
-    NSE = nse = nash_sutcliffe_efficiency
-    NNSE = nnse = normalized_nash_sutcliffe_efficiency
-    WI = wi = willmott_index
-    R = r = PCC = pcc = pearson_correlation_coefficient
-    AR = ar = APCC = apcc = absolute_pearson_correlation_coefficient
-    RSQ = rsq = R2s = r2s = pearson_correlation_coefficient_square
-    CI = ci = confidence_index
-    COD = cod = R2 = r2 = coefficient_of_determination
-    ACOD = acod = AR2 = ar2 = adjusted_coefficient_of_determination
-    DRV = drv = deviation_of_runoff_volume
-    KGE = kge = kling_gupta_efficiency
-    PCD = pcd = prediction_of_change_in_direction
-    CE = ce = cross_entropy
-    KLD = kld = kullback_leibler_divergence
-    JSD = jsd = jensen_shannon_divergence
-    VAF = vaf = variance_accounted_for
-    RAE = rae = relative_absolute_error
-    A10 = a10 = a10_index
-    A20 = a20 = a20_index
-    A30 = a30 = a30_index
-    NRMSE = nrmse = normalized_root_mean_square_error
-    RSE = rse = residual_standard_error
-    COV = cov = covariance
-    COR = cor = correlation
-    EC = ec = efficiency_coefficient
-    OI = oi = overall_index
-    CRM = crm = coefficient_of_residual_mass
-    GINI = gini = gini_coefficient
-    GINI_WIKI = gini_wiki = gini_coefficient_wiki
-
-    RE = re = RB = rb = single_relative_bias = single_relative_error
-    AE = ae = single_absolute_error
-    SE = se = single_squared_error
-    SLE = sle = single_squared_log_error
+# !/usr/bin/env python
+# Created by "Thieu" at 18:07, 18/07/2020 ----------%
+#       Email: nguyenthieu2102@gmail.com            %
+#       Github: https://github.com/thieu1995        %
+# --------------------------------------------------%
+
+from permetrics.evaluator import Evaluator
+from permetrics.utils.regressor_util import *
+from permetrics.utils.data_util import *
+import numpy as np
+
+
+class RegressionMetric(Evaluator):
+    """
+    Defines a RegressionMetric class that hold all regression metrics (for both regression and time-series problems)
+
+    + An extension of scikit-learn metrics section, with the addition of many more regression metrics.
+    + https://scikit-learn.org/stable/modules/model_evaluation.html#classification-metrics
+    + Some methods in scikit-learn can't generate the multi-output metrics, we re-implement all of them and allow multi-output metrics
+    + Therefore, we support calculate the multi-output metrics for all methods
+
+    Parameters
+    ----------
+    y_true: tuple, list, np.ndarray, default = None
+        The ground truth values.
+
+    y_pred: tuple, list, np.ndarray, default = None
+        The prediction values.
+
+    decimal: int, default = 5
+        The number of fractional parts after the decimal point
+    """
+
+    SUPPORT = {
+        "EVS": {"type": "max", "range": "(-inf, 1]", "best": "1"},
+        "ME": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "MBE": {"type": "unknown", "range": "(-inf, +inf)", "best": "0"},
+        "MAE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "MSE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "RMSE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "MSLE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "MedAE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "MRE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "MRB": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "MPE": {"type": "unknown", "range": "(-inf, +inf)", "best": "0"},
+        "MAPE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "SMAPE": {"type": "min", "range": "[0, 1]", "best": "0"},
+        "MAAPE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "MASE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "NSE": {"type": "max", "range": "(-inf, 1]", "best": "1"},
+        "NNSE": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "WI": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "R": {"type": "max", "range": "[-1, 1]", "best": "1"},
+        "PCC": {"type": "max", "range": "[-1, 1]", "best": "1"},
+        "AR": {"type": "max", "range": "[-1, 1]", "best": "1"},
+        "APCC": {"type": "max", "range": "[-1, 1]", "best": "1"},
+        "R2S": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "RSQ": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "R2": {"type": "max", "range": "(-inf, 1]", "best": "1"},
+        "COD": {"type": "max", "range": "(-inf, 1]", "best": "1"},
+        "AR2": {"type": "max", "range": "(-inf, 1]", "best": "1"},
+        "ACOD": {"type": "max", "range": "(-inf, 1]", "best": "1"},
+        "CI": {"type": "max", "range": "(-inf, 1]", "best": "1"},
+        "DRV": {"type": "min", "range": "[1, +inf)", "best": "1"},
+        "KGE": {"type": "max", "range": "(-inf, 1]", "best": "1"},
+        "GINI": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "GINI_WIKI": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "PCD": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "CE": {"type": "unknown", "range": "(-inf, 0]", "best": "unknown"},
+        "KLD": {"type": "unknown", "range": "(-inf, +inf)", "best": "0"},
+        "JSD": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "VAF": {"type": "max", "range": "(-inf, 100%)", "best": "100"},
+        "RAE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "A10": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "A20": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "A30": {"type": "max", "range": "[0, 1]", "best": "1"},
+        "NRMSE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "RSE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "RE": {"type": "unknown", "range": "(-inf, +inf)", "best": "0"},
+        "RB": {"type": "unknown", "range": "(-inf, +inf)", "best": "0"},
+        "AE": {"type": "unknown", "range": "(-inf, +inf)", "best": "0"},
+        "SE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "SLE": {"type": "min", "range": "[0, +inf)", "best": "0"},
+        "COV": {"type": "max", "range": "(-inf, +inf)", "best": "no best"},
+        "COR": {"type": "max", "range": "[-1, 1]", "best": "1"},
+        "EC": {"type": "max", "range": "(-inf, 1]", "best": "1"},
+        "OI": {"type": "max", "range": "(-inf, 1]", "best": "1"},
+        "CRM": {"type": "min", "range": "(-inf, +inf)", "best": "0"},
+    }
+
+    def __init__(self, y_true=None, y_pred=None, decimal=5, **kwargs):
+        super().__init__(y_true, y_pred, decimal, **kwargs)
+        if kwargs is None: kwargs = {}
+        self.set_keyword_arguments(kwargs)
+        self.one_dim = False
+
+    @staticmethod
+    def get_support(name=None, verbose=True):
+        if name == "all":
+            if verbose:
+                for key, value in RegressionMetric.SUPPORT.items():
+                    print(f"Metric {key} : {value}")
+                return RegressionMetric.SUPPORT
+        if name not in list(RegressionMetric.SUPPORT.keys()):
+            raise ValueError(f"RegressionMetric doesn't support metric named: {name}")
+        else:
+            if verbose:
+                print(f"Metric {name}: {RegressionMetric.SUPPORT[name]}")
+            return RegressionMetric.SUPPORT[name]
+
+    def get_processed_data(self, y_true=None, y_pred=None, decimal=None, **kwargs):
+        """
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            clean (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred)
+            decimal (int): The number of fractional parts after the decimal point
+
+        Returns:
+            y_true_final: y_true used in evaluation process.
+            y_pred_final: y_pred used in evaluation process
+            one_dim: is y_true has 1 dimensions or not
+            decimal: The number of fractional parts after the decimal point
+        """
+        decimal = self.decimal if decimal is None else decimal
+        if (y_true is not None) and (y_pred is not None):
+            y_true, y_pred = format_regression_data_type(y_true, y_pred)
+            y_true, y_pred, one_dim = format_regression_data(y_true, y_pred)
+        else:
+            if (self.y_true is not None) and (self.y_pred is not None):
+                y_true, y_pred = format_regression_data_type(self.y_true, self.y_pred)
+                y_true, y_pred, one_dim = format_regression_data(y_true, y_pred)
+            else:
+                raise ValueError("y_true or y_pred is None. You need to pass y_true and y_pred to object creation or function called.")
+        return y_true, y_pred, one_dim, decimal
+
+    def explained_variance_score(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Explained Variance Score (EVS). Best possible score is 1.0, greater value is better. Range = (-inf, 1.0]
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in denominator (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): EVS metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(1 - np.var(y_true - y_pred) / np.var(y_true), decimal)
+        else:
+            result = 1 - np.var(y_true - y_pred, axis=0) / np.var(y_true, axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def max_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Max Error (ME): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): ME metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.max(np.abs(y_true - y_pred)), decimal)
+        else:
+            result = np.max(np.abs(y_true - y_pred), axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def mean_bias_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Mean Bias Error (MBE): Best possible score is 0.0. Range = (-inf, +inf)
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): MBE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.mean(y_pred - y_true), decimal)
+        else:
+            result = np.mean(y_pred - y_true, axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def mean_absolute_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Mean Absolute Error (MAE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): MAE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.sum(np.abs(y_pred - y_true)) / len(y_true), decimal)
+        else:
+            result = np.sum(np.abs(y_pred - y_true), axis=0) / len(y_true)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def mean_squared_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Mean Squared Error (MSE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): MSE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        score = calculate_mse(y_true, y_pred, one_dim)
+        return np.round(score, decimal) if one_dim else self.get_multi_output_result(score, multi_output, decimal)
+
+    def root_mean_squared_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Root Mean Squared Error (RMSE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): RMSE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        score = np.sqrt(calculate_mse(y_true, y_pred, one_dim))
+        return np.round(score, decimal) if one_dim else self.get_multi_output_result(score, multi_output, decimal)
+
+    def mean_squared_log_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, **kwargs):
+        """
+        Mean Squared Log Error (MSLE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+        Link: https://peltarion.com/knowledge-center/documentation/modeling-view/build-an-ai-model/loss-functions/mean-squared-logarithmic-error-(msle)
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = True)
+
+        Returns:
+            result (float, int, np.ndarray): MSLE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.sum(np.log((y_true + 1) / (y_pred+1)) ** 2) / len(y_true), decimal)
+        else:
+            result = np.sum(np.log((y_true + 1) / (y_pred + 1)) ** 2, axis=0) / len(y_true)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def median_absolute_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Median Absolute Error (MedAE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): MedAE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.median(np.abs(y_true - y_pred)), decimal)
+        else:
+            result = np.median(np.abs(y_true - y_pred), axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def mean_relative_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False, **kwargs):
+        """
+        Mean Relative Error (MRE) - Mean Relative Bias (MRB): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): MRE (MRB) metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 0)
+        else:
+            y_true[y_true == 0] = self.EPSILON
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.mean(np.abs((y_pred - y_true) / y_true)), decimal)
+        else:
+            result = np.mean(np.abs((y_pred - y_true) / y_true), axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def mean_percentage_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False, **kwargs):
+        """
+        Mean Percentage Error (MPE): Best possible score is 0.0. Range = (-inf, +inf)
+        Link: https://www.dataquest.io/blog/understanding-regression-error-metrics/
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): MPE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 0)
+        else:
+            y_true[y_true == 0] = self.EPSILON
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.mean((y_true - y_pred) / y_true), decimal)
+        else:
+            result = np.mean((y_true - y_pred) / y_true, axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def mean_absolute_percentage_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False, **kwargs):
+        """
+        Mean Absolute Percentage Error (MAPE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): MAPE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 0)
+        else:
+            y_true[y_true == 0] = self.EPSILON
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.mean(np.abs(y_true - y_pred) / np.abs(y_true)), decimal)
+        else:
+            result = np.mean(np.abs(y_true - y_pred) / np.abs(y_true), axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def symmetric_mean_absolute_percentage_error(self, y_true=None, y_pred=None, multi_output="raw_values",
+                                                 decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Symmetric Mean Absolute Percentage Error (SMAPE): Best possible score is 0.0, smaller value is better. Range = [0, 1]
+        If you want percentage then multiply with 100%
+
+        Link: https://en.wikipedia.org/wiki/Symmetric_mean_absolute_percentage_error
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): SMAPE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.mean(np.abs(y_pred - y_true) / (np.abs(y_true) + np.abs(y_pred))), decimal)
+        else:
+            result = np.mean(np.abs(y_pred - y_true) / (np.abs(y_true) + np.abs(y_pred)), axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def mean_arctangent_absolute_percentage_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None,
+                                                  non_zero=False, positive=False, **kwargs):
+        """
+        Mean Arctangent Absolute Percentage Error (MAAPE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Link: https://support.numxl.com/hc/en-us/articles/115001223463-MAAPE-Mean-Arctangent-Absolute-Percentage-Error
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): MAAPE metric for single column or multiple columns (radian values)
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.mean(np.arctan(np.abs((y_true - y_pred)/y_true))), decimal)
+        else:
+            result = np.mean(np.arctan(np.abs((y_true - y_pred)/y_true)), axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def mean_absolute_scaled_error(self, y_true=None, y_pred=None, m=1, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Mean Absolute Scaled Error (MASE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Link: https://en.wikipedia.org/wiki/Mean_absolute_scaled_error
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            m (int): m = 1 for non-seasonal data, m > 1 for seasonal data
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): MASE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.mean(np.abs(y_true - y_pred)) / np.mean(np.abs(y_true[m:] - y_true[:-m])), decimal)
+        else:
+            result = np.mean(np.abs(y_true - y_pred), axis=0) / np.mean(np.abs(y_true[m:] - y_true[:-m]), axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def nash_sutcliffe_efficiency(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Nash-Sutcliffe Efficiency (NSE): Best possible score is 1.0, bigger value is better. Range = (-inf, 1]
+
+        Link: https://agrimetsoft.com/calculators/Nash%20Sutcliffe%20model%20Efficiency%20coefficient
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): NSE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        nse = calculate_nse(y_true, y_pred, one_dim)
+        return np.round(nse, decimal) if one_dim else self.get_multi_output_result(nse, multi_output, decimal)
+
+    def normalized_nash_sutcliffe_efficiency(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None,
+                                             non_zero=False, positive=False, **kwargs):
+        """
+        Normalize Nash-Sutcliffe Efficiency (NNSE): Best possible score is 1.0, bigger value is better. Range = [0, 1]
+
+        Link: https://agrimetsoft.com/calculators/Nash%20Sutcliffe%20model%20Efficiency%20coefficient
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): NSE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        nse = calculate_nse(y_true, y_pred, one_dim)
+        nnse = 1 / (2 - nse)
+        return np.round(nnse, decimal) if one_dim else self.get_multi_output_result(nnse, multi_output, decimal)
+
+    def willmott_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Willmott Index (WI): Best possible score is 1.0, bigger value is better. Range = [0, 1]
+
+        Notes
+        ~~~~~
+        + Reference evapotranspiration for Londrina, Paraná, Brazil: performance of different estimation methods
+        + https://www.researchgate.net/publication/319699360_Reference_evapotranspiration_for_Londrina_Parana_Brazil_performance_of_different_estimation_methods
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): WI metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        wi = calculate_wi(y_true, y_pred, one_dim)
+        return np.round(wi, decimal) if one_dim else self.get_multi_output_result(wi, multi_output, decimal)
+
+    def coefficient_of_determination(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Coefficient of Determination (COD/R2): Best possible score is 1.0, bigger value is better. Range = (-inf, 1]
+
+        Notes
+        ~~~~~
+            + https://scikit-learn.org/stable/modules/model_evaluation.html#r2-score
+            + Scikit-learn and other websites denoted COD as R^2 (or R squared), it leads to the misunderstanding of R^2 in which R is PCC.
+            + We should denote it as COD or R2 only.
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): R2 metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(1 - np.sum((y_true - y_pred) ** 2) / np.sum((y_true - np.mean(y_true)) ** 2), decimal)
+        else:
+            result = 1 - np.sum((y_true - y_pred) ** 2, axis=0) / np.sum((y_true - np.mean(y_true, axis=0)) ** 2, axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def adjusted_coefficient_of_determination(self, y_true=None, y_pred=None, X_shape=None, multi_output="raw_values", decimal=None,
+                                              non_zero=False, positive=False, **kwargs):
+        """
+        Adjusted Coefficient of Determination (ACOD/AR2): Best possible score is 1.0, bigger value is better. Range = (-inf, 1]
+
+        Notes
+        ~~~~~
+            + https://dziganto.github.io/data%20science/linear%20regression/machine%20learning/python/Linear-Regression-101-Metrics/
+            + Scikit-learn and other websites denoted COD as R^2 (or R squared), it leads to the misunderstanding of R^2 in which R is PCC.
+            + We should denote it as COD or R2 only.
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            X_shape (tuple, list, np.ndarray): The shape of X_train dataset
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): AR2 metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if X_shape is None:
+            raise ValueError("You need to pass the shape of X_train dataset to calculate Adjusted R2.")
+        if len(X_shape) != 2 or X_shape[0] < 4 or X_shape[1] < 1:
+            raise ValueError("You need to pass the real shape of X_train dataset to calculate Adjusted R2.")
+        dft = X_shape[0] - 1.0
+        dfe = X_shape[0] - X_shape[1] - 1.0
+        df_final = dft/dfe
+        if one_dim:
+            return np.round(1 - df_final * np.sum((y_true - y_pred) ** 2) / np.sum((y_true - np.mean(y_true)) ** 2), decimal)
+        else:
+            result = 1 - df_final * np.sum((y_true - y_pred) ** 2, axis=0) / np.sum((y_true - np.mean(y_true, axis=0)) ** 2, axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def pearson_correlation_coefficient(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Pearson’s Correlation Coefficient (PCC or R): Best possible score is 1.0, bigger value is better. Range = [-1, 1]
+        Notes
+        ~~~~~
+            + Reference evapotranspiration for Londrina, Paraná, Brazil: performance of different estimation methods
+            + Remember no absolute in the equations
+            + https://en.wikipedia.org/wiki/Pearson_correlation_coefficient
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): R metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        pcc = calculate_pcc(y_true, y_pred, one_dim)
+        return np.round(pcc, decimal) if one_dim else self.get_multi_output_result(pcc, multi_output, decimal)
+
+    def absolute_pearson_correlation_coefficient(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None,
+                                                 non_zero=False, positive=False, **kwargs):
+        """
+        Absolute Pearson’s Correlation Coefficient (APCC or AR): Best possible score is 1.0, bigger value is better. Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): AR metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        pcc = calculate_absolute_pcc(y_true, y_pred, one_dim)
+        return np.round(pcc, decimal) if one_dim else self.get_multi_output_result(pcc, multi_output, decimal)
+
+    def pearson_correlation_coefficient_square(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None,
+                                               non_zero=False, positive=False, **kwargs):
+        """
+        (Pearson’s Correlation Index)^2 = R^2 = R2s (R square): Best possible score is 1.0, bigger value is better. Range = [0, 1]
+        Notes
+        ~~~~~
+            + Do not misunderstand between R2s and R2 (Coefficient of Determination), they are different
+            + Most of online tutorials (article, wikipedia,...) or even scikit-learn library are denoted the wrong R2s and R2.
+            + R^2 = R2s = R squared should be (Pearson’s Correlation Index)^2
+            + Meanwhile, R2 = Coefficient of Determination
+            + https://en.wikipedia.org/wiki/Pearson_correlation_coefficient
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): R2s metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        pcc = calculate_pcc(y_true, y_pred, one_dim)
+        return np.round(pcc**2, decimal) if one_dim else self.get_multi_output_result(pcc**2, multi_output, decimal)
+
+    def confidence_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Confidence Index (or Performance Index): CI (PI): Best possible score is 1.0, bigger value is better. Range = (-inf, 1]
+
+        Notes
+        ~~~~~
+        - Reference evapotranspiration for Londrina, Paraná, Brazil: performance of different estimation methods
+        - > 0.85,          Excellent
+        - 0.76-0.85,       Very good
+        - 0.66-0.75,       Good
+        - 0.61-0.65,       Satisfactory
+        - 0.51-0.60,       Poor
+        - 0.41-0.50,       Bad
+        - < 0.40,          Very bad
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): CI (PI) metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        r = calculate_pcc(y_true, y_pred, one_dim)
+        d = calculate_wi(y_true, y_pred, one_dim)
+        return np.round(r*d, decimal) if one_dim else self.get_multi_output_result(r*d, multi_output, decimal)
+
+    def deviation_of_runoff_volume(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Deviation of Runoff Volume (DRV): Best possible score is 1.0, smaller value is better. Range = [1, +inf)
+        Link: https://rstudio-pubs-static.s3.amazonaws.com/433152_56d00c1e29724829bad5fc4fd8c8ebff.html
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): DRV metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.sum(y_pred) / np.sum(y_true), decimal)
+        else:
+            result = np.sum(y_pred, axis=0) / np.sum(y_true, axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def kling_gupta_efficiency(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Kling-Gupta Efficiency (KGE): Best possible score is 1, bigger value is better. Range = (-inf, 1]
+        Link: https://rstudio-pubs-static.s3.amazonaws.com/433152_56d00c1e29724829bad5fc4fd8c8ebff.html
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): KGE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            m1, m2 = np.mean(y_true), np.mean(y_pred)
+            r = np.sum((y_true - m1) * (y_pred - m2)) / (np.sqrt(np.sum((y_true - m1) ** 2)) * np.sqrt(np.sum((y_pred - m2) ** 2)))
+            beta = m2 / m1
+            gamma = (np.std(y_pred) / m2) / (np.std(y_true) / m1)
+            return np.round(1 - np.sqrt((r - 1) ** 2 + (beta - 1) ** 2 + (gamma - 1) ** 2), decimal)
+        else:
+            m1, m2 = np.mean(y_true, axis=0), np.mean(y_pred, axis=0)
+            num_r = np.sum((y_true - m1) * (y_pred - m2), axis=0)
+            den_r = np.sqrt(np.sum((y_true - m1) ** 2, axis=0)) * np.sqrt(np.sum((y_pred - m2) ** 2, axis=0))
+            r = num_r / den_r
+            beta = m2 / m1
+            gamma = (np.std(y_pred, axis=0) / m2) / (np.std(y_true, axis=0) / m1)
+            result = 1 - np.sqrt((r - 1) ** 2 + (beta - 1) ** 2 + (gamma - 1) ** 2)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def prediction_of_change_in_direction(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Prediction of Change in Direction (PCD): Best possible score is 1.0, bigger value is better. Range = [0, 1]
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): PCD metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            d = np.diff(y_true)
+            dp = np.diff(y_pred)
+            return np.round(np.mean(np.sign(d) == np.sign(dp)), decimal)
+        else:
+            d = np.diff(y_true, axis=0)
+            dp = np.diff(y_pred, axis=0)
+            result = np.mean(np.sign(d) == np.sign(dp), axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def cross_entropy(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=True, **kwargs):
+        """
+        Cross Entropy (CE) or Entropy (E): Range = (-inf, 0]. Can't give comment about this one
+
+        Notes
+        ~~~~~
+            + Greater value of Entropy, the greater the uncertainty for probability distribution and smaller the value the less the uncertainty
+            + https://datascience.stackexchange.com/questions/20296/cross-entropy-loss-explanation
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = True)
+
+        Returns:
+            result (float, int, np.ndarray): CE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        else:
+            y_pred[y_pred == 0] = self.EPSILON
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        entropy = calculate_entropy(y_true, y_pred, one_dim)
+        return np.round(entropy, decimal) if one_dim else self.get_multi_output_result(entropy, multi_output, decimal)
+
+    def kullback_leibler_divergence(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, **kwargs):
+        """
+        Kullback-Leibler Divergence (KLD): Best possible score is 0.0 . Range = (-inf, +inf)
+        Link: https://machinelearningmastery.com/divergence-between-probability-distributions/
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = True)
+
+        Returns:
+            result (float, int, np.ndarray): KLD metric (bits) for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        else:
+            y_pred[y_pred == 0] = self.EPSILON
+        y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round(np.sum(y_true * np.log2(y_true / y_pred)), decimal)
+        else:
+            score = np.sum(y_true * np.log2(y_true / y_pred), axis=0)
+            return self.get_multi_output_result(score, multi_output, decimal)
+
+    def jensen_shannon_divergence(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=True, **kwargs):
+        """
+        Jensen-Shannon Divergence (JSD): Best possible score is 0.0 (identical), smaller value is better . Range = [0, +inf)
+        Link: https://machinelearningmastery.com/divergence-between-probability-distributions/
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = True)
+
+        Returns:
+            result (float, int, np.ndarray): JSD metric (bits) for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            m = 0.5 * (y_true + y_pred)
+            score = 0.5 * np.sum(y_true * np.log2(y_true / m)) + 0.5 * np.sum(y_pred * np.log2(y_pred / m))
+            return np.round(score, decimal)
+        else:
+            m = 0.5 * (y_true + y_pred)
+            score = 0.5 * np.sum(y_true * np.log2(y_true / m), axis=0) + 0.5 * np.sum(y_pred * np.log2(y_pred / m), axis=0)
+            return self.get_multi_output_result(score, multi_output, decimal)
+
+    def variance_accounted_for(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Variance Accounted For between 2 signals (VAF): Best possible score is 100% (identical signal), bigger value is better. Range = (-inf, 100%]
+
+        Link: https://www.dcsc.tudelft.nl/~jwvanwingerden/lti/doc/html/vaf.html
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): VAF metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 0)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+
+        if one_dim:
+            return np.round((1 - np.var(y_true - y_pred) / np.var(y_true)) * 100, decimal)
+        else:
+            result = (1 - np.var(y_true - y_pred, axis=0) / np.var(y_true, axis=0)) * 100
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def relative_absolute_error(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Relative Absolute Error (RAE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Notes
+        ~~~~~
+            + https://stackoverflow.com/questions/59499222/how-to-make-a-function-of-mae-and-rae-without-using-librarymetrics
+            + https://www.statisticshowto.com/relative-absolute-error
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): RAE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            numerator = np.power(np.sum((y_pred - y_true)**2), 1/2)
+            denominator = np.power(np.sum(y_true**2), 1/2)
+            return np.round(numerator/denominator, decimal)
+        else:
+            numerator = np.power(np.sum((y_pred - y_true) ** 2, axis=0), 1 / 2)
+            denominator = np.power(np.sum(y_true ** 2, axis=0), 1 / 2)
+            return self.get_multi_output_result(numerator/denominator, multi_output, decimal)
+
+    def a10_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False, **kwargs):
+        """
+        A10 index (A10): Best possible score is 1.0, bigger value is better. Range = [0, 1]
+
+        Notes
+        ~~~~~
+            + a10-index is engineering index for evaluating artificial intelligence models by showing the number of samples
+            + that fit the prediction values with a deviation of ±10% compared to experimental values
+            + https://www.mdpi.com/2076-3417/9/18/3715/htm
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): A10 metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        else:
+            y_pred[y_pred == 0] = self.EPSILON
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+
+        if one_dim:
+            div = y_true / y_pred
+            div = np.where(np.logical_and(div >= 0.9, div <= 1.1), 1, 0)
+            return np.round(np.mean(div), decimal)
+        else:
+            div = y_true / y_pred
+            div = np.where(np.logical_and(div >= 0.9, div <= 1.1), 1, 0)
+            return self.get_multi_output_result(np.mean(div, axis=0), multi_output, decimal)
+
+    def a20_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False, **kwargs):
+        """
+        A20 index (A20): Best possible score is 1.0, bigger value is better. Range = [0, 1]
+
+        Notes
+        ~~~~~
+            + a20-index evaluated metric by showing the number of samples that fit the prediction values with a deviation of ±20% compared to experimental values
+            + https://www.mdpi.com/2076-3417/9/18/3715/htm
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): A20 metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        else:
+            y_pred[y_pred == 0] = self.EPSILON
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            div = y_true / y_pred
+            div = np.where(np.logical_and(div >= 0.8, div <= 1.2), 1, 0)
+            return np.round(np.mean(div), decimal)
+        else:
+            div = y_true / y_pred
+            div = np.where(np.logical_and(div >= 0.8, div <= 1.2), 1, 0)
+            return self.get_multi_output_result(np.mean(div, axis=0), multi_output, decimal)
+
+    def a30_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=True, positive=False, **kwargs):
+        """
+        A30 index (A30): Best possible score is 1.0, bigger value is better. Range = [0, 1]
+
+        Note: a30-index evaluated metric by showing the number of samples that fit the prediction values with a deviation of ±30% compared to experimental values
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): A30 metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        else:
+            y_pred[y_pred == 0] = self.EPSILON
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            div = y_true / y_pred
+            div = np.where(np.logical_and(div >= 0.7, div <= 1.3), 1, 0)
+            return np.round(np.mean(div), decimal)
+        else:
+            div = y_true / y_pred
+            div = np.where(np.logical_and(div >= 0.7, div <= 1.3), 1, 0)
+            return self.get_multi_output_result(np.mean(div, axis=0), multi_output, decimal)
+
+    def normalized_root_mean_square_error(self, y_true=None, y_pred=None, model=0, multi_output="raw_values", decimal=None,
+                                          non_zero=False, positive=False, **kwargs):
+        """
+        Normalized Root Mean Square Error (NRMSE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Link: https://medium.com/microsoftazure/how-to-better-evaluate-the-goodness-of-fit-of-regressions-990dbf1c0091
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            model (int): Normalize RMSE by different ways, (Optional, default = 0, valid values = [0, 1, 2, 3]
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): NRMSE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            rmse = np.sqrt(np.mean((y_pred - y_true) ** 2))
+            if model == 1:
+                result = rmse / np.mean(y_pred)
+            elif model == 2:
+                result = rmse / (np.max(y_true) - np.min(y_true))
+            elif model == 3:
+                result = np.sqrt(np.sum(np.log((y_pred + 1) / (y_true + 1)) ** 2) / len(y_true))
+            else:
+                result = rmse / y_pred.std()
+            return np.round(result, decimal)
+        else:
+            rmse = np.sqrt(np.sum((y_pred - y_true) ** 2, axis=0) / len(y_true))
+            if model == 1:
+                result = rmse / np.mean(y_pred, axis=0)
+            elif model == 2:
+                result = rmse / (np.max(y_true, axis=0) - np.min(y_true, axis=0))
+            elif model == 3:
+                result = np.sqrt(np.sum(np.log((y_pred + 1) / (y_true + 1)) ** 2, axis=0) / len(y_true))
+            else:
+                result = rmse / y_pred.std(axis=0)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def residual_standard_error(self, y_true=None, y_pred=None, n_paras=None, multi_output="raw_values", decimal=None,
+                                non_zero=False, positive=False, **kwargs):
+        """
+        Residual Standard Error (RSE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Links:
+            + https://www.statology.org/residual-standard-error-r/
+            + https://machinelearningmastery.com/degrees-of-freedom-in-machine-learning/
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            n_paras (int): The number of model's parameters
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): RSE metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if n_paras is None:
+            n_paras = len(y_true) / 2
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            ss_residuals = np.sum((y_true - y_pred)**2)
+            df_residuals = len(y_true) - n_paras - 1
+            return np.round(np.sqrt(ss_residuals / df_residuals), decimal)
+        else:
+            ss_residuals = np.sum((y_true - y_pred) ** 2, axis=0)
+            df_residuals = len(y_true) - n_paras - 1
+            score = np.sqrt(ss_residuals / df_residuals)
+            return self.get_multi_output_result(score, multi_output, decimal)
+
+    def covariance(self, y_true=None, y_pred=None, sample=False, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Covariance (COV): There is no best value, bigger value is better. Range = [-inf, +inf)
+            + is a measure of the relationship between two random variables
+            + evaluates how much – to what extent – the variables change together
+            + does not assess the dependency between variables
+            + Positive covariance: Indicates that two variables tend to move in the same direction.
+            + Negative covariance: Reveals that two variables tend to move in inverse directions.
+
+        Links:
+            + https://corporatefinanceinstitute.com/resources/data-science/covariance/
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            sample (bool): sample covariance or population covariance. See the website above for more details
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): COV metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        denominator = len(y_true) - 1 if sample else len(y_true)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            s1 = y_true - np.mean(y_true)
+            s2 = y_pred - np.mean(y_pred)
+            return np.round(np.dot(s1, s2) / denominator, decimal)
+        else:
+            s1 = y_true - np.mean(y_true, axis=0)
+            s2 = y_pred - np.mean(y_pred, axis=0)
+            return self.get_multi_output_result(np.sum(s1 * s2, axis=0) / denominator, multi_output, decimal)
+
+    def correlation(self, y_true=None, y_pred=None, sample=False, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Correlation (COR): Best possible value = 1, bigger value is better. Range = [-1, +1]
+            + measures the strength of the relationship between variables
+            + is the scaled measure of covariance. It is dimensionless.
+            + the correlation coefficient is always a pure value and not measured in any units.
+
+        Links:
+            + https://corporatefinanceinstitute.com/resources/data-science/covariance/
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            sample (bool): sample covariance or population covariance. See the website above for more details
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): COR metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        denominator = len(y_true) - 1 if sample else len(y_true)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            s1 = y_true - np.mean(y_true)
+            s2 = y_pred - np.mean(y_pred)
+            return np.round((np.dot(s1, s2) / denominator) / (np.std(y_true) * np.std(y_pred)), decimal)
+        else:
+            s1 = y_true - np.mean(y_true, axis=0)
+            s2 = y_pred - np.mean(y_pred, axis=0)
+            cov = np.sum(s1 * s2, axis=0) / denominator
+            den = np.std(y_true, axis=0) * np.std(y_pred, axis=0)
+            return self.get_multi_output_result(cov / den, multi_output, decimal)
+
+    def efficiency_coefficient(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Efficiency Coefficient (EC): Best possible value = 1, bigger value is better. Range = [-inf, +1]
+
+        Links:
+            + https://doi.org/10.1016/j.solener.2019.01.037
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): EC metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        score = calculate_ec(y_true, y_pred, one_dim)
+        return np.round(score, decimal) if one_dim else self.get_multi_output_result(score, multi_output, decimal)
+
+    def overall_index(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Overall Index (OI): Best possible value = 1, bigger value is better. Range = [-inf, +1]
+
+        Links:
+            + https://doi.org/10.1016/j.solener.2019.01.037
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): OI metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        ec = calculate_ec(y_true, y_pred, one_dim)
+        rmse = np.sqrt(calculate_mse(y_true, y_pred, one_dim))
+        if one_dim:
+            score = (1 - rmse / (np.max(y_true) - np.min(y_true)) + ec) / 2.0
+            return np.round(score, decimal)
+        else:
+            score = (1 - rmse / (np.max(y_true, axis=0) - np.min(y_true, axis=0)) + ec) / 2.0
+            return self.get_multi_output_result(score, multi_output, decimal)
+
+    def coefficient_of_residual_mass(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Coefficient of Residual Mass (CRM): Best possible value = 0.0, smaller value is better. Range = [-inf, +inf]
+
+        Links:
+            + https://doi.org/10.1016/j.csite.2022.101797
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): CRM metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            return np.round((np.sum(y_pred) - np.sum(y_true)) / np.sum(y_true), decimal)
+        else:
+            score = (np.sum(y_pred, axis=0) - np.sum(y_true, axis=0)) / np.sum(y_true, axis=0)
+            return self.get_multi_output_result(score, multi_output, decimal)
+
+    def gini_coefficient(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Gini coefficient (Gini): Best possible score is 1, bigger value is better. Range = [0, 1]
+
+        Notes
+        ~~~~~
+            + This version is based on below repository matlab code.
+            + https://github.com/benhamner/Metrics/blob/master/MATLAB/metrics/gini.m
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): Gini metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            idx_sort = np.argsort(-y_pred)
+            population_delta = 1.0 / len(y_true)
+            accumulated_population_percentage_sum, accumulated_loss_percentage_sum, score = 0, 0, 0
+            total_losses = np.sum(y_true)
+            for i in range(0, len(y_true)):
+                accumulated_loss_percentage_sum += y_true[idx_sort[i]] / total_losses
+                accumulated_population_percentage_sum += population_delta
+                score += accumulated_loss_percentage_sum - accumulated_population_percentage_sum
+            score = score / len(y_true)
+            return np.round(score, decimal)
+        else:
+            col = y_true.shape[1]
+            idx_sort = np.argsort(-y_pred, axis=0)
+            population_delta = 1.0 / len(y_true)
+            accumulated_population_percentage_sum, accumulated_loss_percentage_sum, score = np.zeros(col), np.zeros(col), np.zeros(col)
+            total_losses = np.sum(y_true, axis=0)
+            for i in range(0, col):
+                for j in range(0, len(y_true)):
+                    accumulated_loss_percentage_sum[i] += y_true[idx_sort[j, i], i] / total_losses[i]
+                    accumulated_population_percentage_sum[i] += population_delta
+                    score[i] += accumulated_loss_percentage_sum[i] - accumulated_population_percentage_sum[i]
+            result = score / len(y_true)
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def gini_coefficient_wiki(self, y_true=None, y_pred=None, multi_output="raw_values", decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Gini coefficient (Gini): Best possible score is 1, bigger value is better. Range = [0, 1]
+
+        Notes
+        ~~~~~
+            + This version is based on wiki page, may be is the true version
+            + https://en.wikipedia.org/wiki/Gini_coefficient
+            + Gini coefficient can theoretically range from 0 (complete equality) to 1 (complete inequality)
+            + It is sometimes expressed as a percentage ranging between 0 and 100.
+            + If negative values are possible, then the Gini coefficient could theoretically be more than 1.
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            multi_output: Can be "raw_values" or list weights of variables such as [0.5, 0.2, 0.3] for 3 columns, (Optional, default = "raw_values")
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (float, int, np.ndarray): Gini metric for single column or multiple columns
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        if one_dim:
+            y = np.concatenate((y_true, y_pred), axis=0)
+            score = 0
+            for i in range(0, len(y)):
+                score += np.sum(np.abs(y[i] - y))
+            score = score / (2 * len(y) * np.sum(y))
+            return np.round(score, decimal)
+        else:
+            y = np.concatenate((y_true, y_pred), axis=0)
+            col = y.shape[1]
+            d = len(y)
+            score = np.zeros(col)
+            for k in range(0, col):
+                for i in range(0, d):
+                    for j in range(0, d):
+                        score[k] += np.abs(y[i, k] - y[j, k])
+            result = score / (2 * len(y) ** 2 * np.mean(y, axis=0))
+            return self.get_multi_output_result(result, multi_output, decimal)
+
+    def single_relative_error(self, y_true=None, y_pred=None, decimal=None, non_zero=True, positive=False, **kwargs):
+        """
+        Relative Error (RE): Best possible score is 0.0, smaller value is better. Range = (-inf, +inf)
+
+        Note: Computes the relative error between two numbers, or for element between a pair of list, tuple or numpy arrays.
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (np.ndarray): RE metric
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 0)
+        else:
+            y_true[y_true == 0] = self.EPSILON
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        return np.round(y_pred / y_true - 1, decimal)
+
+    def single_absolute_error(self, y_true=None, y_pred=None, decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Absolute Error (AE): Best possible score is 0.0, smaller value is better. Range = (-inf, +inf)
+
+        Note: Computes the absolute error between two numbers, or for element between a pair of list, tuple or numpy arrays.
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (np.ndarray): AE metric
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        return np.round(np.abs(y_true) - np.abs(y_pred), decimal)
+
+    def single_squared_error(self, y_true=None, y_pred=None, decimal=None, non_zero=False, positive=False, **kwargs):
+        """
+        Squared Error (SE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Note: Computes the squared error between two numbers, or for element between a pair of list, tuple or numpy arrays.
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = False)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = False)
+
+        Returns:
+            result (np.ndarray): SE metric
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 2)
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        return np.round((y_true - y_pred) ** 2, decimal)
+
+    def single_squared_log_error(self, y_true=None, y_pred=None, decimal=None, non_zero=True, positive=True, **kwargs):
+        """
+        Squared Log Error (SLE): Best possible score is 0.0, smaller value is better. Range = [0, +inf)
+
+        Note: Computes the squared log error between two numbers, or for element between a pair of list, tuple or numpy arrays.
+
+        Args:
+            y_true (tuple, list, np.ndarray): The ground truth values
+            y_pred (tuple, list, np.ndarray): The prediction values
+            decimal (int): The number of fractional parts after the decimal point (Optional, default = 5)
+            non_zero (bool): Remove all rows contain 0 value in y_pred (some methods have denominator is y_pred) (Optional, default = True)
+            positive (bool): Calculate metric based on positive values only or not (Optional, default = True)
+
+        Returns:
+            result (np.ndarray): SLE metric
+        """
+        y_true, y_pred, one_dim, decimal = self.get_processed_data(y_true, y_pred, decimal)
+        if non_zero:
+            y_true, y_pred = get_regression_non_zero_data(y_true, y_pred, one_dim, 1)
+        else:
+            y_pred[y_pred == 0] = self.EPSILON
+        if positive:
+            y_true, y_pred = get_regression_positive_data(y_true, y_pred, one_dim, 2)
+        return np.round((np.log(y_true) - np.log(y_pred)) ** 2, decimal)
+
+    EVS = explained_variance_score
+    ME = max_error
+    MBE = mean_bias_error
+    MAE = mean_absolute_error
+    MSE = mean_squared_error
+    RMSE = root_mean_squared_error
+    MSLE = mean_squared_log_error
+    MedAE = median_absolute_error
+    MRE = MRB = mean_relative_bias = mean_relative_error
+    MPE = mean_percentage_error
+    MAPE = mean_absolute_percentage_error
+    SMAPE = symmetric_mean_absolute_percentage_error
+    MAAPE = mean_arctangent_absolute_percentage_error
+    MASE = mean_absolute_scaled_error
+    NSE = nash_sutcliffe_efficiency
+    NNSE = normalized_nash_sutcliffe_efficiency
+    WI = willmott_index
+    R = PCC = pearson_correlation_coefficient
+    AR = APCC = absolute_pearson_correlation_coefficient
+    RSQ = R2S = pearson_correlation_coefficient_square
+    CI = confidence_index
+    COD = R2 = coefficient_of_determination
+    ACOD = AR2 = adjusted_coefficient_of_determination
+    DRV = deviation_of_runoff_volume
+    KGE = kling_gupta_efficiency
+    PCD = prediction_of_change_in_direction
+    CE = cross_entropy
+    KLD = kullback_leibler_divergence
+    JSD = jensen_shannon_divergence
+    VAF = variance_accounted_for
+    RAE = relative_absolute_error
+    A10 = a10_index
+    A20 = a20_index
+    A30 = a30_index
+    NRMSE = normalized_root_mean_square_error
+    RSE = residual_standard_error
+    COV = covariance
+    COR = correlation
+    EC = efficiency_coefficient
+    OI = overall_index
+    CRM = coefficient_of_residual_mass
+    GINI = gini_coefficient
+    GINI_WIKI = gini_coefficient_wiki
+
+    RE = RB = single_relative_bias = single_relative_error
+    AE = single_absolute_error
+    SE = single_squared_error
+    SLE = single_squared_log_error
```

### Comparing `permetrics-1.4.0/permetrics/utils/data_util.py` & `permetrics-1.4.1/permetrics/utils/data_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,204 +1,205 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 12:12, 19/05/2022 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import numpy as np
-import copy as cp
-from permetrics.utils.encoder import LabelEncoder
-
-
-def format_regression_data_type(y_true, y_pred):
-    if isinstance(y_true, (list, tuple, np.ndarray)) and isinstance(y_pred, (list, tuple, np.ndarray)):
-        ## Remove all dimensions of size 1
-        y_true, y_pred = np.squeeze(np.asarray(y_true, dtype='float64')), np.squeeze(np.asarray(y_pred, dtype='float64'))
-        if y_true.ndim == y_pred.ndim:
-            return y_true, y_pred
-        else:
-            raise ValueError("y_true and y_pred must have the same number of dimensions.")
-    else:
-        raise TypeError("y_true and y_pred must be lists, tuples or numpy arrays.")
-
-
-def format_regression_data(y_true: np.ndarray, y_pred: np.ndarray):
-    if y_true.ndim == y_pred.ndim == 1:
-        ## Remove all Nan in y_pred
-        y_true = y_true[~np.isnan(y_pred)]
-        y_pred = y_pred[~np.isnan(y_pred)]
-        ## Remove all Inf in y_pred
-        y_true = y_true[np.isfinite(y_pred)]
-        y_pred = y_pred[np.isfinite(y_pred)]
-        return y_true, y_pred, True
-    elif y_true.ndim == y_pred.ndim > 1:
-        ## Remove all row with Nan in y_pred
-        y_true = y_true[~np.isnan(y_pred).any(axis=1)]
-        y_pred = y_pred[~np.isnan(y_pred).any(axis=1)]
-        ## Remove all row with Inf in y_pred
-        y_true = y_true[np.isfinite(y_pred).all(axis=1)]
-        y_pred = y_pred[np.isfinite(y_pred).all(axis=1)]
-        return y_true, y_pred, False
-
-
-def get_regression_non_zero_data(y_true, y_pred, one_dim=True, rule_idx=0):
-    """
-    Get non-zero data based on rule
-
-    Args:
-        y_true (tuple, list, np.ndarray): The ground truth values
-        y_pred (tuple, list, np.ndarray): The prediction values
-        one_dim (bool): is y_true has 1 dimensions or not
-        rule_idx (int): valid values [0, 1, 2] corresponding to [y_true, y_pred, both true and pred]
-
-    Returns:
-        y_true: y_true with positive values based on rule
-        y_pred: y_pred with positive values based on rule
-
-    """
-    if rule_idx == 0:
-        y_rule = cp.deepcopy(y_true)
-    elif rule_idx == 1:
-        y_rule = cp.deepcopy(y_pred)
-    else:
-        if one_dim:
-            y_true_non, y_pred_non = y_true[y_true != 0], y_pred[y_true != 0]
-            y_true, y_pred = y_true_non[y_pred_non != 0], y_pred_non[y_pred_non != 0]
-        else:
-            y_true_non, y_pred_non = y_true[~np.any(y_true == 0, axis=1)], y_pred[~np.any(y_true == 0, axis=1)]
-            y_true, y_pred = y_true_non[~np.any(y_pred_non == 0, axis=1)], y_pred_non[~np.any(y_pred_non == 0, axis=1)]
-        return y_true, y_pred
-    if one_dim:
-        y_true, y_pred = y_true[y_rule != 0], y_pred[y_rule != 0]
-    else:
-        y_true, y_pred = y_true[~np.any(y_rule == 0, axis=1)], y_pred[~np.any(y_rule == 0, axis=1)]
-    return y_true, y_pred
-
-
-def get_regression_positive_data(y_true, y_pred, one_dim=True, rule_idx=0):
-    """
-    Get positive data based on rule
-
-    Args:
-        y_true (tuple, list, np.ndarray): The ground truth values
-        y_pred (tuple, list, np.ndarray): The prediction values
-        one_dim (bool): is y_true has 1 dimensions or not
-        rule_idx (int): valid values [0, 1, 2] corresponding to [y_true, y_pred, both true and pred]
-
-    Returns:
-        y_true: y_true with positive values based on rule
-        y_pred: y_pred with positive values based on rule
-    """
-    if rule_idx == 0:
-        y_rule = cp.deepcopy(y_true)
-    elif rule_idx == 1:
-        y_rule = cp.deepcopy(y_pred)
-    else:
-        if one_dim:
-            y_true_non, y_pred_non = y_true[y_true > 0], y_pred[y_true > 0]
-            y_true, y_pred = y_true_non[y_pred_non > 0], y_pred_non[y_pred_non > 0]
-        else:
-            y_true_non, y_pred_non = y_true[np.all(y_true > 0, axis=1)], y_pred[np.all(y_true > 0, axis=1)]
-            y_true, y_pred = y_true_non[np.all(y_pred_non > 0, axis=1)], y_pred_non[np.all(y_pred_non > 0, axis=1)]
-        return y_true, y_pred
-    if one_dim:
-        y_true, y_pred = y_true[y_rule > 0], y_pred[y_rule > 0]
-    else:
-        y_true, y_pred = y_true[np.all(y_rule > 0, axis=1)], y_pred[np.all(y_rule > 0, axis=1)]
-    return y_true, y_pred
-
-
-def format_classification_data(y_true: np.ndarray, y_pred: np.ndarray):
-    if not (isinstance(y_true, (list, tuple, np.ndarray)) and isinstance(y_pred, (list, tuple, np.ndarray))):
-        raise TypeError("y_true and y_pred must be lists, tuples or numpy arrays.")
-    else:
-        ## Remove all dimensions of size 1
-        y_true, y_pred = np.squeeze(np.asarray(y_true)), np.squeeze(np.asarray(y_pred))
-        if not (y_true.ndim == y_pred.ndim):
-            raise TypeError("y_true and y_pred must have the same number of dimensions.")
-        else:
-            if np.issubdtype(y_true.dtype, np.number):
-                var_type = "number"
-                if y_true.ndim > 1:
-                    y_true, y_pred = y_true.argmax(axis=1), y_pred.argmax(axis=1)
-            else:
-                var_type = "string"
-                if y_true.ndim > 1:
-                    raise ValueError("y_true and y_pred have n_dim > 1 need to be a number.")
-            unique_true, unique_pred = sorted(np.unique(y_true)), sorted(np.unique(y_pred))
-            if not (len(unique_pred) <= len(unique_true) and np.isin(unique_pred, unique_true).all()):
-                raise ValueError("Existed at least one new label in y_pred.")
-            else:
-                binary = len(unique_true) == 2
-            return y_true, y_pred, binary, var_type
-
-
-def format_y_score(y_true: np.ndarray, y_score: np.ndarray):
-    binary = True
-    if not (isinstance(y_true, (list, tuple, np.ndarray)) and isinstance(y_score, (list, tuple, np.ndarray))):
-        raise TypeError("y_true and y_score must be lists, tuples or numpy arrays.")
-    else:
-        y_true, y_score = np.squeeze(np.asarray(y_true)), np.squeeze(np.asarray(y_score))
-        if y_true.ndim == y_score.ndim:
-            if len(np.unique(y_true)) != 2:
-                raise TypeError("y_true should have two classes only or y_score must have shape (n_examples, n_labels)")
-            else:
-                if np.issubdtype(y_true.dtype, np.number):
-                    return y_true, y_score, binary, "number"
-                else:
-                    return y_true, y_score, binary, "string"
-        else:
-            if len(np.unique(y_true)) <= 2:
-                raise TypeError("y_score must have shape (n_examples, n_labels) in case of multi-classification problem")
-            else:
-                if np.issubdtype(y_true.dtype, np.number):
-                    return y_true, y_score, not binary, "number"
-                else:
-                    return y_true, y_score, not binary, "string"
-
-
-def is_consecutive_and_start_zero(vector):
-    if sorted(vector) == list(range(min(vector), max(vector) + 1)):
-        if 0 in vector:
-            return True
-    return False
-
-
-def format_external_clustering_data(y_true: np.ndarray, y_pred: np.ndarray):
-    """
-    Need both of y_true and y_pred to format
-    """
-    if not (isinstance(y_true, (list, tuple, np.ndarray)) and isinstance(y_pred, (list, tuple, np.ndarray))):
-        raise TypeError("To calculate external clustering metrics, y_true and y_pred must be lists, tuples or numpy arrays.")
-    else:
-        ## Remove all dimensions of size 1
-        y_true, y_pred = np.squeeze(np.asarray(y_true)), np.squeeze(np.asarray(y_pred))
-        if not (y_true.ndim == y_pred.ndim):
-            raise TypeError("To calculate external clustering metrics, y_true and y_pred must have the same number of dimensions.")
-        else:
-            if y_true.ndim == 1:
-                if np.issubdtype(y_true.dtype, np.number):
-                    if is_consecutive_and_start_zero(y_true):
-                        return y_true, y_pred, None
-                le = LabelEncoder()
-                y_true = le.fit_transform(y_true)
-                y_pred = le.transform(y_pred)
-                return y_true, y_pred, le
-            else:
-                raise TypeError("To calculate clustering metrics, y_true and y_pred must be a 1-D vector.")
-
-
-def format_internal_clustering_data(labels: np.ndarray):
-    if not (isinstance(labels, (list, tuple, np.ndarray))):
-        raise TypeError("To calculate internal clustering metrics, labels must be lists, tuples or numpy arrays.")
-    else:
-        ## Remove all dimensions of size 1
-        labels = np.squeeze(np.asarray(labels))
-        if labels.ndim == 1:
-            if np.issubdtype(labels.dtype, np.number):
-                if is_consecutive_and_start_zero(labels):
-                    return labels, None
-            le = LabelEncoder()
-            labels = le.fit_transform(labels)
-            return labels, le
-        else:
-            raise TypeError("To calculate clustering metrics, labels must be a 1-D vector.")
+#!/usr/bin/env python
+# Created by "Thieu" at 12:12, 19/05/2022 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import numpy as np
+import copy as cp
+from permetrics.utils.encoder import LabelEncoder
+
+
+def format_regression_data_type(y_true, y_pred):
+    if isinstance(y_true, (list, tuple, np.ndarray)) and isinstance(y_pred, (list, tuple, np.ndarray)):
+        ## Remove all dimensions of size 1
+        y_true, y_pred = np.squeeze(np.asarray(y_true, dtype='float64')), np.squeeze(np.asarray(y_pred, dtype='float64'))
+        if y_true.ndim == y_pred.ndim:
+            return y_true, y_pred
+        else:
+            raise ValueError("y_true and y_pred must have the same number of dimensions.")
+    else:
+        raise TypeError("y_true and y_pred must be lists, tuples or numpy arrays.")
+
+
+def format_regression_data(y_true: np.ndarray, y_pred: np.ndarray):
+    if y_true.ndim == y_pred.ndim == 1:
+        ## Remove all Nan in y_pred
+        y_true = y_true[~np.isnan(y_pred)]
+        y_pred = y_pred[~np.isnan(y_pred)]
+        ## Remove all Inf in y_pred
+        y_true = y_true[np.isfinite(y_pred)]
+        y_pred = y_pred[np.isfinite(y_pred)]
+        return y_true, y_pred, True
+    elif y_true.ndim == y_pred.ndim > 1:
+        ## Remove all row with Nan in y_pred
+        y_true = y_true[~np.isnan(y_pred).any(axis=1)]
+        y_pred = y_pred[~np.isnan(y_pred).any(axis=1)]
+        ## Remove all row with Inf in y_pred
+        y_true = y_true[np.isfinite(y_pred).all(axis=1)]
+        y_pred = y_pred[np.isfinite(y_pred).all(axis=1)]
+        return y_true, y_pred, False
+
+
+def get_regression_non_zero_data(y_true, y_pred, one_dim=True, rule_idx=0):
+    """
+    Get non-zero data based on rule
+
+    Args:
+        y_true (tuple, list, np.ndarray): The ground truth values
+        y_pred (tuple, list, np.ndarray): The prediction values
+        one_dim (bool): is y_true has 1 dimensions or not
+        rule_idx (int): valid values [0, 1, 2] corresponding to [y_true, y_pred, both true and pred]
+
+    Returns:
+        y_true: y_true with positive values based on rule
+        y_pred: y_pred with positive values based on rule
+
+    """
+    if rule_idx == 0:
+        y_rule = cp.deepcopy(y_true)
+    elif rule_idx == 1:
+        y_rule = cp.deepcopy(y_pred)
+    else:
+        if one_dim:
+            y_true_non, y_pred_non = y_true[y_true != 0], y_pred[y_true != 0]
+            y_true, y_pred = y_true_non[y_pred_non != 0], y_pred_non[y_pred_non != 0]
+        else:
+            y_true_non, y_pred_non = y_true[~np.any(y_true == 0, axis=1)], y_pred[~np.any(y_true == 0, axis=1)]
+            y_true, y_pred = y_true_non[~np.any(y_pred_non == 0, axis=1)], y_pred_non[~np.any(y_pred_non == 0, axis=1)]
+        return y_true, y_pred
+    if one_dim:
+        y_true, y_pred = y_true[y_rule != 0], y_pred[y_rule != 0]
+    else:
+        y_true, y_pred = y_true[~np.any(y_rule == 0, axis=1)], y_pred[~np.any(y_rule == 0, axis=1)]
+    return y_true, y_pred
+
+
+def get_regression_positive_data(y_true, y_pred, one_dim=True, rule_idx=0):
+    """
+    Get positive data based on rule
+
+    Args:
+        y_true (tuple, list, np.ndarray): The ground truth values
+        y_pred (tuple, list, np.ndarray): The prediction values
+        one_dim (bool): is y_true has 1 dimensions or not
+        rule_idx (int): valid values [0, 1, 2] corresponding to [y_true, y_pred, both true and pred]
+
+    Returns:
+        y_true: y_true with positive values based on rule
+        y_pred: y_pred with positive values based on rule
+    """
+    if rule_idx == 0:
+        y_rule = cp.deepcopy(y_true)
+    elif rule_idx == 1:
+        y_rule = cp.deepcopy(y_pred)
+    else:
+        if one_dim:
+            y_true_non, y_pred_non = y_true[y_true > 0], y_pred[y_true > 0]
+            y_true, y_pred = y_true_non[y_pred_non > 0], y_pred_non[y_pred_non > 0]
+        else:
+            y_true_non, y_pred_non = y_true[np.all(y_true > 0, axis=1)], y_pred[np.all(y_true > 0, axis=1)]
+            y_true, y_pred = y_true_non[np.all(y_pred_non > 0, axis=1)], y_pred_non[np.all(y_pred_non > 0, axis=1)]
+        return y_true, y_pred
+    if one_dim:
+        y_true, y_pred = y_true[y_rule > 0], y_pred[y_rule > 0]
+    else:
+        y_true, y_pred = y_true[np.all(y_rule > 0, axis=1)], y_pred[np.all(y_rule > 0, axis=1)]
+    return y_true, y_pred
+
+
+def format_classification_data(y_true: np.ndarray, y_pred: np.ndarray):
+    if not (isinstance(y_true, (list, tuple, np.ndarray)) and isinstance(y_pred, (list, tuple, np.ndarray))):
+        raise TypeError("y_true and y_pred must be lists, tuples or numpy arrays.")
+    else:
+        ## Remove all dimensions of size 1
+        y_true, y_pred = np.squeeze(np.asarray(y_true)), np.squeeze(np.asarray(y_pred))
+        if not (y_true.ndim == y_pred.ndim):
+            raise TypeError("y_true and y_pred must have the same number of dimensions.")
+        else:
+            if np.issubdtype(y_true.dtype, np.number):
+                var_type = "number"
+                if y_true.ndim > 1:
+                    y_true, y_pred = y_true.argmax(axis=1), y_pred.argmax(axis=1)
+            else:
+                var_type = "string"
+                if y_true.ndim > 1:
+                    raise ValueError("y_true and y_pred have n_dim > 1 need to be a number.")
+            unique_true, unique_pred = sorted(np.unique(y_true)), sorted(np.unique(y_pred))
+            if not (len(unique_pred) <= len(unique_true) and np.isin(unique_pred, unique_true).all()):
+                raise ValueError("Existed at least one new label in y_pred.")
+            else:
+                binary = len(unique_true) == 2
+            return y_true, y_pred, binary, var_type
+
+
+def format_y_score(y_true: np.ndarray, y_score: np.ndarray):
+    binary = True
+    if not (isinstance(y_true, (list, tuple, np.ndarray)) and isinstance(y_score, (list, tuple, np.ndarray))):
+        raise TypeError("y_true and y_score must be lists, tuples or numpy arrays.")
+    else:
+        y_true, y_score = np.squeeze(np.asarray(y_true)), np.squeeze(np.asarray(y_score))
+        if y_true.ndim == y_score.ndim:
+            if len(np.unique(y_true)) != 2:
+                raise TypeError("y_true should have two classes only or y_score must have shape (n_examples, n_labels)")
+            else:
+                if np.issubdtype(y_true.dtype, np.number):
+                    return y_true, y_score, binary, "number"
+                else:
+                    return y_true, y_score, binary, "string"
+        else:
+            if len(np.unique(y_true)) <= 2:
+                raise TypeError("y_score must have shape (n_examples, n_labels) in case of multi-classification problem")
+            else:
+                if np.issubdtype(y_true.dtype, np.number):
+                    return y_true, y_score, not binary, "number"
+                else:
+                    return y_true, y_score, not binary, "string"
+
+
+def is_consecutive_and_start_zero(vector):
+    if sorted(vector) == list(range(min(vector), max(vector) + 1)):
+        if 0 in vector:
+            return True
+    return False
+
+
+def format_external_clustering_data(y_true: np.ndarray, y_pred: np.ndarray):
+    """
+    Need both of y_true and y_pred to format
+    """
+    if not (isinstance(y_true, (list, tuple, np.ndarray)) and isinstance(y_pred, (list, tuple, np.ndarray))):
+        raise TypeError("To calculate external clustering metrics, y_true and y_pred must be lists, tuples or numpy arrays.")
+    else:
+        ## Remove all dimensions of size 1
+        y_true, y_pred = np.squeeze(np.asarray(y_true)), np.squeeze(np.asarray(y_pred))
+        if not (y_true.ndim == y_pred.ndim):
+            raise TypeError("To calculate external clustering metrics, y_true and y_pred must have the same number of dimensions.")
+        else:
+            if y_true.ndim == 1:
+                if np.issubdtype(y_true.dtype, np.number):
+                    if is_consecutive_and_start_zero(y_true):
+                        return y_true, y_pred, None
+                le = LabelEncoder()
+                y_true = le.fit_transform(y_true)
+                y_pred = le.transform(y_pred)
+                return y_true, y_pred, le
+            else:
+                raise TypeError("To calculate clustering metrics, y_true and y_pred must be a 1-D vector.")
+
+
+def format_internal_clustering_data(labels: np.ndarray):
+    if not (isinstance(labels, (list, tuple, np.ndarray))):
+        raise TypeError("To calculate internal clustering metrics, labels must be lists, tuples or numpy arrays.")
+    else:
+        ## Remove all dimensions of size 1
+        labels = np.squeeze(np.asarray(labels))
+        if labels.ndim == 1:
+            if np.issubdtype(labels.dtype, np.number):
+                labels = np.round(labels).astype(int)
+                if is_consecutive_and_start_zero(labels):
+                    return labels, None
+            le = LabelEncoder()
+            labels = le.fit_transform(labels)
+            return labels, le
+        else:
+            raise TypeError("To calculate clustering metrics, labels must be a 1-D vector.")
```

### Comparing `permetrics-1.4.0/permetrics/utils/encoder.py` & `permetrics-1.4.1/permetrics/utils/encoder.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-#!/usr/bin/env python
-# Created by "Thieu" at 06:18, 26/07/2023 ----------%                                                                               
-#       Email: nguyenthieu2102@gmail.com            %                                                    
-#       Github: https://github.com/thieu1995        %                         
-# --------------------------------------------------%
-
-import numpy as np
-
-
-class LabelEncoder:
-    def __init__(self):
-        self.classes_ = None
-        self.encoded_classes_ = None
-
-    def fit(self, y):
-        self.classes_, indices = np.unique(y, return_inverse=True)
-        self.encoded_classes_ = np.arange(len(self.classes_))
-        return self
-
-    def transform(self, y):
-        return np.searchsorted(self.classes_, y)
-
-    def inverse_transform(self, y):
-        return self.classes_[y]
-
-    def fit_transform(self, y):
-        self.fit(y)
-        return self.transform(y)
+#!/usr/bin/env python
+# Created by "Thieu" at 06:18, 26/07/2023 ----------%                                                                               
+#       Email: nguyenthieu2102@gmail.com            %                                                    
+#       Github: https://github.com/thieu1995        %                         
+# --------------------------------------------------%
+
+import numpy as np
+
+
+class LabelEncoder:
+    def __init__(self):
+        self.classes_ = None
+        self.encoded_classes_ = None
+
+    def fit(self, y):
+        self.classes_, indices = np.unique(y, return_inverse=True)
+        self.encoded_classes_ = np.arange(len(self.classes_))
+        return self
+
+    def transform(self, y):
+        return np.searchsorted(self.classes_, y)
+
+    def inverse_transform(self, y):
+        return self.classes_[y]
+
+    def fit_transform(self, y):
+        self.fit(y)
+        return self.transform(y)
```

