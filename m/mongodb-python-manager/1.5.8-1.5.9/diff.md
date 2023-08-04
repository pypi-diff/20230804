# Comparing `tmp/mongodb_python_manager-1.5.8.tar.gz` & `tmp/mongodb_python_manager-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongodb_python_manager-1.5.8.tar", max compression
+gzip compressed data, was "mongodb_python_manager-1.5.9.tar", max compression
```

## Comparing `mongodb_python_manager-1.5.8.tar` & `mongodb_python_manager-1.5.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1080 2023-07-27 09:59:52.406521 mongodb_python_manager-1.5.8/LICENSE
--rw-r--r--   0        0        0     5051 2023-07-27 09:59:52.406740 mongodb_python_manager-1.5.8/README.md
--rw-r--r--   0        0        0    10043 2023-07-31 10:34:49.730009 mongodb_python_manager-1.5.8/mongodb_python_manager/__init__.py
--rw-r--r--   0        0        0      779 2023-07-31 10:34:39.727575 mongodb_python_manager-1.5.8/pyproject.toml
--rw-r--r--   0        0        0     6037 1970-01-01 00:00:00.000000 mongodb_python_manager-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-27 09:59:52.406521 mongodb_python_manager-1.5.9/LICENSE
+-rw-r--r--   0        0        0     5051 2023-07-27 09:59:52.406740 mongodb_python_manager-1.5.9/README.md
+-rw-r--r--   0        0        0    10035 2023-08-04 10:41:58.264912 mongodb_python_manager-1.5.9/mongodb_python_manager/__init__.py
+-rw-r--r--   0        0        0      779 2023-08-04 10:41:50.215345 mongodb_python_manager-1.5.9/pyproject.toml
+-rw-r--r--   0        0        0     6037 1970-01-01 00:00:00.000000 mongodb_python_manager-1.5.9/PKG-INFO
```

### Comparing `mongodb_python_manager-1.5.8/LICENSE` & `mongodb_python_manager-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mongodb_python_manager-1.5.8/README.md` & `mongodb_python_manager-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `mongodb_python_manager-1.5.8/mongodb_python_manager/__init__.py` & `mongodb_python_manager-1.5.9/mongodb_python_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             raise ValueError("MongoDB database name is not set")
 
         self.uri = f"mongodb+srv://{mongo_db_user}:{mongo_db_password}@{mongo_db_cluster}/{mongodb_db_name}?retryWrites=true&w=majority"
         self.mongodb_db_name = mongodb_db_name
         self.mongodb_collection_name = None
 
     def __version__(self):
-        return "1.5.8"
+        return "1.5.9"
 
     def get_client(self) -> tuple((pymongo.MongoClient, str)):
         """
         Get client to MongoDB
         """
         client = pymongo.MongoClient(
             self.uri,
@@ -72,15 +72,15 @@
         """
         Get collection from MongoDB database and collection specified in the constructor of the class MongoDB
         """
         self.client = self.get_client()
         if self.mongodb_collection_name is None:
             raise ValueError("Collection name is not set")
         else:
-            return self.client.get_database(self.mongodb_db_name).get_collection(self.mongodb_collection_name)
+            return self.get_db().get_collection(self.mongodb_collection_name)
 
     def get_uri(self) -> str:
         """
         Get MongoDB URI
         """
         return self.uri
 
@@ -124,15 +124,15 @@
         collection = self.get_collection()
         collection_name = self.get_collection_name()
         item_id = f"{collection_name.lower()}-{str(uuid.uuid4())}-{datetime.datetime.now().strftime('%Y_%m_%d_%H_%M_%S')}"
 
         if not "date" in item.keys():
             item["date"] = datetime.datetime.now()
 
-        item[f"{collection_name}_id"] = item_id
+        item[f"{collection_name.lower()}_id"] = item_id
 
         collection.insert_one(item)
 
     def insert_many_document_in_collection(self, items: list):
         """
         Insert document to MongoDB database and collection specified in the constructor of the class MongoDB
 
@@ -150,21 +150,22 @@
         """
         collection = self.get_collection()
         collection_name = self.get_collection_name()
         items_id = [
             f"{collection_name.lower()}-{str(uuid.uuid4())}-{datetime.datetime.now().strftime('%Y_%m_%d_%H_%M_%S')}" for item in items]
 
         logger.info(
-            f"Add to {len(items)} items in {collection_name} id & date.")
+            f"Add to {len(items)} items in {collection_name} id & date."
+        )
 
         for item, item_id in tqdm(zip(items, items_id)):
             if not "date" in item.keys():
                 item["date"] = datetime.datetime.now()
 
-            item[f"{collection_name}_id"] = item_id
+            item[f"{collection_name.lower()}_id"] = item_id
 
         collection.insert_many(items)
         logger.info(f"Insert {len(items)} items in {collection_name}.")
 
     def update_document_in_collection(self, item: dict, collection_id: str, collection_id_name: str = None):
         """
         Update document in MongoDB database and collection specified in the constructor of the class MongoDB
```

### Comparing `mongodb_python_manager-1.5.8/pyproject.toml` & `mongodb_python_manager-1.5.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mongodb-python-manager"
-version = "1.5.8"
+version = "1.5.9"
 description = "The `MongoDBManager` class is a wrapper around the `pymongo` package, designed to simplify the usage of MongoDB in Python applications. It provides convenient methods for connecting to a MongoDB cluster, accessing a specific database and collection, and performing common CRUD operations."
 authors = ["louis_giron <louis@giron-dom.eu>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "mongodb_python_manager"}]
 
 [tool.poetry.dependencies]
```

### Comparing `mongodb_python_manager-1.5.8/PKG-INFO` & `mongodb_python_manager-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongodb-python-manager
-Version: 1.5.8
+Version: 1.5.9
 Summary: The `MongoDBManager` class is a wrapper around the `pymongo` package, designed to simplify the usage of MongoDB in Python applications. It provides convenient methods for connecting to a MongoDB cluster, accessing a specific database and collection, and performing common CRUD operations.
 License: MIT
 Author: louis_giron
 Author-email: louis@giron-dom.eu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

