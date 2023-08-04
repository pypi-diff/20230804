# Comparing `tmp/sqlalchemy_orm_manager-0.0.2.tar.gz` & `tmp/sqlalchemy_orm_manager-0.0.3.tar.gz`

## Comparing `sqlalchemy_orm_manager-0.0.2.tar` & `sqlalchemy_orm_manager-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/Pipfile
--rw-r--r--   0        0        0    22994 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/Pipfile.lock
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/decorators.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/exceptions.py
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/managers.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/meta.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/pagination.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/tests/test_manager.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/LICENSE
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/README.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4583 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/Pipfile
+-rw-r--r--   0        0        0    22994 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/Pipfile.lock
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/pytest.ini
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/sqlalchemy_manager/__init__.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/sqlalchemy_manager/decorators.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/sqlalchemy_manager/exceptions.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/sqlalchemy_manager/managers.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/sqlalchemy_manager/meta.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/sqlalchemy_manager/pagination.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/tests/test_manager.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/README.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 sqlalchemy_orm_manager-0.0.3/PKG-INFO
```

### Comparing `sqlalchemy_orm_manager-0.0.2/Pipfile.lock` & `sqlalchemy_orm_manager-0.0.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/decorators.py` & `sqlalchemy_orm_manager-0.0.3/sqlalchemy_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/managers.py` & `sqlalchemy_orm_manager-0.0.3/sqlalchemy_manager/managers.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/meta.py` & `sqlalchemy_orm_manager-0.0.3/sqlalchemy_manager/meta.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.2/sqlalchemy_manager/pagination.py` & `sqlalchemy_orm_manager-0.0.3/sqlalchemy_manager/pagination.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.2/tests/conftest.py` & `sqlalchemy_orm_manager-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.2/tests/test_manager.py` & `sqlalchemy_orm_manager-0.0.3/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.2/.gitignore` & `sqlalchemy_orm_manager-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.2/LICENSE` & `sqlalchemy_orm_manager-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_orm_manager-0.0.2/README.md` & `sqlalchemy_orm_manager-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,130 +1,118 @@
-A fully typed generic manager class to easily create CRUD operations for SQLAlchemy models. Designed to use in FastAPI
-projects.
+Metadata-Version: 2.1
+Name: sqlalchemy_orm_manager
+Version: 0.0.3
+Summary: A base manager class to handle CRUD on SQLAlchemy models.
+Project-URL: Homepage, https://github.com/nakeeon/SQLAlchemy-Manager
+Author-email: Nazar Kaliuzhnyi <kaluzghnyy@gmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: sqlalchemy>=1.4
+Description-Content-Type: text/markdown
 
-# Table of content
+A fully typed generic manager class to easily create CRUD operations for SQLAlchemy models.
 
-1. [Quick start](#quick-start)
+# Table of contents
+
+1. [Quick Start](#quick-start)
     - [Manager](#manager)
     - [Searching](#searching)
 2. [Pagination](#pagination)
     - [Paginator](#paginator)
     - [Pagination model](#pagination-model)
 
 ## Quick start
 
-Assume you have an SQLAlchemy model `User` and you want to perform CRUD on this model. You can simply create a manager
-for the model like this:
+Assume you have an SQLAlchemy model `User`, and want to perform CRUD on this model. You can simply create a manager
+for the model:
 
 ```python
 from sqlalchemy_manager import Manager
 
 from .models import User
 
 
 class UserManager(Manager[User]):
     pass
 ```
 
-`Manager` is a generic class, you need to pass an SQLAlchemy model as it's type (`Manager[User]`) to configure the
-manager to operate the model.
+The package also has `AsyncManager`. You can import and use it in the same way.
+
+```python
+from sqlalchemy_manager import AsynManager
+
+from .models import User
+
+
+class UserManager(AsynManager[User]):
+    pass
+```
 
-By passing an SQLAlchemy model as manager's type you will also get type hints and autocompletion in your IDE.
+`Manager` is a generic class. You need to pass an SQLAlchemy model as its type (`Manager[User]`) to configure the
+manager to operate on the model.
 
-That's it. You can now use the manager to do CRUD operations. You need to pass an SQlAlchemy session to a method as
-first argument. It can be `Session` or `AsyncSession`.
+Passing an SQLAlchemy model as the manager's type, you will also get type hints and autocompletion in your IDE.
+
+That's it. You can now use the manager to do CRUD operations. You must initialize a manager by passing a session
+instance. It should be `Session` for the `Manager` and `AsyncSession` for the `AsyncManage`.
 
 ```python
-UserManager.create(session, User(firstname="Bob"))
-UserManager.get(session, id=1)
-UserManager.delete(session, id=1)
+UserManager(session).create(User(firstname="Bob"))
+UserManager(session).get(id=1)
+UserManager(session).delete(id=1)
+
+# Using AsyncManager
+await UserManager(async_session).get(id=1)
 ```
 
 ### Manager
 
-`Manager` class contains general CRUD methods alongside some extra methods such as `get_or_create` and `search`.
+The `Manager` class contains general CRUD and extra methods such as `get_or_create` or `search`.
 
 List of all methods:
 
     - get
     - create
     - delete
     - get_or_create
     - search
     - update
 
-It is also has async methods, simple add `async_` to a method name, e.g. `async_create`, `async_delete` etc.
-
-`Manager` can accept either an SQLAlchemy model instance or a pydantic model instance.
-
-```python
-from sqlalchemy_manager import Manager
-from pydantic import BaseModel
-
-from app.db import session
-from app.managers import UserManager
-
-
-class User(BaseModel):
-    firstname: str
-
-
-user = User(firstname="Bob")
-UserManager.create(session, user)  # ok
-```
-
 ### Searching
 
-Manager has `search` and `async_search` methods. It accepts search params as a pydantic model called `Params`. Each
-manager has its own search params model defined inside the class.
+The `Manager` has a `search` method. It accepts a list of SQLAlchemy expressions and simple `kwargs`.
 
 ```python
-from sqlalchemy_manager import Manager
-from pydantic import BaseModel
-
-from .models import User
-
+UserManager(session).search(age=10, gender="male")
 
-class UserManager(Manager[User]):
-    class Params(BaseModel):
-        age: int
-        gender: str
-```
-
-Now `search` and `async_search` of `UserManager` will accept only `age` and `gender` params by validating them using
-the `Params`
-model.
-
-You can pass either a `dict` or manager's `Params` object.
-
-```python
-UserManager.search(session, **{'age': 10, 'gender': 'male'})  # okay
-UserManager.search(session, UserManager.Params(age=10, gender='male'))  # okay
-
-UserManager.search(session, **{'age': 10, 'name': 'Bob'})  # validation error
+UserManager(session).search(User.age >= 10)
 ```
 
 ## Pagination
 
-You usually need a pagination when do search. `Manager` comes with simple builtin pagination for `search`
-and `async_search` methods.
+You usually need pagination when searching. `Manager` comes with simple built-in pagination for `search` method.
 
-These methods accept `page` argument to return a limited set of items belonging to the page.
+The method accepts the `page` argument to return a limited set of items belonging to the page.
 
-In `fastapi_manager.pagination` you can find `Paginator` and `Pagination` classes.
+In `sqlalchemy_manager.pagination`, you can find `Paginator` and `Pagination` classes.
 
 ### Paginator
 
-`Paginator` is responsible for doing the pagination and is used by manager's `search` and `async_search` methods.
-It does an offset limit pagination under the hood, and operates with `page` and `per_page` properties.
-Its main method `paginate` returns `Pagination` object which tells the structure of the pagination.
+`Paginator` is responsible for doing the pagination and is used by the manager's `search` method.
+It does an offset limit pagination under the hood and operates with `page` and `per_page` properties.
+Its primary method, `paginate,` returns the `Pagination` instance.
+
+`AsyncManager` uses `AsyncPaginator`.
 
-It has two properties: `per_page = 25` and `order_by = 'id'` that can be customized.
+`Paginator` has two properties: `per_page = 25` and `order_by = 'id'` that can be customized.
 
-You can customize it by inherit the `Paginator` and override these params in your own class:
+You can customize it by inheriting the `Paginator` and overriding these params in your class:
 
 ```python
 from sqlalchemy_manager import Manager, Paginator
 
 
 class CustomPaginator(Paginator):
     per_page = 100
@@ -133,17 +121,18 @@
 
 class UserManager(Manager[User]):
     paginator_class = CustomPaginator
 ```
 
 ### Pagination model
 
-`Pagination` is a pydantic model that describes the structure of the pagination object to be returned.
+`Pagination` is a dataclass that describes the structure of the pagination object to return.
 
 ```python
-class Pagination(BaseModel):
+@dataclass
+class Pagination:
     page: int
     results: Union[Sequence, List]
     total: int
     has_prev: bool
     has_next: bool
 ```
```

### Comparing `sqlalchemy_orm_manager-0.0.2/pyproject.toml` & `sqlalchemy_orm_manager-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sqlalchemy_orm_manager"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Nazar Kaliuzhnyi", email = "kaluzghnyy@gmail.com" },
 ]
 description = "A base manager class to handle CRUD on SQLAlchemy models."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

