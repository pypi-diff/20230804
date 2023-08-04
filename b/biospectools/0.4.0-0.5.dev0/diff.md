# Comparing `tmp/biospectools-0.4.0.tar.gz` & `tmp/biospectools-0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biospectools-0.4.0.tar", last modified: Thu Feb  2 15:36:55 2023, max compression
+gzip compressed data, was "biospectools-0.5.dev0.tar", last modified: Fri Aug  4 17:13:53 2023, max compression
```

## Comparing `biospectools-0.4.0.tar` & `biospectools-0.5.dev0.tar`

### file list

```diff
@@ -1,34 +1,43 @@
-drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-02-02 15:36:55.261776 biospectools-0.4.0/
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      384 2023-02-02 15:36:55.261776 biospectools-0.4.0/PKG-INFO
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      885 2022-06-02 21:41:46.000000 biospectools-0.4.0/README.md
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      182 2022-06-02 21:41:46.000000 biospectools-0.4.0/pyproject.toml
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      899 2023-02-02 15:36:55.261776 biospectools-0.4.0/setup.cfg
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)       69 2022-06-02 21:41:46.000000 biospectools-0.4.0/setup.py
-drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-02-02 15:36:55.257776 biospectools-0.4.0/src/
-drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-02-02 15:36:55.257776 biospectools-0.4.0/src/biospectools/
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      128 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/__init__.py
-drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-02-02 15:36:55.257776 biospectools-0.4.0/src/biospectools/models/
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)       44 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/models/__init__.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    34460 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/models/_pls.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    14734 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/models/sparse_pls.py
-drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-02-02 15:36:55.261776 biospectools-0.4.0/src/biospectools/preprocessing/
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      365 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/preprocessing/__init__.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     2399 2022-06-02 21:41:46.000000 biospectools-0.4.0/src/biospectools/preprocessing/criterions.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    11496 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/preprocessing/dsae.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    14550 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/preprocessing/emsc.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    10909 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/preprocessing/fringe_emsc.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     9726 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/preprocessing/me_emsc.py
-drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-02-02 15:36:55.261776 biospectools-0.4.0/src/biospectools/private/
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      499 2022-06-02 21:41:46.000000 biospectools-0.4.0/src/biospectools/private/__init__.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)        0 2022-06-02 21:41:46.000000 biospectools-0.4.0/src/biospectools/py.typed
-drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-02-02 15:36:55.261776 biospectools-0.4.0/src/biospectools/utils/
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)       36 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/utils/__init__.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      825 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/utils/deprecated.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     2619 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/utils/downloads.py
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     3130 2023-02-02 15:18:03.000000 biospectools-0.4.0/src/biospectools/utils/interpolate.py
-drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-02-02 15:36:55.257776 biospectools-0.4.0/src/biospectools.egg-info/
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      384 2023-02-02 15:36:55.000000 biospectools-0.4.0/src/biospectools.egg-info/PKG-INFO
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      840 2023-02-02 15:36:55.000000 biospectools-0.4.0/src/biospectools.egg-info/SOURCES.txt
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)        1 2023-02-02 15:36:55.000000 biospectools-0.4.0/src/biospectools.egg-info/dependency_links.txt
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      213 2023-02-02 15:36:55.000000 biospectools-0.4.0/src/biospectools.egg-info/requires.txt
--rw-rw-r--   0 pisarik   (1000) pisarik   (1000)       13 2023-02-02 15:36:55.000000 biospectools-0.4.0/src/biospectools.egg-info/top_level.txt
+drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-08-04 17:13:53.022116 biospectools-0.5.dev0/
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      387 2023-08-04 17:13:53.022116 biospectools-0.5.dev0/PKG-INFO
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      885 2022-06-02 21:41:46.000000 biospectools-0.5.dev0/README.md
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      182 2022-06-02 21:41:46.000000 biospectools-0.5.dev0/pyproject.toml
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      902 2023-08-04 17:13:53.022116 biospectools-0.5.dev0/setup.cfg
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)       69 2022-06-02 21:41:46.000000 biospectools-0.5.dev0/setup.py
+drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-08-04 17:13:53.018116 biospectools-0.5.dev0/src/
+drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-08-04 17:13:53.018116 biospectools-0.5.dev0/src/biospectools/
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      128 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/__init__.py
+drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-08-04 17:13:53.022116 biospectools-0.5.dev0/src/biospectools/jupyter/
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)       78 2023-08-04 17:03:28.000000 biospectools-0.5.dev0/src/biospectools/jupyter/__init__.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    12447 2023-08-04 17:04:00.000000 biospectools-0.5.dev0/src/biospectools/jupyter/hyperspectral_image_viewers.py
+drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-08-04 17:13:53.022116 biospectools-0.5.dev0/src/biospectools/models/
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)       44 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/models/__init__.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    34460 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/models/_pls.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    14734 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/models/sparse_pls.py
+drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-08-04 17:13:53.022116 biospectools-0.5.dev0/src/biospectools/preprocessing/
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      365 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/preprocessing/__init__.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     2399 2022-06-02 21:41:46.000000 biospectools-0.5.dev0/src/biospectools/preprocessing/criterions.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    11496 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/preprocessing/dsae.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    14550 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/preprocessing/emsc.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    10909 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/preprocessing/fringe_emsc.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     9726 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/preprocessing/me_emsc.py
+drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-08-04 17:13:53.022116 biospectools-0.5.dev0/src/biospectools/private/
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      499 2022-06-02 21:41:46.000000 biospectools-0.5.dev0/src/biospectools/private/__init__.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)        0 2022-06-02 21:41:46.000000 biospectools-0.5.dev0/src/biospectools/py.typed
+drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-08-04 17:13:53.022116 biospectools-0.5.dev0/src/biospectools/utils/
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)       36 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/utils/__init__.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      825 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/utils/deprecated.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     2619 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/utils/downloads.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     3130 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/src/biospectools/utils/interpolate.py
+drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-08-04 17:13:53.022116 biospectools-0.5.dev0/src/biospectools.egg-info/
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      387 2023-08-04 17:13:53.000000 biospectools-0.5.dev0/src/biospectools.egg-info/PKG-INFO
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     1044 2023-08-04 17:13:53.000000 biospectools-0.5.dev0/src/biospectools.egg-info/SOURCES.txt
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)        1 2023-08-04 17:13:53.000000 biospectools-0.5.dev0/src/biospectools.egg-info/dependency_links.txt
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)      213 2023-08-04 17:13:53.000000 biospectools-0.5.dev0/src/biospectools.egg-info/requires.txt
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)       13 2023-08-04 17:13:53.000000 biospectools-0.5.dev0/src/biospectools.egg-info/top_level.txt
+drwxrwxr-x   0 pisarik   (1000) pisarik   (1000)        0 2023-08-04 17:13:53.022116 biospectools-0.5.dev0/tests/
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     1796 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/tests/test_dsae.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    13982 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/tests/test_emsc.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     4103 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/tests/test_fringe_emsc.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)    10564 2023-02-02 15:18:03.000000 biospectools-0.5.dev0/tests/test_me_emsc.py
+-rw-rw-r--   0 pisarik   (1000) pisarik   (1000)     1183 2022-06-02 21:41:46.000000 biospectools-0.5.dev0/tests/test_sparse_pls.py
```

### Comparing `biospectools-0.4.0/README.md` & `biospectools-0.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `biospectools-0.4.0/setup.cfg` & `biospectools-0.5.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = biospectools
-version = 0.4.0
+version = 0.5.dev0
 author = BioSpecNorway Group
 description = Python tools for processing spectral data
 url = https://github.com/BioSpecNorway/biospectools
 project_urls = 
 	BiospecNorway Group = https://www.nmbu.no/en/faculty/realtek/research/groups/biospectroscopy
 
 [options]
```

### Comparing `biospectools-0.4.0/src/biospectools/models/_pls.py` & `biospectools-0.5.dev0/src/biospectools/models/_pls.py`

 * *Files identical despite different names*

### Comparing `biospectools-0.4.0/src/biospectools/models/sparse_pls.py` & `biospectools-0.5.dev0/src/biospectools/models/sparse_pls.py`

 * *Files identical despite different names*

### Comparing `biospectools-0.4.0/src/biospectools/preprocessing/criterions.py` & `biospectools-0.5.dev0/src/biospectools/preprocessing/criterions.py`

 * *Files identical despite different names*

### Comparing `biospectools-0.4.0/src/biospectools/preprocessing/dsae.py` & `biospectools-0.5.dev0/src/biospectools/preprocessing/dsae.py`

 * *Files identical despite different names*

### Comparing `biospectools-0.4.0/src/biospectools/preprocessing/emsc.py` & `biospectools-0.5.dev0/src/biospectools/preprocessing/emsc.py`

 * *Files identical despite different names*

### Comparing `biospectools-0.4.0/src/biospectools/preprocessing/fringe_emsc.py` & `biospectools-0.5.dev0/src/biospectools/preprocessing/fringe_emsc.py`

 * *Files identical despite different names*

### Comparing `biospectools-0.4.0/src/biospectools/preprocessing/me_emsc.py` & `biospectools-0.5.dev0/src/biospectools/preprocessing/me_emsc.py`

 * *Files identical despite different names*

### Comparing `biospectools-0.4.0/src/biospectools/utils/deprecated.py` & `biospectools-0.5.dev0/src/biospectools/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `biospectools-0.4.0/src/biospectools/utils/downloads.py` & `biospectools-0.5.dev0/src/biospectools/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `biospectools-0.4.0/src/biospectools/utils/interpolate.py` & `biospectools-0.5.dev0/src/biospectools/utils/interpolate.py`

 * *Files identical despite different names*

