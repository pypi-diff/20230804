# Comparing `tmp/pyfireconsole-0.0.2.tar.gz` & `tmp/pyfireconsole-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfireconsole-0.0.2.tar", last modified: Thu Aug  3 09:03:37 2023, max compression
+gzip compressed data, was "pyfireconsole-0.0.3.tar", last modified: Fri Aug  4 09:52:26 2023, max compression
```

## Comparing `pyfireconsole-0.0.2.tar` & `pyfireconsole-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-03 09:03:37.834541 pyfireconsole-0.0.2/
--rw-r--r--   0 tanji      (501) staff       (20)     1069 2023-08-02 11:27:52.000000 pyfireconsole-0.0.2/LICENSE
--rw-r--r--   0 tanji      (501) staff       (20)     5939 2023-08-03 09:03:37.834360 pyfireconsole-0.0.2/PKG-INFO
--rw-r--r--   0 tanji      (501) staff       (20)     5424 2023-08-03 08:59:22.000000 pyfireconsole-0.0.2/README.md
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-03 09:03:37.831397 pyfireconsole-0.0.2/pyfireconsole/
--rw-r--r--   0 tanji      (501) staff       (20)      211 2023-08-03 05:24:39.000000 pyfireconsole-0.0.2/pyfireconsole/__init__.py
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-03 09:03:37.832332 pyfireconsole-0.0.2/pyfireconsole/console/
--rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-03 05:24:39.000000 pyfireconsole-0.0.2/pyfireconsole/console/__init__.py
--rw-r--r--   0 tanji      (501) staff       (20)     1796 2023-08-03 05:24:39.000000 pyfireconsole-0.0.2/pyfireconsole/console/pyfireconsole.py
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-03 09:03:37.832876 pyfireconsole-0.0.2/pyfireconsole/db/
--rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.2/pyfireconsole/db/__init__.py
--rw-r--r--   0 tanji      (501) staff       (20)     1245 2023-08-02 11:34:51.000000 pyfireconsole-0.0.2/pyfireconsole/db/connection.py
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-03 09:03:37.833254 pyfireconsole-0.0.2/pyfireconsole/models/
--rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.2/pyfireconsole/models/__init__.py
--rw-r--r--   0 tanji      (501) staff       (20)     4408 2023-08-03 05:26:37.000000 pyfireconsole-0.0.2/pyfireconsole/models/firestore_model.py
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-03 09:03:37.833920 pyfireconsole-0.0.2/pyfireconsole/queries/
--rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.2/pyfireconsole/queries/__init__.py
--rw-r--r--   0 tanji      (501) staff       (20)     1763 2023-08-03 08:39:40.000000 pyfireconsole-0.0.2/pyfireconsole/queries/query.py
--rw-r--r--   0 tanji      (501) staff       (20)      824 2023-08-02 11:34:51.000000 pyfireconsole-0.0.2/pyfireconsole/queries/query_manager.py
-drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-03 09:03:37.832078 pyfireconsole-0.0.2/pyfireconsole.egg-info/
--rw-r--r--   0 tanji      (501) staff       (20)     5939 2023-08-03 09:03:37.000000 pyfireconsole-0.0.2/pyfireconsole.egg-info/PKG-INFO
--rw-r--r--   0 tanji      (501) staff       (20)      561 2023-08-03 09:03:37.000000 pyfireconsole-0.0.2/pyfireconsole.egg-info/SOURCES.txt
--rw-r--r--   0 tanji      (501) staff       (20)        1 2023-08-03 09:03:37.000000 pyfireconsole-0.0.2/pyfireconsole.egg-info/dependency_links.txt
--rw-r--r--   0 tanji      (501) staff       (20)      130 2023-08-03 09:03:37.000000 pyfireconsole-0.0.2/pyfireconsole.egg-info/requires.txt
--rw-r--r--   0 tanji      (501) staff       (20)       14 2023-08-03 09:03:37.000000 pyfireconsole-0.0.2/pyfireconsole.egg-info/top_level.txt
--rw-r--r--   0 tanji      (501) staff       (20)      470 2023-08-03 09:03:20.000000 pyfireconsole-0.0.2/pyproject.toml
--rw-r--r--   0 tanji      (501) staff       (20)       38 2023-08-03 09:03:37.834590 pyfireconsole-0.0.2/setup.cfg
--rw-r--r--   0 tanji      (501) staff       (20)      892 2023-08-03 09:03:22.000000 pyfireconsole-0.0.2/setup.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.830631 pyfireconsole-0.0.3/
+-rw-r--r--   0 tanji      (501) staff       (20)     1069 2023-08-02 11:27:52.000000 pyfireconsole-0.0.3/LICENSE
+-rw-r--r--   0 tanji      (501) staff       (20)     5880 2023-08-04 09:52:26.830449 pyfireconsole-0.0.3/PKG-INFO
+-rw-r--r--   0 tanji      (501) staff       (20)     5366 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/README.md
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.826426 pyfireconsole-0.0.3/pyfireconsole/
+-rw-r--r--   0 tanji      (501) staff       (20)      251 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/__init__.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.827908 pyfireconsole-0.0.3/pyfireconsole/console/
+-rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-03 05:24:39.000000 pyfireconsole-0.0.3/pyfireconsole/console/__init__.py
+-rw-r--r--   0 tanji      (501) staff       (20)     1797 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/console/pyfireconsole.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.828415 pyfireconsole-0.0.3/pyfireconsole/db/
+-rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.3/pyfireconsole/db/__init__.py
+-rw-r--r--   0 tanji      (501) staff       (20)     1285 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/db/connection.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.828821 pyfireconsole-0.0.3/pyfireconsole/models/
+-rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.3/pyfireconsole/models/__init__.py
+-rw-r--r--   0 tanji      (501) staff       (20)     5013 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/models/pyfire_model.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.830167 pyfireconsole-0.0.3/pyfireconsole/queries/
+-rw-r--r--   0 tanji      (501) staff       (20)        0 2023-08-02 11:34:51.000000 pyfireconsole-0.0.3/pyfireconsole/queries/__init__.py
+-rw-r--r--   0 tanji      (501) staff       (20)      959 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/queries/abstract_query.py
+-rw-r--r--   0 tanji      (501) staff       (20)      371 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/queries/all_query.py
+-rw-r--r--   0 tanji      (501) staff       (20)      540 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/queries/get_query.py
+-rw-r--r--   0 tanji      (501) staff       (20)      768 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/queries/query_runner.py
+-rw-r--r--   0 tanji      (501) staff       (20)      651 2023-08-04 09:47:45.000000 pyfireconsole-0.0.3/pyfireconsole/queries/where_query.py
+drwxr-xr-x   0 tanji      (501) staff       (20)        0 2023-08-04 09:52:26.827576 pyfireconsole-0.0.3/pyfireconsole.egg-info/
+-rw-r--r--   0 tanji      (501) staff       (20)     5880 2023-08-04 09:52:26.000000 pyfireconsole-0.0.3/pyfireconsole.egg-info/PKG-INFO
+-rw-r--r--   0 tanji      (501) staff       (20)      673 2023-08-04 09:52:26.000000 pyfireconsole-0.0.3/pyfireconsole.egg-info/SOURCES.txt
+-rw-r--r--   0 tanji      (501) staff       (20)        1 2023-08-04 09:52:26.000000 pyfireconsole-0.0.3/pyfireconsole.egg-info/dependency_links.txt
+-rw-r--r--   0 tanji      (501) staff       (20)      130 2023-08-04 09:52:26.000000 pyfireconsole-0.0.3/pyfireconsole.egg-info/requires.txt
+-rw-r--r--   0 tanji      (501) staff       (20)       14 2023-08-04 09:52:26.000000 pyfireconsole-0.0.3/pyfireconsole.egg-info/top_level.txt
+-rw-r--r--   0 tanji      (501) staff       (20)      520 2023-08-04 09:48:03.000000 pyfireconsole-0.0.3/pyproject.toml
+-rw-r--r--   0 tanji      (501) staff       (20)       38 2023-08-04 09:52:26.830677 pyfireconsole-0.0.3/setup.cfg
+-rw-r--r--   0 tanji      (501) staff       (20)      892 2023-08-04 09:49:06.000000 pyfireconsole-0.0.3/setup.py
```

### Comparing `pyfireconsole-0.0.2/LICENSE` & `pyfireconsole-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfireconsole-0.0.2/PKG-INFO` & `pyfireconsole-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pyfireconsole
-Version: 0.0.2
+Version: 0.0.3
 Summary: An interactive console for Firestore based on Python ORM
 Home-page: https://github.com/tan-z-tan/pyfireconsole
 Author: Makoto Tanji
 Author-email: tanji.makoto@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyFireConsole
 <h1 style="text-align: center;">
-  <img src="https://raw.githubusercontent.com/tan-z-tan/pyfireconsole/main/logo.png" alt="PyFireConsole" height="120">
+  <img src="https://raw.githubusercontent.com/tan-z-tan/pyfireconsole/main/logo.png" alt="PyFireConsole">
 </h1>
 
 ## Introduction
 Inspired by Rails console, PyFireConsole provides a seamless interface to Google's Firestore in Python, simplifying tasks such as connection, ORM, and data associations. It makes managing Firestore a breeze.
 
 ## Features
 - Model Definition and ORM: Define your Firestore data models within Python and use object-relational mapping (ORM) for easier data manipulation and querying.
@@ -31,36 +30,36 @@
 pip install pyfireconsole
 ```
 
 ## Getting Started
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.firestore_model import Collection, DocumentRef, FirestoreModel
+from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
 from pyfireconsole.db.connection import FirestoreConnection
 
 # Define your models 
-class User(FirestoreModel):
+class User(PyfireDoc):
     name: str
     email: str
 
-class Publisher(FirestoreModel):
+class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
-class Tag(FirestoreModel):
+class Tag(PyfireDoc):
     name: str
 
-class Book(FirestoreModel):
+class Book(PyfireDoc):
     title: str
     user_id: str
-    FirestoreModel.belongs_to(User)  # Make accessible via book.user
+    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
-    tags: Collection[Tag] = Collection(Tag)
+    tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
 
 # Initialize FirestoreConnection using your default credentials of gcloud. (use `gcloud auth application-default login` or set GOOGLE_APPLICATION_CREDENTIALS)
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 
 # Or you can specify service_account_key_path
@@ -111,36 +110,36 @@
 This feature is inspired by the Rails console.
 
 How to setup interactive console:
 
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.firestore_model import Collection, DocumentRef, FirestoreModel
+from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
 from pyfireconsole.db.connection import FirestoreConnection
 from pyfireconsole import PyFireConsole
 
-class User(FirestoreModel):
+class User(PyfireDoc):
     name: str
     email: str
 
-class Publisher(FirestoreModel):
+class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
-class Tag(FirestoreModel):
+class Tag(PyfireDoc):
     name: str
 
-class Book(FirestoreModel):
+class Book(PyfireDoc):
     title: str
     user_id: str
-    FirestoreModel.belongs_to(User)  # Make accessible via book.user
+    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
-    tags: Collection[Tag] = Collection(Tag)
+    tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 PyFireConsole().run()
 ```
```

### Comparing `pyfireconsole-0.0.2/README.md` & `pyfireconsole-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-# PyFireConsole
 <h1 style="text-align: center;">
-  <img src="https://raw.githubusercontent.com/tan-z-tan/pyfireconsole/main/logo.png" alt="PyFireConsole" height="120">
+  <img src="https://raw.githubusercontent.com/tan-z-tan/pyfireconsole/main/logo.png" alt="PyFireConsole">
 </h1>
 
 ## Introduction
 Inspired by Rails console, PyFireConsole provides a seamless interface to Google's Firestore in Python, simplifying tasks such as connection, ORM, and data associations. It makes managing Firestore a breeze.
 
 ## Features
 - Model Definition and ORM: Define your Firestore data models within Python and use object-relational mapping (ORM) for easier data manipulation and querying.
@@ -16,36 +15,36 @@
 pip install pyfireconsole
 ```
 
 ## Getting Started
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.firestore_model import Collection, DocumentRef, FirestoreModel
+from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
 from pyfireconsole.db.connection import FirestoreConnection
 
 # Define your models 
-class User(FirestoreModel):
+class User(PyfireDoc):
     name: str
     email: str
 
-class Publisher(FirestoreModel):
+class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
-class Tag(FirestoreModel):
+class Tag(PyfireDoc):
     name: str
 
-class Book(FirestoreModel):
+class Book(PyfireDoc):
     title: str
     user_id: str
-    FirestoreModel.belongs_to(User)  # Make accessible via book.user
+    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
-    tags: Collection[Tag] = Collection(Tag)
+    tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
 
 # Initialize FirestoreConnection using your default credentials of gcloud. (use `gcloud auth application-default login` or set GOOGLE_APPLICATION_CREDENTIALS)
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 
 # Or you can specify service_account_key_path
@@ -96,36 +95,36 @@
 This feature is inspired by the Rails console.
 
 How to setup interactive console:
 
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.firestore_model import Collection, DocumentRef, FirestoreModel
+from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
 from pyfireconsole.db.connection import FirestoreConnection
 from pyfireconsole import PyFireConsole
 
-class User(FirestoreModel):
+class User(PyfireDoc):
     name: str
     email: str
 
-class Publisher(FirestoreModel):
+class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
-class Tag(FirestoreModel):
+class Tag(PyfireDoc):
     name: str
 
-class Book(FirestoreModel):
+class Book(PyfireDoc):
     title: str
     user_id: str
-    FirestoreModel.belongs_to(User)  # Make accessible via book.user
+    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
-    tags: Collection[Tag] = Collection(Tag)
+    tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 PyFireConsole().run()
 ```
 
 
@@ -143,8 +142,8 @@
 
 ## Contributing
 Your contributions to PyFireConsole are warmly welcomed! Feel free to submit a pull request directly if you have any improvements or features to suggest. For any questions or issues, please create an issue on Github. Thank you for your interest in improving PyFireConsole!
 
 ## License
 PyFireConsole is released under the MIT License.
 
-This means you are free to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software. This permission is granted provided that the above copyright notice and this permission notice are included in all copies or substantial portions of the software.
+This means you are free to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software. This permission is granted provided that the above copyright notice and this permission notice are included in all copies or substantial portions of the software.
```

### Comparing `pyfireconsole-0.0.2/pyfireconsole/console/pyfireconsole.py` & `pyfireconsole-0.0.3/pyfireconsole/console/pyfireconsole.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Optional
-from IPython.terminal.embed import embed
-import os
-import sys
 import glob
 import importlib.util
 import inspect
+import os
+import sys
+from typing import Optional
+
+from IPython.terminal.embed import embed
 
 
 class PyFireConsole:
     def __init__(self, model_dir: Optional[str] = None):
         self.model_dir = model_dir
 
     def run(self, reset_global=False):
```

### Comparing `pyfireconsole-0.0.2/pyfireconsole/db/connection.py` & `pyfireconsole-0.0.3/pyfireconsole/db/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-import google.auth
-from google.cloud import firestore
-from google.oauth2.service_account import Credentials as ServiceAccountCredentials
 from typing import Optional
 
+from google.cloud import firestore
+from google.oauth2.service_account import Credentials as ServiceAccountCredentials  # type: ignore
+
 
 class FirestoreConnection:
     _instance: Optional['FirestoreConnection'] = None
+    db: Optional[firestore.Client] = None
 
     def __new__(cls, *args, **kwargs):
         if cls._instance is None:
             cls._instance = super().__new__(cls, *args, **kwargs)
             cls._instance.db = None  # デフォルトではdbオブジェクトはNoneとして初期化
         return cls._instance
```

### Comparing `pyfireconsole-0.0.2/pyfireconsole/models/firestore_model.py` & `pyfireconsole-0.0.3/pyfireconsole/models/pyfire_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,125 @@
 from typing import Generic, Iterable, Optional, Type, TypeVar
-from pydantic import BaseModel
+
 import inflect
-from pyfireconsole.queries.query_manager import QueryManager
+from pydantic import BaseModel
 
+from pyfireconsole.queries.query_runner import QueryRunner
 
-ModelType = TypeVar('ModelType', bound='FirestoreModel')
+ModelType = TypeVar('ModelType', bound='PyfireDoc')
 
 
-class Collection(Generic[ModelType]):
-    parent_model: Optional['FirestoreModel'] = None
-    model_class: Optional[Type[ModelType]] = None
-    _collection: Optional[Iterable[ModelType]] = None
+class PyfireCollection(Generic[ModelType]):
+    model_class: Type[ModelType]
+    _parent_model: Optional['PyfireDoc']
+    _collection: Iterable[ModelType] = []
 
     def __init__(self, model_class: Type[ModelType]):
         self.model_class = model_class
+        self._parent_model = None
 
-    def __iter__(self):
-        self._collection = self.parent_model._get_subcollection(self)
-        for model in self._collection:
-            model._parent = self.parent_model
-            yield model
+    def obj_ref_key(self) -> str:
+        """ Represents the key of firestore entity """
+        return self.obj_collection_name()
 
-    @classmethod
-    def __get_validators__(cls):
-        breakpoint()
-        yield cls.validate
+    def set_parent(self, parent_model: 'PyfireDoc'):
+        self._parent_model = parent_model
 
-    @classmethod
-    def validate(cls, v, _):
-        breakpoint()
-        if isinstance(v, cls):
-            return v
-
-        if isinstance(v, Type) and issubclass(v, FirestoreModel):
-            return cls(v)
-
-        raise ValueError("Invalid value for a Collection field")
-
-    def set_parent(self, parent_model: 'FirestoreModel'):
-        self.parent_model = parent_model
-        self._collection = None  # Invalidate cached data
+    def obj_collection_name(self) -> str:
+        leaf_collection_name = self.model_class.collection_name()
+        if self._parent_model is None:
+            return leaf_collection_name  # e.g. "users"
+        else:
+            return f"{self._parent_model.obj_ref_key()}/{leaf_collection_name}"  # e.g. "users/123/books"
+
+    def __iter__(self):
+        docs = QueryRunner(self.obj_ref_key()).all()
+
+        for doc in docs:
+            obj = self.model_class(**doc)
+            obj._parent = self._parent_model
+            yield obj
+
+    def where(self, field: str, operator: str, value: str) -> 'PyfireCollection[ModelType]':
+        coll = PyfireCollection(self.model_class)
+        if self._parent_model is not None:
+            coll.set_parent(self._parent_model)
+        docs = QueryRunner(self.obj_collection_name()).where(field, operator, value)
+        coll._collection = [self.model_class.model_validate(d) for d in docs]
+        return coll
+
+    def __str__(self) -> str:
+        if self._parent_model is None:
+            return f"{self.__class__.__name__}[{self.model_class.__name__}]"
+        return f"{self.__class__.__name__}[{self.model_class.__name__}](parent={self._parent_model.__class__.__name__})"
 
 
 class DocumentRef(BaseModel, Generic[ModelType]):
     path: str
 
     # TODO: Implement reference class so that we can do this like this:
     # book.user_ref.get() => User object
 
 
-class FirestoreModel(BaseModel):
+class PyfireDoc(BaseModel):
     class Config:
         arbitrary_types_allowed = True
 
-    id: str
-    _parent: Optional['FirestoreModel'] = None  # when a model is a subcollection, this is the parent model
+    id: str  # Firestore document id
+    _parent: Optional[PyfireCollection] = None  # when a model is a subcollection, this is the parent model
 
     def __init__(self, **data):
         super().__init__(**data)
         self._setup_collections()
 
     def _setup_collections(self):
         # Set the parent of all the collections
         for name, _ in self.__annotations__.items():
-            attr = getattr(self, name)
-            if isinstance(attr, Collection):
+            attr = getattr(self, name, None)
+            if isinstance(attr, PyfireCollection):
                 attr.set_parent(self)
             elif isinstance(attr, DocumentRef):
                 pass
 
-    def _get_subcollection(self, collection: Collection) -> Iterable[ModelType]:
-        collection_name = f"{self.obj_collection_name()}/{self.id}/{inflect.engine().plural(collection.model_class.__name__).lower()}"
-        query_manager = QueryManager(collection_name)
-        for id, data in query_manager.all():
-            yield collection.model_class(**data, id=id)
-
-    def obj_collection_name(self) -> str:
+    def obj_ref_key(self) -> str:
+        """ Represents the key of firestore entity """
         db_name = self.__class__.collection_name()
         if self._parent is None:
-            return db_name
+            return f"{db_name}/{self.id}"
         else:
-            return f"{self._parent.obj_collection_name()}/{self._parent.id}/{db_name}"
+            return f"{self._parent.obj_ref_key()}/{db_name}/{self.id}"
 
-    def save(self):
-        raise NotImplementedError("save() is not implemented")
+    def save(self) -> None:
+        raise NotImplementedError
 
     @classmethod
-    def find(cls, id: str, allow_empty: bool = False) -> ModelType:
-        query_manager = QueryManager(cls.collection_name())
-        d = query_manager.get(id)
+    def find(cls, id: str, allow_empty: bool = False) -> 'PyfireDoc':
+        d = QueryRunner(cls.collection_name()).get(id)
 
         if d is None:
             if allow_empty:
-                empty_doc = cls.model_construct(id=id)
-                empty_doc._setup_collections()
-                return empty_doc
+                return cls.empty_doc(id)
             else:
                 raise ValueError(f"Could not find {cls.__name__} with id {id}")
         return cls.model_validate(d)
 
     @classmethod
-    def empty_doc(cls, id) -> ModelType:
-        return cls(id=id)
+    def empty_doc(cls, id) -> 'PyfireDoc':
+        doc = cls.model_construct(id=id)
+        doc._setup_collections()
+        return doc
 
     @classmethod
-    def where(cls, field: str, operator: str, value: str) -> list[ModelType]:
-        query_manager = QueryManager(cls.collection_name())
-        docs = query_manager.where(field, operator, value)
-        return [cls.model_validate(d) for d in docs]
+    def where(cls, field: str, operator: str, value: str) -> PyfireCollection['PyfireDoc']:
+        coll = PyfireCollection(cls)
+        docs = QueryRunner(cls.collection_name()).where(field, operator, value)
+        coll._collection = [cls.model_validate(d) for d in docs]
+        return coll
+        # docs = QueryRunner(cls.collection_name()).where(field, operator, value)
+        # return [cls.model_validate(d) for d in docs]
 
     @classmethod
     def collection_name(cls) -> str:
         """
         Override this method to change the name of the collection in Firestore
         """
         return inflect.engine().plural(cls.__name__).lower()
@@ -124,7 +132,10 @@
                 return model_class.find(model_id)
             else:
                 return None
 
         db_field = db_field or f"{model_class.__name__.lower()}_id"
         attr_name = attr_name or model_class.__name__.lower()
         setattr(cls, model_class.__name__.lower(), property(getter_method))
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}({super().__str__()})"
```

### Comparing `pyfireconsole-0.0.2/pyfireconsole.egg-info/PKG-INFO` & `pyfireconsole-0.0.3/pyfireconsole.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pyfireconsole
-Version: 0.0.2
+Version: 0.0.3
 Summary: An interactive console for Firestore based on Python ORM
 Home-page: https://github.com/tan-z-tan/pyfireconsole
 Author: Makoto Tanji
 Author-email: tanji.makoto@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyFireConsole
 <h1 style="text-align: center;">
-  <img src="https://raw.githubusercontent.com/tan-z-tan/pyfireconsole/main/logo.png" alt="PyFireConsole" height="120">
+  <img src="https://raw.githubusercontent.com/tan-z-tan/pyfireconsole/main/logo.png" alt="PyFireConsole">
 </h1>
 
 ## Introduction
 Inspired by Rails console, PyFireConsole provides a seamless interface to Google's Firestore in Python, simplifying tasks such as connection, ORM, and data associations. It makes managing Firestore a breeze.
 
 ## Features
 - Model Definition and ORM: Define your Firestore data models within Python and use object-relational mapping (ORM) for easier data manipulation and querying.
@@ -31,36 +30,36 @@
 pip install pyfireconsole
 ```
 
 ## Getting Started
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.firestore_model import Collection, DocumentRef, FirestoreModel
+from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
 from pyfireconsole.db.connection import FirestoreConnection
 
 # Define your models 
-class User(FirestoreModel):
+class User(PyfireDoc):
     name: str
     email: str
 
-class Publisher(FirestoreModel):
+class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
-class Tag(FirestoreModel):
+class Tag(PyfireDoc):
     name: str
 
-class Book(FirestoreModel):
+class Book(PyfireDoc):
     title: str
     user_id: str
-    FirestoreModel.belongs_to(User)  # Make accessible via book.user
+    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
-    tags: Collection[Tag] = Collection(Tag)
+    tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
 
 # Initialize FirestoreConnection using your default credentials of gcloud. (use `gcloud auth application-default login` or set GOOGLE_APPLICATION_CREDENTIALS)
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 
 # Or you can specify service_account_key_path
@@ -111,36 +110,36 @@
 This feature is inspired by the Rails console.
 
 How to setup interactive console:
 
 ```python
 from datetime import datetime
 from typing import Optional
-from pyfireconsole.models.firestore_model import Collection, DocumentRef, FirestoreModel
+from pyfireconsole.models.pyfire_model import PyfireDoc, PyfireCollection, DocumentRef
 from pyfireconsole.db.connection import FirestoreConnection
 from pyfireconsole import PyFireConsole
 
-class User(FirestoreModel):
+class User(PyfireDoc):
     name: str
     email: str
 
-class Publisher(FirestoreModel):
+class Publisher(PyfireDoc):
     name: str
     address: Optional[str]
 
-class Tag(FirestoreModel):
+class Tag(PyfireDoc):
     name: str
 
-class Book(FirestoreModel):
+class Book(PyfireDoc):
     title: str
     user_id: str
-    FirestoreModel.belongs_to(User)  # Make accessible via book.user
+    PyfireDoc.belongs_to(User)  # Make accessible via book.user
     published_at: datetime
     authors: list[str]
-    tags: Collection[Tag] = Collection(Tag)
+    tags: PyfireCollection[Tag] = PyfireCollection(Tag)
     publisher_ref: DocumentRef[Publisher]
 
 FirestoreConnection().initialize(project_id="YOUR-PROJECT-ID")
 PyFireConsole().run()
 ```
```

### Comparing `pyfireconsole-0.0.2/pyfireconsole.egg-info/SOURCES.txt` & `pyfireconsole-0.0.3/pyfireconsole.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,11 +9,14 @@
 pyfireconsole.egg-info/requires.txt
 pyfireconsole.egg-info/top_level.txt
 pyfireconsole/console/__init__.py
 pyfireconsole/console/pyfireconsole.py
 pyfireconsole/db/__init__.py
 pyfireconsole/db/connection.py
 pyfireconsole/models/__init__.py
-pyfireconsole/models/firestore_model.py
+pyfireconsole/models/pyfire_model.py
 pyfireconsole/queries/__init__.py
-pyfireconsole/queries/query.py
-pyfireconsole/queries/query_manager.py
+pyfireconsole/queries/abstract_query.py
+pyfireconsole/queries/all_query.py
+pyfireconsole/queries/get_query.py
+pyfireconsole/queries/query_runner.py
+pyfireconsole/queries/where_query.py
```

### Comparing `pyfireconsole-0.0.2/setup.py` & `pyfireconsole-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyfireconsole',
-    version='0.0.2',
+    version='0.0.3',
     author='Makoto Tanji',
     author_email='tanji.makoto@gmail.com',
     description='An interactive console for Firestore based on Python ORM',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/tan-z-tan/pyfireconsole',
     packages=find_packages(),
     python_requires='>=3.10.0',
     install_requires=[
         'google-cloud-firestore>=2.0.0,<3.0.0',
         'google-auth>=2.0.0,<3.0.0',
-        'inflect>=7.0.0,<8.0.0',
+        'inflect>=6.0.0,<8.0.0',
         'pydantic>=2.0.1,<3.0.0',
-        'ipython>=8.0.1,<9.0.0',
+        'ipython>=7.0.1,<9.0.0',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.10',
     ],
```

