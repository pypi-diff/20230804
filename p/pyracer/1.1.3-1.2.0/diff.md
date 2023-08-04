# Comparing `tmp/pyracer-1.1.3.tar.gz` & `tmp/pyracer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracer-1.1.3.tar", last modified: Sat Jul 22 11:04:07 2023, max compression
+gzip compressed data, was "pyracer-1.2.0.tar", last modified: Fri Aug  4 11:32:48 2023, max compression
```

## Comparing `pyracer-1.1.3.tar` & `pyracer-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:04:07.880756 pyracer-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-22 11:03:57.000000 pyracer-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-22 11:04:07.880756 pyracer-1.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:04:07.880756 pyracer-1.1.3/RACER/
--rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-07-22 11:03:57.000000 pyracer-1.1.3/RACER/RACER.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-22 11:03:57.000000 pyracer-1.1.3/RACER/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-22 11:03:57.000000 pyracer-1.1.3/RACER/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 11:03:57.000000 pyracer-1.1.3/RACER/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-22 11:03:57.000000 pyracer-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 11:04:07.880756 pyracer-1.1.3/pyracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-22 11:04:07.000000 pyracer-1.1.3/pyracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-22 11:04:07.000000 pyracer-1.1.3/pyracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 11:04:07.000000 pyracer-1.1.3/pyracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 11:04:07.000000 pyracer-1.1.3/pyracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-22 11:04:07.000000 pyracer-1.1.3/pyracer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 11:04:07.880756 pyracer-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-22 11:03:57.000000 pyracer-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:32:48.504139 pyracer-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-04 11:32:38.000000 pyracer-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-04 11:32:48.504139 pyracer-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:32:48.500139 pyracer-1.2.0/RACER/
+-rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-08-04 11:32:38.000000 pyracer-1.2.0/RACER/RACER.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 11:32:38.000000 pyracer-1.2.0/RACER/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-08-04 11:32:38.000000 pyracer-1.2.0/RACER/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 11:32:38.000000 pyracer-1.2.0/RACER/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-08-04 11:32:38.000000 pyracer-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:32:48.500139 pyracer-1.2.0/pyracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-04 11:32:48.000000 pyracer-1.2.0/pyracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-04 11:32:48.000000 pyracer-1.2.0/pyracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:32:48.000000 pyracer-1.2.0/pyracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 11:32:48.000000 pyracer-1.2.0/pyracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 11:32:48.000000 pyracer-1.2.0/pyracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 11:32:48.504139 pyracer-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:32:38.000000 pyracer-1.2.0/setup.py
```

### Comparing `pyracer-1.1.3/LICENSE` & `pyracer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracer-1.1.3/PKG-INFO` & `pyracer-1.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.1.3
+Version: 1.2.0
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
 Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyracer-1.1.3/RACER/RACER.py` & `pyracer-1.2.0/RACER/RACER.py`

 * *Files identical despite different names*

### Comparing `pyracer-1.1.3/README.md` & `pyracer-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# RACER
+# PyRACER
 
-Unofficial Python implementation of the RACER classification algorithm described by [Basiri et. al, 2019](https://link.springer.com/article/10.1007/s00521-017-3117-2).
-RACER is designed specifically for discrete datasets and therefore uses the entropy-based MDLP discretization algorithm by [Fayyad and Irani, 1993](http://web.donga.ac.kr/kjunwoo/files/Multi%20interval%20discretization%20of%20continuous%20valued%20attributes%20for%20classification%20learning.pdf) for binary tasks and an [optimal binning strategy](https://arxiv.org/abs/2001.08025) for the multiclass case. The code is also heavily documented for ease of use.
+PyRACER is an unofficial Python implementation of the RACER classification algorithm described by [Basiri et. al, 2019](https://link.springer.com/article/10.1007/s00521-017-3117-2).
+RACER is designed specifically for discrete datasets and therefore uses the entropy-based MDLP discretization algorithm by [Fayyad and Irani, 1993](http://web.donga.ac.kr/kjunwoo/files/Multi%20interval%20discretization%20of%20continuous%20valued%20attributes%20for%20classification%20learning.pdf) for binary tasks and an [optimal binning strategy](https://arxiv.org/abs/2001.08025) for the multiclass case. [The code is also heavily documented for ease of use](https://pyracer.readthedocs.io/en/latest/).
 
 Please consider citing this work if you use it in an academic setting.
 
 [![Documentation Status](https://readthedocs.org/projects/pyracer/badge/?version=latest)](https://pyracer.readthedocs.io/en/latest/?badge=latest) [![DOI](https://zenodo.org/badge/656323287.svg)](https://zenodo.org/badge/latestdoi/656323287)
 
 ## Installation
 [![PyPI version](https://badge.fury.io/py/pyracer.svg)](https://badge.fury.io/py/pyracer)
 ```bash
 $ pip install pyracer
 ```
 
 ## Usage
-RACER is designed to be consistent with Scikit-learn estimator API which makes it very easy to use.
+PyRACER is designed to be consistent with Scikit-learn estimator API which makes it very easy to use.
 
 
 The following example demonstrates the use of RACER on the Zoo dataset. Take a look at [examples](https://github.com/Adversarian/RACER/tree/main/examples) for more use cases.
 ### Data Obtention and Cleaning
 ```python
 from RACER import RACER, RACERPreprocessor
 from sklearn.model_selection import train_test_split
@@ -51,14 +51,16 @@
 
 X = df.drop(columns=['animal_name', 'type']).astype('category')
 Y = df[['type']].astype('category')
 ```
 
 ### RACER Preprocessing Step
 RACER requires a preprocessing step to be performed on the data **prior to** splitting into test and train portions. This step discretizes continous features and then converts each feature into a [dummy encoded](https://datascience.stackexchange.com/questions/98172/what-is-the-difference-between-one-hot-and-dummy-encoding) variable. Note that since different discretization methods are used for multiclass and binary classification tasks you need to either specify the task using the `target` keyword argument or leave it to default to `"auto"` which attempts to infer your task when you call `fit_transform(X,y)` from the number of unique values in `y`.
+
+RACERPreprocessor now also supports separate `fit` and `transform` functions but it is still recommended to use `fit_transform` or perform `fit` on the entire dataset prior to splitting. This ensures that new unseen values are not left out of the transformation at test time.
 ```python
 X, Y = RACERPreprocessor(target="multiclass").fit_transform(X, Y)
 
 X_train, X_test, Y_train, Y_test = train_test_split(X,Y, random_state=1, test_size=0.3)
 ```
 
 ### Fitting RACER on the Dataset
@@ -86,14 +88,15 @@
 	[111001101110101010011110000010101010] --> [0000010] (5) | 0.9535714285714285
 	[101011101011111101111110101000011011] --> [0010000] (2) | 0.9528571428571428
 	[101001101001110101011110001000101010] --> [0000100] (4) | 0.9521428571428571
 	[101001101010101010011010100000101010] --> [0000001] (6) | 0.9507142857142856
 ```
 ## To Do
 - ~Add another example notebook featuring Scikit-learn's built-in datasets.~
+- ~Replace `pandas.get_dummies()` with Scikit-learn's `OneHotEncoder` for better consistency.~
 - Unify discretization algorithms for all tasks.
 - Better docs!
 
 ## Issues and Feature Requests
 Found a problem within the implementation or an inconsistency with the original algorithm? Or maybe you would like to request a feature? Please feel free to [submit a PR](https://github.com/Adversarian/RACER/pulls) or [create a new issue](https://github.com/Adversarian/RACER/issues).
 
 ## Official Paper
```

### Comparing `pyracer-1.1.3/pyracer.egg-info/PKG-INFO` & `pyracer-1.2.0/pyracer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.1.3
+Version: 1.2.0
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
 Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyracer-1.1.3/setup.py` & `pyracer-1.2.0/setup.py`

 * *Files identical despite different names*

