# Comparing `tmp/lightgbm_embedding-0.1.1.tar.gz` & `tmp/lightgbm_embedding-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightgbm_embedding-0.1.1.tar", max compression
+gzip compressed data, was "lightgbm_embedding-0.1.2.tar", max compression
```

## Comparing `lightgbm_embedding-0.1.1.tar` & `lightgbm_embedding-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2022-04-24 22:52:19.040077 lightgbm_embedding-0.1.1/LICENSE
--rw-r--r--   0        0        0     6561 2022-04-30 23:06:13.031145 lightgbm_embedding-0.1.1/lightgbm_embedding/__init__.py
--rw-r--r--   0        0        0      811 2022-04-30 23:06:06.077520 lightgbm_embedding-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      791 2022-04-25 13:52:47.989252 lightgbm_embedding-0.1.1/README.md
--rw-r--r--   0        0        0     1502 2022-04-30 23:07:34.430810 lightgbm_embedding-0.1.1/setup.py
--rw-r--r--   0        0        0     1525 2022-04-30 23:07:34.430810 lightgbm_embedding-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-08-04 12:52:05.856084 lightgbm_embedding-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6559 2023-08-04 13:21:34.476309 lightgbm_embedding-0.1.2/lightgbm_embedding/__init__.py
+-rw-r--r--   0        0        0      897 2023-08-04 13:46:17.555229 lightgbm_embedding-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      791 2023-08-04 12:52:05.856084 lightgbm_embedding-0.1.2/README.md
+-rw-r--r--   0        0        0     1537 1970-01-01 00:00:00.000000 lightgbm_embedding-0.1.2/setup.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 lightgbm_embedding-0.1.2/PKG-INFO
```

### Comparing `lightgbm_embedding-0.1.1/LICENSE` & `lightgbm_embedding-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightgbm_embedding-0.1.1/lightgbm_embedding/__init__.py` & `lightgbm_embedding-0.1.2/lightgbm_embedding/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-__version__ = "0.1.1"
-
+__version__ = "0.1.2"
 
 import numpy as np
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.multiclass import type_of_target
 from sklearn.utils.validation import check_is_fitted
 from lightgbm import LGBMClassifier, LGBMRegressor
 from scipy.special import expit
```

### Comparing `lightgbm_embedding-0.1.1/pyproject.toml` & `lightgbm_embedding-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [tool.poetry]
 name = "lightgbm_embedding"
-version = "0.1.1"
+version = "0.1.2"
 description = "Feature embeddings with LightGBM"
 authors = ["Atilla Karaahmetoğlu <atilla.karaahmetoglu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 keywords = ["nlp", "turkish"]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+scipy = ">=1.10.0, < 1.11.0"
+python = ">=3.8, <3.12"
 pandas = "^1.0.0"
 scikit-learn = "^1.0.0"
 lightgbm = "^3.0.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
```

### Comparing `lightgbm_embedding-0.1.1/README.md` & `lightgbm_embedding-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lightgbm_embedding-0.1.1/setup.py` & `lightgbm_embedding-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 packages = \
 ['lightgbm_embedding']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['lightgbm>=3.0.0,<4.0.0', 'pandas>=1.0.0,<2.0.0', 'scikit-learn>=1.0.0,<2.0.0']
+['lightgbm>=3.0.0,<4.0.0',
+ 'pandas>=1.0.0,<2.0.0',
+ 'scikit-learn>=1.0.0,<2.0.0',
+ 'scipy>=1.10.0,<1.11.0']
 
 setup_kwargs = {
     'name': 'lightgbm-embedding',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Feature embeddings with LightGBM',
     'long_description': '# LightGBM Embeddings\n\nFeature embeddings with LightGBM\n\n## Installation\n\n    pip install lightgbm-embedding\n\n## Examples\n```python\nimport pandas as pd\nfrom sklearn.model_selection import train_test_split\nfrom lightgbm_embedding import LightgbmEmbedding\n\ndf = pd.read_csv(\n    "https://gist.githubusercontent.com/curran/a08a1080b88344b0c8a7/raw/0e7a9b0a5d22642a06d3d5b9bcbad9890c8ee534/iris.csv"\n)\ncols = df.columns[:-1]\ntarget = df.columns[-1]\nnum_classes = df[target].nunique()\n\nX_train, X_test = train_test_split(\n    df, test_size=0.2, stratify=df[target], random_state=42\n)\n\nn_dim = 20\nemb = LightgbmEmbedding(n_dim=n_dim)\nemb.fit(X_train[cols], X_train[target])\nX_train_embed = emb.transform(X_train[cols])\nX_test_embed = emb.transform(X_test[cols])\n```\n',
     'author': 'Atilla Karaahmetoğlu',
     'author_email': 'atilla.karaahmetoglu@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `lightgbm_embedding-0.1.1/PKG-INFO` & `lightgbm_embedding-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: lightgbm-embedding
-Version: 0.1.1
+Version: 0.1.2
 Summary: Feature embeddings with LightGBM
 License: MIT
 Keywords: nlp,turkish
 Author: Atilla Karaahmetoğlu
 Author-email: atilla.karaahmetoglu@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: lightgbm (>=3.0.0,<4.0.0)
 Requires-Dist: pandas (>=1.0.0,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0.0,<2.0.0)
+Requires-Dist: scipy (>=1.10.0,<1.11.0)
 Description-Content-Type: text/markdown
 
 # LightGBM Embeddings
 
 Feature embeddings with LightGBM
 
 ## Installation
```

