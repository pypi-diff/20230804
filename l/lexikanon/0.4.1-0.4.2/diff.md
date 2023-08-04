# Comparing `tmp/lexikanon-0.4.1.tar.gz` & `tmp/lexikanon-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikanon-0.4.1.tar", max compression
+gzip compressed data, was "lexikanon-0.4.2.tar", max compression
```

## Comparing `lexikanon-0.4.1.tar` & `lexikanon-0.4.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1071 2023-08-03 02:36:07.821254 lexikanon-0.4.1/LICENSE
--rw-r--r--   0        0        0     2129 2023-08-03 02:36:07.821254 lexikanon-0.4.1/README.md
--rw-r--r--   0        0        0     3218 2023-08-03 02:36:45.805957 lexikanon-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      184 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/__cli__.py
--rw-r--r--   0        0        0      473 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/__init__.py
--rw-r--r--   0        0        0       22 2023-08-03 02:36:45.753956 lexikanon-0.4.1/src/lexikanon/_version.py
--rw-r--r--   0        0        0        0 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/__init__.py
--rw-r--r--   0        0        0      177 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/about/lexikanon.yaml
--rw-r--r--   0        0        0      214 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/__init__.yaml
--rw-r--r--   0        0        0       79 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/formal_en.yaml
--rw-r--r--   0        0        0      114 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
--rw-r--r--   0        0        0       68 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/formal_ko.yaml
--rw-r--r--   0        0        0      363 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
--rw-r--r--   0        0        0       94 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/informal_ko.yaml
--rw-r--r--   0        0        0      102 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/spaces/__init__.yaml
--rw-r--r--   0        0        0      151 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
--rw-r--r--   0        0        0       53 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/pipe/extract_nouns.yaml
--rw-r--r--   0        0        0      128 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/pipe/extract_tokens.yaml
--rw-r--r--   0        0        0      130 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/pipe/tokenize_dataset.yaml
--rw-r--r--   0        0        0      376 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/run/extract_tokens.yaml
--rw-r--r--   0        0        0      260 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/run/tokenize_dataset.yaml
--rw-r--r--   0        0        0      205 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/stopwords/__init__.yaml
--rw-r--r--   0        0        0      542 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/__init__.yaml
--rw-r--r--   0        0        0      262 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/mecab.yaml
--rw-r--r--   0        0        0      171 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/nltk.yaml
--rw-r--r--   0        0        0      109 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/simple.yaml
--rw-r--r--   0        0        0      143 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
--rw-r--r--   0        0        0      179 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
--rw-r--r--   0        0        0       61 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/normalizers/__init__.py
--rw-r--r--   0        0        0    10513 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/normalizers/normalizer.py
--rw-r--r--   0        0        0        0 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/pipe/__init__.py
--rw-r--r--   0        0        0     3430 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/pipe/tokenize.py
--rw-r--r--   0        0        0      195 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/project.toml
--rw-r--r--   0        0        0        0 2023-08-03 02:36:07.825254 lexikanon-0.4.1/src/lexikanon/py.typed
--rw-r--r--   0        0        0  2355775 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
--rw-r--r--   0        0        0       58 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/stopwords/__init__.py
--rw-r--r--   0        0        0     5153 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/stopwords/stopwords.py
--rw-r--r--   0        0        0      181 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/tokenizers/__init__.py
--rw-r--r--   0        0        0     9301 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/tokenizers/base.py
--rw-r--r--   0        0        0      818 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/tokenizers/mecab.py
--rw-r--r--   0        0        0     3159 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/tokenizers/nltk.py
--rw-r--r--   0        0        0    14339 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/__init__.py
--rw-r--r--   0        0        0     8294 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/hangle.py
--rw-r--r--   0        0        0      255 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/hanja/__init__.py
--rw-r--r--   0        0        0     2123 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/hanja/hangul.py
--rw-r--r--   0        0        0     2813 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/hanja/impl.py
--rw-r--r--   0        0        0      427 2023-08-03 02:36:07.841254 lexikanon-0.4.1/src/lexikanon/utils/hanja/table.py
--rw-r--r--   0        0        0   522443 2023-08-03 02:36:07.845254 lexikanon-0.4.1/src/lexikanon/utils/hanja/table.yml
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 lexikanon-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-04 08:20:23.207776 lexikanon-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2129 2023-08-04 08:20:23.207776 lexikanon-0.4.2/README.md
+-rw-r--r--   0        0        0     3218 2023-08-04 08:20:56.184239 lexikanon-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/__cli__.py
+-rw-r--r--   0        0        0      473 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-04 08:20:56.148238 lexikanon-0.4.2/src/lexikanon/_version.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/__init__.py
+-rw-r--r--   0        0        0      177 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/about/lexikanon.yaml
+-rw-r--r--   0        0        0      214 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/formal_en.yaml
+-rw-r--r--   0        0        0      114 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
+-rw-r--r--   0        0        0       68 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/formal_ko.yaml
+-rw-r--r--   0        0        0      363 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
+-rw-r--r--   0        0        0       94 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/informal_ko.yaml
+-rw-r--r--   0        0        0      102 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/spaces/__init__.yaml
+-rw-r--r--   0        0        0      151 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
+-rw-r--r--   0        0        0       53 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/pipe/extract_nouns.yaml
+-rw-r--r--   0        0        0      128 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/pipe/extract_tokens.yaml
+-rw-r--r--   0        0        0      130 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/pipe/tokenize_dataset.yaml
+-rw-r--r--   0        0        0      376 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/run/extract_tokens.yaml
+-rw-r--r--   0        0        0      260 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/run/tokenize_dataset.yaml
+-rw-r--r--   0        0        0      205 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/stopwords/__init__.yaml
+-rw-r--r--   0        0        0      542 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/__init__.yaml
+-rw-r--r--   0        0        0      262 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/mecab.yaml
+-rw-r--r--   0        0        0      174 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/nltk.yaml
+-rw-r--r--   0        0        0      109 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/simple.yaml
+-rw-r--r--   0        0        0      143 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
+-rw-r--r--   0        0        0      179 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
+-rw-r--r--   0        0        0       61 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/normalizers/__init__.py
+-rw-r--r--   0        0        0    10513 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/normalizers/normalizer.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/pipe/__init__.py
+-rw-r--r--   0        0        0     3430 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/pipe/tokenize.py
+-rw-r--r--   0        0        0      195 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/project.toml
+-rw-r--r--   0        0        0        0 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/py.typed
+-rw-r--r--   0        0        0  2355775 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
+-rw-r--r--   0        0        0       58 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/stopwords/__init__.py
+-rw-r--r--   0        0        0     5153 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/stopwords/stopwords.py
+-rw-r--r--   0        0        0      181 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/tokenizers/__init__.py
+-rw-r--r--   0        0        0     9301 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/tokenizers/base.py
+-rw-r--r--   0        0        0      818 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/tokenizers/mecab.py
+-rw-r--r--   0        0        0     3159 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/tokenizers/nltk.py
+-rw-r--r--   0        0        0    14339 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/__init__.py
+-rw-r--r--   0        0        0     8294 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/hangle.py
+-rw-r--r--   0        0        0      255 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/hanja/__init__.py
+-rw-r--r--   0        0        0     2123 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/hanja/hangul.py
+-rw-r--r--   0        0        0     2813 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/hanja/impl.py
+-rw-r--r--   0        0        0      427 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/hanja/table.py
+-rw-r--r--   0        0        0   522443 2023-08-04 08:20:23.227776 lexikanon-0.4.2/src/lexikanon/utils/hanja/table.yml
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 lexikanon-0.4.2/PKG-INFO
```

### Comparing `lexikanon-0.4.1/LICENSE` & `lexikanon-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/README.md` & `lexikanon-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/pyproject.toml` & `lexikanon-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lexikanon"
-version = "0.4.1"
+version = "0.4.2"
 description = "A Python Library for Tokenizers"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://lexikanon.entelecheia.ai"
 repository = "https://github.com/entelecheia/lexikanon"
 readme = "README.md"
 packages = [{ include = "lexikanon", from = "src" }]
```

### Comparing `lexikanon-0.4.1/src/lexikanon/conf/tokenizer/__init__.yaml` & `lexikanon-0.4.2/src/lexikanon/conf/tokenizer/__init__.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/normalizers/normalizer.py` & `lexikanon-0.4.2/src/lexikanon/normalizers/normalizer.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/pipe/tokenize.py` & `lexikanon-0.4.2/src/lexikanon/pipe/tokenize.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic` & `lexikanon-0.4.2/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/stopwords/stopwords.py` & `lexikanon-0.4.2/src/lexikanon/stopwords/stopwords.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/tokenizers/base.py` & `lexikanon-0.4.2/src/lexikanon/tokenizers/base.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/tokenizers/mecab.py` & `lexikanon-0.4.2/src/lexikanon/tokenizers/mecab.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/tokenizers/nltk.py` & `lexikanon-0.4.2/src/lexikanon/tokenizers/nltk.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/utils/__init__.py` & `lexikanon-0.4.2/src/lexikanon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/utils/hangle.py` & `lexikanon-0.4.2/src/lexikanon/utils/hangle.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/utils/hanja/hangul.py` & `lexikanon-0.4.2/src/lexikanon/utils/hanja/hangul.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/utils/hanja/impl.py` & `lexikanon-0.4.2/src/lexikanon/utils/hanja/impl.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/src/lexikanon/utils/hanja/table.yml` & `lexikanon-0.4.2/src/lexikanon/utils/hanja/table.yml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.1/PKG-INFO` & `lexikanon-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lexikanon
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Python Library for Tokenizers
 Home-page: https://lexikanon.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

