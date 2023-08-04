# Comparing `tmp/lexikanon-0.4.2.tar.gz` & `tmp/lexikanon-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexikanon-0.4.2.tar", max compression
+gzip compressed data, was "lexikanon-0.4.3.tar", max compression
```

## Comparing `lexikanon-0.4.2.tar` & `lexikanon-0.4.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1071 2023-08-04 08:20:23.207776 lexikanon-0.4.2/LICENSE
--rw-r--r--   0        0        0     2129 2023-08-04 08:20:23.207776 lexikanon-0.4.2/README.md
--rw-r--r--   0        0        0     3218 2023-08-04 08:20:56.184239 lexikanon-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      184 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/__cli__.py
--rw-r--r--   0        0        0      473 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/__init__.py
--rw-r--r--   0        0        0       22 2023-08-04 08:20:56.148238 lexikanon-0.4.2/src/lexikanon/_version.py
--rw-r--r--   0        0        0        0 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/__init__.py
--rw-r--r--   0        0        0      177 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/about/lexikanon.yaml
--rw-r--r--   0        0        0      214 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/__init__.yaml
--rw-r--r--   0        0        0       79 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/formal_en.yaml
--rw-r--r--   0        0        0      114 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
--rw-r--r--   0        0        0       68 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/formal_ko.yaml
--rw-r--r--   0        0        0      363 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
--rw-r--r--   0        0        0       94 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/informal_ko.yaml
--rw-r--r--   0        0        0      102 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/spaces/__init__.yaml
--rw-r--r--   0        0        0      151 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
--rw-r--r--   0        0        0       53 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/pipe/extract_nouns.yaml
--rw-r--r--   0        0        0      128 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/pipe/extract_tokens.yaml
--rw-r--r--   0        0        0      130 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/pipe/tokenize_dataset.yaml
--rw-r--r--   0        0        0      376 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/run/extract_tokens.yaml
--rw-r--r--   0        0        0      260 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/run/tokenize_dataset.yaml
--rw-r--r--   0        0        0      205 2023-08-04 08:20:23.207776 lexikanon-0.4.2/src/lexikanon/conf/stopwords/__init__.yaml
--rw-r--r--   0        0        0      542 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/__init__.yaml
--rw-r--r--   0        0        0      262 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/mecab.yaml
--rw-r--r--   0        0        0      174 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/nltk.yaml
--rw-r--r--   0        0        0      109 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/simple.yaml
--rw-r--r--   0        0        0      143 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
--rw-r--r--   0        0        0      179 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
--rw-r--r--   0        0        0       61 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/normalizers/__init__.py
--rw-r--r--   0        0        0    10513 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/normalizers/normalizer.py
--rw-r--r--   0        0        0        0 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/pipe/__init__.py
--rw-r--r--   0        0        0     3430 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/pipe/tokenize.py
--rw-r--r--   0        0        0      195 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/project.toml
--rw-r--r--   0        0        0        0 2023-08-04 08:20:23.211776 lexikanon-0.4.2/src/lexikanon/py.typed
--rw-r--r--   0        0        0  2355775 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
--rw-r--r--   0        0        0       58 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/stopwords/__init__.py
--rw-r--r--   0        0        0     5153 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/stopwords/stopwords.py
--rw-r--r--   0        0        0      181 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/tokenizers/__init__.py
--rw-r--r--   0        0        0     9301 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/tokenizers/base.py
--rw-r--r--   0        0        0      818 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/tokenizers/mecab.py
--rw-r--r--   0        0        0     3159 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/tokenizers/nltk.py
--rw-r--r--   0        0        0    14339 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/__init__.py
--rw-r--r--   0        0        0     8294 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/hangle.py
--rw-r--r--   0        0        0      255 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/hanja/__init__.py
--rw-r--r--   0        0        0     2123 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/hanja/hangul.py
--rw-r--r--   0        0        0     2813 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/hanja/impl.py
--rw-r--r--   0        0        0      427 2023-08-04 08:20:23.223776 lexikanon-0.4.2/src/lexikanon/utils/hanja/table.py
--rw-r--r--   0        0        0   522443 2023-08-04 08:20:23.227776 lexikanon-0.4.2/src/lexikanon/utils/hanja/table.yml
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 lexikanon-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-04 12:10:02.201323 lexikanon-0.4.3/LICENSE
+-rw-r--r--   0        0        0     2129 2023-08-04 12:10:02.201323 lexikanon-0.4.3/README.md
+-rw-r--r--   0        0        0     3218 2023-08-04 12:10:34.422028 lexikanon-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      184 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/__cli__.py
+-rw-r--r--   0        0        0      473 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-04 12:10:34.378027 lexikanon-0.4.3/src/lexikanon/_version.py
+-rw-r--r--   0        0        0        0 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/__init__.py
+-rw-r--r--   0        0        0      177 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/about/lexikanon.yaml
+-rw-r--r--   0        0        0      214 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/normalizer/__init__.yaml
+-rw-r--r--   0        0        0       79 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/normalizer/formal_en.yaml
+-rw-r--r--   0        0        0      114 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/normalizer/formal_en_parantheses.yaml
+-rw-r--r--   0        0        0       68 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/normalizer/formal_ko.yaml
+-rw-r--r--   0        0        0      363 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/normalizer/ftfy/__init__.yaml
+-rw-r--r--   0        0        0       94 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/normalizer/informal_ko.yaml
+-rw-r--r--   0        0        0      102 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/normalizer/spaces/__init__.yaml
+-rw-r--r--   0        0        0      151 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/normalizer/special_characters/__init__.yaml
+-rw-r--r--   0        0        0       53 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/pipe/extract_nouns.yaml
+-rw-r--r--   0        0        0      128 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/pipe/extract_tokens.yaml
+-rw-r--r--   0        0        0      130 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/pipe/tokenize_dataset.yaml
+-rw-r--r--   0        0        0      364 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/run/extract_tokens.yaml
+-rw-r--r--   0        0        0      248 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/run/tokenize_dataset.yaml
+-rw-r--r--   0        0        0      205 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/stopwords/__init__.yaml
+-rw-r--r--   0        0        0      542 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/tokenizer/__init__.yaml
+-rw-r--r--   0        0        0      262 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/tokenizer/mecab.yaml
+-rw-r--r--   0        0        0      174 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/tokenizer/nltk.yaml
+-rw-r--r--   0        0        0      109 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/tokenizer/simple.yaml
+-rw-r--r--   0        0        0      143 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/tokenizer/tagger/mecab.yaml
+-rw-r--r--   0        0        0      179 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/conf/tokenizer/tagger/nltk.yaml
+-rw-r--r--   0        0        0       61 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/normalizers/__init__.py
+-rw-r--r--   0        0        0    10513 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/normalizers/normalizer.py
+-rw-r--r--   0        0        0        0 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/pipe/__init__.py
+-rw-r--r--   0        0        0     3793 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/pipe/tokenize.py
+-rw-r--r--   0        0        0      195 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/project.toml
+-rw-r--r--   0        0        0        0 2023-08-04 12:10:02.205323 lexikanon-0.4.3/src/lexikanon/py.typed
+-rw-r--r--   0        0        0  2355775 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic
+-rw-r--r--   0        0        0       58 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/stopwords/__init__.py
+-rw-r--r--   0        0        0     5153 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/stopwords/stopwords.py
+-rw-r--r--   0        0        0      209 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/tokenizers/__init__.py
+-rw-r--r--   0        0        0     9301 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/tokenizers/base.py
+-rw-r--r--   0        0        0      818 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/tokenizers/mecab.py
+-rw-r--r--   0        0        0     3159 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/tokenizers/nltk.py
+-rw-r--r--   0        0        0    14339 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/utils/__init__.py
+-rw-r--r--   0        0        0     8294 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/utils/hangle.py
+-rw-r--r--   0        0        0      255 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/utils/hanja/__init__.py
+-rw-r--r--   0        0        0     2123 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/utils/hanja/hangul.py
+-rw-r--r--   0        0        0     2813 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/utils/hanja/impl.py
+-rw-r--r--   0        0        0      427 2023-08-04 12:10:02.217323 lexikanon-0.4.3/src/lexikanon/utils/hanja/table.py
+-rw-r--r--   0        0        0   522443 2023-08-04 12:10:02.221323 lexikanon-0.4.3/src/lexikanon/utils/hanja/table.yml
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 lexikanon-0.4.3/PKG-INFO
```

### Comparing `lexikanon-0.4.2/LICENSE` & `lexikanon-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/README.md` & `lexikanon-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/pyproject.toml` & `lexikanon-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "lexikanon"
-version = "0.4.2"
+version = "0.4.3"
 description = "A Python Library for Tokenizers"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://lexikanon.entelecheia.ai"
 repository = "https://github.com/entelecheia/lexikanon"
 readme = "README.md"
 packages = [{ include = "lexikanon", from = "src" }]
 
 [tool.poetry.scripts]
 lexikanon = 'lexikanon.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.17.2"
+hyfi = "^1.18.1"
 ftfy = "^6.1.1"
 nltk = "^3.8.1"
 ekonlpy = "^2.0.2"
 # hyfi = { path = "../hyfi", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `lexikanon-0.4.2/src/lexikanon/conf/tokenizer/__init__.yaml` & `lexikanon-0.4.3/src/lexikanon/conf/tokenizer/__init__.yaml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/normalizers/normalizer.py` & `lexikanon-0.4.3/src/lexikanon/normalizers/normalizer.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/pipe/tokenize.py` & `lexikanon-0.4.3/src/lexikanon/pipe/tokenize.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,45 @@
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from datasets import Dataset
 
 from lexikanon import HyFI
 
 logger = HyFI.getLogger(__name__)
 
 
 def tokenize_dataset(
     data: Dataset,
-    tokenizer_config_name: str = "simple",
+    tokenizer: Union[str, Dict[str, Any]] = "simple",
     num_workers: int = 1,
     batched: bool = True,
     batch_size: int = 1000,
     text_col: str = "bodyText",
     token_col: str = "tokenizedText",
     remove_columns: Optional[Union[List[str], str]] = None,
     load_from_cache_file: bool = True,
     num_heads: Optional[int] = 1,
     num_tails: Optional[int] = 1,
     verbose: bool = False,
 ) -> Dataset:
     def pos_tagging(batch):
-        tokenizer = HyFI.instantiate_config(f"tokenizer={tokenizer_config_name}")
+        if isinstance(tokenizer, str):
+            _tokenizer_ = HyFI.instantiate_config(
+                f"tokenizer={tokenizer}",
+            )
+        else:
+            _tokenizer_ = HyFI.instantiate(
+                tokenizer,
+            )
         batch_tokens = []
         for text in batch[text_col]:
             sentences = text.split("\n")
             tokens = []
             for sentence in sentences:
-                tokens.extend(tokenizer(sentence))
+                tokens.extend(_tokenizer_(sentence))
             batch_tokens.append(tokens)
         return {token_col: batch_tokens}
 
     data = data.map(
         pos_tagging,
         num_proc=num_workers,
         batched=batched,
@@ -49,15 +56,15 @@
             num_tails = min(num_tails, len(data))
             print(data[-num_tails:][token_col])
     return data
 
 
 def extract_tokens(
     data: Dataset,
-    tokenizer_config_name: str = "simple",
+    tokenizer: Union[str, Dict[str, Any]] = "simple",
     num_workers: int = 1,
     batched: bool = True,
     batch_size: int = 1000,
     token_col: str = "tokenizedText",
     extracted_col: str = "extractedTokens",
     nouns_only: bool = False,
     postags: Optional[List[str]] = None,
@@ -68,19 +75,26 @@
     remove_columns: Optional[Union[List[str], str]] = None,
     load_from_cache_file: bool = True,
     num_heads: Optional[int] = 1,
     num_tails: Optional[int] = 1,
     verbose: bool = False,
 ) -> Dataset:
     def pos_tagging(batch):
-        tokenizer = HyFI.instantiate_config(f"tokenizer={tokenizer_config_name}")
+        if isinstance(tokenizer, str):
+            _tokenizer_ = HyFI.instantiate_config(
+                f"tokenizer={tokenizer}",
+            )
+        else:
+            _tokenizer_ = HyFI.instantiate(
+                tokenizer,
+            )
         batch_tokens = []
         for tokens in batch[token_col]:
             batch_tokens.append(
-                tokenizer.extract(
+                _tokenizer_.extract(
                     tokens,
                     nouns_only=nouns_only,
                     postags=postags,
                     stop_postags=stop_postags,
                     strip_pos=strip_pos,
                     postag_delim=postag_delim,
                     postag_length=postag_length,
```

### Comparing `lexikanon-0.4.2/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic` & `lexikanon-0.4.3/src/lexikanon/resources/dictionaries/mecab/ekon_v1.dic`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/stopwords/stopwords.py` & `lexikanon-0.4.3/src/lexikanon/stopwords/stopwords.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/tokenizers/base.py` & `lexikanon-0.4.3/src/lexikanon/tokenizers/base.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/tokenizers/mecab.py` & `lexikanon-0.4.3/src/lexikanon/tokenizers/mecab.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/tokenizers/nltk.py` & `lexikanon-0.4.3/src/lexikanon/tokenizers/nltk.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/utils/__init__.py` & `lexikanon-0.4.3/src/lexikanon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/utils/hangle.py` & `lexikanon-0.4.3/src/lexikanon/utils/hangle.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/utils/hanja/hangul.py` & `lexikanon-0.4.3/src/lexikanon/utils/hanja/hangul.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/utils/hanja/impl.py` & `lexikanon-0.4.3/src/lexikanon/utils/hanja/impl.py`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/src/lexikanon/utils/hanja/table.yml` & `lexikanon-0.4.3/src/lexikanon/utils/hanja/table.yml`

 * *Files identical despite different names*

### Comparing `lexikanon-0.4.2/PKG-INFO` & `lexikanon-0.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: lexikanon
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python Library for Tokenizers
 Home-page: https://lexikanon.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: ekonlpy (>=2.0.2,<3.0.0)
 Requires-Dist: ftfy (>=6.1.1,<7.0.0)
-Requires-Dist: hyfi (>=1.17.2,<2.0.0)
+Requires-Dist: hyfi (>=1.18.1,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Project-URL: Repository, https://github.com/entelecheia/lexikanon
 Description-Content-Type: text/markdown
 
 # Lexikanon
 
 [![pypi-image]][pypi-url]
```

