# Comparing `tmp/salinic-0.2.3.tar.gz` & `tmp/salinic-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salinic-0.2.3.tar", max compression
+gzip compressed data, was "salinic-0.2.4.tar", max compression
```

## Comparing `salinic-0.2.3.tar` & `salinic-0.2.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    10226 2023-08-04 04:18:35.196754 salinic-0.2.3/LICENSE
--rw-r--r--   0        0        0     1725 2023-08-04 04:18:35.196754 salinic-0.2.3/README.md
--rw-r--r--   0        0        0      470 2023-08-04 04:18:35.196754 salinic-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      321 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/__init__.py
--rw-r--r--   0        0        0      344 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/engine.py
--rw-r--r--   0        0        0      285 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/field.py
--rw-r--r--   0        0        0     1250 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/schema.py
--rw-r--r--   0        0        0      228 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/search.py
--rw-r--r--   0        0        0      118 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/search_query.py
--rw-r--r--   0        0        0     3840 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/session.py
--rw-r--r--   0        0        0      564 2023-08-04 04:18:35.196754 salinic-0.2.3/salinic/utils.py
--rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 salinic-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    10226 2023-08-04 05:46:24.918937 salinic-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1695 2023-08-04 05:46:24.918937 salinic-0.2.4/README.md
+-rw-r--r--   0        0        0      470 2023-08-04 05:46:24.922937 salinic-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/__init__.py
+-rw-r--r--   0        0        0      344 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/engine.py
+-rw-r--r--   0        0        0      285 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/field.py
+-rw-r--r--   0        0        0     1250 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/schema.py
+-rw-r--r--   0        0        0      228 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/search.py
+-rw-r--r--   0        0        0      118 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/search_query.py
+-rw-r--r--   0        0        0     3840 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/session.py
+-rw-r--r--   0        0        0      601 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/types.py
+-rw-r--r--   0        0        0      564 2023-08-04 05:46:24.922937 salinic-0.2.4/salinic/utils.py
+-rw-r--r--   0        0        0     2252 1970-01-01 00:00:00.000000 salinic-0.2.4/PKG-INFO
```

### Comparing `salinic-0.2.3/LICENSE` & `salinic-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `salinic-0.2.3/README.md` & `salinic-0.2.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,32 +14,32 @@
     from typing import Optional
     from typing_extensions import Annotated
 
     from salinic.field import IdField, KeywordField, TextField
     from salinic.schema import Schema
 
 
-    class IndexEntity(Schema):
+    class Index(Schema):
         id: Annotated[str, IdField(primary_key=True)]
         user_id: str
         parent_id: str
         title: Annotated[str, TextField()]
-        text: Annotated[Optional[str], TextField(default=None)]
-        tags: Annotated[Optional[list[str]], KeywordField(default=None)]
+        text: Annotated[Optional[str], TextField()] = None
+        tags: Annotated[Optional[list[str]], KeywordField()] = []
 
 
 Index your documents:
 
         from salinic import Session, create_engine
 
         engine = create_engine("xapian:////search_index")
         session = Session(engine)
 
         for document in all_your_documents():
-            entity = IndexEntity(
+            entity = Index(
                 id=str(document.id),
                 user_id=str(document.user_id),
                 parent_id=document.parent_id,
                 title=document.title,
                 text=document.text,
                 tags=document.tags
             )
@@ -49,11 +49,11 @@
 Search your documents:
 
         from salinic import Session, create_engine
 
         engine = create_engine("xapian:////search_index")
         session = Session(engine)
 
-        sq = Search(IndexEntity).query(" your query string ")
+        sq = Search(Index).query(" your query string ")
 
         for found in session.exec(sq):
             print(found)  # found is instance of IndexEntity
```

### Comparing `salinic-0.2.3/salinic/schema.py` & `salinic-0.2.4/salinic/schema.py`

 * *Files identical despite different names*

### Comparing `salinic-0.2.3/salinic/session.py` & `salinic-0.2.4/salinic/session.py`

 * *Files identical despite different names*

### Comparing `salinic-0.2.3/salinic/utils.py` & `salinic-0.2.4/salinic/utils.py`

 * *Files identical despite different names*

### Comparing `salinic-0.2.3/PKG-INFO` & `salinic-0.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salinic
-Version: 0.2.3
+Version: 0.2.4
 Summary: Search abstraction layer
 Author: Eugen Ciur
 Author-email: eugen@papermerge.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -30,32 +30,32 @@
     from typing import Optional
     from typing_extensions import Annotated
 
     from salinic.field import IdField, KeywordField, TextField
     from salinic.schema import Schema
 
 
-    class IndexEntity(Schema):
+    class Index(Schema):
         id: Annotated[str, IdField(primary_key=True)]
         user_id: str
         parent_id: str
         title: Annotated[str, TextField()]
-        text: Annotated[Optional[str], TextField(default=None)]
-        tags: Annotated[Optional[list[str]], KeywordField(default=None)]
+        text: Annotated[Optional[str], TextField()] = None
+        tags: Annotated[Optional[list[str]], KeywordField()] = []
 
 
 Index your documents:
 
         from salinic import Session, create_engine
 
         engine = create_engine("xapian:////search_index")
         session = Session(engine)
 
         for document in all_your_documents():
-            entity = IndexEntity(
+            entity = Index(
                 id=str(document.id),
                 user_id=str(document.user_id),
                 parent_id=document.parent_id,
                 title=document.title,
                 text=document.text,
                 tags=document.tags
             )
@@ -65,12 +65,12 @@
 Search your documents:
 
         from salinic import Session, create_engine
 
         engine = create_engine("xapian:////search_index")
         session = Session(engine)
 
-        sq = Search(IndexEntity).query(" your query string ")
+        sq = Search(Index).query(" your query string ")
 
         for found in session.exec(sq):
             print(found)  # found is instance of IndexEntity
```

