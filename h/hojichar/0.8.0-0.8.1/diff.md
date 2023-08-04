# Comparing `tmp/hojichar-0.8.0.tar.gz` & `tmp/hojichar-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hojichar-0.8.0.tar", max compression
+gzip compressed data, was "hojichar-0.8.1.tar", max compression
```

## Comparing `hojichar-0.8.0.tar` & `hojichar-0.8.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2023-07-30 15:25:29.668113 hojichar-0.8.0/LICENSE
--rw-r--r--   0        0        0    14271 2023-07-30 15:25:29.668113 hojichar-0.8.0/README.md
--rw-r--r--   0        0        0      547 2023-07-30 15:25:49.828322 hojichar-0.8.0/hojichar/__init__.py
--rw-r--r--   0        0        0     5689 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/cli.py
--rw-r--r--   0        0        0       42 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/core/__init__.py
--rw-r--r--   0        0        0     5039 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/core/composition.py
--rw-r--r--   0        0        0     5638 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/core/filter_interface.py
--rw-r--r--   0        0        0     6221 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/core/inspection.py
--rw-r--r--   0        0        0     1087 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/core/models.py
--rw-r--r--   0        0        0      147 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/__init__.py
--rw-r--r--   0        0        0      941 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/adult_keywords_en.txt
--rw-r--r--   0        0        0    18091 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/adult_keywords_ja.txt
--rw-r--r--   0        0        0      426 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/advertisement_keywords_ja.txt
--rw-r--r--   0        0        0     1740 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/discrimination_keywords_ja.txt
--rw-r--r--   0        0        0       67 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/dummy_ng_words.txt
--rw-r--r--   0        0        0      577 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/header_footer_keywords_ja.txt
--rw-r--r--   0        0        0      665 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/dict/violence_keywords_ja.txt
--rw-r--r--   0        0        0      711 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/filters/__init__.py
--rw-r--r--   0        0        0    12104 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/filters/deduplication.py
--rw-r--r--   0        0        0    23939 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/filters/document_filters.py
--rw-r--r--   0        0        0     1606 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/filters/token_filters.py
--rw-r--r--   0        0        0     2530 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/filters/tokenization.py
--rw-r--r--   0        0        0        0 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/py.typed
--rw-r--r--   0        0        0      595 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/utils/__init__.py
--rw-r--r--   0        0        0     1716 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/utils/io_iter.py
--rw-r--r--   0        0        0     3380 2023-07-30 15:25:29.668113 hojichar-0.8.0/hojichar/utils/load_compose.py
--rw-r--r--   0        0        0     1920 2023-07-30 15:25:29.672114 hojichar-0.8.0/hojichar/utils/process.py
--rw-r--r--   0        0        0     1788 2023-07-30 15:25:49.828322 hojichar-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    15042 1970-01-01 00:00:00.000000 hojichar-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-04 01:32:14.808367 hojichar-0.8.1/LICENSE
+-rw-r--r--   0        0        0    14271 2023-08-04 01:32:14.808367 hojichar-0.8.1/README.md
+-rw-r--r--   0        0        0      547 2023-08-04 01:32:35.280477 hojichar-0.8.1/hojichar/__init__.py
+-rw-r--r--   0        0        0     5819 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/cli.py
+-rw-r--r--   0        0        0       42 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/core/__init__.py
+-rw-r--r--   0        0        0     5039 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/core/composition.py
+-rw-r--r--   0        0        0     5638 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/core/filter_interface.py
+-rw-r--r--   0        0        0     6221 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/core/inspection.py
+-rw-r--r--   0        0        0     1087 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/core/models.py
+-rw-r--r--   0        0        0      147 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/dict/__init__.py
+-rw-r--r--   0        0        0      941 2023-08-04 01:32:14.808367 hojichar-0.8.1/hojichar/dict/adult_keywords_en.txt
+-rw-r--r--   0        0        0    18091 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/adult_keywords_ja.txt
+-rw-r--r--   0        0        0      426 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/advertisement_keywords_ja.txt
+-rw-r--r--   0        0        0     1740 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/discrimination_keywords_ja.txt
+-rw-r--r--   0        0        0       67 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/dummy_ng_words.txt
+-rw-r--r--   0        0        0      577 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/header_footer_keywords_ja.txt
+-rw-r--r--   0        0        0      665 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/dict/violence_keywords_ja.txt
+-rw-r--r--   0        0        0      711 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/filters/__init__.py
+-rw-r--r--   0        0        0    12104 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/filters/deduplication.py
+-rw-r--r--   0        0        0    23939 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/filters/document_filters.py
+-rw-r--r--   0        0        0     1606 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/filters/token_filters.py
+-rw-r--r--   0        0        0     2530 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/filters/tokenization.py
+-rw-r--r--   0        0        0        0 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/py.typed
+-rw-r--r--   0        0        0      595 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/utils/__init__.py
+-rw-r--r--   0        0        0     1716 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/utils/io_iter.py
+-rw-r--r--   0        0        0     3380 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/utils/load_compose.py
+-rw-r--r--   0        0        0     1920 2023-08-04 01:32:14.812367 hojichar-0.8.1/hojichar/utils/process.py
+-rw-r--r--   0        0        0     1788 2023-08-04 01:32:35.276477 hojichar-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    15042 1970-01-01 00:00:00.000000 hojichar-0.8.1/PKG-INFO
```

### Comparing `hojichar-0.8.0/LICENSE` & `hojichar-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/README.md` & `hojichar-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/__init__.py` & `hojichar-0.8.1/hojichar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 .. include:: ../README.md
 """
 from .core.composition import Compose
 from .core.filter_interface import Filter, TokenFilter
 from .core.models import Document, Token
 from .filters import deduplication, document_filters, token_filters, tokenization
 
-__version__ = "0.8.0"  # Replaced by poetry-dynamic-versioning when deploying
+__version__ = "0.8.1"  # Replaced by poetry-dynamic-versioning when deploying
 
 __all__ = [
     "core",
     "filters",
     "utils",
     "Compose",
     "Filter",
```

### Comparing `hojichar-0.8.0/hojichar/cli.py` & `hojichar-0.8.1/hojichar/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,20 @@
     parser.add_argument(
         "--jobs",
         "-j",
         default=None,
         type=int,
         help="The number ob parallel jobs. By default, the nuber of the CPU core.",
     )
+    parser.add_argument(
+        "--version",
+        "-v",
+        action="version",
+        version=hojichar.__version__,
+    )
     args = parser.parse_args()
     return args
 
 
 def init_worker(filter: hojichar.Compose, args: argparse.Namespace) -> None:
     signal.signal(signal.SIGINT, signal.SIG_IGN)
     global MAIN_FILTER, CLI_ARGS
```

### Comparing `hojichar-0.8.0/hojichar/core/composition.py` & `hojichar-0.8.1/hojichar/core/composition.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/core/filter_interface.py` & `hojichar-0.8.1/hojichar/core/filter_interface.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/core/inspection.py` & `hojichar-0.8.1/hojichar/core/inspection.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/core/models.py` & `hojichar-0.8.1/hojichar/core/models.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/dict/adult_keywords_en.txt` & `hojichar-0.8.1/hojichar/dict/adult_keywords_en.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/dict/adult_keywords_ja.txt` & `hojichar-0.8.1/hojichar/dict/adult_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/dict/discrimination_keywords_ja.txt` & `hojichar-0.8.1/hojichar/dict/discrimination_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/dict/header_footer_keywords_ja.txt` & `hojichar-0.8.1/hojichar/dict/header_footer_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/dict/violence_keywords_ja.txt` & `hojichar-0.8.1/hojichar/dict/violence_keywords_ja.txt`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/filters/__init__.py` & `hojichar-0.8.1/hojichar/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/filters/deduplication.py` & `hojichar-0.8.1/hojichar/filters/deduplication.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/filters/document_filters.py` & `hojichar-0.8.1/hojichar/filters/document_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/filters/token_filters.py` & `hojichar-0.8.1/hojichar/filters/token_filters.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/filters/tokenization.py` & `hojichar-0.8.1/hojichar/filters/tokenization.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/utils/__init__.py` & `hojichar-0.8.1/hojichar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/utils/io_iter.py` & `hojichar-0.8.1/hojichar/utils/io_iter.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/utils/load_compose.py` & `hojichar-0.8.1/hojichar/utils/load_compose.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/hojichar/utils/process.py` & `hojichar-0.8.1/hojichar/utils/process.py`

 * *Files identical despite different names*

### Comparing `hojichar-0.8.0/pyproject.toml` & `hojichar-0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hojichar"
-version = "0.8.0"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
+version = "0.8.1"                                     # Versioning by git tag dinamically with https://github.com/mtkennerly/poetry-dynamic-versioning
 description = "Text preprocessing management system."
 license = "Apache-2.0"
 authors = ["kenta.shinzato <hoppiece@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/HojiChar/HojiChar"
 repository = "https://github.com/HojiChar/HojiChar"
```

### Comparing `hojichar-0.8.0/PKG-INFO` & `hojichar-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hojichar
-Version: 0.8.0
+Version: 0.8.1
 Summary: Text preprocessing management system.
 Home-page: https://github.com/HojiChar/HojiChar
 License: Apache-2.0
 Author: kenta.shinzato
 Author-email: hoppiece@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

