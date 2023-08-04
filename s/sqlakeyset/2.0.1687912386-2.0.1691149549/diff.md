# Comparing `tmp/sqlakeyset-2.0.1687912386.tar.gz` & `tmp/sqlakeyset-2.0.1691149549.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlakeyset-2.0.1687912386.tar", max compression
+gzip compressed data, was "sqlakeyset-2.0.1691149549.tar", max compression
```

## Comparing `sqlakeyset-2.0.1687912386.tar` & `sqlakeyset-2.0.1691149549.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1210 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/LICENSE
--rw-r--r--   0        0        0     8265 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/README.rst
--rw-r--r--   0        0        0     1295 2023-06-28 00:33:06.064446 sqlakeyset-2.0.1687912386/pyproject.toml
--rw-r--r--   0        0        0      631 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/__init__.py
--rw-r--r--   0        0        0     2767 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/asyncio.py
--rw-r--r--   0        0        0    14716 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/columns.py
--rw-r--r--   0        0        0       37 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/constants.py
--rw-r--r--   0        0        0    14213 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/paging.py
--rw-r--r--   0        0        0    10324 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/results.py
--rw-r--r--   0        0        0      347 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/serial/__init__.py
--rw-r--r--   0        0        0     5546 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/serial/serial.py
--rw-r--r--   0        0        0     2097 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/sqla.py
--rw-r--r--   0        0        0     2613 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/sqla13.py
--rw-r--r--   0        0        0     1571 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/sqla14.py
--rw-r--r--   0        0        0     4199 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/sqla20.py
--rw-r--r--   0        0        0      768 2023-06-28 00:33:00.912524 sqlakeyset-2.0.1687912386/sqlakeyset/types.py
--rw-r--r--   0        0        0     9125 1970-01-01 00:00:00.000000 sqlakeyset-2.0.1687912386/PKG-INFO
+-rw-r--r--   0        0        0     1210 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/LICENSE
+-rw-r--r--   0        0        0     8444 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/README.rst
+-rw-r--r--   0        0        0     1295 2023-08-04 11:45:49.961016 sqlakeyset-2.0.1691149549/pyproject.toml
+-rw-r--r--   0        0        0      631 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/__init__.py
+-rw-r--r--   0        0        0     2767 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/asyncio.py
+-rw-r--r--   0        0        0    14716 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/columns.py
+-rw-r--r--   0        0        0       37 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/constants.py
+-rw-r--r--   0        0        0    14213 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/paging.py
+-rw-r--r--   0        0        0    10324 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/results.py
+-rw-r--r--   0        0        0      347 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/serial/__init__.py
+-rw-r--r--   0        0        0     5754 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/serial/serial.py
+-rw-r--r--   0        0        0     2097 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/sqla.py
+-rw-r--r--   0        0        0     2613 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/sqla13.py
+-rw-r--r--   0        0        0     1571 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/sqla14.py
+-rw-r--r--   0        0        0     4199 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/sqla20.py
+-rw-r--r--   0        0        0      768 2023-08-04 11:45:45.233198 sqlakeyset-2.0.1691149549/sqlakeyset/types.py
+-rw-r--r--   0        0        0     9304 1970-01-01 00:00:00.000000 sqlakeyset-2.0.1691149549/PKG-INFO
```

### Comparing `sqlakeyset-2.0.1687912386/LICENSE` & `sqlakeyset-2.0.1691149549/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/README.rst` & `sqlakeyset-2.0.1691149549/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: sqlakeyset
+Version: 2.0.1691149549
+Summary: offset-free paging for sqlalchemy
+Home-page: https://github.com/djrobstep/sqlakeyset
+License: Unlicense
+Author: Robert Lechte
+Author-email: robertlechte@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: packaging (>=20.0)
+Requires-Dist: python-dateutil
+Requires-Dist: sqlalchemy (>=1.3.11)
+Requires-Dist: typing_extensions (>=4,<5)
+Project-URL: Repository, https://github.com/djrobstep/sqlakeyset
+Description-Content-Type: text/x-rst
+
 sqlakeyset: offset-free paging for sqlalchemy
 =============================================
 
 .. image:: https://img.shields.io/circleci/build/gh/djrobstep/sqlakeyset?label=tests
     :alt: Tests
     :target: https://circleci.com/gh/djrobstep/sqlakeyset
     
@@ -9,14 +32,18 @@
     :alt: PyPI
     :target: https://pypi.org/project/sqlakeyset/
     
 .. image:: https://img.shields.io/conda/vn/conda-forge/sqlakeyset.svg
     :alt: conda-forge
     :target: https://anaconda.org/conda-forge/sqlakeyset
 
+.. image:: https://readthedocs.org/projects/sqlakeyset/badge/
+   :alt: Documentation @ readthedocs
+   :target: https://sqlakeyset.readthedocs.io/
+
 sqlakeyset implements keyset-based paging for SQLAlchemy (both ORM and core). **Now with full SQLAlchemy 2 support and type hints!**
 
 This library is tested with PostgreSQL, MariaDB/MySQL and SQLite. It should work with many other SQLAlchemy-supported databases, too; but caveat emptor - you should verify the results are correct.
 
 **Notice:** In accordance with Python end-of-life dates, we've stopped supporting Python versions earlier than 3.7. If you really need it, the latest version to support Python 2 is 0.1.1559103842 and Python 3.4 is 1.0.1679209451, but you'll miss out on all the latest features and bugfixes from the latest version. You should be upgrading anyway!
 
 Background
@@ -170,20 +197,21 @@
 
 - If you're using the in-built keyset serialization, this only handles basic data/column types so far (strings, ints, floats, datetimes, dates, booleans, and a few others). The serialization can be extended to serialize more advanced types as necessary (documentation on this is forthcoming).
 
 
 Documentation
 -------------
 
-Other than this README, there is some basic sphinx documentation, which you can build yourself with e.g. ``make -C doc html``. Hopefully this will be available more conveniently soon - watch this space.
+Other than this README, there is some more detailed API documentation autogenerated from docstrings, which you can `read online at readthedocs.io <https://sqlakeyset.readthedocs.io/>`_ or build yourself with e.g. ``make -C doc html``.
 
 
 Installation
 ------------
 
 Assuming you have `pip <https://pip.pypa.io>`_ installed, all you need to do is install as follows:
 
 .. code-block:: shell
 
     $ pip install sqlakeyset
 
 This will install sqlakeyset and also sqlalchemy if not already installed. Obviously you'll need the necessary database driver for your chosen database to be installed also.
+
```

### Comparing `sqlakeyset-2.0.1687912386/pyproject.toml` & `sqlakeyset-2.0.1691149549/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sqlakeyset"
-version = "2.0.1687912386"
+version = "2.0.1691149549"
 authors = [ "Robert Lechte <robertlechte@gmail.com>", "Anthony Carapetis <anthony.carapetis@gmail.com>",]
 license = "Unlicense"
 readme = "README.rst"
 description = "offset-free paging for sqlalchemy"
 repository = "https://github.com/djrobstep/sqlakeyset"
 homepage = "https://github.com/djrobstep/sqlakeyset"
```

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/__init__.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/asyncio.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/asyncio.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/columns.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/columns.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/paging.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/paging.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/results.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/results.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/serial/serial.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/serial/serial.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import datetime
 import base64
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type, TypeVar
 import uuid
 import dateutil.parser
 import csv
 from io import StringIO
+from contextlib import suppress
 
 
 class InvalidPage(ValueError):
     """An invalid page marker (in either tuple or bookmark string form) was
     provided to a paging method."""
 
 
@@ -78,21 +79,34 @@
     (decimal.Decimal, "n"),
     (uuid.UUID, "uuid"),
     (datetime.datetime, "dt", dateutil.parser.parse),
     (datetime.date, "d", parsedate),
     (datetime.time, "t"),
 ]
 
+
 # These special values are serialized without prefix codes.
 BUILTINS = {
     "x": None,
     "true": True,
     "false": False,
 }
-BUILTINS_INV = {v: k for k, v in BUILTINS.items()}
+
+
+class NotABuiltin(Exception):
+    pass
+
+
+def invert_builtin(x) -> str:
+    for k, v in BUILTINS.items():
+        if x is v:
+            return k
+
+    raise NotABuiltin()
+
 
 T = TypeVar("T")
 
 
 def deserialize_int(s: str) -> int:
     return int(s)
 
@@ -144,37 +158,42 @@
         return self.join(self.serialize_value(_) for _ in values)
 
     def unserialize_values(self, s: str) -> Optional[Tuple]:
         if s == "":
             return None
         return tuple(self.unserialize_value(_) for _ in self.split(s))
 
+    def get_serializer(self, x):
+        for cls in type(x).__mro__:
+            with suppress(KeyError):
+                return self.serializers[cls]
+
+        return None
+
     def serialize_value(self, x) -> str:
-        try:
-            serializer = self.serializers[type(x)]
-        except KeyError:
-            pass  # fall through to builtins
-        else:
-            try:
-                c, x = serializer(x)
-            except Exception as e:
-                raise PageSerializationError(
-                    "Custom bookmark serializer " "encountered error"
-                ) from e
-            else:
-                return "{}:{}".format(c, x)
+        with suppress(NotABuiltin):
+            return invert_builtin(x)
 
-        try:
-            return BUILTINS_INV[x]
-        except KeyError:
+        serializer = self.get_serializer(x)
+
+        if serializer is None:
             raise UnregisteredType(
                 "Don't know how to serialize type of {} ({}). "
                 "Use custom_bookmark_type to register it.".format(x, type(x))
             )
 
+        try:
+            c, x = serializer(x)
+        except Exception as e:
+            raise PageSerializationError(
+                "Custom bookmark serializer " "encountered error"
+            ) from e
+
+        return "{}:{}".format(c, x)
+
     def unserialize_value(self, x: str):
         try:
             c, v = x.split(":", 1)
         except ValueError:
             # Must be a builtin
             try:
                 return BUILTINS[x]
```

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/sqla.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/sqla.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/sqla13.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/sqla13.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/sqla14.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/sqla14.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/sqla20.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/sqla20.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/sqlakeyset/types.py` & `sqlakeyset-2.0.1691149549/sqlakeyset/types.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1687912386/PKG-INFO` & `sqlakeyset-2.0.1691149549/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: sqlakeyset
-Version: 2.0.1687912386
-Summary: offset-free paging for sqlalchemy
-Home-page: https://github.com/djrobstep/sqlakeyset
-License: Unlicense
-Author: Robert Lechte
-Author-email: robertlechte@gmail.com
-Requires-Python: >=3.7,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: packaging (>=20.0)
-Requires-Dist: python-dateutil
-Requires-Dist: sqlalchemy (>=1.3.11)
-Requires-Dist: typing_extensions (>=4,<5)
-Project-URL: Repository, https://github.com/djrobstep/sqlakeyset
-Description-Content-Type: text/x-rst
-
 sqlakeyset: offset-free paging for sqlalchemy
 =============================================
 
 .. image:: https://img.shields.io/circleci/build/gh/djrobstep/sqlakeyset?label=tests
     :alt: Tests
     :target: https://circleci.com/gh/djrobstep/sqlakeyset
     
@@ -32,14 +9,18 @@
     :alt: PyPI
     :target: https://pypi.org/project/sqlakeyset/
     
 .. image:: https://img.shields.io/conda/vn/conda-forge/sqlakeyset.svg
     :alt: conda-forge
     :target: https://anaconda.org/conda-forge/sqlakeyset
 
+.. image:: https://readthedocs.org/projects/sqlakeyset/badge/
+   :alt: Documentation @ readthedocs
+   :target: https://sqlakeyset.readthedocs.io/
+
 sqlakeyset implements keyset-based paging for SQLAlchemy (both ORM and core). **Now with full SQLAlchemy 2 support and type hints!**
 
 This library is tested with PostgreSQL, MariaDB/MySQL and SQLite. It should work with many other SQLAlchemy-supported databases, too; but caveat emptor - you should verify the results are correct.
 
 **Notice:** In accordance with Python end-of-life dates, we've stopped supporting Python versions earlier than 3.7. If you really need it, the latest version to support Python 2 is 0.1.1559103842 and Python 3.4 is 1.0.1679209451, but you'll miss out on all the latest features and bugfixes from the latest version. You should be upgrading anyway!
 
 Background
@@ -193,21 +174,20 @@
 
 - If you're using the in-built keyset serialization, this only handles basic data/column types so far (strings, ints, floats, datetimes, dates, booleans, and a few others). The serialization can be extended to serialize more advanced types as necessary (documentation on this is forthcoming).
 
 
 Documentation
 -------------
 
-Other than this README, there is some basic sphinx documentation, which you can build yourself with e.g. ``make -C doc html``. Hopefully this will be available more conveniently soon - watch this space.
+Other than this README, there is some more detailed API documentation autogenerated from docstrings, which you can `read online at readthedocs.io <https://sqlakeyset.readthedocs.io/>`_ or build yourself with e.g. ``make -C doc html``.
 
 
 Installation
 ------------
 
 Assuming you have `pip <https://pip.pypa.io>`_ installed, all you need to do is install as follows:
 
 .. code-block:: shell
 
     $ pip install sqlakeyset
 
 This will install sqlakeyset and also sqlalchemy if not already installed. Obviously you'll need the necessary database driver for your chosen database to be installed also.
-
```

