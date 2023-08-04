# Comparing `tmp/citrusdb-0.5.2.tar.gz` & `tmp/citrusdb-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citrusdb-0.5.2.tar", last modified: Fri Aug  4 10:07:18 2023, max compression
+gzip compressed data, was "citrusdb-0.5.3.tar", last modified: Fri Aug  4 10:33:46 2023, max compression
```

## Comparing `citrusdb-0.5.2.tar` & `citrusdb-0.5.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.619748 citrusdb-0.5.2/
--rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.5.2/LICENSE
--rw-r--r--   0 debabrata   (501) staff       (20)     2300 2023-08-04 10:07:18.619629 citrusdb-0.5.2/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)     1717 2023-08-04 10:05:38.000000 citrusdb-0.5.2/README.md
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.616413 citrusdb-0.5.2/citrusdb/
--rw-r--r--   0 debabrata   (501) staff       (20)      281 2023-06-16 18:28:46.000000 citrusdb-0.5.2/citrusdb/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.617290 citrusdb-0.5.2/citrusdb/api/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.2/citrusdb/api/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     4050 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/api/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     9141 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/api/local.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.617407 citrusdb-0.5.2/citrusdb/db/
--rw-r--r--   0 debabrata   (501) staff       (20)     1426 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/db/__init__.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.617597 citrusdb-0.5.2/citrusdb/db/index/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.2/citrusdb/db/index/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-12 11:56:56.000000 citrusdb-0.5.2/citrusdb/db/index/hnswlib.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.617927 citrusdb-0.5.2/citrusdb/db/postgres/
--rw-r--r--   0 debabrata   (501) staff       (20)     7767 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/db/postgres/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1866 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/db/postgres/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1533 2023-06-27 16:19:28.000000 citrusdb-0.5.2/citrusdb/db/postgres/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.618327 citrusdb-0.5.2/citrusdb/db/sqlite/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.2/citrusdb/db/sqlite/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     5989 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/db/sqlite/db.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1836 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/db/sqlite/queries.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1382 2023-06-27 16:19:28.000000 citrusdb-0.5.2/citrusdb/db/sqlite/query_builder.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.618835 citrusdb-0.5.2/citrusdb/embedding/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.2/citrusdb/embedding/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.5.2/citrusdb/embedding/openai.py
--rw-r--r--   0 debabrata   (501) staff       (20)      297 2023-08-04 09:37:45.000000 citrusdb-0.5.2/citrusdb/embedding/utils.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.619197 citrusdb-0.5.2/citrusdb/utils/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.2/citrusdb/utils/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)      236 2023-06-27 16:19:28.000000 citrusdb-0.5.2/citrusdb/utils/types.py
--rw-r--r--   0 debabrata   (501) staff       (20)     1479 2023-08-04 10:05:38.000000 citrusdb-0.5.2/citrusdb/utils/utils.py
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.616938 citrusdb-0.5.2/citrusdb.egg-info/
--rw-r--r--   0 debabrata   (501) staff       (20)     2300 2023-08-04 10:07:18.000000 citrusdb-0.5.2/citrusdb.egg-info/PKG-INFO
--rw-r--r--   0 debabrata   (501) staff       (20)      820 2023-08-04 10:07:18.000000 citrusdb-0.5.2/citrusdb.egg-info/SOURCES.txt
--rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-08-04 10:07:18.000000 citrusdb-0.5.2/citrusdb.egg-info/dependency_links.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       79 2023-08-04 10:07:18.000000 citrusdb-0.5.2/citrusdb.egg-info/requires.txt
--rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-08-04 10:07:18.000000 citrusdb-0.5.2/citrusdb.egg-info/top_level.txt
-drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:07:18.619482 citrusdb-0.5.2/cloud-temp/
--rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.5.2/cloud-temp/__init__.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2248 2023-06-16 13:03:05.000000 citrusdb-0.5.2/cloud-temp/index.py
--rw-r--r--   0 debabrata   (501) staff       (20)     2826 2023-06-16 18:18:23.000000 citrusdb-0.5.2/cloud-temp/main-pg.py
--rw-r--r--   0 debabrata   (501) staff       (20)      724 2023-08-04 10:07:00.000000 citrusdb-0.5.2/pyproject.toml
--rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-08-04 10:07:18.619779 citrusdb-0.5.2/setup.cfg
--rw-r--r--   0 debabrata   (501) staff       (20)      964 2023-08-04 10:07:14.000000 citrusdb-0.5.2/setup.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.346307 citrusdb-0.5.3/
+-rw-r--r--   0 debabrata   (501) staff       (20)    11346 2023-04-17 04:38:54.000000 citrusdb-0.5.3/LICENSE
+-rw-r--r--   0 debabrata   (501) staff       (20)     2300 2023-08-04 10:33:46.346156 citrusdb-0.5.3/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)     1717 2023-08-04 10:05:38.000000 citrusdb-0.5.3/README.md
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.343104 citrusdb-0.5.3/citrusdb/
+-rw-r--r--   0 debabrata   (501) staff       (20)      281 2023-06-16 18:28:46.000000 citrusdb-0.5.3/citrusdb/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.343987 citrusdb-0.5.3/citrusdb/api/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.3/citrusdb/api/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     4050 2023-08-04 10:05:38.000000 citrusdb-0.5.3/citrusdb/api/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     9141 2023-08-04 10:05:38.000000 citrusdb-0.5.3/citrusdb/api/local.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.344092 citrusdb-0.5.3/citrusdb/db/
+-rw-r--r--   0 debabrata   (501) staff       (20)     1426 2023-08-04 10:05:38.000000 citrusdb-0.5.3/citrusdb/db/__init__.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.344278 citrusdb-0.5.3/citrusdb/db/index/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.3/citrusdb/db/index/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1605 2023-06-12 11:56:56.000000 citrusdb-0.5.3/citrusdb/db/index/hnswlib.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.344599 citrusdb-0.5.3/citrusdb/db/postgres/
+-rw-r--r--   0 debabrata   (501) staff       (20)     8174 2023-08-04 10:31:37.000000 citrusdb-0.5.3/citrusdb/db/postgres/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1866 2023-08-04 10:05:38.000000 citrusdb-0.5.3/citrusdb/db/postgres/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1533 2023-06-27 16:19:28.000000 citrusdb-0.5.3/citrusdb/db/postgres/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.345022 citrusdb-0.5.3/citrusdb/db/sqlite/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.3/citrusdb/db/sqlite/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     5989 2023-08-04 10:05:38.000000 citrusdb-0.5.3/citrusdb/db/sqlite/db.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1836 2023-08-04 10:05:38.000000 citrusdb-0.5.3/citrusdb/db/sqlite/queries.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1382 2023-06-27 16:19:28.000000 citrusdb-0.5.3/citrusdb/db/sqlite/query_builder.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.345318 citrusdb-0.5.3/citrusdb/embedding/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-05-15 17:55:08.000000 citrusdb-0.5.3/citrusdb/embedding/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      402 2023-05-15 17:55:08.000000 citrusdb-0.5.3/citrusdb/embedding/openai.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      297 2023-08-04 09:37:45.000000 citrusdb-0.5.3/citrusdb/embedding/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.345600 citrusdb-0.5.3/citrusdb/utils/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-12 11:56:56.000000 citrusdb-0.5.3/citrusdb/utils/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      236 2023-06-27 16:19:28.000000 citrusdb-0.5.3/citrusdb/utils/types.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     1479 2023-08-04 10:05:38.000000 citrusdb-0.5.3/citrusdb/utils/utils.py
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.343644 citrusdb-0.5.3/citrusdb.egg-info/
+-rw-r--r--   0 debabrata   (501) staff       (20)     2300 2023-08-04 10:33:46.000000 citrusdb-0.5.3/citrusdb.egg-info/PKG-INFO
+-rw-r--r--   0 debabrata   (501) staff       (20)      820 2023-08-04 10:33:46.000000 citrusdb-0.5.3/citrusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)        1 2023-08-04 10:33:46.000000 citrusdb-0.5.3/citrusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       79 2023-08-04 10:33:46.000000 citrusdb-0.5.3/citrusdb.egg-info/requires.txt
+-rw-r--r--   0 debabrata   (501) staff       (20)       20 2023-08-04 10:33:46.000000 citrusdb-0.5.3/citrusdb.egg-info/top_level.txt
+drwxr-xr-x   0 debabrata   (501) staff       (20)        0 2023-08-04 10:33:46.345953 citrusdb-0.5.3/cloud-temp/
+-rw-r--r--   0 debabrata   (501) staff       (20)        0 2023-06-01 10:48:15.000000 citrusdb-0.5.3/cloud-temp/__init__.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2248 2023-06-16 13:03:05.000000 citrusdb-0.5.3/cloud-temp/index.py
+-rw-r--r--   0 debabrata   (501) staff       (20)     2826 2023-06-16 18:18:23.000000 citrusdb-0.5.3/cloud-temp/main-pg.py
+-rw-r--r--   0 debabrata   (501) staff       (20)      724 2023-08-04 10:33:24.000000 citrusdb-0.5.3/pyproject.toml
+-rw-r--r--   0 debabrata   (501) staff       (20)       38 2023-08-04 10:33:46.346344 citrusdb-0.5.3/setup.cfg
+-rw-r--r--   0 debabrata   (501) staff       (20)      964 2023-08-04 10:33:35.000000 citrusdb-0.5.3/setup.py
```

### Comparing `citrusdb-0.5.2/LICENSE` & `citrusdb-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/PKG-INFO` & `citrusdb-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.5.2
+Version: 0.5.3
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `citrusdb-0.5.2/README.md` & `citrusdb-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb/api/index.py` & `citrusdb-0.5.3/citrusdb/api/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb/api/local.py` & `citrusdb-0.5.3/citrusdb/api/local.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb/db/__init__.py` & `citrusdb-0.5.3/citrusdb/db/__init__.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb/db/index/hnswlib.py` & `citrusdb-0.5.3/citrusdb/db/index/hnswlib.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb/db/postgres/db.py` & `citrusdb-0.5.3/citrusdb/db/postgres/db.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,19 +111,30 @@
         name: Name of index
         include: Dictionary of columns to be returned
         """
         index_details = self.get_index_details(name)
         if index_details is None:
             raise ValueError(f"Index '{name}' does not exist")
 
+        cols = [sql.Identifier("id")]
+        if include["document"]:
+            cols.append(sql.Identifier("text"))
+            if include["metadata"]:
+                cols.append(sql.Identifier("metadata"))
+        elif include["metadata"]:
+            cols.append(sql.Identifier("metadata"))
+
         index_id = index_details[0]
         parameters = (index_id,)
         with self._pool.connection() as conn:
             with conn.cursor() as cur:
-                cur.execute(queries.GET_ALL_VECTORS, parameters)
+                query = sql.SQL(queries.GET_ALL_VECTORS).format(
+                    sql.SQL(", ").join(cols)
+                )
+                cur.execute(query, parameters)
                 rows = cur.fetchall()
                 return [convert_row_to_dict(row=row, include=include, with_embedding=True) for row in rows]
 
     def get_vector_ids_of_results(
         self,
         name: str,
         results: List[List[int]],
```

### Comparing `citrusdb-0.5.2/citrusdb/db/postgres/queries.py` & `citrusdb-0.5.3/citrusdb/db/postgres/queries.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb/db/postgres/query_builder.py` & `citrusdb-0.5.3/citrusdb/db/postgres/query_builder.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb/db/sqlite/db.py` & `citrusdb-0.5.3/citrusdb/db/sqlite/db.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb/db/sqlite/queries.py` & `citrusdb-0.5.3/citrusdb/db/sqlite/queries.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb/db/sqlite/query_builder.py` & `citrusdb-0.5.3/citrusdb/db/sqlite/query_builder.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb/utils/utils.py` & `citrusdb-0.5.3/citrusdb/utils/utils.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/citrusdb.egg-info/PKG-INFO` & `citrusdb-0.5.3/citrusdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citrusdb
-Version: 0.5.2
+Version: 0.5.3
 Summary: open-source vector database. store and retrieve embeddings for your next project!
 Home-page: https://github.com/0xDebabrata/citrus
 Author: Debabrata Mondal
 Author-email: Debabrata Mondal <debabrata.js@protonmail.com>
 Project-URL: Homepage, https://github.com/0xDebabrata/citrus
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `citrusdb-0.5.2/citrusdb.egg-info/SOURCES.txt` & `citrusdb-0.5.3/citrusdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/cloud-temp/index.py` & `citrusdb-0.5.3/cloud-temp/index.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/cloud-temp/main-pg.py` & `citrusdb-0.5.3/cloud-temp/main-pg.py`

 * *Files identical despite different names*

### Comparing `citrusdb-0.5.2/pyproject.toml` & `citrusdb-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "citrusdb"
-version = "0.5.2"
+version = "0.5.3"
 
 authors = [
   { name="Debabrata Mondal", email="debabrata.js@protonmail.com" },
 ]
 description = "open-source vector database. store and retrieve embeddings for your next project!"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `citrusdb-0.5.2/setup.py` & `citrusdb-0.5.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="citrusdb",
-    version="0.5.2",
+    version="0.5.3",
     author="Debabrata Mondal",
     author_email="debabrata.js@protonmail.com",
     description="(distributed) vector database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0xDebabrata/citrus",
     packages=(
```

