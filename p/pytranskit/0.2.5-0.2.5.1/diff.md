# Comparing `tmp/pytranskit-0.2.5.tar.gz` & `tmp/pytranskit-0.2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytranskit-0.2.5.tar", last modified: Fri Aug  4 03:23:39 2023, max compression
+gzip compressed data, was "pytranskit-0.2.5.1.tar", last modified: Fri Aug  4 04:29:06 2023, max compression
```

## Comparing `pytranskit-0.2.5.tar` & `pytranskit-0.2.5.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.158732 pytranskit-0.2.5/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    35147 2023-08-04 02:59:31.000000 pytranskit-0.2.5/LICENSE
--rw-r--r--   0 qpb3vt     (504) staff       (20)     9666 2023-08-04 03:23:39.159416 pytranskit-0.2.5/PKG-INFO
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     8732 2023-08-04 02:59:31.000000 pytranskit-0.2.5/README.md
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.061984 pytranskit-0.2.5/pytranskit/
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.096912 pytranskit-0.2.5/pytranskit/TBM/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    33100 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/TBM_CLOT.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    38729 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/TBM_PLOT.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    31009 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/TBM_RCDT.py
--rw-rw-r--   0 qpb3vt     (504) staff       (20)        0 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     6534 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/preprocessing.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4144 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/TBM/utils.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)       69 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/__init__.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.110815 pytranskit-0.2.5/pytranskit/classification/
--rw-rw-r--   0 qpb3vt     (504) staff       (20)     5956 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/RSCDT_NS.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5229 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/cdt_ns.py
--rw-rw-r--   0 qpb3vt     (504) staff       (20)     9452 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/inv_enc.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5925 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/rcdt_ns.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5995 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/rcdt_ns_3d.py
--rw-rw-r--   0 qpb3vt     (504) staff       (20)    12854 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/scdt_nls.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5458 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/scdt_ns.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    10191 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/classification/utils.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.113293 pytranskit-0.2.5/pytranskit/optrans/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)       45 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/__init__.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.132606 pytranskit-0.2.5/pytranskit/optrans/continuous/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)      192 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4254 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/base.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     6127 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/cdt.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    11074 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/clot.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     7934 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/radoncdt.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     8936 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/radoncdt3D.py
--rw-rw-r--   0 qpb3vt     (504) staff       (20)     4149 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/radonscdt.py
--rw-rw-r--   0 qpb3vt     (504) staff       (20)     5534 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/continuous/scdt.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.141659 pytranskit-0.2.5/pytranskit/optrans/decomposition/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)      206 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/decomposition/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     9281 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/decomposition/cca.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     3976 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/decomposition/modes.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    14626 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/decomposition/plda.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.151038 pytranskit-0.2.5/pytranskit/optrans/utils/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)      362 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/utils/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4822 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/utils/data_utils.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4541 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/utils/validation.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     2408 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/utils/visualize.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.154789 pytranskit-0.2.5/pytranskit/optrans/visualization/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)      275 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/visualization/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    14276 2023-08-04 02:59:31.000000 pytranskit-0.2.5/pytranskit/optrans/visualization/visualize.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 03:23:39.086115 pytranskit-0.2.5/pytranskit.egg-info/
--rw-r--r--   0 qpb3vt     (504) staff       (20)     9666 2023-08-04 03:23:39.000000 pytranskit-0.2.5/pytranskit.egg-info/PKG-INFO
--rw-r--r--   0 qpb3vt     (504) staff       (20)     1460 2023-08-04 03:23:39.000000 pytranskit-0.2.5/pytranskit.egg-info/SOURCES.txt
--rw-r--r--   0 qpb3vt     (504) staff       (20)        1 2023-08-04 03:23:39.000000 pytranskit-0.2.5/pytranskit.egg-info/dependency_links.txt
--rw-r--r--   0 qpb3vt     (504) staff       (20)       11 2023-08-04 03:23:39.000000 pytranskit-0.2.5/pytranskit.egg-info/top_level.txt
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)       79 2023-08-04 03:23:39.165199 pytranskit-0.2.5/setup.cfg
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     1084 2023-08-04 03:22:36.000000 pytranskit-0.2.5/setup.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.447311 pytranskit-0.2.5.1/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    35147 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/LICENSE
+-rw-r--r--   0 qpb3vt     (504) staff       (20)     9668 2023-08-04 04:29:06.447587 pytranskit-0.2.5.1/PKG-INFO
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     8732 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/README.md
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.157827 pytranskit-0.2.5.1/pytranskit/
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.225397 pytranskit-0.2.5.1/pytranskit/TBM/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    33100 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/TBM_CLOT.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    38729 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/TBM_PLOT.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    31009 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/TBM_RCDT.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)        0 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     6534 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/preprocessing.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4144 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/utils.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)       69 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/__init__.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.299356 pytranskit-0.2.5.1/pytranskit/classification/
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     5955 2023-08-04 03:43:11.000000 pytranskit-0.2.5.1/pytranskit/classification/RSCDT_NS.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5229 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/cdt_ns.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     9452 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/inv_enc.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5925 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/rcdt_ns.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5995 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/rcdt_ns_3d.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)    12854 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/scdt_nls.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5458 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/scdt_ns.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    10191 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/utils.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.307126 pytranskit-0.2.5.1/pytranskit/optrans/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)       45 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/__init__.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.365610 pytranskit-0.2.5.1/pytranskit/optrans/continuous/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      192 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4254 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/base.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     6127 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/cdt.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    11074 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/clot.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     7934 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/radoncdt.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     8936 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/radoncdt3D.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     4149 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/radonscdt.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     5948 2023-08-04 03:50:12.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/scdt.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.399451 pytranskit-0.2.5.1/pytranskit/optrans/decomposition/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      206 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/decomposition/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     9281 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/decomposition/cca.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     3976 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/decomposition/modes.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    14626 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/decomposition/plda.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.427768 pytranskit-0.2.5.1/pytranskit/optrans/utils/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      362 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/utils/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4822 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/utils/data_utils.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4541 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/utils/validation.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     2408 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/utils/visualize.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.446055 pytranskit-0.2.5.1/pytranskit/optrans/visualization/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      275 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/visualization/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    14276 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/visualization/visualize.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.174713 pytranskit-0.2.5.1/pytranskit.egg-info/
+-rw-r--r--   0 qpb3vt     (504) staff       (20)     9668 2023-08-04 04:29:06.000000 pytranskit-0.2.5.1/pytranskit.egg-info/PKG-INFO
+-rw-r--r--   0 qpb3vt     (504) staff       (20)     1460 2023-08-04 04:29:06.000000 pytranskit-0.2.5.1/pytranskit.egg-info/SOURCES.txt
+-rw-r--r--   0 qpb3vt     (504) staff       (20)        1 2023-08-04 04:29:06.000000 pytranskit-0.2.5.1/pytranskit.egg-info/dependency_links.txt
+-rw-r--r--   0 qpb3vt     (504) staff       (20)       11 2023-08-04 04:29:06.000000 pytranskit-0.2.5.1/pytranskit.egg-info/top_level.txt
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)       79 2023-08-04 04:29:06.453579 pytranskit-0.2.5.1/setup.cfg
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     1086 2023-08-04 04:28:37.000000 pytranskit-0.2.5.1/setup.py
```

### Comparing `pytranskit-0.2.5/LICENSE` & `pytranskit-0.2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/PKG-INFO` & `pytranskit-0.2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytranskit
-Version: 0.2.5
+Version: 0.2.5.1
 Summary: Python transport based signal processing toolkit.
 Home-page: https://github.com/rohdelab/PyTransKit
 Author: Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Naqib Sad Pathan, Yan Zhuang, Gustavo Rohde
 Author-email: ar3fx@virginia.edu, xuwangyin@gmail.com, gustavo.rohde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pytranskit-0.2.5/README.md` & `pytranskit-0.2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/TBM/TBM_CLOT.py` & `pytranskit-0.2.5.1/pytranskit/TBM/TBM_CLOT.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/TBM/TBM_PLOT.py` & `pytranskit-0.2.5.1/pytranskit/TBM/TBM_PLOT.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/TBM/TBM_RCDT.py` & `pytranskit-0.2.5.1/pytranskit/TBM/TBM_RCDT.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/TBM/preprocessing.py` & `pytranskit-0.2.5.1/pytranskit/TBM/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/TBM/utils.py` & `pytranskit-0.2.5.1/pytranskit/TBM/utils.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/classification/RSCDT_NS.py` & `pytranskit-0.2.5.1/pytranskit/classification/RSCDT_NS.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 arXiv preprint arXiv:2307.15339.
 """
 
 import numpy as np
 import numpy.linalg as LA
 import multiprocessing as mp
 
-from npytranskit.optrans.continuous.radonscdt import RadonSCDT
+from pytranskit.optrans.continuous.radonscdt import RadonSCDT
 
 eps = 1e-6
 x0_range = [0, 1]
 x_range = [0, 1]
 Rdown = 1  # downsample radon projections (w.r.t. angles)
 theta = np.linspace(0, 176, 45// Rdown)
```

### Comparing `pytranskit-0.2.5/pytranskit/classification/cdt_ns.py` & `pytranskit-0.2.5.1/pytranskit/classification/cdt_ns.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/classification/inv_enc.py` & `pytranskit-0.2.5.1/pytranskit/classification/inv_enc.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/classification/rcdt_ns.py` & `pytranskit-0.2.5.1/pytranskit/classification/rcdt_ns.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/classification/rcdt_ns_3d.py` & `pytranskit-0.2.5.1/pytranskit/classification/rcdt_ns_3d.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/classification/scdt_nls.py` & `pytranskit-0.2.5.1/pytranskit/classification/scdt_nls.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/classification/scdt_ns.py` & `pytranskit-0.2.5.1/pytranskit/classification/scdt_ns.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/classification/utils.py` & `pytranskit-0.2.5.1/pytranskit/classification/utils.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/continuous/base.py` & `pytranskit-0.2.5.1/pytranskit/optrans/continuous/base.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/continuous/cdt.py` & `pytranskit-0.2.5.1/pytranskit/optrans/continuous/cdt.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/continuous/clot.py` & `pytranskit-0.2.5.1/pytranskit/optrans/continuous/clot.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/continuous/radoncdt.py` & `pytranskit-0.2.5.1/pytranskit/optrans/continuous/radoncdt.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/continuous/radoncdt3D.py` & `pytranskit-0.2.5.1/pytranskit/optrans/continuous/radoncdt3D.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/continuous/radonscdt.py` & `pytranskit-0.2.5.1/pytranskit/optrans/continuous/radonscdt.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/continuous/scdt.py` & `pytranskit-0.2.5.1/pytranskit/optrans/continuous/scdt.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,7 +163,19 @@
         if Massneg>0.:
             Ineg = self.itransform(Ineghat)*Massneg
         else:
             Ineg = np.zeros(len(Ineghat))
         return Ipos - Ineg
         #return self.itransform(Ipos)*Masspos-self.itransform(Ineg)*Massneg
 
+    def calc_scdt(self, sig1, t1, s0, t0):
+        # sig1: (0, columns)
+        # t1: domain of sig1
+        
+        scdt = SCDT(reference=s0,x0=t0)
+        Ipos, Ineg, Imasspos, Imassneg = scdt.stransform(sig1, t1)
+        
+        if self.rm_edge:
+            shat = np.concatenate((Ipos[1:-2],Ineg[1:-2]),axis=0)
+        else:
+            shat = np.concatenate((Ipos[:-1],Ineg[:-1]),axis=0)
+        return shat
```

### Comparing `pytranskit-0.2.5/pytranskit/optrans/decomposition/cca.py` & `pytranskit-0.2.5.1/pytranskit/optrans/decomposition/cca.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/decomposition/modes.py` & `pytranskit-0.2.5.1/pytranskit/optrans/decomposition/modes.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/decomposition/plda.py` & `pytranskit-0.2.5.1/pytranskit/optrans/decomposition/plda.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/utils/data_utils.py` & `pytranskit-0.2.5.1/pytranskit/optrans/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/utils/validation.py` & `pytranskit-0.2.5.1/pytranskit/optrans/utils/validation.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/utils/visualize.py` & `pytranskit-0.2.5.1/pytranskit/optrans/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit/optrans/visualization/visualize.py` & `pytranskit-0.2.5.1/pytranskit/optrans/visualization/visualize.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/pytranskit.egg-info/PKG-INFO` & `pytranskit-0.2.5.1/pytranskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytranskit
-Version: 0.2.5
+Version: 0.2.5.1
 Summary: Python transport based signal processing toolkit.
 Home-page: https://github.com/rohdelab/PyTransKit
 Author: Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Naqib Sad Pathan, Yan Zhuang, Gustavo Rohde
 Author-email: ar3fx@virginia.edu, xuwangyin@gmail.com, gustavo.rohde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pytranskit-0.2.5/pytranskit.egg-info/SOURCES.txt` & `pytranskit-0.2.5.1/pytranskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5/setup.py` & `pytranskit-0.2.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description=fh.read()
 
 setuptools.setup(
   name="pytranskit",
-  version="0.2.5",
+  version="0.2.5.1",
   author="Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Naqib Sad Pathan, Yan Zhuang, Gustavo Rohde",
   author_email="ar3fx@virginia.edu, xuwangyin@gmail.com, gustavo.rohde@gmail.com",
   description="Python transport based signal processing toolkit.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/rohdelab/PyTransKit",
   packages=setuptools.find_packages(),
```

