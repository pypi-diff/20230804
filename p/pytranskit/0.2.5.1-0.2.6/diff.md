# Comparing `tmp/pytranskit-0.2.5.1.tar.gz` & `tmp/pytranskit-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytranskit-0.2.5.1.tar", last modified: Fri Aug  4 04:29:06 2023, max compression
+gzip compressed data, was "pytranskit-0.2.6.tar", last modified: Fri Aug  4 04:35:52 2023, max compression
```

## Comparing `pytranskit-0.2.5.1.tar` & `pytranskit-0.2.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.447311 pytranskit-0.2.5.1/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    35147 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/LICENSE
--rw-r--r--   0 qpb3vt     (504) staff       (20)     9668 2023-08-04 04:29:06.447587 pytranskit-0.2.5.1/PKG-INFO
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     8732 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/README.md
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.157827 pytranskit-0.2.5.1/pytranskit/
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.225397 pytranskit-0.2.5.1/pytranskit/TBM/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    33100 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/TBM_CLOT.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    38729 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/TBM_PLOT.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    31009 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/TBM_RCDT.py
--rw-rw-r--   0 qpb3vt     (504) staff       (20)        0 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     6534 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/preprocessing.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4144 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/TBM/utils.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)       69 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/__init__.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.299356 pytranskit-0.2.5.1/pytranskit/classification/
--rw-rw-r--   0 qpb3vt     (504) staff       (20)     5955 2023-08-04 03:43:11.000000 pytranskit-0.2.5.1/pytranskit/classification/RSCDT_NS.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5229 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/cdt_ns.py
--rw-rw-r--   0 qpb3vt     (504) staff       (20)     9452 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/inv_enc.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5925 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/rcdt_ns.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5995 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/rcdt_ns_3d.py
--rw-rw-r--   0 qpb3vt     (504) staff       (20)    12854 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/scdt_nls.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5458 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/scdt_ns.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    10191 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/classification/utils.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.307126 pytranskit-0.2.5.1/pytranskit/optrans/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)       45 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/__init__.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.365610 pytranskit-0.2.5.1/pytranskit/optrans/continuous/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)      192 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4254 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/base.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     6127 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/cdt.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    11074 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/clot.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     7934 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/radoncdt.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     8936 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/radoncdt3D.py
--rw-rw-r--   0 qpb3vt     (504) staff       (20)     4149 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/radonscdt.py
--rw-rw-r--   0 qpb3vt     (504) staff       (20)     5948 2023-08-04 03:50:12.000000 pytranskit-0.2.5.1/pytranskit/optrans/continuous/scdt.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.399451 pytranskit-0.2.5.1/pytranskit/optrans/decomposition/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)      206 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/decomposition/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     9281 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/decomposition/cca.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     3976 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/decomposition/modes.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    14626 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/decomposition/plda.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.427768 pytranskit-0.2.5.1/pytranskit/optrans/utils/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)      362 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/utils/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4822 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/utils/data_utils.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4541 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/utils/validation.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     2408 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/utils/visualize.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.446055 pytranskit-0.2.5.1/pytranskit/optrans/visualization/
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)      275 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/visualization/__init__.py
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)    14276 2023-08-04 02:59:31.000000 pytranskit-0.2.5.1/pytranskit/optrans/visualization/visualize.py
-drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:29:06.174713 pytranskit-0.2.5.1/pytranskit.egg-info/
--rw-r--r--   0 qpb3vt     (504) staff       (20)     9668 2023-08-04 04:29:06.000000 pytranskit-0.2.5.1/pytranskit.egg-info/PKG-INFO
--rw-r--r--   0 qpb3vt     (504) staff       (20)     1460 2023-08-04 04:29:06.000000 pytranskit-0.2.5.1/pytranskit.egg-info/SOURCES.txt
--rw-r--r--   0 qpb3vt     (504) staff       (20)        1 2023-08-04 04:29:06.000000 pytranskit-0.2.5.1/pytranskit.egg-info/dependency_links.txt
--rw-r--r--   0 qpb3vt     (504) staff       (20)       11 2023-08-04 04:29:06.000000 pytranskit-0.2.5.1/pytranskit.egg-info/top_level.txt
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)       79 2023-08-04 04:29:06.453579 pytranskit-0.2.5.1/setup.cfg
--rwxr-xr-x   0 qpb3vt     (504) staff       (20)     1086 2023-08-04 04:28:37.000000 pytranskit-0.2.5.1/setup.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:35:52.512830 pytranskit-0.2.6/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    35147 2023-08-04 02:59:31.000000 pytranskit-0.2.6/LICENSE
+-rw-r--r--   0 qpb3vt     (504) staff       (20)     9666 2023-08-04 04:35:52.513226 pytranskit-0.2.6/PKG-INFO
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     8732 2023-08-04 02:59:31.000000 pytranskit-0.2.6/README.md
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:35:52.410868 pytranskit-0.2.6/pytranskit/
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:35:52.450926 pytranskit-0.2.6/pytranskit/TBM/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    33100 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/TBM/TBM_CLOT.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    38729 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/TBM/TBM_PLOT.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    31009 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/TBM/TBM_RCDT.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)        0 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/TBM/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     6534 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/TBM/preprocessing.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4144 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/TBM/utils.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)       69 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/__init__.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:35:52.466578 pytranskit-0.2.6/pytranskit/classification/
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     5955 2023-08-04 03:43:11.000000 pytranskit-0.2.6/pytranskit/classification/RSCDT_NS.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/classification/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5229 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/classification/cdt_ns.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     9452 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/classification/inv_enc.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5925 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/classification/rcdt_ns.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5995 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/classification/rcdt_ns_3d.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)    12854 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/classification/scdt_nls.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     5458 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/classification/scdt_ns.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    10191 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/classification/utils.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:35:52.469742 pytranskit-0.2.6/pytranskit/optrans/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)       45 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/__init__.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:35:52.490384 pytranskit-0.2.6/pytranskit/optrans/continuous/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      192 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/continuous/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4254 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/continuous/base.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     6127 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/continuous/cdt.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    11074 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/continuous/clot.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     7934 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/continuous/radoncdt.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     8936 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/continuous/radoncdt3D.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     4149 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/continuous/radonscdt.py
+-rw-rw-r--   0 qpb3vt     (504) staff       (20)     5948 2023-08-04 03:50:12.000000 pytranskit-0.2.6/pytranskit/optrans/continuous/scdt.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:35:52.499630 pytranskit-0.2.6/pytranskit/optrans/decomposition/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      206 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/decomposition/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     9281 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/decomposition/cca.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     3976 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/decomposition/modes.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    14626 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/decomposition/plda.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:35:52.507557 pytranskit-0.2.6/pytranskit/optrans/utils/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      362 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/utils/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4822 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/utils/data_utils.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     4541 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/utils/validation.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     2408 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/utils/visualize.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:35:52.511427 pytranskit-0.2.6/pytranskit/optrans/visualization/
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)      275 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/visualization/__init__.py
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)    14276 2023-08-04 02:59:31.000000 pytranskit-0.2.6/pytranskit/optrans/visualization/visualize.py
+drwxr-xr-x   0 qpb3vt     (504) staff       (20)        0 2023-08-04 04:35:52.434083 pytranskit-0.2.6/pytranskit.egg-info/
+-rw-r--r--   0 qpb3vt     (504) staff       (20)     9666 2023-08-04 04:35:52.000000 pytranskit-0.2.6/pytranskit.egg-info/PKG-INFO
+-rw-r--r--   0 qpb3vt     (504) staff       (20)     1460 2023-08-04 04:35:52.000000 pytranskit-0.2.6/pytranskit.egg-info/SOURCES.txt
+-rw-r--r--   0 qpb3vt     (504) staff       (20)        1 2023-08-04 04:35:52.000000 pytranskit-0.2.6/pytranskit.egg-info/dependency_links.txt
+-rw-r--r--   0 qpb3vt     (504) staff       (20)       11 2023-08-04 04:35:52.000000 pytranskit-0.2.6/pytranskit.egg-info/top_level.txt
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)       79 2023-08-04 04:35:52.518504 pytranskit-0.2.6/setup.cfg
+-rwxr-xr-x   0 qpb3vt     (504) staff       (20)     1084 2023-08-04 04:35:22.000000 pytranskit-0.2.6/setup.py
```

### Comparing `pytranskit-0.2.5.1/LICENSE` & `pytranskit-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/PKG-INFO` & `pytranskit-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytranskit
-Version: 0.2.5.1
+Version: 0.2.6
 Summary: Python transport based signal processing toolkit.
 Home-page: https://github.com/rohdelab/PyTransKit
 Author: Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Naqib Sad Pathan, Yan Zhuang, Gustavo Rohde
 Author-email: ar3fx@virginia.edu, xuwangyin@gmail.com, gustavo.rohde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pytranskit-0.2.5.1/README.md` & `pytranskit-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/TBM/TBM_CLOT.py` & `pytranskit-0.2.6/pytranskit/TBM/TBM_CLOT.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/TBM/TBM_PLOT.py` & `pytranskit-0.2.6/pytranskit/TBM/TBM_PLOT.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/TBM/TBM_RCDT.py` & `pytranskit-0.2.6/pytranskit/TBM/TBM_RCDT.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/TBM/preprocessing.py` & `pytranskit-0.2.6/pytranskit/TBM/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/TBM/utils.py` & `pytranskit-0.2.6/pytranskit/TBM/utils.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/classification/RSCDT_NS.py` & `pytranskit-0.2.6/pytranskit/classification/RSCDT_NS.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/classification/cdt_ns.py` & `pytranskit-0.2.6/pytranskit/classification/cdt_ns.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/classification/inv_enc.py` & `pytranskit-0.2.6/pytranskit/classification/inv_enc.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/classification/rcdt_ns.py` & `pytranskit-0.2.6/pytranskit/classification/rcdt_ns.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/classification/rcdt_ns_3d.py` & `pytranskit-0.2.6/pytranskit/classification/rcdt_ns_3d.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/classification/scdt_nls.py` & `pytranskit-0.2.6/pytranskit/classification/scdt_nls.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/classification/scdt_ns.py` & `pytranskit-0.2.6/pytranskit/classification/scdt_ns.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/classification/utils.py` & `pytranskit-0.2.6/pytranskit/classification/utils.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/continuous/base.py` & `pytranskit-0.2.6/pytranskit/optrans/continuous/base.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/continuous/cdt.py` & `pytranskit-0.2.6/pytranskit/optrans/continuous/cdt.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/continuous/clot.py` & `pytranskit-0.2.6/pytranskit/optrans/continuous/clot.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/continuous/radoncdt.py` & `pytranskit-0.2.6/pytranskit/optrans/continuous/radoncdt.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/continuous/radoncdt3D.py` & `pytranskit-0.2.6/pytranskit/optrans/continuous/radoncdt3D.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/continuous/radonscdt.py` & `pytranskit-0.2.6/pytranskit/optrans/continuous/radonscdt.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/continuous/scdt.py` & `pytranskit-0.2.6/pytranskit/optrans/continuous/scdt.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/decomposition/cca.py` & `pytranskit-0.2.6/pytranskit/optrans/decomposition/cca.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/decomposition/modes.py` & `pytranskit-0.2.6/pytranskit/optrans/decomposition/modes.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/decomposition/plda.py` & `pytranskit-0.2.6/pytranskit/optrans/decomposition/plda.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/utils/data_utils.py` & `pytranskit-0.2.6/pytranskit/optrans/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/utils/validation.py` & `pytranskit-0.2.6/pytranskit/optrans/utils/validation.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/utils/visualize.py` & `pytranskit-0.2.6/pytranskit/optrans/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit/optrans/visualization/visualize.py` & `pytranskit-0.2.6/pytranskit/optrans/visualization/visualize.py`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/pytranskit.egg-info/PKG-INFO` & `pytranskit-0.2.6/pytranskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytranskit
-Version: 0.2.5.1
+Version: 0.2.6
 Summary: Python transport based signal processing toolkit.
 Home-page: https://github.com/rohdelab/PyTransKit
 Author: Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Naqib Sad Pathan, Yan Zhuang, Gustavo Rohde
 Author-email: ar3fx@virginia.edu, xuwangyin@gmail.com, gustavo.rohde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pytranskit-0.2.5.1/pytranskit.egg-info/SOURCES.txt` & `pytranskit-0.2.6/pytranskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytranskit-0.2.5.1/setup.py` & `pytranskit-0.2.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description=fh.read()
 
 setuptools.setup(
   name="pytranskit",
-  version="0.2.5.1",
+  version="0.2.6",
   author="Abu Hasnat Mohammad Rubaiyat, Xuwang Yin, Liam Cattell, Soheil Kolouri, Mohammad Shifat-E-Rabbi, Naqib Sad Pathan, Yan Zhuang, Gustavo Rohde",
   author_email="ar3fx@virginia.edu, xuwangyin@gmail.com, gustavo.rohde@gmail.com",
   description="Python transport based signal processing toolkit.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/rohdelab/PyTransKit",
   packages=setuptools.find_packages(),
```

