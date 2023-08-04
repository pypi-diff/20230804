# Comparing `tmp/openprotein_python-0.1.1b7.tar.gz` & `tmp/openprotein_python-0.1.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openprotein_python-0.1.1b7.tar", max compression
+gzip compressed data, was "openprotein_python-0.1.1b8.tar", max compression
```

## Comparing `openprotein_python-0.1.1b7.tar` & `openprotein_python-0.1.1b8.tar`

### file list

```diff
@@ -1,19 +1,27 @@
--rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.1.1b7/LICENSE.txt
--rw-r--r--   0        0        0     2925 2023-08-04 03:37:46.856592 openprotein_python-0.1.1b7/README.md
--rw-r--r--   0        0        0     2101 2023-08-04 03:26:20.802155 openprotein_python-0.1.1b7/openprotein_python/__init__.py
--rw-r--r--   0        0        0      120 2023-08-04 03:53:10.661261 openprotein_python-0.1.1b7/openprotein_python/_version.py
--rw-r--r--   0        0        0      127 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b7/openprotein_python/api/__init__.py
--rw-r--r--   0        0        0    13265 2023-08-04 03:26:28.274225 openprotein_python-0.1.1b7/openprotein_python/api/data.py
--rw-r--r--   0        0        0     8575 2023-08-04 03:26:31.494255 openprotein_python-0.1.1b7/openprotein_python/api/design.py
--rw-r--r--   0        0        0    22251 2023-08-04 03:26:35.154289 openprotein_python-0.1.1b7/openprotein_python/api/embedding.py
--rw-r--r--   0        0        0    14423 2023-08-04 03:26:37.454311 openprotein_python-0.1.1b7/openprotein_python/api/jobs.py
--rw-r--r--   0        0        0    41938 2023-08-04 03:26:41.162346 openprotein_python-0.1.1b7/openprotein_python/api/poet.py
--rw-r--r--   0        0        0    17793 2023-08-04 03:26:54.222468 openprotein_python-0.1.1b7/openprotein_python/api/predict.py
--rw-r--r--   0        0        0    19488 2023-08-04 03:26:57.478499 openprotein_python-0.1.1b7/openprotein_python/api/train.py
--rw-r--r--   0        0        0     3083 2023-08-04 03:30:00.392216 openprotein_python-0.1.1b7/openprotein_python/base.py
--rw-r--r--   0        0        0      170 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b7/openprotein_python/config.py
--rw-r--r--   0        0        0     1146 2023-08-02 06:48:12.506765 openprotein_python-0.1.1b7/openprotein_python/errors.py
--rw-r--r--   0        0        0     1055 2023-08-02 06:28:11.916350 openprotein_python-0.1.1b7/openprotein_python/fasta.py
--rw-r--r--   0        0        0     8636 2023-08-04 03:26:25.866202 openprotein_python-0.1.1b7/openprotein_python/models.py
--rw-r--r--   0        0        0      554 2023-08-04 04:07:30.169379 openprotein_python-0.1.1b7/pyproject.toml
--rw-r--r--   0        0        0     3751 1970-01-01 00:00:00.000000 openprotein_python-0.1.1b7/PKG-INFO
+-rw-r--r--   0        0        0     1543 2023-08-02 06:48:12.466765 openprotein_python-0.1.1b8/LICENSE.txt
+-rw-r--r--   0        0        0     2925 2023-08-04 03:37:46.856592 openprotein_python-0.1.1b8/README.md
+-rw-r--r--   0        0        0     2101 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/__init__.py
+-rw-r--r--   0        0        0      120 2023-08-04 06:46:01.435537 openprotein_python-0.1.1b8/openprotein_python/_version.py
+-rw-r--r--   0        0        0      127 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/__init__.py
+-rw-r--r--   0        0        0      337 2023-08-04 06:44:47.298834 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    13440 2023-08-04 06:44:47.298834 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/data.cpython-38.pyc
+-rw-r--r--   0        0        0     9314 2023-08-04 06:44:47.738838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/design.cpython-38.pyc
+-rw-r--r--   0        0        0    23908 2023-08-04 06:44:47.750838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/embedding.cpython-38.pyc
+-rw-r--r--   0        0        0    14445 2023-08-04 06:44:47.706838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/jobs.cpython-38.pyc
+-rw-r--r--   0        0        0    39618 2023-08-04 06:44:47.750838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/poet.cpython-38.pyc
+-rw-r--r--   0        0        0    16779 2023-08-04 06:44:47.742838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/predict.cpython-38.pyc
+-rw-r--r--   0        0        0    18101 2023-08-04 06:44:47.742838 openprotein_python-0.1.1b8/openprotein_python/api/__pycache__/train.cpython-38.pyc
+-rw-r--r--   0        0        0    13265 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/data.py
+-rw-r--r--   0        0        0     8575 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/design.py
+-rw-r--r--   0        0        0    22251 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/embedding.py
+-rw-r--r--   0        0        0    14423 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/jobs.py
+-rw-r--r--   0        0        0    41938 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/poet.py
+-rw-r--r--   0        0        0    17793 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/predict.py
+-rw-r--r--   0        0        0    19488 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/api/train.py
+-rw-r--r--   0        0        0     3083 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/base.py
+-rw-r--r--   0        0        0      170 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/config.py
+-rw-r--r--   0        0        0     1146 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/errors.py
+-rw-r--r--   0        0        0     1055 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/fasta.py
+-rw-r--r--   0        0        0     8636 2023-08-04 06:44:36.034727 openprotein_python-0.1.1b8/openprotein_python/models.py
+-rw-r--r--   0        0        0      558 2023-08-04 06:45:54.967476 openprotein_python-0.1.1b8/pyproject.toml
+-rw-r--r--   0        0        0     3755 1970-01-01 00:00:00.000000 openprotein_python-0.1.1b8/PKG-INFO
```

### Comparing `openprotein_python-0.1.1b7/LICENSE.txt` & `openprotein_python-0.1.1b8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/README.md` & `openprotein_python-0.1.1b8/README.md`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/__init__.py` & `openprotein_python-0.1.1b8/openprotein_python/__init__.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/api/data.py` & `openprotein_python-0.1.1b8/openprotein_python/api/data.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/api/design.py` & `openprotein_python-0.1.1b8/openprotein_python/api/design.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/api/embedding.py` & `openprotein_python-0.1.1b8/openprotein_python/api/embedding.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/api/jobs.py` & `openprotein_python-0.1.1b8/openprotein_python/api/jobs.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/api/poet.py` & `openprotein_python-0.1.1b8/openprotein_python/api/poet.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/api/predict.py` & `openprotein_python-0.1.1b8/openprotein_python/api/predict.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/api/train.py` & `openprotein_python-0.1.1b8/openprotein_python/api/train.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/base.py` & `openprotein_python-0.1.1b8/openprotein_python/base.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/errors.py` & `openprotein_python-0.1.1b8/openprotein_python/errors.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/fasta.py` & `openprotein_python-0.1.1b8/openprotein_python/fasta.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/openprotein_python/models.py` & `openprotein_python-0.1.1b8/openprotein_python/models.py`

 * *Files identical despite different names*

### Comparing `openprotein_python-0.1.1b7/pyproject.toml` & `openprotein_python-0.1.1b8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "openprotein_python"
-version = "0.1.1b7"
+version = "0.1.1b8"
 description = "OpenProtein Python interface."
 license = "MIT"
 readme = "README.md"
 homepage = "https://docs.openprotein.ai/"
 authors = ["OpenProtein <info@ne47.bio>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-requests = ">2"
-pydantic = ">1"
-tqdm = ">4"
-pandas = ">1"
+requests = ">=2"
+pydantic = ">=1"
+tqdm = ">=4"
+pandas = ">=1"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openprotein_python-0.1.1b7/PKG-INFO` & `openprotein_python-0.1.1b8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openprotein-python
-Version: 0.1.1b7
+Version: 0.1.1b8
 Summary: OpenProtein Python interface.
 Home-page: https://docs.openprotein.ai/
 License: MIT
 Author: OpenProtein
 Author-email: info@ne47.bio
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,18 +12,18 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: pandas (>1)
-Requires-Dist: pydantic (>1)
-Requires-Dist: requests (>2)
-Requires-Dist: tqdm (>4)
+Requires-Dist: pandas (>=1)
+Requires-Dist: pydantic (>=1)
+Requires-Dist: requests (>=2)
+Requires-Dist: tqdm (>=4)
 Description-Content-Type: text/markdown
 
 # openprotein-python
 Python interface for the OpenProtein.AI REST API.
 
 ## Installation
```

