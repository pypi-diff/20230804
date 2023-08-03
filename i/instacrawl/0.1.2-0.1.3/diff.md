# Comparing `tmp/instacrawl-0.1.2.tar.gz` & `tmp/instacrawl-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instacrawl-0.1.2.tar", max compression
+gzip compressed data, was "instacrawl-0.1.3.tar", max compression
```

## Comparing `instacrawl-0.1.2.tar` & `instacrawl-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-08-03 00:31:26.417628 instacrawl-0.1.2/README.md
--rw-r--r--   0        0        0      123 2023-08-03 22:21:33.186069 instacrawl-0.1.2/instacrawl/__init__.py
--rw-r--r--   0        0        0     1549 2023-08-03 18:21:10.090362 instacrawl-0.1.2/instacrawl/__main__.py
--rw-r--r--   0        0        0    19796 2023-08-03 15:00:36.161900 instacrawl-0.1.2/instacrawl/analysis.py
--rw-r--r--   0        0        0    11537 2023-08-03 14:57:04.543184 instacrawl-0.1.2/instacrawl/cli_utils.py
--rw-r--r--   0        0        0       86 2023-08-03 15:01:47.156347 instacrawl-0.1.2/instacrawl/console.py
--rw-r--r--   0        0        0    47521 2023-08-03 22:21:48.024639 instacrawl-0.1.2/instacrawl/insta.py
--rw-r--r--   0        0        0    17346 2023-08-03 15:57:25.477020 instacrawl-0.1.2/instacrawl/prompts.py
--rw-r--r--   0        0        0     7856 2023-08-03 15:03:09.852583 instacrawl-0.1.2/instacrawl/steps.py
--rw-r--r--   0        0        0      570 2023-08-03 15:03:33.274542 instacrawl-0.1.2/instacrawl/verbose.py
--rw-r--r--   0        0        0      938 2023-08-03 22:22:04.804463 instacrawl-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 instacrawl-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 00:31:26.417628 instacrawl-0.1.3/README.md
+-rw-r--r--   0        0        0      123 2023-08-03 22:29:44.075564 instacrawl-0.1.3/instacrawl/__init__.py
+-rw-r--r--   0        0        0     1549 2023-08-03 18:21:10.090362 instacrawl-0.1.3/instacrawl/__main__.py
+-rw-r--r--   0        0        0    19796 2023-08-03 15:00:36.161900 instacrawl-0.1.3/instacrawl/analysis.py
+-rw-r--r--   0        0        0    11537 2023-08-03 14:57:04.543184 instacrawl-0.1.3/instacrawl/cli_utils.py
+-rw-r--r--   0        0        0       86 2023-08-03 15:01:47.156347 instacrawl-0.1.3/instacrawl/console.py
+-rw-r--r--   0        0        0    47521 2023-08-03 22:21:48.024639 instacrawl-0.1.3/instacrawl/insta.py
+-rw-r--r--   0        0        0    17346 2023-08-03 15:57:25.477020 instacrawl-0.1.3/instacrawl/prompts.py
+-rw-r--r--   0        0        0     7856 2023-08-03 15:03:09.852583 instacrawl-0.1.3/instacrawl/steps.py
+-rw-r--r--   0        0        0      570 2023-08-03 15:03:33.274542 instacrawl-0.1.3/instacrawl/verbose.py
+-rw-r--r--   0        0        0      954 2023-08-03 22:29:52.450080 instacrawl-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1520 1970-01-01 00:00:00.000000 instacrawl-0.1.3/PKG-INFO
```

### Comparing `instacrawl-0.1.2/instacrawl/__main__.py` & `instacrawl-0.1.3/instacrawl/__main__.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.2/instacrawl/analysis.py` & `instacrawl-0.1.3/instacrawl/analysis.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.2/instacrawl/cli_utils.py` & `instacrawl-0.1.3/instacrawl/cli_utils.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.2/instacrawl/insta.py` & `instacrawl-0.1.3/instacrawl/insta.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.2/instacrawl/prompts.py` & `instacrawl-0.1.3/instacrawl/prompts.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.2/instacrawl/steps.py` & `instacrawl-0.1.3/instacrawl/steps.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.2/instacrawl/verbose.py` & `instacrawl-0.1.3/instacrawl/verbose.py`

 * *Files identical despite different names*

### Comparing `instacrawl-0.1.2/pyproject.toml` & `instacrawl-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "instacrawl"
-version = "0.1.2"
+version = "0.1.3"
 description = "A simple CLI Instagram crawler with a focus on algorithm analytics."
 authors = [
   "Analetta Ehler <annie.ehler.4@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/annie444/instacrawl"
@@ -31,12 +31,13 @@
 pandas = "^2.0.3"
 typing-extensions = "^4.7.1"
 transformers = "^4.31.0"
 scikit-learn = "^1.3.0"
 requests = "^2.31.0"
 python-dotenv = "^1.0.0"
 html5lib = "^1.1"
+timm = "^0.9.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `instacrawl-0.1.2/PKG-INFO` & `instacrawl-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instacrawl
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple CLI Instagram crawler with a focus on algorithm analytics.
 Home-page: https://github.com/annie444/instacrawl
 License: MIT
 Author: Analetta Ehler
 Author-email: annie.ehler.4@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -24,14 +24,15 @@
 Requires-Dist: pynput (>=1.7.6,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.5.2,<14.0.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Requires-Dist: selenium (>=4.11.2,<5.0.0)
 Requires-Dist: selenium-wire (>=5.1.0,<6.0.0)
+Requires-Dist: timm (>=0.9.2,<0.10.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: transformers (>=4.31.0,<5.0.0)
 Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.7.1,<5.0.0)
 Project-URL: Repository, https://github.com/annie444/instacrawl
 Description-Content-Type: text/markdown
```

