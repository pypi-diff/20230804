# Comparing `tmp/salinic-0.2.2.tar.gz` & `tmp/salinic-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salinic-0.2.2.tar", max compression
+gzip compressed data, was "salinic-0.2.3.tar", max compression
```

## Comparing `salinic-0.2.2.tar` & `salinic-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10226 2023-07-31 05:58:32.255512 salinic-0.2.2/LICENSE
--rw-r--r--   0        0        0     1624 2023-07-31 05:58:32.255512 salinic-0.2.2/README.md
--rw-r--r--   0        0        0      470 2023-07-31 05:58:32.255512 salinic-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      321 2023-07-31 05:58:32.255512 salinic-0.2.2/salinic/__init__.py
--rw-r--r--   0        0        0      344 2023-07-31 05:58:32.255512 salinic-0.2.2/salinic/engine.py
--rw-r--r--   0        0        0      285 2023-07-31 05:58:32.255512 salinic-0.2.2/salinic/field.py
--rw-r--r--   0        0        0      534 2023-07-31 05:58:32.255512 salinic-0.2.2/salinic/schema.py
--rw-r--r--   0        0        0      228 2023-07-31 05:58:32.255512 salinic-0.2.2/salinic/search.py
--rw-r--r--   0        0        0      118 2023-07-31 05:58:32.255512 salinic-0.2.2/salinic/search_query.py
--rw-r--r--   0        0        0     3213 2023-07-31 05:58:32.255512 salinic-0.2.2/salinic/session.py
--rw-r--r--   0        0        0       67 2023-07-31 05:58:32.255512 salinic-0.2.2/salinic/utils.py
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 salinic-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    10226 2023-08-04 04:18:35.196754 salinic-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1725 2023-08-04 04:18:35.196754 salinic-0.2.3/README.md
+-rw-r--r--   0        0        0      470 2023-08-04 04:18:35.196754 salinic-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/__init__.py
+-rw-r--r--   0        0        0      344 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/engine.py
+-rw-r--r--   0        0        0      285 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/field.py
+-rw-r--r--   0        0        0     1250 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/schema.py
+-rw-r--r--   0        0        0      228 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/search.py
+-rw-r--r--   0        0        0      118 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/search_query.py
+-rw-r--r--   0        0        0     3840 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/session.py
+-rw-r--r--   0        0        0      564 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/utils.py
+-rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 salinic-0.2.3/PKG-INFO
```

### Comparing `salinic-0.2.2/LICENSE` & `salinic-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `salinic-0.2.2/README.md` & `salinic-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [![Tests](https://github.com/papermerge/salinic/actions/workflows/tests.yml/badge.svg)](https://github.com/papermerge/salinic/actions/workflows/tests.yml)
 
 # Salinic
 
-Salinic - provides modular search. It features a unified, familiar API that
+Salinic - provides modular search. It features a unified API that
 allows you to plug in different search backends.
-Currently it supports only Xapian backend.
-
+Currently, it supports only Xapian backend.
 
 
 ## Usage
 
 Declare your search schema:
 
     from typing import Optional
+    from typing_extensions import Annotated
 
     from salinic.field import IdField, KeywordField, TextField
     from salinic.schema import Schema
 
 
     class IndexEntity(Schema):
-        id: str = IdField(primary_key=True)
+        id: Annotated[str, IdField(primary_key=True)]
         user_id: str
         parent_id: str
-        title: str = TextField()
-        text: Optional[str] = TextField()
-        tags: list[str] | None = KeywordField()
+        title: Annotated[str, TextField()]
+        text: Annotated[Optional[str], TextField(default=None)]
+        tags: Annotated[Optional[list[str]], KeywordField(default=None)]
 
 
 Index your documents:
 
         from salinic import Session, create_engine
 
         engine = create_engine("xapian:////search_index")
```

### Comparing `salinic-0.2.2/PKG-INFO` & `salinic-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salinic
-Version: 0.2.2
+Version: 0.2.3
 Summary: Search abstraction layer
 Author: Eugen Ciur
 Author-email: eugen@papermerge.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,37 +14,37 @@
 Requires-Dist: xapianpy (>=1.4.22.post2305071405,<2.0.0)
 Description-Content-Type: text/markdown
 
 [![Tests](https://github.com/papermerge/salinic/actions/workflows/tests.yml/badge.svg)](https://github.com/papermerge/salinic/actions/workflows/tests.yml)
 
 # Salinic
 
-Salinic - provides modular search. It features a unified, familiar API that
+Salinic - provides modular search. It features a unified API that
 allows you to plug in different search backends.
-Currently it supports only Xapian backend.
-
+Currently, it supports only Xapian backend.
 
 
 ## Usage
 
 Declare your search schema:
 
     from typing import Optional
+    from typing_extensions import Annotated
 
     from salinic.field import IdField, KeywordField, TextField
     from salinic.schema import Schema
 
 
     class IndexEntity(Schema):
-        id: str = IdField(primary_key=True)
+        id: Annotated[str, IdField(primary_key=True)]
         user_id: str
         parent_id: str
-        title: str = TextField()
-        text: Optional[str] = TextField()
-        tags: list[str] | None = KeywordField()
+        title: Annotated[str, TextField()]
+        text: Annotated[Optional[str], TextField(default=None)]
+        tags: Annotated[Optional[list[str]], KeywordField(default=None)]
 
 
 Index your documents:
 
         from salinic import Session, create_engine
 
         engine = create_engine("xapian:////search_index")
```

