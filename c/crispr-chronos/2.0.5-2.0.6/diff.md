# Comparing `tmp/crispr_chronos-2.0.5.tar.gz` & `tmp/crispr_chronos-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispr_chronos-2.0.5.tar", last modified: Tue Aug  1 14:10:42 2023, max compression
+gzip compressed data, was "crispr_chronos-2.0.6.tar", last modified: Fri Aug  4 14:38:45 2023, max compression
```

## Comparing `crispr_chronos-2.0.5.tar` & `crispr_chronos-2.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dempster (579957976) 1594166068        0 2023-08-01 14:10:42.717541 crispr_chronos-2.0.5/
--rw-r--r--   0 dempster (579957976) 1594166068     1469 2023-07-31 13:46:53.000000 crispr_chronos-2.0.5/LICENSE
--rw-r--r--   0 dempster (579957976) 1594166068      190 2023-08-01 14:10:42.717165 crispr_chronos-2.0.5/PKG-INFO
--rw-r--r--   0 dempster (579957976) 1594166068    14669 2023-07-31 13:49:05.000000 crispr_chronos-2.0.5/README.md
-drwxr-xr-x   0 dempster (579957976) 1594166068        0 2023-08-01 14:10:42.713094 crispr_chronos-2.0.5/chronos/
--rw-r--r--   0 dempster (579957976) 1594166068      122 2023-06-20 15:44:04.000000 crispr_chronos-2.0.5/chronos/__init__.py
--rw-r--r--   0 dempster (579957976) 1594166068     4944 2023-02-15 15:25:46.000000 crispr_chronos-2.0.5/chronos/copy_correction.py
--rw-r--r--   0 dempster (579957976) 1594166068    56693 2023-07-24 13:40:29.000000 crispr_chronos-2.0.5/chronos/evaluations.py
--rw-r--r--   0 dempster (579957976) 1594166068     2678 2023-06-20 15:04:45.000000 crispr_chronos-2.0.5/chronos/fetch_parameters.py
--rw-r--r--   0 dempster (579957976) 1594166068    10164 2023-05-03 13:54:29.000000 crispr_chronos-2.0.5/chronos/figshare.py
--rw-r--r--   0 dempster (579957976) 1594166068   122473 2023-07-14 20:13:46.000000 crispr_chronos-2.0.5/chronos/model.py
--rw-r--r--   0 dempster (579957976) 1594166068    17413 2023-07-20 17:03:41.000000 crispr_chronos-2.0.5/chronos/plotting.py
--rw-r--r--   0 dempster (579957976) 1594166068    39967 2023-06-20 14:23:31.000000 crispr_chronos-2.0.5/chronos/reports.py
-drwxr-xr-x   0 dempster (579957976) 1594166068        0 2023-08-01 14:10:42.716500 crispr_chronos-2.0.5/crispr_chronos.egg-info/
--rw-r--r--   0 dempster (579957976) 1594166068      190 2023-08-01 14:10:42.000000 crispr_chronos-2.0.5/crispr_chronos.egg-info/PKG-INFO
--rw-r--r--   0 dempster (579957976) 1594166068      389 2023-08-01 14:10:42.000000 crispr_chronos-2.0.5/crispr_chronos.egg-info/SOURCES.txt
--rw-r--r--   0 dempster (579957976) 1594166068        1 2023-08-01 14:10:42.000000 crispr_chronos-2.0.5/crispr_chronos.egg-info/dependency_links.txt
--rw-r--r--   0 dempster (579957976) 1594166068      180 2023-08-01 14:10:42.000000 crispr_chronos-2.0.5/crispr_chronos.egg-info/requires.txt
--rw-r--r--   0 dempster (579957976) 1594166068        8 2023-08-01 14:10:42.000000 crispr_chronos-2.0.5/crispr_chronos.egg-info/top_level.txt
--rw-r--r--   0 dempster (579957976) 1594166068       38 2023-08-01 14:10:42.717655 crispr_chronos-2.0.5/setup.cfg
--rw-r--r--   0 dempster (579957976) 1594166068      782 2023-07-31 14:34:39.000000 crispr_chronos-2.0.5/setup.py
+drwxr-xr-x   0 dempster (579957976) 1594166068        0 2023-08-04 14:38:45.078980 crispr_chronos-2.0.6/
+-rw-r--r--   0 dempster (579957976) 1594166068     1469 2023-07-31 13:46:53.000000 crispr_chronos-2.0.6/LICENSE
+-rw-r--r--   0 dempster (579957976) 1594166068      190 2023-08-04 14:38:45.078482 crispr_chronos-2.0.6/PKG-INFO
+-rw-r--r--   0 dempster (579957976) 1594166068    14806 2023-08-01 15:44:43.000000 crispr_chronos-2.0.6/README.md
+drwxr-xr-x   0 dempster (579957976) 1594166068        0 2023-08-04 14:38:45.070043 crispr_chronos-2.0.6/chronos/
+-rw-r--r--   0 dempster (579957976) 1594166068      122 2023-06-20 15:44:04.000000 crispr_chronos-2.0.6/chronos/__init__.py
+-rw-r--r--   0 dempster (579957976) 1594166068     4944 2023-02-15 15:25:46.000000 crispr_chronos-2.0.6/chronos/copy_correction.py
+-rw-r--r--   0 dempster (579957976) 1594166068    56693 2023-07-24 13:40:29.000000 crispr_chronos-2.0.6/chronos/evaluations.py
+-rw-r--r--   0 dempster (579957976) 1594166068     2678 2023-06-20 15:04:45.000000 crispr_chronos-2.0.6/chronos/fetch_parameters.py
+-rw-r--r--   0 dempster (579957976) 1594166068    10164 2023-05-03 13:54:29.000000 crispr_chronos-2.0.6/chronos/figshare.py
+-rw-r--r--   0 dempster (579957976) 1594166068   122473 2023-07-14 20:13:46.000000 crispr_chronos-2.0.6/chronos/model.py
+-rw-r--r--   0 dempster (579957976) 1594166068    17413 2023-07-20 17:03:41.000000 crispr_chronos-2.0.6/chronos/plotting.py
+-rw-r--r--   0 dempster (579957976) 1594166068    39964 2023-08-04 14:34:57.000000 crispr_chronos-2.0.6/chronos/reports.py
+drwxr-xr-x   0 dempster (579957976) 1594166068        0 2023-08-04 14:38:45.077242 crispr_chronos-2.0.6/crispr_chronos.egg-info/
+-rw-r--r--   0 dempster (579957976) 1594166068      190 2023-08-04 14:38:45.000000 crispr_chronos-2.0.6/crispr_chronos.egg-info/PKG-INFO
+-rw-r--r--   0 dempster (579957976) 1594166068      389 2023-08-04 14:38:45.000000 crispr_chronos-2.0.6/crispr_chronos.egg-info/SOURCES.txt
+-rw-r--r--   0 dempster (579957976) 1594166068        1 2023-08-04 14:38:45.000000 crispr_chronos-2.0.6/crispr_chronos.egg-info/dependency_links.txt
+-rw-r--r--   0 dempster (579957976) 1594166068      180 2023-08-04 14:38:45.000000 crispr_chronos-2.0.6/crispr_chronos.egg-info/requires.txt
+-rw-r--r--   0 dempster (579957976) 1594166068        8 2023-08-04 14:38:45.000000 crispr_chronos-2.0.6/crispr_chronos.egg-info/top_level.txt
+-rw-r--r--   0 dempster (579957976) 1594166068       38 2023-08-04 14:38:45.079235 crispr_chronos-2.0.6/setup.cfg
+-rw-r--r--   0 dempster (579957976) 1594166068      782 2023-08-04 14:36:43.000000 crispr_chronos-2.0.6/setup.py
```

### Comparing `crispr_chronos-2.0.5/LICENSE` & `crispr_chronos-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crispr_chronos-2.0.5/README.md` & `crispr_chronos-2.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,21 @@
 
 As of 2023/07/14, `pip` will not correctly install tensorflow on Macs with the M1 chip. You can try the instructions here: https://caffeinedev.medium.com/how-to-install-tensorflow-on-m1-mac-8e9b91d93706 but they appear to fail for python 3.10. Reversion to 3.8 led to success. Make sure you can import tensorflow in python without the kernel hanging before proceeding. 
 
 If you followed those instructions, you may find that running the vignette with multiple libraries could also cause the error "cannot assign a device for operation ReadVariableOp." Uninstalling tensorflow-metal will fix this error but may disable running on the GPU. But in general we do not recommend running Chronos on the GPU.
 
 ## Installing Chronos
 
-Download, navigate to the Chronos directory, and run 
+If you have `pip` installed, you can install Chronos from pyPI with
 
-`    $ python pip .`
+`    $ pip install crispr_chronos`
 
-in a terminal window. Chronos `model` requires `python 3` with the packages `tensorflow 2.x`, `numpy`, `pandas`,`h5py`. However, additional modules require additional packages which will be installed by default if missing: `patsy`, `statsmodels`, `scipy`, `matplotlib`, `seaborn`, `adjust_text`, `scikit-learn`, `umap`, `reportlab`.
+However, we recommend downloading this repository as well to run the vignette and download the DepMap trained Chronos parameters.
+
+Chronos `model` requires `python 3` with the packages `tensorflow 2.x`, `numpy`, `pandas`,`h5py`. However, additional modules require additional packages which will be installed by default if missing: `patsy`, `statsmodels`, `scipy`, `matplotlib`, `seaborn`, `adjust_text`, `scikit-learn`, `umap`, `reportlab`.
 
 # Getting Started
 If you have jupyter notebook, you should run through `Vignette.ipynb`. This will both verify that you have a working installation and demonstrate a typical workflow for Chronos. Chronos is meant to be run in a python environment. 
 
 To run Chronos, you need a minimum of three Pandas dataframes:
 
 1. A matrix of raw readcounts, where the columns are targeting sgRNAs, the rows are pDNA sequencing samples or replicate samples, and the entries are the number of reads of the given sgRNA in the given sample. Notice that in Chronos matrices, GUIDES and GENES are always COLUMNS and SAMPLES are always ROWS. Readcounts can have null values as long as no column or row is entirely null.
```

### Comparing `crispr_chronos-2.0.5/chronos/copy_correction.py` & `crispr_chronos-2.0.6/chronos/copy_correction.py`

 * *Files identical despite different names*

### Comparing `crispr_chronos-2.0.5/chronos/evaluations.py` & `crispr_chronos-2.0.6/chronos/evaluations.py`

 * *Files identical despite different names*

### Comparing `crispr_chronos-2.0.5/chronos/fetch_parameters.py` & `crispr_chronos-2.0.6/chronos/fetch_parameters.py`

 * *Files identical despite different names*

### Comparing `crispr_chronos-2.0.5/chronos/figshare.py` & `crispr_chronos-2.0.6/chronos/figshare.py`

 * *Files identical despite different names*

### Comparing `crispr_chronos-2.0.5/chronos/model.py` & `crispr_chronos-2.0.6/chronos/model.py`

 * *Files identical despite different names*

### Comparing `crispr_chronos-2.0.5/chronos/plotting.py` & `crispr_chronos-2.0.6/chronos/plotting.py`

 * *Files identical despite different names*

### Comparing `crispr_chronos-2.0.5/chronos/reports.py` & `crispr_chronos-2.0.6/chronos/reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import numpy as np
 import pandas as pd
 import os
 from matplotlib import pyplot as plt
 import seaborn as sns
 
-from cds.plotting import density_scatter, dict_plot
+from .plotting import density_scatter, dict_plot
 from scipy.stats import pearsonr
 from statsmodels.stats.multitest import fdrcorrection
 
 
 def load_chronos_data_for_qc(directory, gene_effect_file="gene_effect.hdf5"):
 	'''
 	Loads the results of a Chronos run saved to the `directory` using the `Chronos.save` method in a `dict`
```

### Comparing `crispr_chronos-2.0.5/setup.py` & `crispr_chronos-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	"reports": ["reportlab>=3.6"],
 	"model": ["numpy>=1.2", "pandas>=1.3", "tensorflow>2", "h5py>=3.7"]
 }
 extras_require['all'] = sorted(set.union(*[set(v) for v in extras_require.values()]))
 
 setup(
 	name='crispr_chronos',
-	version='2.0.5',
+	version='2.0.6',
 	author="BroadInstitute CDS",
 	description="Time series modeling of CRISPR perturbation readcounts in biological data",
 	packages=find_packages(),
 	package_data={'': ['*.r']},
 	install_requires=extras_require['all']
 	#extras_require = extras_require
 )
```

