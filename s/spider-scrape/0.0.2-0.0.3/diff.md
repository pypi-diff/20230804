# Comparing `tmp/spider_scrape-0.0.2.tar.gz` & `tmp/spider_scrape-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spider_scrape-0.0.2.tar", max compression
+gzip compressed data, was "spider_scrape-0.0.3.tar", max compression
```

## Comparing `spider_scrape-0.0.2.tar` & `spider_scrape-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1118 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/LICENSE
--rw-r--r--   0        0        0      379 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/README.md
--rw-r--r--   0        0        0      802 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      190 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/spider_scrape/__init__.py
--rw-r--r--   0        0        0     1853 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/spider_scrape/arango_db.py
--rw-r--r--   0        0        0     1735 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/spider_scrape/bs.py
--rw-r--r--   0        0        0      455 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/spider_scrape/db.py
--rw-r--r--   0        0        0      746 2023-07-30 11:02:59.116864 spider_scrape-0.0.2/spider_scrape/scraper.py
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 spider_scrape-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1118 2023-08-04 07:10:56.741370 spider_scrape-0.0.3/LICENSE
+-rw-r--r--   0        0        0      379 2023-08-04 07:10:56.741370 spider_scrape-0.0.3/README.md
+-rw-r--r--   0        0        0      854 2023-08-04 07:10:56.741370 spider_scrape-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      190 2023-08-04 07:10:56.741370 spider_scrape-0.0.3/spider_scrape/__init__.py
+-rw-r--r--   0        0        0     2062 2023-08-04 07:10:56.741370 spider_scrape-0.0.3/spider_scrape/arango_db.py
+-rw-r--r--   0        0        0     1735 2023-08-04 07:10:56.741370 spider_scrape-0.0.3/spider_scrape/bs.py
+-rw-r--r--   0        0        0      455 2023-08-04 07:10:56.741370 spider_scrape-0.0.3/spider_scrape/db.py
+-rw-r--r--   0        0        0        0 2023-08-04 07:10:56.741370 spider_scrape-0.0.3/spider_scrape/py.typed
+-rw-r--r--   0        0        0      746 2023-08-04 07:10:56.741370 spider_scrape-0.0.3/spider_scrape/scraper.py
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 spider_scrape-0.0.3/PKG-INFO
```

### Comparing `spider_scrape-0.0.2/LICENSE` & `spider_scrape-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spider_scrape-0.0.2/pyproject.toml` & `spider_scrape-0.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spider-scrape"
-version = "0.0.2"
+version = "0.0.3"
 description = "Website Scrape Tool"
 authors = ["Philip May <philip@may.la>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "spider_scrape"}]
 
 [build-system]
@@ -20,14 +20,17 @@
 mdformat = "*"
 
 [tool.poetry.group.lint.dependencies]
 black = "*"
 ruff = "*"
 mypy = "*"
 
+[tool.poetry.group.test.dependencies]
+pytest = "*"
+
 [tool.poetry.extras]
 arango = ["python-arango"]
 
 [tool.black]
 line-length = 119
 target-versions = ["py38", "py39", "py310", "py311"]
```

### Comparing `spider_scrape-0.0.2/spider_scrape/arango_db.py` & `spider_scrape-0.0.3/spider_scrape/arango_db.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # This software is distributed under the terms of the MIT license
 # which is available at https://opensource.org/licenses/MIT
 
 """ArangoDB tools package."""
 
 from contextlib import closing
-from typing import Sequence, Union
+from typing import Optional, Sequence, Union
 
-from arango import ArangoClient
+from arango import ArangoClient  # type: ignore
 from attr import define, field
 
 from spider_scrape.db import DataManager
 
 
 @define
 class ArangoDataManager(DataManager):
     hosts: Union[str, Sequence[str]]
     db_name: str
     username: str
     password: str
     collection_name: str
     attribute_name: str
     batch_size: int = field(default=20)
+    aql_overwrite: Optional[str] = field(default=None)
 
     def get_arango_client(self):
         arango_client = ArangoClient(hosts=self.hosts)
         return arango_client
 
     def get_connection(self, arango_client):
         connection = arango_client.db(self.db_name, username=self.username, password=self.password)
@@ -34,16 +35,20 @@
         with closing(self.get_arango_client()) as arango_client:
             connection = self.get_connection(arango_client)
             bind_vars = {
                 "@coll": self.collection_name,
                 "attribute": self.attribute_name,
                 "batch_size": self.batch_size,
             }
+            if self.aql_overwrite is None:
+                aql = "FOR doc IN @@coll FILTER !HAS(doc, @attribute) LIMIT @batch_size RETURN doc"
+            else:
+                aql = self.aql_overwrite
             cursor = connection.aql.execute(
-                "FOR doc IN @@coll FILTER !HAS(doc, @attribute) LIMIT @batch_size RETURN doc",
+                aql,
                 bind_vars=bind_vars,
                 batch_size=self.batch_size,
             )
             with closing(cursor) as closing_cursor:
                 batch = closing_cursor.batch()
         return batch
```

### Comparing `spider_scrape-0.0.2/spider_scrape/bs.py` & `spider_scrape-0.0.3/spider_scrape/bs.py`

 * *Files identical despite different names*

### Comparing `spider_scrape-0.0.2/spider_scrape/scraper.py` & `spider_scrape-0.0.3/spider_scrape/scraper.py`

 * *Files identical despite different names*

### Comparing `spider_scrape-0.0.2/PKG-INFO` & `spider_scrape-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spider-scrape
-Version: 0.0.2
+Version: 0.0.3
 Summary: Website Scrape Tool
 License: MIT
 Author: Philip May
 Author-email: philip@may.la
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

