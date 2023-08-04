# Comparing `tmp/retakesearch-0.1.27.tar.gz` & `tmp/retakesearch-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.1.27.tar", max compression
+gzip compressed data, was "retakesearch-0.1.28.tar", max compression
```

## Comparing `retakesearch-0.1.27.tar` & `retakesearch-0.1.28.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-08-03 04:48:37.874287 retakesearch-0.1.27/README.md
--rw-r--r--   0        0        0      429 2023-08-03 04:49:02.458485 retakesearch-0.1.27/pyproject.toml
--rw-r--r--   0        0        0      174 2023-08-03 04:48:37.874287 retakesearch-0.1.27/retakesearch/__init__.py
--rw-r--r--   0        0        0     1818 2023-08-03 04:48:37.874287 retakesearch-0.1.27/retakesearch/client.py
--rw-r--r--   0        0        0     4523 2023-08-03 04:48:37.874287 retakesearch-0.1.27/retakesearch/index.py
--rw-r--r--   0        0        0      159 2023-08-03 04:48:37.874287 retakesearch-0.1.27/retakesearch/search.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 retakesearch-0.1.27/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 16:44:52.106936 retakesearch-0.1.28/README.md
+-rw-r--r--   0        0        0      429 2023-08-03 16:45:14.551557 retakesearch-0.1.28/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-08-03 16:44:52.106936 retakesearch-0.1.28/retakesearch/__init__.py
+-rw-r--r--   0        0        0     1818 2023-08-03 16:44:52.106936 retakesearch-0.1.28/retakesearch/client.py
+-rw-r--r--   0        0        0     4654 2023-08-03 16:44:52.106936 retakesearch-0.1.28/retakesearch/index.py
+-rw-r--r--   0        0        0      159 2023-08-03 16:44:52.106936 retakesearch-0.1.28/retakesearch/search.py
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 retakesearch-0.1.28/PKG-INFO
```

### Comparing `retakesearch-0.1.27/retakesearch/client.py` & `retakesearch-0.1.28/retakesearch/client.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.1.27/retakesearch/index.py` & `retakesearch-0.1.28/retakesearch/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,26 +14,32 @@
 
 
 class Table:
     def __init__(
         self,
         name: str,
         columns: List[str],
+        schema: str = "public",
         transform: Optional[Dict[str, Any]] = None,
         relationship: Optional[Dict[str, Any]] = None,
         children: Optional[List["Table"]] = None,
     ):
         self.name = name
         self.columns = columns
         self.transform = transform
+        self.schema = schema
         self.relationship = relationship
         self.children = children
 
     def to_schema(self) -> Dict[str, Any]:
-        schema: Dict[str, Any] = {"table": self.name, "columns": self.columns}
+        schema: Dict[str, Any] = {
+            "table": self.name,
+            "columns": self.columns,
+            "schema": self.schema,
+        }
 
         if self.transform:
             schema["transform"] = self.transform
 
         if self.relationship:
             schema["relationship"] = self.relationship
```

### Comparing `retakesearch-0.1.27/PKG-INFO` & `retakesearch-0.1.28/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.1.27
+Version: 0.1.28
 Summary: Python client for Retake: universal search infra for developers
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

