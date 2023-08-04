# Comparing `tmp/nbcpu-0.5.0.tar.gz` & `tmp/nbcpu-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbcpu-0.5.0.tar", max compression
+gzip compressed data, was "nbcpu-0.6.0.tar", max compression
```

## Comparing `nbcpu-0.5.0.tar` & `nbcpu-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1071 2023-07-29 20:34:59.258586 nbcpu-0.5.0/LICENSE
--rw-r--r--   0        0        0     3306 2023-07-29 20:34:59.258586 nbcpu-0.5.0/README.md
--rw-r--r--   0        0        0     2985 2023-07-29 20:35:26.435073 nbcpu-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      180 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/__cli__.py
--rw-r--r--   0        0        0      473 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/__init__.py
--rw-r--r--   0        0        0       22 2023-07-29 20:35:26.391072 nbcpu-0.5.0/src/nbcpu/_version.py
--rw-r--r--   0        0        0        0 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/conf/__init__.py
--rw-r--r--   0        0        0      275 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/conf/about/nbcpu.yaml
--rw-r--r--   0        0        0      674 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/conf/fetcher/khmer.yaml
--rw-r--r--   0        0        0      697 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/conf/fetcher/phnompenh.yaml
--rw-r--r--   0        0        0        0 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/fetcher/__init__.py
--rw-r--r--   0        0        0    12088 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/fetcher/base.py
--rw-r--r--   0        0        0     4049 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/fetcher/khmer.py
--rw-r--r--   0        0        0     4704 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/fetcher/phnompenh.py
--rw-r--r--   0        0        0        0 2023-07-29 20:34:59.262586 nbcpu-0.5.0/src/nbcpu/py.typed
--rw-r--r--   0        0        0     4049 1970-01-01 00:00:00.000000 nbcpu-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-04 09:10:49.582825 nbcpu-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3306 2023-08-04 09:10:49.582825 nbcpu-0.6.0/README.md
+-rw-r--r--   0        0        0     3006 2023-08-04 09:11:22.114725 nbcpu-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/__cli__.py
+-rw-r--r--   0        0        0      484 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-04 09:11:22.070725 nbcpu-0.6.0/src/nbcpu/_version.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/conf/__init__.py
+-rw-r--r--   0        0        0      275 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/conf/about/nbcpu.yaml
+-rw-r--r--   0        0        0      676 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/conf/fetcher/khmer.yaml
+-rw-r--r--   0        0        0      698 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/conf/fetcher/phnompenh.yaml
+-rw-r--r--   0        0        0        0 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/fetcher/__init__.py
+-rw-r--r--   0        0        0    11793 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/fetcher/base.py
+-rw-r--r--   0        0        0     4049 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/fetcher/khmer.py
+-rw-r--r--   0        0        0     4704 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/fetcher/phnompenh.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:10:49.586825 nbcpu-0.6.0/src/nbcpu/py.typed
+-rw-r--r--   0        0        0     4091 1970-01-01 00:00:00.000000 nbcpu-0.6.0/PKG-INFO
```

### Comparing `nbcpu-0.5.0/LICENSE` & `nbcpu-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbcpu-0.5.0/README.md` & `nbcpu-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nbcpu-0.5.0/pyproject.toml` & `nbcpu-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [tool.poetry]
 name = "nbcpu"
-version = "0.5.0"
+version = "0.6.0"
 description = "Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.github.io/nbcpu"
 repository = "https://github.com/entelecheia/nbcpu"
 readme = "README.md"
 packages = [{ include = "nbcpu", from = "src" }]
 
 [tool.poetry.scripts]
 nbcpu = 'nbcpu.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 click = "^8.1.3"
-hyfi = "^1.12.5"
+hyfi = "^1.18.1"
 # hyfi = { path = "../hyfi", develop = true }
+lexikanon = "^0.4.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `nbcpu-0.5.0/src/nbcpu/conf/fetcher/khmer.yaml` & `nbcpu-0.6.0/src/nbcpu/conf/fetcher/khmer.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 _target_: nbcpu.fetcher.khmer.KhmerFetcher
 _config_name_: khmer
-_config_group_: fetcher
+_config_group_: /fetcher
 search_url: https://www.khmertimeskh.com/page/{page}/?s={keyword}
 search_keywords:
 - NBC
 - Exchange Rate
 - De-dollarization
 - Inflation
 - GDP
@@ -20,15 +20,15 @@
 - Bank
 - Economy
 - Securities Exchange
 - National Bank of Cambodia
 start_page: 1
 max_num_pages: 2
 max_num_articles: 10
-output_dir: workspace/datasets/fetcher/khmer
+output_dir: workspace/datasets//fetcher/khmer
 link_filename: links.jsonl
 article_filename: articles.jsonl
 overwrite_existing: false
 key_field: url
 delay_between_requests: 0.0
 num_workers: 1
 print_every: 10
```

### Comparing `nbcpu-0.5.0/src/nbcpu/conf/fetcher/phnompenh.yaml` & `nbcpu-0.6.0/src/nbcpu/conf/fetcher/phnompenh.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 _target_: nbcpu.fetcher.phnompenh.PhnompenhFetcher
 _config_name_: phnompenh
-_config_group_: fetcher
+_config_group_: /fetcher
 search_url: https://phnompenhpost.com/search/node/{keyword}?page={page}
 search_keywords:
 - NBC
 - Exchange Rate
 - De-dollarization
 - Inflation
 - GDP
```

### Comparing `nbcpu-0.5.0/src/nbcpu/fetcher/base.py` & `nbcpu-0.6.0/src/nbcpu/fetcher/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 
 class BaseFetcher(BaseModel):
     """
     Base Fetcher
     """
 
     _config_name_: str = "base"
-    _config_group_: str = "fetcher"
+    _config_group_: str = "/fetcher"
 
     search_url: str = ""
     search_keywords: List[str] = []
     start_page: int = 1
     max_num_pages: Optional[int] = 2
     max_num_articles: Optional[int] = 10
-    output_dir: str = f"workspace/datasets/{_config_group_}/{_config_name_}"
+    output_dir: str = f"workspace/datasets{_config_group_}/{_config_name_}"
     link_filename: str = "links.jsonl"
     article_filename: str = "articles.jsonl"
     overwrite_existing: bool = False
     key_field: str = "url"
     delay_between_requests: float = 0.0
     num_workers: int = 1
     print_every: int = 10
@@ -117,23 +117,18 @@
             parse_page_func=parse_page_func,
             link_urls=link_urls,
             start_page=self.start_page,
             max_num_pages=self.max_num_pages,
             link_filepath=self.link_filepath_tmp,
             delay_between_requests=self.delay_between_requests,
         )
-        if num_workers > 1:
-            links = self._fetch_links_mp(
-                num_workers,
-                fetch_links_func,
-            )
-        else:
-            for keyword in self.search_keywords_encoded:
-                links = fetch_links_func(keyword)
-        if links:
+        if links := self._fetch_links_mp(
+            num_workers,
+            fetch_links_func,
+        ):
             self.save_links(links)
         else:
             logger.info("No more links found")
 
     def save_links(self, links: List[dict]):
         self._links.extend(links)
         original_len = len(self._links)
@@ -170,19 +165,15 @@
             overwrite_existing=self.overwrite_existing,
             article_filepath=self.article_filepath_tmp,
             max_num_articles=self.max_num_articles,
             delay_between_requests=self.delay_between_requests,
             print_every=self.print_every,
             verbose=self.verbose,
         )
-        if num_workers > 1:
-            articles = self._fetch_articles_mp(num_workers, fetch_articles_func)
-        else:
-            articles = fetch_articles_func(self.links)
-        if articles:
+        if articles := self._fetch_articles_mp(num_workers, fetch_articles_func):
             self.save_articles(articles)
         else:
             logger.info("No more articles found")
 
     def save_articles(self, articles: List[dict]):
         self._articles.extend(articles)
         original_len = len(self._articles)
```

### Comparing `nbcpu-0.5.0/src/nbcpu/fetcher/khmer.py` & `nbcpu-0.6.0/src/nbcpu/fetcher/khmer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 class KhmerFetcher(BaseFetcher):
     """
     Fetcher for Khmer Times.
     """
 
     _config_name_: str = "khmer"
-    _config_group_: str = "fetcher"
-    output_dir: str = f"workspace/datasets/{_config_group_}/{_config_name_}"
+    _config_group_: str = "/fetcher"
+    output_dir: str = f"workspace/datasets{_config_group_}/{_config_name_}"
 
     search_url: str = "https://www.khmertimeskh.com/page/{page}/?s={keyword}"
     search_keywords: List[str] = [
         "NBC",
         "Exchange Rate",
         "De-dollarization",
         "Inflation",
```

### Comparing `nbcpu-0.5.0/src/nbcpu/fetcher/phnompenh.py` & `nbcpu-0.6.0/src/nbcpu/fetcher/phnompenh.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 class PhnompenhFetcher(BaseFetcher):
     """
     Fetcher for Phnom Penh Post.
     """
 
     _config_name_: str = "phnompenh"
-    _config_group_: str = "fetcher"
-    output_dir: str = f"workspace/datasets/{_config_group_}/{_config_name_}"
+    _config_group_: str = "/fetcher"
+    output_dir: str = f"workspace/datasets{_config_group_}/{_config_name_}"
 
     start_page: int = 0
     delay_between_requests: float = 20.0
     search_url: str = "https://phnompenhpost.com/search/node/{keyword}?page={page}"
     search_keywords: List[str] = [
         "NBC",
         "Exchange Rate",
```

### Comparing `nbcpu-0.5.0/PKG-INFO` & `nbcpu-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nbcpu
-Version: 0.5.0
+Version: 0.6.0
 Summary: Quantifying Central Bank Policy Uncertainty in a Highly Dollarized Economy: A Topic Modeling Approach
 Home-page: https://entelecheia.github.io/nbcpu
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
-Requires-Dist: hyfi (>=1.12.5,<2.0.0)
+Requires-Dist: hyfi (>=1.18.1,<2.0.0)
+Requires-Dist: lexikanon (>=0.4.2,<0.5.0)
 Project-URL: Repository, https://github.com/entelecheia/nbcpu
 Description-Content-Type: text/markdown
 
 # Measuring Central Bank Policy Uncertainty
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

