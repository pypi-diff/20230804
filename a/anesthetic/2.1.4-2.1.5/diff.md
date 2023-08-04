# Comparing `tmp/anesthetic-2.1.4.tar.gz` & `tmp/anesthetic-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anesthetic-2.1.4.tar", last modified: Tue Aug  1 18:05:53 2023, max compression
+gzip compressed data, was "anesthetic-2.1.5.tar", last modified: Fri Aug  4 11:52:51 2023, max compression
```

## Comparing `anesthetic-2.1.4.tar` & `anesthetic-2.1.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:05:53.853000 anesthetic-2.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-01 18:05:42.000000 anesthetic-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-08-01 18:05:53.853000 anesthetic-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-01 18:05:42.000000 anesthetic-2.1.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:05:53.845000 anesthetic-2.1.4/anesthetic/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/_code_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/_format.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:05:53.845000 anesthetic-2.1.4/anesthetic/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/examples/_matplotlib_agg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/examples/perfect_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:05:53.849000 anesthetic-2.1.4/anesthetic/gui/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/gui/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/gui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/kde.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    54734 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:05:53.849000 anesthetic-2.1.4/anesthetic/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/plotting/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:05:53.849000 anesthetic-2.1.4/anesthetic/plotting/_matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/plotting/_matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/plotting/_matplotlib/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/plotting/_matplotlib/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/plotting/_matplotlib/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/plotting/_matplotlib/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:05:53.853000 anesthetic-2.1.4/anesthetic/read/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/read/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/read/cobaya.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/read/getdist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/read/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/read/multinest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/read/polychord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/read/ultranest.py
--rw-r--r--   0 runner    (1001) docker     (123)    50784 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-08-01 18:05:42.000000 anesthetic-2.1.4/anesthetic/weighted_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:05:53.845000 anesthetic-2.1.4/anesthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-08-01 18:05:53.000000 anesthetic-2.1.4/anesthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-01 18:05:53.000000 anesthetic-2.1.4/anesthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:05:53.000000 anesthetic-2.1.4/anesthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 18:05:53.000000 anesthetic-2.1.4/anesthetic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-01 18:05:53.000000 anesthetic-2.1.4/anesthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 18:05:53.000000 anesthetic-2.1.4/anesthetic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-01 18:05:42.000000 anesthetic-2.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-01 18:05:53.853000 anesthetic-2.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:05:53.853000 anesthetic-2.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-08-01 18:05:42.000000 anesthetic-2.1.4/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-01 18:05:42.000000 anesthetic-2.1.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-08-01 18:05:42.000000 anesthetic-2.1.4/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-08-01 18:05:42.000000 anesthetic-2.1.4/tests/test_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    28539 2023-08-01 18:05:42.000000 anesthetic-2.1.4/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-08-01 18:05:42.000000 anesthetic-2.1.4/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    65301 2023-08-01 18:05:42.000000 anesthetic-2.1.4/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-01 18:05:42.000000 anesthetic-2.1.4/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-01 18:05:42.000000 anesthetic-2.1.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34365 2023-08-01 18:05:42.000000 anesthetic-2.1.4/tests/test_weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:52:51.356742 anesthetic-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-04 11:52:42.000000 anesthetic-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-08-04 11:52:51.356742 anesthetic-2.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-04 11:52:42.000000 anesthetic-2.1.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:52:51.352742 anesthetic-2.1.5/anesthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/_code_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:52:51.352742 anesthetic-2.1.5/anesthetic/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/examples/_matplotlib_agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/examples/perfect_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:52:51.352742 anesthetic-2.1.5/anesthetic/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/gui/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/gui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54718 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:52:51.352742 anesthetic-2.1.5/anesthetic/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/plotting/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:52:51.352742 anesthetic-2.1.5/anesthetic/plotting/_matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/plotting/_matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/plotting/_matplotlib/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/plotting/_matplotlib/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/plotting/_matplotlib/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/plotting/_matplotlib/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:52:51.356742 anesthetic-2.1.5/anesthetic/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/read/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/read/cobaya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/read/getdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/read/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/read/multinest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/read/polychord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/read/ultranest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50784 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-08-04 11:52:42.000000 anesthetic-2.1.5/anesthetic/weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:52:51.352742 anesthetic-2.1.5/anesthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-08-04 11:52:51.000000 anesthetic-2.1.5/anesthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-04 11:52:51.000000 anesthetic-2.1.5/anesthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:52:51.000000 anesthetic-2.1.5/anesthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 11:52:51.000000 anesthetic-2.1.5/anesthetic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-04 11:52:51.000000 anesthetic-2.1.5/anesthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 11:52:51.000000 anesthetic-2.1.5/anesthetic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-04 11:52:42.000000 anesthetic-2.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-04 11:52:51.356742 anesthetic-2.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:52:51.356742 anesthetic-2.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-04 11:52:42.000000 anesthetic-2.1.5/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-08-04 11:52:42.000000 anesthetic-2.1.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-08-04 11:52:42.000000 anesthetic-2.1.5/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-08-04 11:52:42.000000 anesthetic-2.1.5/tests/test_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27503 2023-08-04 11:52:42.000000 anesthetic-2.1.5/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2023-08-04 11:52:42.000000 anesthetic-2.1.5/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64834 2023-08-04 11:52:42.000000 anesthetic-2.1.5/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-08-04 11:52:42.000000 anesthetic-2.1.5/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-08-04 11:52:42.000000 anesthetic-2.1.5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34365 2023-08-04 11:52:42.000000 anesthetic-2.1.5/tests/test_weighted_pandas.py
```

### Comparing `anesthetic-2.1.4/LICENSE` & `anesthetic-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/PKG-INFO` & `anesthetic-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.1.4
+Version: 2.1.5
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -55,15 +55,15 @@
 Provides-Extra: all
 License-File: LICENSE
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.1.4
+:Version: 2.1.5
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.1.4/README.rst` & `anesthetic-2.1.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.1.4
+:Version: 2.1.5
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.1.4/anesthetic/__init__.py` & `anesthetic-2.1.5/anesthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/_code_utils.py` & `anesthetic-2.1.5/anesthetic/_code_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/_format.py` & `anesthetic-2.1.5/anesthetic/_format.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/boundary.py` & `anesthetic-2.1.5/anesthetic/boundary.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/examples/perfect_ns.py` & `anesthetic-2.1.5/anesthetic/examples/perfect_ns.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/examples/utils.py` & `anesthetic-2.1.5/anesthetic/examples/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/gui/plot.py` & `anesthetic-2.1.5/anesthetic/gui/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/gui/widgets.py` & `anesthetic-2.1.5/anesthetic/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/kde.py` & `anesthetic-2.1.5/anesthetic/kde.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/labelled_pandas.py` & `anesthetic-2.1.5/anesthetic/labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/plot.py` & `anesthetic-2.1.5/anesthetic/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,14 @@
 import numpy as np
 from pandas import Series, DataFrame
 import matplotlib.pyplot as plt
 from scipy.stats import gaussian_kde
 from scipy.special import erf
 from matplotlib.gridspec import GridSpec, GridSpecFromSubplotSpec
 from matplotlib.axes import Axes
-try:
-    from astropy.visualization import hist
-except ImportError:
-    pass
-try:
-    from anesthetic.kde import fastkde_1d, fastkde_2d
-except ImportError:
-    pass
 import matplotlib.cbook as cbook
 import matplotlib.lines as mlines
 from matplotlib.ticker import MaxNLocator, AutoMinorLocator
 from matplotlib.colors import LinearSegmentedColormap
 from matplotlib.transforms import Affine2D
 from anesthetic.utils import nest_level
 from anesthetic.utils import (sample_compression_1d, quantile,
@@ -764,16 +756,17 @@
     else:
         edgecolor = color
 
     q = kwargs.pop('q', 5)
     q = quantile_plot_interval(q=q)
 
     try:
+        from anesthetic.kde import fastkde_1d
         x, p, xmin, xmax = fastkde_1d(data, xmin, xmax)
-    except NameError:
+    except ImportError:
         raise ImportError("You need to install fastkde to use fastkde")
     p /= p.max()
     i = ((x > quantile(x, q[0], p)) & (x < quantile(x, q[-1], p)))
 
     area = np.trapz(x=x[i], y=p[i]) if density else 1
     ans = ax.plot(x[i], p[i]/area, color=color, *args, **kwargs)
 
@@ -967,18 +960,19 @@
     q = quantile_plot_interval(q=q)
     xmin = quantile(data, q[0], weights)
     xmax = quantile(data, q[-1], weights)
     range = kwargs.pop('range', (xmin, xmax))
 
     if isinstance(bins, str) and bins in ['knuth', 'freedman', 'blocks']:
         try:
+            from astropy.visualization import hist
             h, edges, bars = hist(data, ax=ax, bins=bins,
                                   range=range, histtype=histtype,
                                   color=color, *args, **kwargs)
-        except NameError:
+        except ImportError:
             raise ImportError("You need to install astropy to use astropyhist")
     else:
         h, edges, bars = ax.hist(data, weights=weights, bins=bins,
                                  range=range, histtype=histtype,
                                  color=color, *args, **kwargs)
 
     if histtype == 'bar' and not density:
@@ -1044,18 +1038,19 @@
     cmap = kwargs.pop('cmap', None)
     facecolor, edgecolor, cmap = set_colors(c=color, fc=facecolor,
                                             ec=edgecolor, cmap=cmap)
 
     kwargs.pop('q', None)
 
     try:
+        from anesthetic.kde import fastkde_2d
         x, y, pdf, xmin, xmax, ymin, ymax = fastkde_2d(data_x, data_y,
                                                        xmin=xmin, xmax=xmax,
                                                        ymin=ymin, ymax=ymax)
-    except NameError:
+    except ImportError:
         raise ImportError("You need to install fastkde to use fastkde")
 
     levels = iso_probability_contours(pdf, contours=levels)
 
     i = (pdf >= levels[0]*0.5).any(axis=0)
     j = (pdf >= levels[0]*0.5).any(axis=1)
```

### Comparing `anesthetic-2.1.4/anesthetic/plotting/_core.py` & `anesthetic-2.1.5/anesthetic/plotting/_core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/plotting/_matplotlib/__init__.py` & `anesthetic-2.1.5/anesthetic/plotting/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/plotting/_matplotlib/boxplot.py` & `anesthetic-2.1.5/anesthetic/plotting/_matplotlib/boxplot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/plotting/_matplotlib/core.py` & `anesthetic-2.1.5/anesthetic/plotting/_matplotlib/core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/plotting/_matplotlib/hist.py` & `anesthetic-2.1.5/anesthetic/plotting/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/read/chain.py` & `anesthetic-2.1.5/anesthetic/read/chain.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/read/cobaya.py` & `anesthetic-2.1.5/anesthetic/read/cobaya.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/read/getdist.py` & `anesthetic-2.1.5/anesthetic/read/getdist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/read/hdf.py` & `anesthetic-2.1.5/anesthetic/read/hdf.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/read/multinest.py` & `anesthetic-2.1.5/anesthetic/read/multinest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/read/polychord.py` & `anesthetic-2.1.5/anesthetic/read/polychord.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/read/ultranest.py` & `anesthetic-2.1.5/anesthetic/read/ultranest.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 """Read NestedSamples from UltraNest results."""
 import os
 import json
 from anesthetic.samples import NestedSamples
-try:
-    import h5py
-except ImportError:
-    pass
 
 
 def read_ultranest(root, *args, **kwargs):
     """Read UltraNest files.
 
     Parameters
     ----------
@@ -19,14 +15,18 @@
 
     """
     with open(os.path.join(root, 'info', 'results.json')) as infofile:
         labels = json.load(infofile)['paramnames']
     num_params = len(labels)
 
     filepath = os.path.join(root, 'results', 'points.hdf5')
+    try:
+        import h5py
+    except ImportError:
+        raise ImportError('h5py is required to read UltraNest results')
     with h5py.File(filepath, 'r') as fileobj:
         points = fileobj['points']
         _, ncols = points.shape
         x_dim = ncols - 3 - num_params
         logL_birth = points[:, 0]
         logL = points[:, 1]
         samples = points[:, 3+x_dim:3+x_dim+num_params]
```

### Comparing `anesthetic-2.1.4/anesthetic/samples.py` & `anesthetic-2.1.5/anesthetic/samples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/scripts.py` & `anesthetic-2.1.5/anesthetic/scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/utils.py` & `anesthetic-2.1.5/anesthetic/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic/weighted_pandas.py` & `anesthetic-2.1.5/anesthetic/weighted_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/anesthetic.egg-info/PKG-INFO` & `anesthetic-2.1.5/anesthetic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.1.4
+Version: 2.1.5
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -55,15 +55,15 @@
 Provides-Extra: all
 License-File: LICENSE
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.1.4
+:Version: 2.1.5
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.1.4/anesthetic.egg-info/SOURCES.txt` & `anesthetic-2.1.5/anesthetic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/pyproject.toml` & `anesthetic-2.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/tests/test_examples.py` & `anesthetic-2.1.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/tests/test_gui.py` & `anesthetic-2.1.5/tests/test_gui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-import sys
 import anesthetic.examples._matplotlib_agg  # noqa: F401
 from anesthetic import read_chains
 import pytest
 import pandas._testing as tm
-try:
-    import h5py  # noqa: F401
-except ImportError:
-    pass
+from utils import skipif_no_h5py
 
 
 @pytest.fixture(autouse=True)
 def close_figures_on_teardown():
     tm.close()
 
 
 @pytest.mark.parametrize('root', ["./tests/example_data/pc",
                                   "./tests/example_data/mn",
-                                  "./tests/example_data/un"])
+                                  skipif_no_h5py("./tests/example_data/un")])
 def test_gui(root):
-    if 'un' in root and 'h5py' not in sys.modules:
-        pytest.skip("`h5py` not in sys.modules, but needed for ultranest.")
     samples = read_chains(root)
     plotter = samples.gui()
 
     # Type buttons
     plotter.type.buttons.set_active(1)
     assert plotter.type() == 'posterior'
     plotter.type.buttons.set_active(0)
@@ -61,29 +55,25 @@
 
     # Reset button
     plotter.reset.button.on_clicked(plotter.reset_range(None))
 
 
 @pytest.mark.parametrize('root', ["./tests/example_data/pc",
                                   "./tests/example_data/mn",
-                                  "./tests/example_data/un"])
+                                  skipif_no_h5py("./tests/example_data/un")])
 def test_gui_params(root):
-    if 'un' in root and 'h5py' not in sys.modules:
-        pytest.skip("`h5py` not in sys.modules, but needed for ultranest.")
     samples = read_chains(root)
     params = samples.columns.get_level_values(0).to_list()
     plotter = samples.gui()
     assert len(plotter.param_choice.buttons.labels) == len(params)
 
     plotter = samples.gui(params=params[:2])
     assert len(plotter.param_choice.buttons.labels) == 2
 
 
 @pytest.mark.parametrize('root', ["./tests/example_data/pc",
                                   "./tests/example_data/mn",
-                                  "./tests/example_data/un"])
+                                  skipif_no_h5py("./tests/example_data/un")])
 def test_slider_reset_range(root):
-    if 'un' in root and 'h5py' not in sys.modules:
-        pytest.skip("`h5py` not in sys.modules, but needed for ultranest.")
     plotter = read_chains(root).gui()
     plotter.evolution.reset_range(-3, 3)
     assert plotter.evolution.ax.get_xlim() == (-3.0, 3.0)
```

### Comparing `anesthetic-2.1.4/tests/test_labelled_pandas.py` & `anesthetic-2.1.5/tests/test_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/tests/test_plot.py` & `anesthetic-2.1.5/tests/test_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import anesthetic.examples._matplotlib_agg  # noqa: F401
 import pytest
 import numpy as np
-import sys
 import matplotlib.pyplot as plt
 import matplotlib.gridspec as gs
 from anesthetic.plot import (make_1d_axes, make_2d_axes, kde_plot_1d,
                              fastkde_plot_1d, hist_plot_1d, hist_plot_2d,
                              fastkde_contour_plot_2d, kde_contour_plot_2d,
                              scatter_plot_2d, quantile_plot_interval,
                              basic_cmap, AxesSeries, AxesDataFrame)
@@ -16,14 +15,15 @@
 from matplotlib.contour import ContourSet
 from matplotlib.lines import Line2D
 from matplotlib.patches import Patch, Polygon
 from matplotlib.colors import ColorConverter, to_rgba
 from matplotlib.figure import Figure
 from scipy.special import erf
 from scipy.interpolate import interp1d
+from utils import skipif_no_fastkde, astropy_mark_xfail, fastkde_mark_xfail
 
 
 @pytest.fixture(autouse=True)
 def close_figures_on_teardown():
     tm.close()
 
 
@@ -333,118 +333,110 @@
 @pytest.mark.parametrize('upper', [True, False])
 def test_2d_axes_scatter(axesparams, params, upper):
     kwargs = dict(c='k', marker='*')
     fig, axes = make_2d_axes(axesparams, upper=upper)
     axes.scatter(params, **kwargs)
 
 
-@pytest.mark.parametrize('plot_1d', [kde_plot_1d, fastkde_plot_1d])
+@pytest.mark.parametrize('plot_1d', [kde_plot_1d,
+                                     skipif_no_fastkde(fastkde_plot_1d)])
 def test_kde_plot_1d(plot_1d):
     fig, ax = plt.subplots()
     np.random.seed(0)
     data = np.random.randn(1000)
 
-    try:
-        # Check height
-        line, = plot_1d(ax, data)
-        assert isinstance(line, Line2D)
-        assert line.get_ydata().max() <= 1
-
-        # Check arguments are passed onward to underlying function
-        line, = plot_1d(ax, data, color='r')
-        assert line.get_color() == 'r'
-        line, = plot_1d(ax, data, cmap=plt.cm.Blues)
-        assert line.get_color() == plt.cm.Blues(0.68)
-
-        # Check q
-        plot_1d(ax, data, q='1sigma')
-        plot_1d(ax, data, q=0)
-        plot_1d(ax, data, q=1)
-        plot_1d(ax, data, q=5)
-        plot_1d(ax, data, q=10)
-        plot_1d(ax, data, q=0.1)
-        plot_1d(ax, data, q=0.9)
-        plot_1d(ax, data, q=(0.1, 0.9))
-
-        # Check iso-probability code
-        line, fill = plot_1d(ax, data, facecolor=True)
-        plot_1d(ax, data, facecolor=True, levels=[0.8, 0.6, 0.2])
-        line, fill = plot_1d(ax, data, fc='blue', color='k', ec='r')
-        assert np.all(fill[0].get_edgecolor()[0] == to_rgba('r'))
-        assert (to_rgba(line[0].get_color()) == to_rgba('r'))
-        line, fill = plot_1d(ax, data, fc=True, color='k', ec=None)
-        assert len(fill[0].get_edgecolor()) == 0
-        assert (to_rgba(line[0].get_color()) == to_rgba('k'))
-
-        # Check levels
-        with pytest.raises(ValueError):
-            fig, ax = plt.subplots()
-            plot_1d(ax, data, fc=True, levels=[0.68, 0.95])
+    # Check height
+    line, = plot_1d(ax, data)
+    assert isinstance(line, Line2D)
+    assert line.get_ydata().max() <= 1
 
-        # Check xlim, Gaussian (i.e. limits reduced to relevant data range)
-        fig, ax = plt.subplots()
-        data = np.random.randn(1000) * 0.01 + 0.5
-        plot_1d(ax, data)
-        xmin, xmax = ax.get_xlim()
-        assert xmin > 0.4
-        assert xmax < 0.6
-        # Check xlim, Uniform (i.e. data and limits span entire prior boundary)
+    # Check arguments are passed onward to underlying function
+    line, = plot_1d(ax, data, color='r')
+    assert line.get_color() == 'r'
+    line, = plot_1d(ax, data, cmap=plt.cm.Blues)
+    assert line.get_color() == plt.cm.Blues(0.68)
+
+    # Check q
+    plot_1d(ax, data, q='1sigma')
+    plot_1d(ax, data, q=0)
+    plot_1d(ax, data, q=1)
+    plot_1d(ax, data, q=5)
+    plot_1d(ax, data, q=10)
+    plot_1d(ax, data, q=0.1)
+    plot_1d(ax, data, q=0.9)
+    plot_1d(ax, data, q=(0.1, 0.9))
+
+    # Check iso-probability code
+    line, fill = plot_1d(ax, data, facecolor=True)
+    plot_1d(ax, data, facecolor=True, levels=[0.8, 0.6, 0.2])
+    line, fill = plot_1d(ax, data, fc='blue', color='k', ec='r')
+    assert np.all(fill[0].get_edgecolor()[0] == to_rgba('r'))
+    assert (to_rgba(line[0].get_color()) == to_rgba('r'))
+    line, fill = plot_1d(ax, data, fc=True, color='k', ec=None)
+    assert len(fill[0].get_edgecolor()) == 0
+    assert (to_rgba(line[0].get_color()) == to_rgba('k'))
+
+    # Check levels
+    with pytest.raises(ValueError):
         fig, ax = plt.subplots()
-        data = np.random.uniform(size=1000)
-        plot_1d(ax, data, q=0)
-        xmin, xmax = ax.get_xlim()
-        assert xmin <= 0
-        assert xmax >= 1
+        plot_1d(ax, data, fc=True, levels=[0.68, 0.95])
 
-    except ImportError:
-        if 'fastkde' not in sys.modules:
-            pass
+    # Check xlim, Gaussian (i.e. limits reduced to relevant data range)
+    fig, ax = plt.subplots()
+    data = np.random.randn(1000) * 0.01 + 0.5
+    plot_1d(ax, data)
+    xmin, xmax = ax.get_xlim()
+    assert xmin > 0.4
+    assert xmax < 0.6
+    # Check xlim, Uniform (i.e. data and limits span entire prior boundary)
+    fig, ax = plt.subplots()
+    data = np.random.uniform(size=1000)
+    plot_1d(ax, data, q=0)
+    xmin, xmax = ax.get_xlim()
+    assert xmin <= 0
+    assert xmax >= 1
 
 
+@fastkde_mark_xfail
 def test_fastkde_min_max():
     np.random.seed(0)
     data_x = np.random.randn(100)
     data_y = np.random.randn(100)
     xmin, xmax = -1, +1
     ymin, ymax = -1, +1
-    try:
-        _, ax = plt.subplots()
-        line, = fastkde_plot_1d(ax, data_x, xmin=xmin)
-        assert (line.get_xdata() >= xmin).all()
-
-        _, ax = plt.subplots()
-        line, = fastkde_plot_1d(ax, data_x, xmax=xmax)
-        assert (line.get_xdata() <= xmax).all()
-
-        _, ax = plt.subplots()
-        line, = fastkde_plot_1d(ax, data_x, xmin=xmin, xmax=xmax)
-        assert (line.get_xdata() >= xmin).all()
-        assert (line.get_xdata() <= xmax).all()
-
-        _, ax = plt.subplots()
-        fastkde_contour_plot_2d(ax, data_x, data_y, xmin=xmin, ymin=ymin)
-        assert ax.get_xlim()[0] >= xmin
-        assert ax.get_ylim()[0] >= ymin
-
-        _, ax = plt.subplots()
-        fastkde_contour_plot_2d(ax, data_x, data_y, xmax=xmax, ymax=ymax)
-        assert ax.get_xlim()[1] <= xmax
-        assert ax.get_ylim()[1] <= ymax
-
-        _, ax = plt.subplots()
-        fastkde_contour_plot_2d(ax, data_x, data_y,
-                                xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax)
-        assert ax.get_xlim()[0] >= xmin
-        assert ax.get_xlim()[1] <= xmax
-        assert ax.get_ylim()[0] >= ymin
-        assert ax.get_ylim()[1] <= ymax
-
-    except ImportError:
-        if 'fastkde' not in sys.modules:
-            pass
+    _, ax = plt.subplots()
+    line, = fastkde_plot_1d(ax, data_x, xmin=xmin)
+    assert (line.get_xdata() >= xmin).all()
+
+    _, ax = plt.subplots()
+    line, = fastkde_plot_1d(ax, data_x, xmax=xmax)
+    assert (line.get_xdata() <= xmax).all()
+
+    _, ax = plt.subplots()
+    line, = fastkde_plot_1d(ax, data_x, xmin=xmin, xmax=xmax)
+    assert (line.get_xdata() >= xmin).all()
+    assert (line.get_xdata() <= xmax).all()
+
+    _, ax = plt.subplots()
+    fastkde_contour_plot_2d(ax, data_x, data_y, xmin=xmin, ymin=ymin)
+    assert ax.get_xlim()[0] >= xmin
+    assert ax.get_ylim()[0] >= ymin
+
+    _, ax = plt.subplots()
+    fastkde_contour_plot_2d(ax, data_x, data_y, xmax=xmax, ymax=ymax)
+    assert ax.get_xlim()[1] <= xmax
+    assert ax.get_ylim()[1] <= ymax
+
+    _, ax = plt.subplots()
+    fastkde_contour_plot_2d(ax, data_x, data_y,
+                            xmin=xmin, xmax=xmax, ymin=ymin, ymax=ymax)
+    assert ax.get_xlim()[0] >= xmin
+    assert ax.get_xlim()[1] <= xmax
+    assert ax.get_ylim()[0] >= ymin
+    assert ax.get_ylim()[1] <= ymax
 
 
 def test_hist_plot_1d():
     fig, ax = plt.subplots()
     np.random.seed(0)
     data = np.random.randn(1000)
 
@@ -481,27 +473,24 @@
     polygon, = hist_plot_1d(ax, data, histtype='step', color='r', alpha=0.5)[2]
     assert polygon.get_ec() == ColorConverter.to_rgba('r', alpha=0.5)
     polygon, = hist_plot_1d(ax, data, histtype='step', cmap=plt.cm.viridis,
                             color='r')[2]
     assert polygon.get_ec() == ColorConverter.to_rgba('r')
 
 
+@astropy_mark_xfail
 @pytest.mark.parametrize('bins', ['knuth', 'freedman', 'blocks'])
 def test_astropyhist_plot_1d(bins):
-    try:
-        fig, ax = plt.subplots()
-        np.random.seed(0)
-        data = np.random.randn(100)
-        bars = hist_plot_1d(ax, data, histtype='bar', bins=bins)[2]
-        assert np.all([isinstance(b, Patch) for b in bars])
-        assert max([b.get_height() for b in bars]) == 1.
-        assert np.all(np.array([b.get_height() for b in bars]) <= 1.)
-    except ImportError:
-        if 'astropy' not in sys.modules:
-            pass
+    fig, ax = plt.subplots()
+    np.random.seed(0)
+    data = np.random.randn(100)
+    bars = hist_plot_1d(ax, data, histtype='bar', bins=bins)[2]
+    assert np.all([isinstance(b, Patch) for b in bars])
+    assert max([b.get_height() for b in bars]) == 1.
+    assert np.all(np.array([b.get_height() for b in bars]) <= 1.)
 
 
 def test_hist_plot_2d():
     fig, ax = plt.subplots()
     np.random.seed(0)
     data_x, data_y = np.random.randn(2, 1000)
     hist_plot_2d(ax, data_x, data_y)
@@ -524,135 +513,127 @@
 
     fig, ax = plt.subplots()
     data_x, data_y = np.random.randn(2, 1000)
     hist_plot_2d(ax, data_x, data_y, levels=[0.95, 0.68], cmin=50)
     hist_plot_2d(ax, data_x, data_y, levels=[0.95, 0.68], cmax=50)
 
 
-@pytest.mark.parametrize('plot_1d', [kde_plot_1d, fastkde_plot_1d])
+@pytest.mark.parametrize('plot_1d', [kde_plot_1d,
+                                     skipif_no_fastkde(fastkde_plot_1d)])
 @pytest.mark.parametrize('s', [1, 2])
 def test_1d_density_kwarg(plot_1d, s):
-    try:
-        np.random.seed(0)
-        x = np.random.normal(scale=s, size=2000)
-        fig, ax = plt.subplots()
-
-        # hist density = False:
-        h = hist_plot_1d(ax, x, density=False,
-                         bins=np.linspace(-5.5, 5.5, 12))[2]
-        bar_height = h.get_children()[len(h.get_children()) // 2].get_height()
-        assert bar_height == pytest.approx(1, rel=0.1)
-
-        # kde density = False:
-        k = plot_1d(ax, x, density=False)[0]
-        f = interp1d(k.get_xdata(), k.get_ydata(), 'cubic', assume_sorted=True)
-        kde_height = f(0)
-        assert kde_height == pytest.approx(1, rel=0.1)
-
-        # hist density = True:
-        h = hist_plot_1d(ax, x, density=True,
-                         bins=np.linspace(-5.5, 5.5, 12))[2]
-        bar_height = h.get_children()[len(h.get_children()) // 2].get_height()
-        assert bar_height == pytest.approx(erf(0.5 / np.sqrt(2) / s), rel=0.1)
-
-        # kde density = True:
-        k = plot_1d(ax, x, density=True)[0]
-        f = interp1d(k.get_xdata(), k.get_ydata(), 'cubic', assume_sorted=True)
-        kde_height = f(0)
-        gauss_norm = 1 / np.sqrt(2 * np.pi * s**2)
-        assert kde_height == pytest.approx(gauss_norm, rel=0.1)
-
-    except ImportError:
-        if 'fastkde' not in sys.modules:
-            pass
-
+    np.random.seed(0)
+    x = np.random.normal(scale=s, size=2000)
+    fig, ax = plt.subplots()
 
-@pytest.mark.parametrize('contour_plot_2d', [kde_contour_plot_2d,
-                                             fastkde_contour_plot_2d])
+    # hist density = False:
+    h = hist_plot_1d(ax, x, density=False,
+                     bins=np.linspace(-5.5, 5.5, 12))[2]
+    bar_height = h.get_children()[len(h.get_children()) // 2].get_height()
+    assert bar_height == pytest.approx(1, rel=0.1)
+
+    # kde density = False:
+    k = plot_1d(ax, x, density=False)[0]
+    f = interp1d(k.get_xdata(), k.get_ydata(), 'cubic', assume_sorted=True)
+    kde_height = f(0)
+    assert kde_height == pytest.approx(1, rel=0.1)
+
+    # hist density = True:
+    h = hist_plot_1d(ax, x, density=True,
+                     bins=np.linspace(-5.5, 5.5, 12))[2]
+    bar_height = h.get_children()[len(h.get_children()) // 2].get_height()
+    assert bar_height == pytest.approx(erf(0.5 / np.sqrt(2) / s), rel=0.1)
+
+    # kde density = True:
+    k = plot_1d(ax, x, density=True)[0]
+    f = interp1d(k.get_xdata(), k.get_ydata(), 'cubic', assume_sorted=True)
+    kde_height = f(0)
+    gauss_norm = 1 / np.sqrt(2 * np.pi * s**2)
+    assert kde_height == pytest.approx(gauss_norm, rel=0.1)
+
+
+@pytest.mark.parametrize('contour_plot_2d',
+                         [kde_contour_plot_2d,
+                          skipif_no_fastkde(fastkde_contour_plot_2d)])
 def test_contour_plot_2d(contour_plot_2d):
-    try:
-        fig, ax = plt.subplots()
-        np.random.seed(1)
-        data_x = np.random.randn(1000)
-        data_y = np.random.randn(1000)
-        cf, ct = contour_plot_2d(ax, data_x, data_y)
-        assert isinstance(cf, ContourSet)
-        assert isinstance(ct, ContourSet)
-
-        # Check levels
-        with pytest.raises(ValueError):
-            fig, ax = plt.subplots()
-            contour_plot_2d(ax, data_x, data_y, levels=[0.68, 0.95])
+    fig, ax = plt.subplots()
+    np.random.seed(1)
+    data_x = np.random.randn(1000)
+    data_y = np.random.randn(1000)
+    cf, ct = contour_plot_2d(ax, data_x, data_y)
+    assert isinstance(cf, ContourSet)
+    assert isinstance(ct, ContourSet)
 
-        # Check q
+    # Check levels
+    with pytest.raises(ValueError):
         fig, ax = plt.subplots()
-        contour_plot_2d(ax, data_x, data_y, q=0)
+        contour_plot_2d(ax, data_x, data_y, levels=[0.68, 0.95])
 
-        # Check unfilled
-        cmap = basic_cmap('C2')
-        fig, ax = plt.subplots()
-        cf1, ct1 = contour_plot_2d(ax, data_x, data_y, facecolor='C2')
-        cf2, ct2 = contour_plot_2d(ax, data_x, data_y, fc='None', cmap=cmap)
-        # filled `contourf` and unfilled `contour` colors are the same:
-        assert cf1.tcolors[0] == ct2.tcolors[0]
-        assert cf1.tcolors[1] == ct2.tcolors[1]
-        cf, ct = contour_plot_2d(ax, data_x, data_y, edgecolor='C0')
-        assert ct.colors == 'C0'
-        cf, ct = contour_plot_2d(ax, data_x, data_y, ec='C0', cmap=plt.cm.Reds)
-        assert cf.get_cmap() == plt.cm.Reds
-        assert ct.colors == 'C0'
-        fig, ax = plt.subplots()
-        cf, ct = contour_plot_2d(ax, data_x, data_y, fc=None)
-        assert cf is None
-        assert ct.colors is None
-        assert ct.get_cmap()(1.) == to_rgba('C0')
-        cf, ct = contour_plot_2d(ax, data_x, data_y, fc=None, c='C3')
-        assert cf is None
-        assert ct.colors is None
-        assert ct.get_cmap()(1.) == to_rgba('C3')
-        cf, ct = contour_plot_2d(ax, data_x, data_y, fc=None, ec='C1')
-        assert cf is None
-        assert ct.colors == 'C1'
-        cf, ct = contour_plot_2d(ax, data_x, data_y, fc=None, cmap=plt.cm.Reds)
-        assert cf is None
-        assert ct.colors is None
-        assert ct.get_cmap() == plt.cm.Reds
+    # Check q
+    fig, ax = plt.subplots()
+    contour_plot_2d(ax, data_x, data_y, q=0)
 
-        # Check limits, Gaussian (i.e. limits reduced to relevant data range)
-        fig, ax = plt.subplots()
-        data_x = np.random.randn(1000) * 0.01 + 0.5
-        data_y = np.random.randn(1000) * 0.01 + 0.5
-        contour_plot_2d(ax, data_x, data_y)
-        xmin, xmax = ax.get_xlim()
-        ymin, ymax = ax.get_ylim()
-        assert xmin > 0.4
-        assert xmax < 0.6
-        assert ymin > 0.4
-        assert ymax < 0.6
-        # Check limits, Uniform (i.e. data & limits span entire prior boundary)
-        fig, ax = plt.subplots()
-        data_x = np.random.uniform(size=1000)
-        data_y = np.random.uniform(size=1000)
-        contour_plot_2d(ax, data_x, data_y, q=0)
-        xmin, xmax = ax.get_xlim()
-        ymin, ymax = ax.get_ylim()
-        if contour_plot_2d is fastkde_contour_plot_2d:
-            assert xmin <= 0
-            assert xmax >= 1
-            assert ymin <= 0
-            assert ymax >= 1
-        elif contour_plot_2d is kde_contour_plot_2d:
-            assert xmin == pytest.approx(0, abs=0.01)
-            assert xmax == pytest.approx(1, abs=0.01)
-            assert ymin == pytest.approx(0, abs=0.01)
-            assert ymax == pytest.approx(1, abs=0.01)
-
-    except ImportError:
-        if 'fastkde' not in sys.modules:
-            pass
+    # Check unfilled
+    cmap = basic_cmap('C2')
+    fig, ax = plt.subplots()
+    cf1, ct1 = contour_plot_2d(ax, data_x, data_y, facecolor='C2')
+    cf2, ct2 = contour_plot_2d(ax, data_x, data_y, fc='None', cmap=cmap)
+    # filled `contourf` and unfilled `contour` colors are the same:
+    assert cf1.tcolors[0] == ct2.tcolors[0]
+    assert cf1.tcolors[1] == ct2.tcolors[1]
+    cf, ct = contour_plot_2d(ax, data_x, data_y, edgecolor='C0')
+    assert ct.colors == 'C0'
+    cf, ct = contour_plot_2d(ax, data_x, data_y, ec='C0', cmap=plt.cm.Reds)
+    assert cf.get_cmap() == plt.cm.Reds
+    assert ct.colors == 'C0'
+    fig, ax = plt.subplots()
+    cf, ct = contour_plot_2d(ax, data_x, data_y, fc=None)
+    assert cf is None
+    assert ct.colors is None
+    assert ct.get_cmap()(1.) == to_rgba('C0')
+    cf, ct = contour_plot_2d(ax, data_x, data_y, fc=None, c='C3')
+    assert cf is None
+    assert ct.colors is None
+    assert ct.get_cmap()(1.) == to_rgba('C3')
+    cf, ct = contour_plot_2d(ax, data_x, data_y, fc=None, ec='C1')
+    assert cf is None
+    assert ct.colors == 'C1'
+    cf, ct = contour_plot_2d(ax, data_x, data_y, fc=None, cmap=plt.cm.Reds)
+    assert cf is None
+    assert ct.colors is None
+    assert ct.get_cmap() == plt.cm.Reds
+
+    # Check limits, Gaussian (i.e. limits reduced to relevant data range)
+    fig, ax = plt.subplots()
+    data_x = np.random.randn(1000) * 0.01 + 0.5
+    data_y = np.random.randn(1000) * 0.01 + 0.5
+    contour_plot_2d(ax, data_x, data_y)
+    xmin, xmax = ax.get_xlim()
+    ymin, ymax = ax.get_ylim()
+    assert xmin > 0.4
+    assert xmax < 0.6
+    assert ymin > 0.4
+    assert ymax < 0.6
+    # Check limits, Uniform (i.e. data & limits span entire prior boundary)
+    fig, ax = plt.subplots()
+    data_x = np.random.uniform(size=1000)
+    data_y = np.random.uniform(size=1000)
+    contour_plot_2d(ax, data_x, data_y, q=0)
+    xmin, xmax = ax.get_xlim()
+    ymin, ymax = ax.get_ylim()
+    if contour_plot_2d is fastkde_contour_plot_2d:
+        assert xmin <= 0
+        assert xmax >= 1
+        assert ymin <= 0
+        assert ymax >= 1
+    elif contour_plot_2d is kde_contour_plot_2d:
+        assert xmin == pytest.approx(0, abs=0.01)
+        assert xmax == pytest.approx(1, abs=0.01)
+        assert ymin == pytest.approx(0, abs=0.01)
+        assert ymax == pytest.approx(1, abs=0.01)
 
 
 def test_kde_plot_nplot():
     fig, ax = plt.subplots()
     np.random.seed(0)
     data = np.random.randn(1000)
     line, = kde_plot_1d(ax, data, ncompress=1000, nplot_1d=200)
@@ -661,44 +642,40 @@
     fig, ax = plt.subplots()
     np.random.seed(0)
     data_x = np.random.randn(1000)
     data_y = np.random.randn(1000)
     kde_contour_plot_2d(ax, data_x, data_y, ncompress=1000, nplot_2d=900)
 
 
-@pytest.mark.parametrize('contour_plot_2d', [kde_contour_plot_2d,
-                                             fastkde_contour_plot_2d])
+@pytest.mark.parametrize('contour_plot_2d',
+                         [kde_contour_plot_2d,
+                          skipif_no_fastkde(fastkde_contour_plot_2d)])
 @pytest.mark.parametrize('levels', [[0.9],
                                     [0.9, 0.6],
                                     [0.9, 0.6, 0.3],
                                     [0.9, 0.7, 0.5, 0.3]])
 def test_contour_plot_2d_levels(contour_plot_2d, levels):
-    try:
-        np.random.seed(42)
-        x = np.random.randn(1000)
-        y = np.random.randn(1000)
-        cmap = plt.cm.viridis
-
-        fig, (ax1, ax2) = plt.subplots(2)
-        contour_plot_2d(ax1, x, y, levels=levels, cmap=cmap)
-        contour_plot_2d(ax2, x, y, levels=levels, cmap=cmap, fc=None)
-
-        # assert that color between filled and unfilled contours matches
-        # first level
-        color1 = ax1.collections[0].get_facecolor()  # filled face color
-        color2 = ax2.collections[0].get_edgecolor()  # unfilled line color
-        assert_array_equal(color1, color2)
-        # last level
-        color1 = ax1.collections[len(levels)-1].get_facecolor()
-        color2 = ax2.collections[len(levels)-1].get_edgecolor()
-        assert_array_equal(color1, color2)
-
-    except ImportError:
-        if 'fastkde' not in sys.modules:
-            pass
+    np.random.seed(42)
+    x = np.random.randn(1000)
+    y = np.random.randn(1000)
+    cmap = plt.cm.viridis
+
+    fig, (ax1, ax2) = plt.subplots(2)
+    contour_plot_2d(ax1, x, y, levels=levels, cmap=cmap)
+    contour_plot_2d(ax2, x, y, levels=levels, cmap=cmap, fc=None)
+
+    # assert that color between filled and unfilled contours matches
+    # first level
+    color1 = ax1.collections[0].get_facecolor()  # filled face color
+    color2 = ax2.collections[0].get_edgecolor()  # unfilled line color
+    assert_array_equal(color1, color2)
+    # last level
+    color1 = ax1.collections[len(levels)-1].get_facecolor()
+    color2 = ax2.collections[len(levels)-1].get_edgecolor()
+    assert_array_equal(color1, color2)
 
 
 def test_scatter_plot_2d():
     fig, ax = plt.subplots()
     np.random.seed(2)
     data_x = np.random.randn(100)
     data_y = np.random.randn(100)
```

### Comparing `anesthetic-2.1.4/tests/test_reader.py` & `anesthetic-2.1.5/tests/test_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,23 @@
 import anesthetic.examples._matplotlib_agg  # noqa: F401
 import os
-import sys
 import pytest
 import numpy as np
 from numpy.testing import assert_array_equal, assert_array_almost_equal
 from anesthetic.testing import assert_frame_equal
 from anesthetic import MCMCSamples, NestedSamples
 from anesthetic import read_chains
 from anesthetic.read.polychord import read_polychord
 from anesthetic.read.getdist import read_getdist
 from anesthetic.read.cobaya import read_cobaya
 from anesthetic.read.multinest import read_multinest
 from anesthetic.read.ultranest import read_ultranest
 import pandas._testing as tm
 from anesthetic.read.hdf import HDFStore, read_hdf
-try:
-    import h5py  # noqa: F401
-except ImportError:
-    pass
-try:
-    import getdist
-except ImportError:
-    pass
-try:
-    from tables import Array  # noqa: F401
-    pytables_imported = True
-except ImportError:
-    pytables_imported = False
+from utils import pytables_mark_xfail, h5py_mark_xfail, getdist_mark_skip
 
 
 @pytest.fixture(autouse=True)
 def close_figures_on_teardown():
     tm.close()
 
 
@@ -69,49 +56,52 @@
 
     params = [0, 1, 2, 3, 4, 'logL', 'chain']
     assert all(mcmc.drop_labels().columns == params)
     labels = ['', '', '', '', '', r'$\ln\mathcal{L}$', r'$n_\mathrm{chain}$']
     assert_array_equal(mcmc.get_labels(), labels)
 
 
-@pytest.mark.xfail('getdist' not in sys.modules,
-                   raises=NameError,
-                   reason="requires getdist package")
 def test_read_cobayamcmc():
     np.random.seed(3)
     mcmc = read_cobaya('./tests/example_data/cb')
     assert isinstance(mcmc, MCMCSamples)
     w = np.concatenate((
         np.loadtxt("./tests/example_data/cb.1.txt", usecols=0),
         np.loadtxt("./tests/example_data/cb.2.txt", usecols=0)
     ))
     assert_array_equal(mcmc.get_weights(), w)
     params = ['x0', 'x1', 'minuslogprior', 'minuslogprior__0', 'chi2',
               'chi2__norm', 'logL', 'chain']
     assert_array_equal(mcmc.drop_labels().columns, params)
-    if 'getdist' in sys.modules:
-        labels = ['$x_0$', '$x_1$', '', '', r'$\chi^2$',
-                  r'$\chi^2_\mathrm{norm}$', r'$\ln\mathcal{L}$',
-                  r'$n_\mathrm{chain}$']
-        assert_array_equal(mcmc.get_labels(), labels)
+
+    labels = ['$x_0$', '$x_1$', '', '', r'$\chi^2$',
+              r'$\chi^2_\mathrm{norm}$', r'$\ln\mathcal{L}$',
+              r'$n_\mathrm{chain}$']
+
+    if getdist_mark_skip.args[0]:
+        labels[:6] = [''] * 6
+
+    assert_array_equal(mcmc.get_labels(), labels)
 
     mcmc.plot_2d(['x0', 'x1'])
     mcmc.plot_1d(['x0', 'x1'])
 
     # single chain file
     mcmc = read_cobaya('./tests/example_data/cb_single_chain')
     params.remove('chain')
     assert_array_equal(mcmc.drop_labels().columns, params)
     labels.remove(r'$n_\mathrm{chain}$')
     assert_array_equal(mcmc.get_labels(), labels)
     # compare directly with getdist
-    mcmc_gd = getdist.loadMCSamples(
-        file_root="./tests/example_data/cb_single_chain"
-    )
-    assert_array_almost_equal(mcmc.logL, mcmc_gd.loglikes, decimal=15)
+    if not getdist_mark_skip.args[0]:
+        import getdist
+        mcmc_gd = getdist.loadMCSamples(
+            file_root="./tests/example_data/cb_single_chain"
+        )
+        assert_array_almost_equal(mcmc.logL, mcmc_gd.loglikes, decimal=15)
 
 
 def test_read_montepython():
     np.random.seed(3)
     root = './tests/example_data/mp/2019-01-24_200000_'
     mcmc = read_getdist(root)
     w = np.concatenate((
@@ -185,17 +175,15 @@
     labels.remove(r'$\ln\mathcal{L}_\mathrm{birth}$')
     assert_array_equal(ns.get_labels(), labels)
     assert isinstance(ns, NestedSamples)
     ns.plot_2d(['x0', 'x1', 'x2', 'x3'])
     ns.plot_1d(['x0', 'x1', 'x2', 'x3'])
 
 
-@pytest.mark.xfail('h5py' not in sys.modules,
-                   raises=NameError,
-                   reason="ultranest reading requires `h5py` package")
+@h5py_mark_xfail
 def test_read_ultranest():
     np.random.seed(3)
     ns = read_ultranest('./tests/example_data/un')
     params = ['a', 'b', 'c', 'd', 'logL', 'logL_birth', 'nlive']
     assert_array_equal(ns.drop_labels().columns, params)
     labels = ['a',
               'b',
@@ -265,16 +253,15 @@
 def test_regex_escape():
     mcmc_1 = read_chains('./tests/example_data/gd_single+X')
     mcmc_2 = read_chains('./tests/example_data/gd_single')
     assert_frame_equal(mcmc_1, mcmc_2, check_metadata=False)
 
 
 @pytest.mark.parametrize('root', ['pc', 'gd'])
-@pytest.mark.skipif(pytables_imported is False,
-                    reason="requires tables package")
+@pytables_mark_xfail
 def test_hdf5(tmp_path, root):
     samples = read_chains('./tests/example_data/' + root)
     filename = tmp_path / ('test_hdf5' + root + '.h5')
     key = "samples"
 
     with HDFStore(filename) as store:
         store[key] = samples
```

### Comparing `anesthetic-2.1.4/tests/test_samples.py` & `anesthetic-2.1.5/tests/test_samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import anesthetic.examples._matplotlib_agg  # noqa: F401
 
-import sys
 import pytest
 from math import floor, ceil
 import numpy as np
 from pandas import MultiIndex
 import matplotlib.pyplot as plt
 from matplotlib.lines import Line2D
 from matplotlib.patches import Rectangle
@@ -18,14 +17,15 @@
                                 WeightedLabelledDataFrame)
 from numpy.testing import (assert_array_equal, assert_array_almost_equal,
                            assert_array_less, assert_allclose)
 from pandas.testing import assert_frame_equal
 import pandas._testing as tm
 from matplotlib.colors import to_hex
 from scipy.stats import ks_2samp, kstest, norm
+from utils import skipif_no_fastkde, astropy_mark_xfail, fastkde_mark_skip
 
 
 @pytest.fixture(autouse=True)
 def close_figures_on_teardown():
     tm.close()
 
 
@@ -288,18 +288,15 @@
     for y, row in axes.iterrows():
         for x, ax in row.items():
             if ax is not None:
                 handles, labels = ax.get_legend_handles_labels()
                 assert labels == ['l1', 'l2']
 
 
-@pytest.mark.parametrize('kind',
-                         ['kde', 'hist', 'fastkde']
-                         if 'fastkde' in sys.modules else
-                         ['kde', 'hist'])
+@pytest.mark.parametrize('kind', ['kde', 'hist', skipif_no_fastkde('fastkde')])
 def test_plot_2d_colours(kind):
     np.random.seed(3)
     gd = read_chains("./tests/example_data/gd")
     gd.drop(columns='x3', inplace=True, level=0)
     pc = read_chains("./tests/example_data/pc")
     pc.drop(columns='x4', inplace=True, level=0)
     mn = read_chains("./tests/example_data/mn")
@@ -341,71 +338,62 @@
                                     dict(c='r', linestyle=':', linewidth=1),
                                     dict(ec='r', fc='b'),
                                     dict(edgecolor='r', facecolor='b'),
                                     dict(cmap=plt.cm.RdBu),
                                     dict(colormap=plt.cm.RdBu),
                                     dict(cmap="viridis"),
                                     dict(colormap="viridis")])
-@pytest.mark.parametrize(
-    'kind', ['kde', 'hist', 'default',
-             dict(diagonal='fastkde_1d', lower='fastkde_2d')]
-)
+@pytest.mark.parametrize('kind', ['kde', 'hist', 'default',
+                                  skipif_no_fastkde('fastkde')])
 def test_plot_2d_kwargs(kind, kwargs):
-    if isinstance(kind, str) or 'fastkde' in sys.modules:
-        np.random.seed(42)
-        pc = read_chains("./tests/example_data/pc")
-        fig, axes = make_2d_axes(['x0', 'x1'])
-        pc.plot_2d(axes, kind=kind, **kwargs)
+    np.random.seed(42)
+    pc = read_chains("./tests/example_data/pc")
+    fig, axes = make_2d_axes(['x0', 'x1'])
+    pc.plot_2d(axes, kind=kind, **kwargs)
 
 
-def test_plot_1d_colours():
+@pytest.mark.parametrize('kind', ['kde', 'hist', skipif_no_fastkde('fastkde')])
+def test_plot_1d_colours(kind):
     np.random.seed(3)
     gd = read_chains("./tests/example_data/gd")
     gd.drop(columns='x3', inplace=True, level=0)
     pc = read_chains("./tests/example_data/pc")
     pc.drop(columns='x4', inplace=True, level=0)
     mn = read_chains("./tests/example_data/mn")
     mn.drop(columns='x2', inplace=True, level=0)
 
-    kinds = ['kde', 'hist']
-    if 'fastkde' in sys.modules:
-        kinds += ['fastkde']
-
-    for kind in kinds:
-        fig = plt.figure()
-        fig, axes = make_1d_axes(['x0', 'x1', 'x2', 'x3', 'x4'], fig=fig)
-        gd.plot_1d(axes, kind=kind + '_1d', label="gd")
-        pc.plot_1d(axes, kind=kind + '_1d', label="pc")
-        mn.plot_1d(axes, kind=kind + '_1d', label="mn")
-        gd_colors = []
-        pc_colors = []
-        mn_colors = []
-        for x, ax in axes.items():
-            handles, labels = ax.get_legend_handles_labels()
-            for handle, label in zip(handles, labels):
-                if isinstance(handle, Rectangle):
-                    color = to_hex(handle.get_facecolor())
-                else:
-                    color = handle.get_color()
-
-                if label == 'gd':
-                    gd_colors.append(color)
-                elif label == 'pc':
-                    pc_colors.append(color)
-                elif label == 'mn':
-                    mn_colors.append(color)
+    fig = plt.figure()
+    fig, axes = make_1d_axes(['x0', 'x1', 'x2', 'x3', 'x4'], fig=fig)
+    gd.plot_1d(axes, kind=kind + '_1d', label="gd")
+    pc.plot_1d(axes, kind=kind + '_1d', label="pc")
+    mn.plot_1d(axes, kind=kind + '_1d', label="mn")
+    gd_colors = []
+    pc_colors = []
+    mn_colors = []
+    for x, ax in axes.items():
+        handles, labels = ax.get_legend_handles_labels()
+        for handle, label in zip(handles, labels):
+            if isinstance(handle, Rectangle):
+                color = to_hex(handle.get_facecolor())
+            else:
+                color = handle.get_color()
+
+            if label == 'gd':
+                gd_colors.append(color)
+            elif label == 'pc':
+                pc_colors.append(color)
+            elif label == 'mn':
+                mn_colors.append(color)
 
-        assert len(set(gd_colors)) == 1
-        assert len(set(mn_colors)) == 1
-        assert len(set(pc_colors)) == 1
+    assert len(set(gd_colors)) == 1
+    assert len(set(mn_colors)) == 1
+    assert len(set(pc_colors)) == 1
 
 
-@pytest.mark.xfail('astropy' not in sys.modules,
-                   raises=ImportError,
-                   reason="requires astropy package")
+@astropy_mark_xfail
 def test_astropyhist():
     np.random.seed(3)
     ns = read_chains('./tests/example_data/pc')
     ns.plot_1d(['x0', 'x1', 'x2', 'x3'], kind='hist_1d', bins='knuth')
 
 
 def test_hist_levels():
@@ -826,30 +814,28 @@
                               pc.set_beta(1).get_weights())
     assert_array_almost_equal(pc.set_beta(.5).get_weights(),
                               pc.set_beta(.5).get_weights())
     assert_array_equal(pc.set_beta(0).get_weights(),
                        pc.set_beta(0).get_weights())
 
 
-def test_masking():
+@pytest.mark.parametrize('kind', ['kde', 'hist', 'kde_1d', 'hist_1d',
+                                  skipif_no_fastkde('fastkde_1d')])
+def test_masking_1d(kind):
     pc = read_chains("./tests/example_data/pc")
     mask = pc['x0'].to_numpy() > 0
+    pc[mask].plot_1d(['x0', 'x1', 'x2'], kind=kind)
 
-    kinds = ['kde', 'hist']
-    if 'fastkde' in sys.modules:
-        kinds += ['fastkde']
-
-    for kind in kinds:
-        fig, axes = make_1d_axes(['x0', 'x1', 'x2'])
-        pc[mask].plot_1d(axes=axes, kind=kind + '_1d')
-
-    for kind in kinds + ['scatter']:
-        fig, axes = make_2d_axes(['x0', 'x1', 'x2'], upper=False)
-        pc[mask].plot_2d(axes=axes, kind=dict(lower=kind + '_2d',
-                                              diagonal='hist_1d'))
+
+@pytest.mark.parametrize('kind', ['kde', 'scatter', 'scatter_2d', 'kde_2d',
+                                  'hist_2d', skipif_no_fastkde('fastkde_2d')])
+def test_masking_2d(kind):
+    pc = read_chains("./tests/example_data/pc")
+    mask = pc['x0'].to_numpy() > 0
+    pc[mask].plot_2d(['x0', 'x1', 'x2'], kind={'lower': kind})
 
 
 def test_merging():
     np.random.seed(3)
     samples_1 = read_chains('./tests/example_data/pc')
     samples_2 = read_chains('./tests/example_data/pc_250')
     samples = merge_nested_samples([samples_1, samples_2])
@@ -1310,18 +1296,16 @@
         axes = samples[['x0', 'x1', 'x2', 'x3', 'x4']].plot.fastkde_1d()
         assert len(axes.lines) == 5
         plt.close("all")
     except ImportError:
         pass
 
 
-@pytest.mark.parametrize('kind',
-                         ['kde', 'hist', 'kde_1d', 'hist_1d', 'fastkde_1d']
-                         if 'fastkde' in sys.modules else
-                         ['kde', 'hist', 'kde_1d', 'hist_1d'])
+@pytest.mark.parametrize('kind', ['kde', 'hist', 'kde_1d', 'hist_1d',
+                                  skipif_no_fastkde('fastkde_1d')])
 def test_samples_dot_plot_legend(kind):
     samples = read_chains('./tests/example_data/pc')
     fig, ax = plt.subplots()
     getattr(samples.x0.plot, kind)(ax=ax)
     getattr(samples.x1.plot, kind)(ax=ax)
     getattr(samples.x2.plot, kind)(ax=ax)
     ax.legend()
@@ -1366,17 +1350,15 @@
     axes = samples.plot_2d(columns)
     for col, ax in zip(columns, axes.loc[:, 'x0']):
         assert samples.get_label(col) == ax.get_ylabel()
     for col, ax in zip(columns, axes.loc['x4', :]):
         assert samples.get_label(col) == ax.get_xlabel()
 
 
-@pytest.mark.parametrize('kind', ['kde', 'hist', 'fastkde']
-                         if 'fastkde' in sys.modules else
-                         ['kde', 'hist'])
+@pytest.mark.parametrize('kind', ['kde', 'hist', skipif_no_fastkde('fastkde')])
 def test_samples_empty_1d_ylabels(kind):
     samples = read_chains('./tests/example_data/pc')
     columns = ['x0', 'x1', 'x2', 'x3', 'x4']
 
     axes = samples.plot_1d(columns, kind=kind+'_1d')
     for col in columns:
         assert axes[col].get_ylabel() == ''
@@ -1675,15 +1657,15 @@
         gb_verts = [p.get_verts() for p in gb_ax.patches]
         assert_allclose(mcmc_verts, gb_verts)
         mcmc_colors = [p.get_facecolor() for p in mcmc_ax.patches]
         gb_colors = [p.get_facecolor() for p in gb_ax.patches]
         assert_allclose(mcmc_colors, gb_colors)
     plt.close('all')
 
-    if 'fastkde' in sys.modules:
+    if not fastkde_mark_skip.args[0]:
         for param in params:
             _, gb_ax = plt.subplots()
             gb_plots = chains[param].plot.fastkde_1d(ax=gb_ax)
             _, mcmc_ax = plt.subplots()
             for chain, gb_ax in zip([1, 2], gb_plots):
                 mcmc_ax = mcmc.loc[mcmc.chain == chain][param].plot.fastkde_1d(
                         ax=mcmc_ax)
```

### Comparing `anesthetic-2.1.4/tests/test_scripts.py` & `anesthetic-2.1.5/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/tests/test_utils.py` & `anesthetic-2.1.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.4/tests/test_weighted_pandas.py` & `anesthetic-2.1.5/tests/test_weighted_pandas.py`

 * *Files identical despite different names*

