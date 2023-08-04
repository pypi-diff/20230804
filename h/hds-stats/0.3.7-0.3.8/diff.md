# Comparing `tmp/hds-stats-0.3.7.tar.gz` & `tmp/hds-stats-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hds-stats-0.3.7.tar", last modified: Sun Jul 30 00:56:23 2023, max compression
+gzip compressed data, was "hds-stats-0.3.8.tar", last modified: Fri Aug  4 13:48:39 2023, max compression
```

## Comparing `hds-stats-0.3.7.tar` & `hds-stats-0.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-30 00:56:23.396137 hds-stats-0.3.7/
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.7/LICENSE
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-30 00:56:23.395888 hds-stats-0.3.7/PKG-INFO
--rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.7/README.md
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-30 00:56:23.393886 hds-stats-0.3.7/hds_stats/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.7/hds_stats/__init__.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     9519 2023-07-10 06:49:34.000000 hds-stats-0.3.7/hds_stats/ml.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    11856 2023-07-10 06:45:02.000000 hds-stats-0.3.7/hds_stats/plot.py
--rw-r--r--   0 hdsceokevin   (501) staff       (20)    27257 2023-07-30 00:55:30.000000 hds-stats-0.3.7/hds_stats/stat.py
-drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-07-30 00:56:23.395483 hds-stats-0.3.7/hds_stats.egg-info/
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-07-30 00:56:23.000000 hds-stats-0.3.7/hds_stats.egg-info/PKG-INFO
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-07-30 00:56:23.000000 hds-stats-0.3.7/hds_stats.egg-info/SOURCES.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-07-30 00:56:23.000000 hds-stats-0.3.7/hds_stats.egg-info/dependency_links.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-07-30 00:56:23.000000 hds-stats-0.3.7/hds_stats.egg-info/requires.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-07-30 00:56:23.000000 hds-stats-0.3.7/hds_stats.egg-info/top_level.txt
--rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.7/pyproject.toml
--rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-07-30 00:56:23.396231 hds-stats-0.3.7/setup.cfg
--rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-07-30 00:55:46.000000 hds-stats-0.3.7/setup.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-08-04 13:48:39.488951 hds-stats-0.3.8/
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)     1073 2023-04-09 06:26:23.000000 hds-stats-0.3.8/LICENSE
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-08-04 13:48:39.488693 hds-stats-0.3.8/PKG-INFO
+-rw-rw-r--   0 hdsceokevin   (501) staff       (20)       65 2023-04-09 06:26:23.000000 hds-stats-0.3.8/README.md
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-08-04 13:48:39.486526 hds-stats-0.3.8/hds_stats/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      113 2023-07-10 06:13:09.000000 hds-stats-0.3.8/hds_stats/__init__.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     9519 2023-07-10 06:49:34.000000 hds-stats-0.3.8/hds_stats/ml.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    11856 2023-07-10 06:45:02.000000 hds-stats-0.3.8/hds_stats/plot.py
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)    27275 2023-08-04 13:47:41.000000 hds-stats-0.3.8/hds_stats/stat.py
+drwxr-xr-x   0 hdsceokevin   (501) staff       (20)        0 2023-08-04 13:48:39.488285 hds-stats-0.3.8/hds_stats.egg-info/
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      632 2023-08-04 13:48:39.000000 hds-stats-0.3.8/hds_stats.egg-info/PKG-INFO
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      279 2023-08-04 13:48:39.000000 hds-stats-0.3.8/hds_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)        1 2023-08-04 13:48:39.000000 hds-stats-0.3.8/hds_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       72 2023-08-04 13:48:39.000000 hds-stats-0.3.8/hds_stats.egg-info/requires.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       20 2023-08-04 13:48:39.000000 hds-stats-0.3.8/hds_stats.egg-info/top_level.txt
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)      104 2023-04-03 08:08:53.000000 hds-stats-0.3.8/pyproject.toml
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)       38 2023-08-04 13:48:39.489041 hds-stats-0.3.8/setup.cfg
+-rw-r--r--   0 hdsceokevin   (501) staff       (20)     1199 2023-08-04 13:47:53.000000 hds-stats-0.3.8/setup.py
```

### Comparing `hds-stats-0.3.7/LICENSE` & `hds-stats-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.7/PKG-INFO` & `hds-stats-0.3.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.7
+Version: 0.3.8
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.7/hds_stats/ml.py` & `hds-stats-0.3.8/hds_stats/ml.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.7/hds_stats/plot.py` & `hds-stats-0.3.8/hds_stats/plot.py`

 * *Files identical despite different names*

### Comparing `hds-stats-0.3.7/hds_stats/stat.py` & `hds-stats-0.3.8/hds_stats/stat.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     import numpy as np
     import pandas as pd
     import statsmodels.formula.api as smf
     
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     
-    Xvars = set(X.columns)
+    Xvars = list(set(X.columns))
     dat = pd.concat(objs = [X, y], axis = 1)
     
     formula = f'{y.name} ~ 1'
     curr_aic = smf.ols(formula = formula, data = dat).fit().aic
     
     selected = []
     while Xvars:
@@ -85,15 +85,15 @@
     import numpy as np
     import pandas as pd
     import statsmodels.formula.api as smf
     
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     
-    Xvars = set(X.columns)
+    Xvars = list(set(X.columns))
     dat = pd.concat(objs = [X, y], axis = 1)
     
     formula = f'{y.name} ~ {" + ".join(list(Xvars))}'
     curr_aic = smf.ols(formula = formula, data = dat).fit().aic
     
     selected = []
     while Xvars:
@@ -141,15 +141,15 @@
     import numpy as np
     import pandas as pd
     import statsmodels.formula.api as smf
     
     if 'const' in X.columns:
         X = X.drop(labels = ['const'], axis = 1)
     
-    Xvars = set(X.columns)
+    Xvars = list(set(X.columns))
     dat = pd.concat(objs = [X, y], axis = 1)
     
     formula = f'{y.name} ~ 1'
     curr_aic = smf.ols(formula = formula, data = dat).fit().aic
     
     selected = []
     while Xvars:
```

### Comparing `hds-stats-0.3.7/hds_stats.egg-info/PKG-INFO` & `hds-stats-0.3.8/hds_stats.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hds-stats
-Version: 0.3.7
+Version: 0.3.8
 Summary: Useful functions for Statistics and Machine Learning
 Home-page: https://github.com/HelloDataScience/hds-stats
 Author: HelloDataScience
 Author-email: hellodatasciencekorea@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/HelloDataScience/hds-stats/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hds-stats-0.3.7/setup.py` & `hds-stats-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages
 
 with open(file = 'README.md', mode = 'r', encoding = 'UTF-8') as file:
     long_description = file.read()
 
 setup(
     name = 'hds-stats',
-    version = '0.3.7',
+    version = '0.3.8',
     author = 'HelloDataScience',
     author_email = 'hellodatasciencekorea@gmail.com',
     
     description = 'Useful functions for Statistics and Machine Learning',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
```

