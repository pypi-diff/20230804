# Comparing `tmp/coopmongo-0.1.tar.gz` & `tmp/coopmongo-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coopmongo-0.1.tar", last modified: Thu Dec 22 23:03:40 2022, max compression
+gzip compressed data, was "coopmongo-0.2.tar", last modified: Fri Aug  4 21:53:48 2023, max compression
```

## Comparing `coopmongo-0.1.tar` & `coopmongo-0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-12-22 23:03:40.610102 coopmongo-0.1/
--rw-rw-rw-   0        0        0      784 2022-12-22 23:03:40.610102 coopmongo-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       55 2022-12-22 23:00:17.000000 coopmongo-0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-22 23:03:40.588138 coopmongo-0.1/coopmongo/
--rw-rw-rw-   0        0        0        0 2021-08-29 04:28:10.000000 coopmongo-0.1/coopmongo/__init__.py
--rw-rw-rw-   0        0        0       74 2022-12-22 22:54:31.000000 coopmongo-0.1/coopmongo/constants.py
--rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopmongo-0.1/coopmongo/errors.py
--rw-rw-rw-   0        0        0     3108 2022-12-22 22:25:55.000000 coopmongo-0.1/coopmongo/mongoCollectionHandler.py
--rw-rw-rw-   0        0        0     9274 2022-12-22 22:54:31.000000 coopmongo-0.1/coopmongo/mongo_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-22 23:03:40.608102 coopmongo-0.1/coopmongo.egg-info/
--rw-rw-rw-   0        0        0      784 2022-12-22 23:03:40.000000 coopmongo-0.1/coopmongo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2022-12-22 23:03:40.000000 coopmongo-0.1/coopmongo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-22 23:03:40.000000 coopmongo-0.1/coopmongo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-22 23:02:58.000000 coopmongo-0.1/coopmongo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      161 2022-12-22 23:03:40.000000 coopmongo-0.1/coopmongo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-12-22 23:03:40.000000 coopmongo-0.1/coopmongo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-22 23:03:40.611101 coopmongo-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1214 2022-12-22 22:59:29.000000 coopmongo-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 21:53:48.091520 coopmongo-0.2/
+-rw-rw-rw-   0        0        0      784 2023-08-04 21:53:48.090520 coopmongo-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2022-12-22 23:00:17.000000 coopmongo-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 21:53:48.058522 coopmongo-0.2/coopmongo/
+-rw-rw-rw-   0        0        0        0 2021-08-29 04:28:10.000000 coopmongo-0.2/coopmongo/__init__.py
+-rw-rw-rw-   0        0        0      101 2022-12-22 23:21:51.000000 coopmongo-0.2/coopmongo/constants.py
+-rw-rw-rw-   0        0        0      185 2022-12-06 20:55:58.000000 coopmongo-0.2/coopmongo/errors.py
+-rw-rw-rw-   0        0        0     3373 2023-07-11 16:52:57.000000 coopmongo-0.2/coopmongo/mongoCollectionHandler.py
+-rw-rw-rw-   0        0        0     6918 2023-08-04 21:23:40.000000 coopmongo-0.2/coopmongo/mongoCommandStore.py
+-rw-rw-rw-   0        0        0    10056 2023-07-11 16:52:57.000000 coopmongo-0.2/coopmongo/mongo_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 21:53:48.089522 coopmongo-0.2/coopmongo.egg-info/
+-rw-rw-rw-   0        0        0      784 2023-08-04 21:53:47.000000 coopmongo-0.2/coopmongo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2023-08-04 21:53:48.000000 coopmongo-0.2/coopmongo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 21:53:47.000000 coopmongo-0.2/coopmongo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-12-22 23:02:58.000000 coopmongo-0.2/coopmongo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      371 2023-08-04 21:53:47.000000 coopmongo-0.2/coopmongo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-04 21:53:47.000000 coopmongo-0.2/coopmongo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 21:53:48.091520 coopmongo-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1214 2023-08-04 21:53:31.000000 coopmongo-0.2/setup.py
```

### Comparing `coopmongo-0.1/PKG-INFO` & `coopmongo-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopmongo
-Version: 0.1
+Version: 0.2
 Summary: Basic interaction with a mongodb
 Home-page: https://github.com/tylertjburns/coopmongo
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopmongo-0.1/coopmongo/mongoCollectionHandler.py` & `coopmongo-0.2/coopmongo/mongoCollectionHandler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import pymongo as pmon
 import coopmongo.mongo_utils as utils
 from typing import List, Dict, Generic, TypeVar, Callable
+from coopmongo.errors import DuplicateException
 
 T = TypeVar('T')
 class MongoCollectionHandler(Generic[T]):
-    db_name: str
-    collection_name: str
-    client: pmon.MongoClient
-    facade_handler: utils.DocumentFacadeHandler
 
     def __init__(self,
                 db_name: str,
                 collection_name: str,
                 client: pmon.MongoClient = None,
                 uri: str = None,
                 facade_handler: utils.DocumentFacadeHandler = None,
+                dataclass_model: type = None,
                 sample_doc_gen: Callable[[...], T] = None
                 ):
         self.db_name = db_name
         self.collection_name = collection_name
         self.client = client if client is not None else utils.get_client(uri)
         self.facade_handler = facade_handler
+        self.dataclass_model = dataclass_model
         self.sample_doc_gen = sample_doc_gen
         self.tracked_time = {}
 
     @property
     def Collection(self):
         return utils.get_collection(db_name=self.db_name,
                                     collection_name=self.collection_name,
@@ -34,26 +33,32 @@
     def CollectionSize(self):
         return self.Collection.count_documents({})
 
     @property
     def CollectionSizeEstimated(self):
         return self.Collection.estimated_document_count({})
 
-    def add_items(self, items: List[T]) -> List[T]:
-        ret = utils.insert_documents(collection=self.Collection,
-                                     jsonable_objs=items,
-                                     facade_handler=self.facade_handler)
-        return ret
+    def add_items(self, items: List[T], fail_on_duplicate: bool = True) -> List[T]:
+        try:
+            ret = utils.insert_documents(collection=self.Collection,
+                                         jsonable_objs=items,
+                                         facade_handler=self.facade_handler)
+            return ret
+        except DuplicateException as e:
+            if fail_on_duplicate:
+                raise e
+
 
     def get_items(self,
                   ids: List[str] = None,
                   query: Dict=None,
                   limit: int = None) -> List[T]:
         retrieved = utils.get_documents(self.Collection,
                                         facade_handler=self.facade_handler,
+                                        dataclass_model=self.dataclass_model,
                                         query=query,
                                         ids=ids,
                                         limit=limit)
         return retrieved
 
     def find_item(self,
                   id: str) -> T:
```

### Comparing `coopmongo-0.1/coopmongo/mongo_utils.py` & `coopmongo-0.2/coopmongo/mongo_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 import time
 
 import pymongo.collection
 
-from constants import *
+from coopmongo.constants import *
 import urllib.parse
 import pymongo as pmon
 import pymongo.errors
-from typing import Dict, Protocol,List
+from typing import Dict, Protocol, List
 from pydantic import BaseModel, Field
 import uuid
 from fastapi.encoders import jsonable_encoder
-import errors as errors
+import coopmongo.errors as errors
 import logging
 from cooptools.decor import timer
 
-
 logger = logging.getLogger('MongoHandler')
 
 
 class Dictable(Protocol):
     def to_dict(self) -> Dict:
         raise NotImplementedError()
 
+
 class Jsonable(Dictable):
     def to_json(self) -> str:
         raise NotImplementedError()
 
+
 class Storable(Jsonable):
     id: str
 
+
 class DocumentFacade(BaseModel):
     obj_data: Dict
     id: str = Field(default_factory=uuid.uuid4, alias='_id')
 
+
 class DocumentFacadeHandler:
 
     def __init__(self,
                  obj_type: type,
                  facade_type: type = DocumentFacade,
                  data_field_name: str = 'obj_data'):
         self.facade_type = facade_type
@@ -57,41 +60,48 @@
         if query is not None:
             query = {f"{self.data_field_name}.{k}": v for k, v in query.items()}
         else:
             query = {}
 
         return query
 
+
 @timer(logger=logger, log_level=logging.DEBUG)
 def connection_string_uri(user, pw, uri_template) -> str:
     u = urllib.parse.quote(user)
     p = urllib.parse.quote(pw)
     return uri_template.replace(CONNECTION_STRING_USER, u).replace(CONNECTION_STRING_PASS, p)
 
+
 @timer(logger=logger, log_level=logging.DEBUG)
 def get_client(uri: str):
     return pmon.MongoClient(uri)
 
+
 @timer(logger=logger, log_level=logging.DEBUG)
 def get_database(db_name: str, client: pmon.MongoClient = None, uri: str = None):
     if client is None:
         client = get_client(uri)
 
     return client[db_name]
 
+
 @timer(logger=logger, log_level=logging.DEBUG)
 def get_collection(db_name: str, collection_name: str, client: pmon.MongoClient = None, uri: str = None):
     db = get_database(db_name, client=client, uri=uri)
     return db[collection_name]
 
+
 @timer(logger=logger, log_level=logging.INFO)
-def create_index(db_name: str, collection_name: str, index_name: pmon.collection._IndexKeyHint, client: pmon.MongoClient = None, uri: str = None):
+def create_index(db_name: str, collection_name: str, index_name: pmon.collection._IndexKeyHint,
+                 client: pmon.MongoClient = None, uri: str = None):
     collection = get_collection(db_name=db_name, collection_name=collection_name, uri=uri, client=client)
     collection.create_index(index_name)
 
+
 @timer(logger=logger, log_level=logging.DEBUG)
 def _apply_facade(jsonable_objs: List[Storable],
                   facade_handler: DocumentFacadeHandler = None):
     ready_objs = []
     # tic = time.perf_counter()
     for jsonable_obj in jsonable_objs:
         # try to convert the object using the facade (if exists)
@@ -101,37 +111,50 @@
         else:
             jsonable_obj = jsonable_obj.to_dict()
         ready_objs.append(jsonable_obj)
     # toc = time.perf_counter()
     # logger.debug(f"Time to apply facade to documents: {toc - tic} sec")
     return ready_objs
 
+
 @timer(logger=logger, log_level=logging.DEBUG)
 def _remove_facade(docs: List[Dict],
                    facade_handler: DocumentFacadeHandler = None):
     # tic = time.perf_counter()
 
     if facade_handler is not None:
         ret = [facade_handler.obj_from_doc(x) for x in docs]
     else:
         ret = docs
 
     # toc = time.perf_counter()
     # logger.debug(f"Time to remove facade from documents: {toc - tic} sec")
     return ret
 
+
+@timer(logger=logger, log_level=logging.DEBUG)
+def _convert_to_dataclass(docs: List[Dict],
+                          dataclass_model: type):
+    return [dataclass_model(**{k: v for k, v in args.items() if k != '_id'}) for args in docs]
+
+
 @timer(logger=logger, log_level=logging.INFO)
 def insert_documents(collection: pmon.collection.Collection,
                      jsonable_objs: List[Storable],
                      facade_handler: DocumentFacadeHandler = None):
-
     try:
         # handle facade conversion of the documents
         ready_objs = _apply_facade(jsonable_objs, facade_handler=facade_handler)
 
+        for obj in ready_objs:
+            if 'id' in obj.keys():
+                obj['_id'] = obj['id']
+            if 'obj_id' in obj.keys():
+                obj['_id'] = obj['obj_id']
+
         # insert the document(s)
         tic = time.perf_counter()
         if len(jsonable_objs) == 1:
             new_item = collection.insert_one(ready_objs[0])
             created_item = collection.find_one(
                 {"_id": new_item.inserted_id}
             )
@@ -152,48 +175,54 @@
         return created_items
 
     except pymongo.errors.DuplicateKeyError as e:
         raise errors.DuplicateException() from e
     except Exception as e:
         raise e
 
+
 @timer(logger=logger, log_level=logging.INFO)
 def get_documents(collection: pmon.collection.Collection,
                   facade_handler: DocumentFacadeHandler = None,
-                  query: Dict=None,
+                  dataclass_model: type = None,
+                  query: Dict = None,
                   ids: List[str] = None,
                   limit: int = 100):
     # resolve ids
     if ids is not None:
         id_query = {'id': {'$in': ids}}
         query = {**query, **id_query} if query is not None else id_query
 
     # resolve query
     query = query if facade_handler is None else facade_handler.resolve_facade_query(query)
 
-
     # collect items
     tic = time.perf_counter()
     if limit is not None:
         items = list(collection.find(query, limit=limit))
     else:
         items = list(collection.find(query))
     toc = time.perf_counter()
-    logger.debug(f"Time to retrieve documents: {toc-tic} sec")
+    logger.debug(f"Time to retrieve documents: {toc - tic} sec")
 
     # remove facade
-    items = _remove_facade(items, facade_handler=facade_handler)
-
+    if facade_handler is not None:
+        items = _remove_facade(items, facade_handler=facade_handler)
+    # convert dataclass
+    elif dataclass_model is not None:
+        items = _convert_to_dataclass(items,
+                                      dataclass_model=dataclass_model)
 
     return items
 
+
 @timer(logger=logger, log_level=logging.INFO)
 def get_document(collection: pmon.collection.Collection,
                  id: str,
-                 facade_handler: DocumentFacadeHandler=None):
+                 facade_handler: DocumentFacadeHandler = None):
     if facade_handler is None:
         field_name = "_id"
     else:
         field_name = f"{facade_handler.data_field_name}.id"
 
     item = collection.find_one({field_name: id})
     logger.info(f"Document retrieved: {item}")
@@ -202,31 +231,31 @@
         raise errors.NotFoundException()
 
     if facade_handler is not None:
         item = facade_handler.obj_from_doc(item)
 
     return item
 
+
 @timer(logger=logger, log_level=logging.INFO)
 def update_document(collection: pmon.collection.Collection,
                     id: str = None,
                     update_dict: Dict = None,
                     update_obj: Storable = None,
-                    facade_handler: DocumentFacadeHandler=None):
+                    facade_handler: DocumentFacadeHandler = None):
     if update_dict is None and update_obj is None:
         raise ValueError(f"At least one of values or object must be provided")
 
     if update_dict is not None and id is None:
         raise ValueError(f"Id must be provided if update_dict is being used")
 
     if update_obj is not None:
         update_dict = jsonable_encoder(update_obj.to_dict())
         id = update_obj.id
 
-
     # determine id field to be queried
     if facade_handler is None:
         field_name = "_id"
     else:
         field_name = f"{facade_handler.data_field_name}.id"
 
     # resolve update dict
@@ -241,33 +270,35 @@
 
     # retrieve updated doc
     updated_item = get_document(collection=collection, id=id, facade_handler=facade_handler)
     logger.info(f"Document updated: {updated_item}")
 
     return updated_item
 
+
 @timer(logger=logger, log_level=logging.INFO)
 def delete_document(collection: pmon.collection.Collection,
                     id: str,
-                    facade_handler: DocumentFacadeHandler=None):
+                    facade_handler: DocumentFacadeHandler = None):
     if facade_handler is None:
         field_name = "_id"
     else:
         field_name = f"{facade_handler.data_field_name}.id"
 
     delete_result = collection.delete_one({field_name: id})
     if delete_result.deleted_count == 0:
         raise errors.NotFoundException()
 
     logger.info(f"Document deleted: {id}")
 
     return True
 
+
 @timer(logger=logger, log_level=logging.INFO)
 def collection_length(collection: pmon.collection.Collection,
                       query: Dict = None):
-
     filter = {} if query is None else {query, {}}
     return collection.count_documents(filter=filter)
 
+
 if __name__ == "__main__":
     pass
```

### Comparing `coopmongo-0.1/coopmongo.egg-info/PKG-INFO` & `coopmongo-0.2/coopmongo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coopmongo
-Version: 0.1
+Version: 0.2
 Summary: Basic interaction with a mongodb
 Home-page: https://github.com/tylertjburns/coopmongo
 Author: tburns
 Author-email: tyler.tj.burns@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `coopmongo-0.1/setup.py` & `coopmongo-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     README = f.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(name='coopmongo',
-      version='0.1',
+      version='0.2',
       description='Basic interaction with a mongodb',
       url='https://github.com/tylertjburns/coopmongo',
       author='tburns',
       author_email='tyler.tj.burns@gmail.com',
       license='MIT',
       packages=setuptools.find_packages(),
       python_requires=">3.10",
```

