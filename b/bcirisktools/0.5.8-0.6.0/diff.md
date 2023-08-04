# Comparing `tmp/bcirisktools-0.5.8.tar.gz` & `tmp/bcirisktools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcirisktools-0.5.8.tar", last modified: Fri Aug  4 17:16:38 2023, max compression
+gzip compressed data, was "bcirisktools-0.6.0.tar", last modified: Fri Aug  4 17:20:13 2023, max compression
```

## Comparing `bcirisktools-0.5.8.tar` & `bcirisktools-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 17:16:38.185000 bcirisktools-0.5.8/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-08-04 16:27:43.000000 bcirisktools-0.5.8/LICENCE
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-04 17:16:38.179000 bcirisktools-0.5.8/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-08-04 16:27:43.000000 bcirisktools-0.5.8/README.md
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 17:16:38.069000 bcirisktools-0.5.8/bcirisktools/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      385 2023-08-04 16:27:43.000000 bcirisktools-0.5.8/bcirisktools/__init__.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-08-04 16:27:43.000000 bcirisktools-0.5.8/bcirisktools/input_filters.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-08-04 16:27:43.000000 bcirisktools-0.5.8/bcirisktools/metrics_bci.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-08-04 16:27:43.000000 bcirisktools-0.5.8/bcirisktools/modeling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    19201 2023-08-04 17:16:09.000000 bcirisktools-0.5.8/bcirisktools/profiling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-08-04 16:27:43.000000 bcirisktools-0.5.8/bcirisktools/shapley_report.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-08-04 16:27:43.000000 bcirisktools-0.5.8/bcirisktools/stability.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-08-04 16:27:43.000000 bcirisktools-0.5.8/bcirisktools/tree_crt.py
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 17:16:38.157000 bcirisktools-0.5.8/bcirisktools.egg-info/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-04 17:16:37.000000 bcirisktools-0.5.8/bcirisktools.egg-info/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-04 17:16:37.000000 bcirisktools-0.5.8/bcirisktools.egg-info/SOURCES.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-04 17:16:37.000000 bcirisktools-0.5.8/bcirisktools.egg-info/dependency_links.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       63 2023-08-04 17:16:37.000000 bcirisktools-0.5.8/bcirisktools.egg-info/requires.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-04 17:16:37.000000 bcirisktools-0.5.8/bcirisktools.egg-info/top_level.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-08-04 16:27:43.000000 bcirisktools-0.5.8/pyproject.toml
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-04 17:16:38.196000 bcirisktools-0.5.8/setup.cfg
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1019 2023-08-04 17:16:30.000000 bcirisktools-0.5.8/setup.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 17:20:13.397000 bcirisktools-0.6.0/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-08-04 16:27:43.000000 bcirisktools-0.6.0/LICENCE
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-04 17:20:13.391000 bcirisktools-0.6.0/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-08-04 16:27:43.000000 bcirisktools-0.6.0/README.md
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 17:20:13.275000 bcirisktools-0.6.0/bcirisktools/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      385 2023-08-04 16:27:43.000000 bcirisktools-0.6.0/bcirisktools/__init__.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-08-04 16:27:43.000000 bcirisktools-0.6.0/bcirisktools/input_filters.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-08-04 16:27:43.000000 bcirisktools-0.6.0/bcirisktools/metrics_bci.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-08-04 16:27:43.000000 bcirisktools-0.6.0/bcirisktools/modeling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    19391 2023-08-04 17:20:02.000000 bcirisktools-0.6.0/bcirisktools/profiling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-08-04 16:27:43.000000 bcirisktools-0.6.0/bcirisktools/shapley_report.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-08-04 16:27:43.000000 bcirisktools-0.6.0/bcirisktools/stability.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-08-04 16:27:43.000000 bcirisktools-0.6.0/bcirisktools/tree_crt.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-04 17:20:13.366000 bcirisktools-0.6.0/bcirisktools.egg-info/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      573 2023-08-04 17:20:12.000000 bcirisktools-0.6.0/bcirisktools.egg-info/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-04 17:20:12.000000 bcirisktools-0.6.0/bcirisktools.egg-info/SOURCES.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-04 17:20:12.000000 bcirisktools-0.6.0/bcirisktools.egg-info/dependency_links.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       63 2023-08-04 17:20:12.000000 bcirisktools-0.6.0/bcirisktools.egg-info/requires.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-04 17:20:12.000000 bcirisktools-0.6.0/bcirisktools.egg-info/top_level.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-08-04 16:27:43.000000 bcirisktools-0.6.0/pyproject.toml
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-04 17:20:13.400000 bcirisktools-0.6.0/setup.cfg
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1019 2023-08-04 17:20:08.000000 bcirisktools-0.6.0/setup.py
```

### Comparing `bcirisktools-0.5.8/LICENCE` & `bcirisktools-0.6.0/LICENCE`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.8/PKG-INFO` & `bcirisktools-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.5.8
+Version: 0.6.0
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.5.8/README.md` & `bcirisktools-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.8/bcirisktools/input_filters.py` & `bcirisktools-0.6.0/bcirisktools/input_filters.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.8/bcirisktools/metrics_bci.py` & `bcirisktools-0.6.0/bcirisktools/metrics_bci.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.8/bcirisktools/modeling.py` & `bcirisktools-0.6.0/bcirisktools/modeling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.8/bcirisktools/profiling.py` & `bcirisktools-0.6.0/bcirisktools/profiling.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,16 @@
     br_i = df.iloc[idx]["BadRate %"]
     br_next = df.iloc[idx + 1]["BadRate %"] if idx + 1 <= df.shape[0] else -1
     br_previous = df.iloc[idx - 1]["BadRate %"] if idx != 0 else -1
     return br_i, br_next, br_previous
 
 
 def plot_steps(df, x, y):
+    image_url = "https://bitbucket.org/imezade/bcirisktools/raw/cddb3e4b99cf89c8792c2d5027b4525003532628/bcirisktools/bci_logo.png"
+    urllib.request.urlretrieve(image_url, "bci_logo.png")
     bci_logo = Image.open("bci_logo.png")
 
     fig = px.bar(
         df.astype({x: str}),
         x=x,
         y=y,
         animation_frame="step",
```

### Comparing `bcirisktools-0.5.8/bcirisktools/shapley_report.py` & `bcirisktools-0.6.0/bcirisktools/shapley_report.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.8/bcirisktools/stability.py` & `bcirisktools-0.6.0/bcirisktools/stability.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.8/bcirisktools/tree_crt.py` & `bcirisktools-0.6.0/bcirisktools/tree_crt.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.5.8/bcirisktools.egg-info/PKG-INFO` & `bcirisktools-0.6.0/bcirisktools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.5.8
+Version: 0.6.0
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.5.8/setup.py` & `bcirisktools-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.5.8"
+VERSION = "0.6.0"
 DESCRIPTION = "BCI risks tools"
 LONG_DESCRIPTION = "A package that compiles different risk tools used by BCI bank."
 
 # Setting up
 setup(
     name="bcirisktools",
     version=VERSION,
```

