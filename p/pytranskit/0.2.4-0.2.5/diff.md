# Comparing `tmp/pytranskit-0.2.4.tar.gz` & `tmp/pytranskit-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/ar3fx/Desktop/Research/Lagrangian transform/git_repo/PyTransKit/dist/tmpjdoodgb3/pytranskit-0.2.4.tar", last modified: Sun Jul 24 15:36:33 2022, max compression
+gzip compressed data, was "pytranskit-0.2.5.tar", last modified: Fri Aug  4 03:23:39 2023, max compression
```

## Comparing `pytranskit-0.2.4.tar` & `pytranskit-0.2.5.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:36:33.000000 pytranskit-0.2.4/
--rwxr-xr-x   0 ar3fx      (502) staff       (20)    35147 2022-07-24 15:18:12.000000 pytranskit-0.2.4/LICENSE
--rw-r--r--   0 ar3fx      (502) staff       (20)     8844 2022-07-24 15:36:33.000000 pytranskit-0.2.4/PKG-INFO
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     7928 2022-07-24 15:18:12.000000 pytranskit-0.2.4/README.md
-drwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit/
-drwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit/TBM/
--rwxr-xr-x   0 ar3fx      (502) staff       (20)    33100 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/TBM/TBM_CLOT.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)    38729 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/TBM/TBM_PLOT.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)    31009 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/TBM/TBM_RCDT.py
--rw-r--r--   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/TBM/__init__.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     6534 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/TBM/preprocessing.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     4144 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/TBM/utils.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)       69 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/__init__.py
-drwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit/classification/
--rwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/classification/__init__.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     5229 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/classification/cdt_ns.py
--rw-r--r--   0 ar3fx      (502) staff       (20)     9452 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/classification/inv_enc.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     5925 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/classification/rcdt_ns.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     5995 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/classification/rcdt_ns_3d.py
--rw-r--r--   0 ar3fx      (502) staff       (20)    12854 2022-07-24 03:17:57.000000 pytranskit-0.2.4/pytranskit/classification/scdt_nls.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     5458 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/classification/scdt_ns.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)    10191 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/classification/utils.py
-drwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit/optrans/
--rwxr-xr-x   0 ar3fx      (502) staff       (20)       45 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/__init__.py
-drwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit/optrans/continuous/
--rwxr-xr-x   0 ar3fx      (502) staff       (20)      192 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/continuous/__init__.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     4254 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/continuous/base.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     6127 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/continuous/cdt.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)    11074 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/continuous/clot.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     7934 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/continuous/radoncdt.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     8936 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/continuous/radoncdt3D.py
--rw-r--r--   0 ar3fx      (502) staff       (20)     5534 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/continuous/scdt.py
-drwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit/optrans/decomposition/
--rwxr-xr-x   0 ar3fx      (502) staff       (20)      206 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/decomposition/__init__.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     9281 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/decomposition/cca.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     3976 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/decomposition/modes.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)    14626 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/decomposition/plda.py
-drwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit/optrans/utils/
--rwxr-xr-x   0 ar3fx      (502) staff       (20)      362 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/utils/__init__.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     4822 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/utils/data_utils.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     4541 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/utils/validation.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     2408 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/utils/visualize.py
-drwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit/optrans/visualization/
--rwxr-xr-x   0 ar3fx      (502) staff       (20)      275 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/visualization/__init__.py
--rwxr-xr-x   0 ar3fx      (502) staff       (20)    14276 2022-07-24 15:18:12.000000 pytranskit-0.2.4/pytranskit/optrans/visualization/visualize.py
-drwxr-xr-x   0 ar3fx      (502) staff       (20)        0 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit.egg-info/
--rw-r--r--   0 ar3fx      (502) staff       (20)     8844 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit.egg-info/PKG-INFO
--rw-r--r--   0 ar3fx      (502) staff       (20)     1379 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit.egg-info/SOURCES.txt
--rw-r--r--   0 ar3fx      (502) staff       (20)        1 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit.egg-info/dependency_links.txt
--rw-r--r--   0 ar3fx      (502) staff       (20)       11 2022-07-24 15:36:33.000000 pytranskit-0.2.4/pytranskit.egg-info/top_level.txt
--rwxr-xr-x   0 ar3fx      (502) staff       (20)       79 2022-07-24 15:36:33.000000 pytranskit-0.2.4/setup.cfg
--rwxr-xr-x   0 ar3fx      (502) staff       (20)     1066 2022-07-24 03:25:16.000000 pytranskit-0.2.4/setup.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.158732 pytranskit-0.2.5/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    35147 2023-08-04 02:59:31.000000 pytranskit-0.2.5/LICENSE
+-rw-r--r--   0 qpb3vt     (504) staff       (20)     9666 2023-08-04 03:23:39.159416 pytranskit-0.2.5/PKG-INFO
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     8732 2023-08-04 02:59:31.000000 pytranskit-0.2.5/README.md
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.061984 pytranskit-0.2.5/pytranskit/
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.096912 pytranskit-0.2.5/pytranskit/TBM/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    33100 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/TBM_CLOT.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    38729 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/TBM_PLOT.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    31009 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/TBM_RCDT.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)        0 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     6534 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/preprocessing.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4144 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/utils.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)       69 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/__init__.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.110815 pytranskit-0.2.5/pytranskit/classification/
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     5956 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/RSCDT_NS.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5229 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/cdt_ns.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     9452 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/inv_enc.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5925 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/rcdt_ns.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5995 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/rcdt_ns_3d.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)    12854 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/scdt_nls.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5458 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/scdt_ns.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    10191 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/utils.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.113293 pytranskit-0.2.5/pytranskit/optrans/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)       45 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/__init__.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.132606 pytranskit-0.2.5/pytranskit/optrans/continuous/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      192 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4254 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/base.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     6127 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/cdt.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    11074 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/clot.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     7934 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/radoncdt.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     8936 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/radoncdt3D.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     4149 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/radonscdt.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     5534 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/scdt.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.141659 pytranskit-0.2.5/pytranskit/optrans/decomposition/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      206 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/decomposition/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     9281 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/decomposition/cca.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     3976 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/decomposition/modes.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    14626 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/decomposition/plda.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.151038 pytranskit-0.2.5/pytranskit/optrans/utils/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      362 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/utils/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4822 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/utils/data_utils.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4541 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/utils/validation.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     2408 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/utils/visualize.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.154789 pytranskit-0.2.5/pytranskit/optrans/visualization/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      275 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/visualization/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    14276 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/visualization/visualize.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.086115 pytranskit-0.2.5/pytranskit.egg-info/
+-rw-r--r--   0 qpb3vt     (504) staff       (20)     9666 2023-08-04 03:23:39.000000 pytranskit-0.2.5/pytranskit.egg-info/PKG-INFO
+-rw-r--r--   0 qpb3vt     (504) staff       (20)     1460 2023-08-04 03:23:39.000000 pytranskit-0.2.5/pytranskit.egg-info/SOURCES.txt
+-rw-r--r--   0 qpb3vt     (504) staff       (20)        1 2023-08-04 03:23:39.000000 pytranskit-0.2.5/pytranskit.egg-info/dependency_links.txt
+-rw-r--r--   0 qpb3vt     (504) staff       (20)       11 2023-08-04 03:23:39.000000 pytranskit-0.2.5/pytranskit.egg-info/top_level.txt
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)       79 2023-08-04 03:23:39.165199 pytranskit-0.2.5/setup.cfg
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     1084 2023-08-04 03:22:36.000000 pytranskit-0.2.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytranskit-0.2.4/LICENSE` & `pytranskit-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/PKG-INFO` & `pytranskit-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pytranskit
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python transport based signal processing toolkit.
 Home-page: https://github.com/rohdelab/PyTransKit
-Author: Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Yan Zhuang, Gustavo Rohde
+Author: Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Naqib Sad Pathan, Yan Zhuang, Gustavo Rohde
 Author-email: ar3fx@virginia.edu, xuwangyin@gmail.com, gustavo.rohde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -46,27 +46,35 @@
 
 ## Low Level Functions
 ### CDT, SCDT
 - Cumulative Distribution Transform (CDT) [1] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/01_tutorial_cdt.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/01_tutorial_cdt.ipynb)]
     - Videos: [CDT](https://youtu.be/khkSOleeEno), [Code](https://youtu.be/djmaMXp-Kxk)
 - Signed Cumulative Distribution Transform (SCDT) [6] tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/09_tutorial_SCDT_classification.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/09_tutorial_SCDT_classification.ipynb)]
 - SCDT tutorial with domain adaptation [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/10_tutorial_SCDT.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/10_tutorial_SCDT.ipynb)]
+
+
 ### R-CDT
 - Radon-CDT tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/02_tutorial_rcdt.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/02_tutorial_rcdt.ipynb)]
 - 3D Radon-CDT tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/05_tutorial_rcdt3D.ipynb)][[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/05_tutorial_rcdt3D.ipynb)]
+### RSCDT
+- RSCDT tutorial : Forward and Inverse Transform [10][[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/14_RSCDT-Forward%20and%20inverse%20transform%20.ipynb)]
+- RSCDT based nearest subspace method for image classification [10].
+  [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/15_RSCDT_tutorial.ipynb)]
 ### CLOT
 - Continuous Linear Optimal Transport Transform (CLOT) tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/07_tutorial_clot.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/07_tutorial_clot.ipynb)]
 
 ## Classification Examples
 - CDT Nearest Subspace (CDT-NS) classifier for 1D data [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/04_tutorial_CDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/04_tutorial_CDT-NS_classifier.ipynb)]
 - SCDT Nearest Subspace (SCDT-NS) classifier for 1D data [8] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/11_tutorial_SCDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.org/github/rohdelab/PyTransKit/blob/master/tutorials/11_tutorial_SCDT-NS_classifier.ipynb)]
 - SCDT Nearest Local Subspace (SCDT-NLS) classifier for 1D data [9] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/13_tutorial_SCDT-NLS_classifier.ipynb)] [[nbviewer](https://nbviewer.org/github/rohdelab/PyTransKit/blob/master/tutorials/13_tutorial_SCDT-NLS_classifier.ipynb)]
 - Radon-CDT Nearest Subspace (RCDT-NS) classifier for 2D data [4] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/03_tutorial_RCDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/03_tutorial_RCDT-NS_classifier.ipynb)]
 - 3D Radon-CDT Nearest Subspace (3D-RCDT-NS) classifier for 3D data [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/06_tutorial_3DRCDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/06_tutorial_3DRCDT-NS_classifier.ipynb)]
 - Discrete Radon-CDT Nearest Subspace classifier for illumination-invariant Face Recognition [[notebook](https://github.com/rohdelab/drcdt_face)]
+-  RSCDT based nearest subspace method for image classification [10].
+  [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/15_RSCDT_tutorial.ipynb)]
 
 ## Estimation Examples
 - Time delay estimation using CDT [5] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/Examples/Example01_estimation_delay.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/Examples/Example01_estimation_delay.ipynb)]
 - Time delay and linear dispersion estimation using CDT [5] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/Examples/Example02_estimation_delay_linear_dispersion.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/Examples/Example02_estimation_delay_linear_dispersion.ipynb)]
 
 ## Transport-based Morphometry
 - Transport-based Morphometry to detect and visualize cell phenotype differences [7] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/08_tutorial_TBM.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/08_tutorial_TBM.ipynb)]
@@ -78,15 +86,15 @@
 3. [A continuous linear optimal transport approach for pattern analysis in image datasets, Pattern Recognition, March 2016](https://www.sciencedirect.com/science/article/abs/pii/S0031320315003507)
 4. [Radon cumulative distribution transform subspace modeling for image classification, Journal of Mathematical Imaging and Vision, 2021](https://link.springer.com/article/10.1007/s10851-021-01052-0)
 5. [Parametric Signal Estimation Using the Cumulative Distribution Transform, IEEE Transactions on Signal Processing, May 2020](https://ieeexplore.ieee.org/abstract/document/9099391)
 6. [The Signed Cumulative Distribution Transform for 1-D Signal Analysis and Classification, ArXiv 2021](https://arxiv.org/abs/2106.02146)
 7. [Detecting and visualizing cell phenotype differences from microscopy images using transport-based morphometry, PNAS 2014](https://www.pnas.org/content/111/9/3448.short)
 8. [Nearest Subspace Search in the Signed Cumulative Distribution Transform Space for 1D Signal Classification, IEEE International Conference on Acoustics, Speech and Signal Processing, May 2022](https://arxiv.org/abs/2110.05606)
 9. [End-to-End Signal Classification in Signed Cumulative Distribution Transform Space, ArXiv 2022](https://arxiv.org/abs/2205.00348)
-
+10. [Gong, L., Li, S., Pathan, N. S., Rohde, G. K., Rubaiyat, A. H. M., & Thareja, S. (2023). The Radon Signed Cumulative Distribution Transform and its applications in classification of Signed Images. arXiv preprint arXiv:2307.15339.](https://arxiv.org/abs/2307.15339)
 ## Resources
 External website http://imagedatascience.com/transport/
 
 Video [[tutorials](https://www.youtube.com/playlist?list=PLWqC8YvK1oV4pL5KvUsTb7LJdJCmyHvX0)]
 
 ## Authors
 - Abu Hasnat Mohammad Rubaiyat
```

### Comparing `pytranskit-0.2.4/README.md` & `pytranskit-0.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -26,27 +26,35 @@
 
 ## Low Level Functions
 ### CDT, SCDT
 - Cumulative Distribution Transform (CDT) [1] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/01_tutorial_cdt.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/01_tutorial_cdt.ipynb)]
     - Videos: [CDT](https://youtu.be/khkSOleeEno), [Code](https://youtu.be/djmaMXp-Kxk)
 - Signed Cumulative Distribution Transform (SCDT) [6] tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/09_tutorial_SCDT_classification.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/09_tutorial_SCDT_classification.ipynb)]
 - SCDT tutorial with domain adaptation [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/10_tutorial_SCDT.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/10_tutorial_SCDT.ipynb)]
+
+
 ### R-CDT
 - Radon-CDT tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/02_tutorial_rcdt.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/02_tutorial_rcdt.ipynb)]
 - 3D Radon-CDT tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/05_tutorial_rcdt3D.ipynb)][[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/05_tutorial_rcdt3D.ipynb)]
+### RSCDT
+- RSCDT tutorial : Forward and Inverse Transform [10][[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/14_RSCDT-Forward%20and%20inverse%20transform%20.ipynb)]
+- RSCDT based nearest subspace method for image classification [10].
+  [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/15_RSCDT_tutorial.ipynb)]
 ### CLOT
 - Continuous Linear Optimal Transport Transform (CLOT) tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/07_tutorial_clot.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/07_tutorial_clot.ipynb)]
 
 ## Classification Examples
 - CDT Nearest Subspace (CDT-NS) classifier for 1D data [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/04_tutorial_CDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/04_tutorial_CDT-NS_classifier.ipynb)]
 - SCDT Nearest Subspace (SCDT-NS) classifier for 1D data [8] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/11_tutorial_SCDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.org/github/rohdelab/PyTransKit/blob/master/tutorials/11_tutorial_SCDT-NS_classifier.ipynb)]
 - SCDT Nearest Local Subspace (SCDT-NLS) classifier for 1D data [9] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/13_tutorial_SCDT-NLS_classifier.ipynb)] [[nbviewer](https://nbviewer.org/github/rohdelab/PyTransKit/blob/master/tutorials/13_tutorial_SCDT-NLS_classifier.ipynb)]
 - Radon-CDT Nearest Subspace (RCDT-NS) classifier for 2D data [4] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/03_tutorial_RCDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/03_tutorial_RCDT-NS_classifier.ipynb)]
 - 3D Radon-CDT Nearest Subspace (3D-RCDT-NS) classifier for 3D data [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/06_tutorial_3DRCDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/06_tutorial_3DRCDT-NS_classifier.ipynb)]
 - Discrete Radon-CDT Nearest Subspace classifier for illumination-invariant Face Recognition [[notebook](https://github.com/rohdelab/drcdt_face)]
+-  RSCDT based nearest subspace method for image classification [10].
+  [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/15_RSCDT_tutorial.ipynb)]
 
 ## Estimation Examples
 - Time delay estimation using CDT [5] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/Examples/Example01_estimation_delay.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/Examples/Example01_estimation_delay.ipynb)]
 - Time delay and linear dispersion estimation using CDT [5] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/Examples/Example02_estimation_delay_linear_dispersion.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/Examples/Example02_estimation_delay_linear_dispersion.ipynb)]
 
 ## Transport-based Morphometry
 - Transport-based Morphometry to detect and visualize cell phenotype differences [7] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/08_tutorial_TBM.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/08_tutorial_TBM.ipynb)]
@@ -58,15 +66,15 @@
 3. [A continuous linear optimal transport approach for pattern analysis in image datasets, Pattern Recognition, March 2016](https://www.sciencedirect.com/science/article/abs/pii/S0031320315003507)
 4. [Radon cumulative distribution transform subspace modeling for image classification, Journal of Mathematical Imaging and Vision, 2021](https://link.springer.com/article/10.1007/s10851-021-01052-0)
 5. [Parametric Signal Estimation Using the Cumulative Distribution Transform, IEEE Transactions on Signal Processing, May 2020](https://ieeexplore.ieee.org/abstract/document/9099391)
 6. [The Signed Cumulative Distribution Transform for 1-D Signal Analysis and Classification, ArXiv 2021](https://arxiv.org/abs/2106.02146)
 7. [Detecting and visualizing cell phenotype differences from microscopy images using transport-based morphometry, PNAS 2014](https://www.pnas.org/content/111/9/3448.short)
 8. [Nearest Subspace Search in the Signed Cumulative Distribution Transform Space for 1D Signal Classification, IEEE International Conference on Acoustics, Speech and Signal Processing, May 2022](https://arxiv.org/abs/2110.05606)
 9. [End-to-End Signal Classification in Signed Cumulative Distribution Transform Space, ArXiv 2022](https://arxiv.org/abs/2205.00348)
-
+10. [Gong, L., Li, S., Pathan, N. S., Rohde, G. K., Rubaiyat, A. H. M., & Thareja, S. (2023). The Radon Signed Cumulative Distribution Transform and its applications in classification of Signed Images. arXiv preprint arXiv:2307.15339.](https://arxiv.org/abs/2307.15339)
 ## Resources
 External website http://imagedatascience.com/transport/
 
 Video [[tutorials](https://www.youtube.com/playlist?list=PLWqC8YvK1oV4pL5KvUsTb7LJdJCmyHvX0)]
 
 ## Authors
 - Abu Hasnat Mohammad Rubaiyat
```

### Comparing `pytranskit-0.2.4/pytranskit/TBM/TBM_CLOT.py` & `pytranskit-0.2.5/pytranskit/TBM/TBM_CLOT.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/TBM/TBM_PLOT.py` & `pytranskit-0.2.5/pytranskit/TBM/TBM_PLOT.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/TBM/TBM_RCDT.py` & `pytranskit-0.2.5/pytranskit/TBM/TBM_RCDT.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/TBM/preprocessing.py` & `pytranskit-0.2.5/pytranskit/TBM/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/TBM/utils.py` & `pytranskit-0.2.5/pytranskit/TBM/utils.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/classification/cdt_ns.py` & `pytranskit-0.2.5/pytranskit/classification/cdt_ns.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/classification/inv_enc.py` & `pytranskit-0.2.5/pytranskit/classification/inv_enc.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/classification/rcdt_ns.py` & `pytranskit-0.2.5/pytranskit/classification/rcdt_ns.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/classification/rcdt_ns_3d.py` & `pytranskit-0.2.5/pytranskit/classification/rcdt_ns_3d.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/classification/scdt_nls.py` & `pytranskit-0.2.5/pytranskit/classification/scdt_nls.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/classification/scdt_ns.py` & `pytranskit-0.2.5/pytranskit/classification/scdt_ns.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/classification/utils.py` & `pytranskit-0.2.5/pytranskit/classification/utils.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/continuous/base.py` & `pytranskit-0.2.5/pytranskit/optrans/continuous/base.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/continuous/cdt.py` & `pytranskit-0.2.5/pytranskit/optrans/continuous/cdt.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/continuous/clot.py` & `pytranskit-0.2.5/pytranskit/optrans/continuous/clot.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/continuous/radoncdt.py` & `pytranskit-0.2.5/pytranskit/optrans/continuous/radoncdt.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/continuous/radoncdt3D.py` & `pytranskit-0.2.5/pytranskit/optrans/continuous/radoncdt3D.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/continuous/scdt.py` & `pytranskit-0.2.5/pytranskit/optrans/continuous/scdt.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/decomposition/cca.py` & `pytranskit-0.2.5/pytranskit/optrans/decomposition/cca.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/decomposition/modes.py` & `pytranskit-0.2.5/pytranskit/optrans/decomposition/modes.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/decomposition/plda.py` & `pytranskit-0.2.5/pytranskit/optrans/decomposition/plda.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/utils/data_utils.py` & `pytranskit-0.2.5/pytranskit/optrans/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/utils/validation.py` & `pytranskit-0.2.5/pytranskit/optrans/utils/validation.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/utils/visualize.py` & `pytranskit-0.2.5/pytranskit/optrans/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit/optrans/visualization/visualize.py` & `pytranskit-0.2.5/pytranskit/optrans/visualization/visualize.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.4/pytranskit.egg-info/PKG-INFO` & `pytranskit-0.2.5/pytranskit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pytranskit
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python transport based signal processing toolkit.
 Home-page: https://github.com/rohdelab/PyTransKit
-Author: Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Yan Zhuang, Gustavo Rohde
+Author: Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Naqib Sad Pathan, Yan Zhuang, Gustavo Rohde
 Author-email: ar3fx@virginia.edu, xuwangyin@gmail.com, gustavo.rohde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
@@ -46,27 +46,35 @@
 
 ## Low Level Functions
 ### CDT, SCDT
 - Cumulative Distribution Transform (CDT) [1] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/01_tutorial_cdt.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/01_tutorial_cdt.ipynb)]
     - Videos: [CDT](https://youtu.be/khkSOleeEno), [Code](https://youtu.be/djmaMXp-Kxk)
 - Signed Cumulative Distribution Transform (SCDT) [6] tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/09_tutorial_SCDT_classification.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/09_tutorial_SCDT_classification.ipynb)]
 - SCDT tutorial with domain adaptation [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/10_tutorial_SCDT.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/10_tutorial_SCDT.ipynb)]
+
+
 ### R-CDT
 - Radon-CDT tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/02_tutorial_rcdt.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/02_tutorial_rcdt.ipynb)]
 - 3D Radon-CDT tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/05_tutorial_rcdt3D.ipynb)][[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/05_tutorial_rcdt3D.ipynb)]
+### RSCDT
+- RSCDT tutorial : Forward and Inverse Transform [10][[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/14_RSCDT-Forward%20and%20inverse%20transform%20.ipynb)]
+- RSCDT based nearest subspace method for image classification [10].
+  [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/15_RSCDT_tutorial.ipynb)]
 ### CLOT
 - Continuous Linear Optimal Transport Transform (CLOT) tutorial [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/07_tutorial_clot.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/07_tutorial_clot.ipynb)]
 
 ## Classification Examples
 - CDT Nearest Subspace (CDT-NS) classifier for 1D data [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/04_tutorial_CDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/04_tutorial_CDT-NS_classifier.ipynb)]
 - SCDT Nearest Subspace (SCDT-NS) classifier for 1D data [8] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/11_tutorial_SCDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.org/github/rohdelab/PyTransKit/blob/master/tutorials/11_tutorial_SCDT-NS_classifier.ipynb)]
 - SCDT Nearest Local Subspace (SCDT-NLS) classifier for 1D data [9] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/13_tutorial_SCDT-NLS_classifier.ipynb)] [[nbviewer](https://nbviewer.org/github/rohdelab/PyTransKit/blob/master/tutorials/13_tutorial_SCDT-NLS_classifier.ipynb)]
 - Radon-CDT Nearest Subspace (RCDT-NS) classifier for 2D data [4] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/03_tutorial_RCDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/03_tutorial_RCDT-NS_classifier.ipynb)]
 - 3D Radon-CDT Nearest Subspace (3D-RCDT-NS) classifier for 3D data [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/06_tutorial_3DRCDT-NS_classifier.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/06_tutorial_3DRCDT-NS_classifier.ipynb)]
 - Discrete Radon-CDT Nearest Subspace classifier for illumination-invariant Face Recognition [[notebook](https://github.com/rohdelab/drcdt_face)]
+-  RSCDT based nearest subspace method for image classification [10].
+  [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/15_RSCDT_tutorial.ipynb)]
 
 ## Estimation Examples
 - Time delay estimation using CDT [5] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/Examples/Example01_estimation_delay.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/Examples/Example01_estimation_delay.ipynb)]
 - Time delay and linear dispersion estimation using CDT [5] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/Examples/Example02_estimation_delay_linear_dispersion.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/Examples/Example02_estimation_delay_linear_dispersion.ipynb)]
 
 ## Transport-based Morphometry
 - Transport-based Morphometry to detect and visualize cell phenotype differences [7] [[notebook](https://github.com/rohdelab/PyTransKit/blob/master/tutorials/08_tutorial_TBM.ipynb)] [[nbviewer](https://nbviewer.jupyter.org/github/rohdelab/PyTransKit/blob/master/tutorials/08_tutorial_TBM.ipynb)]
@@ -78,15 +86,15 @@
 3. [A continuous linear optimal transport approach for pattern analysis in image datasets, Pattern Recognition, March 2016](https://www.sciencedirect.com/science/article/abs/pii/S0031320315003507)
 4. [Radon cumulative distribution transform subspace modeling for image classification, Journal of Mathematical Imaging and Vision, 2021](https://link.springer.com/article/10.1007/s10851-021-01052-0)
 5. [Parametric Signal Estimation Using the Cumulative Distribution Transform, IEEE Transactions on Signal Processing, May 2020](https://ieeexplore.ieee.org/abstract/document/9099391)
 6. [The Signed Cumulative Distribution Transform for 1-D Signal Analysis and Classification, ArXiv 2021](https://arxiv.org/abs/2106.02146)
 7. [Detecting and visualizing cell phenotype differences from microscopy images using transport-based morphometry, PNAS 2014](https://www.pnas.org/content/111/9/3448.short)
 8. [Nearest Subspace Search in the Signed Cumulative Distribution Transform Space for 1D Signal Classification, IEEE International Conference on Acoustics, Speech and Signal Processing, May 2022](https://arxiv.org/abs/2110.05606)
 9. [End-to-End Signal Classification in Signed Cumulative Distribution Transform Space, ArXiv 2022](https://arxiv.org/abs/2205.00348)
-
+10. [Gong, L., Li, S., Pathan, N. S., Rohde, G. K., Rubaiyat, A. H. M., & Thareja, S. (2023). The Radon Signed Cumulative Distribution Transform and its applications in classification of Signed Images. arXiv preprint arXiv:2307.15339.](https://arxiv.org/abs/2307.15339)
 ## Resources
 External website http://imagedatascience.com/transport/
 
 Video [[tutorials](https://www.youtube.com/playlist?list=PLWqC8YvK1oV4pL5KvUsTb7LJdJCmyHvX0)]
 
 ## Authors
 - Abu Hasnat Mohammad Rubaiyat
```

### Comparing `pytranskit-0.2.4/pytranskit.egg-info/SOURCES.txt` & `pytranskit-0.2.5/pytranskit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 pytranskit.egg-info/top_level.txt
 pytranskit/TBM/TBM_CLOT.py
 pytranskit/TBM/TBM_PLOT.py
 pytranskit/TBM/TBM_RCDT.py
 pytranskit/TBM/__init__.py
 pytranskit/TBM/preprocessing.py
 pytranskit/TBM/utils.py
+pytranskit/classification/RSCDT_NS.py
 pytranskit/classification/__init__.py
 pytranskit/classification/cdt_ns.py
 pytranskit/classification/inv_enc.py
 pytranskit/classification/rcdt_ns.py
 pytranskit/classification/rcdt_ns_3d.py
 pytranskit/classification/scdt_nls.py
 pytranskit/classification/scdt_ns.py
@@ -24,14 +25,15 @@
 pytranskit/optrans/__init__.py
 pytranskit/optrans/continuous/__init__.py
 pytranskit/optrans/continuous/base.py
 pytranskit/optrans/continuous/cdt.py
 pytranskit/optrans/continuous/clot.py
 pytranskit/optrans/continuous/radoncdt.py
 pytranskit/optrans/continuous/radoncdt3D.py
+pytranskit/optrans/continuous/radonscdt.py
 pytranskit/optrans/continuous/scdt.py
 pytranskit/optrans/decomposition/__init__.py
 pytranskit/optrans/decomposition/cca.py
 pytranskit/optrans/decomposition/modes.py
 pytranskit/optrans/decomposition/plda.py
 pytranskit/optrans/utils/__init__.py
 pytranskit/optrans/utils/data_utils.py
```

### Comparing `pytranskit-0.2.4/setup.py` & `pytranskit-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description=fh.read()
 
 setuptools.setup(
   name="pytranskit",
-  version="0.2.4",
-  author="Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Yan Zhuang, Gustavo Rohde",
+  version="0.2.5",
+  author="Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Naqib Sad Pathan, Yan Zhuang, Gustavo Rohde",
   author_email="ar3fx@virginia.edu, xuwangyin@gmail.com, gustavo.rohde@gmail.com",
   description="Python transport based signal processing toolkit.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/rohdelab/PyTransKit",
   packages=setuptools.find_packages(),
   classifiers=[
```

