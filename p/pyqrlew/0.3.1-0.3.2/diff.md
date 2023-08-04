# Comparing `tmp/pyqrlew-0.3.1.tar.gz` & `tmp/pyqrlew-0.3.2.tar.gz`

## Comparing `pyqrlew-0.3.1.tar` & `pyqrlew-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,36 @@
--rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 pyqrlew-0.3.1/Cargo.toml
--rw-r--r--   0     1001      123     4542 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     3539 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/.gitignore
--rw-r--r--   0     1001      123      818 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/.readthedocs.yaml
--rw-r--r--   0     1001      123      719 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/CHANGELOG.md
--rw-r--r--   0     1001      123    11357 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/LICENSE
--rw-r--r--   0     1001      123     1466 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/README.md
--rw-r--r--   0     1001      123      634 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/Makefile
--rw-r--r--   0     1001      123     1212 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/conf.py
--rw-r--r--   0     1001      123      224 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/contributing.md
--rw-r--r--   0     1001      123     1786 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/index.md
--rw-r--r--   0     1001      123      800 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/make.bat
--rw-r--r--   0     1001      123       61 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/docs/requirements.txt
--rw-r--r--   0     1001      123   146621 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/deprecated_demo.ipynb
--rw-r--r--   0     1001      123      189 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/expose_protobufs.py
--rw-r--r--   0     1001      123    45574 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/pyqrlew_display_relations.ipynb
--rw-r--r--   0     1001      123    39156 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/pyqrlew_retail_demo.ipynb
--rw-r--r--   0     1001      123      133 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/requirements.txt
--rw-r--r--   0     1001      123      380 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/examples/simple.py
--rw-r--r--   0     1001      123     1139 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/pyproject.toml
--rw-r--r--   0     1001      123      112 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/python/pyqrlew/__init__.py
--rw-r--r--   0     1001      123       45 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/python/pyqrlew/io/__init__.py
--rw-r--r--   0     1001      123    12628 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/python/pyqrlew/io/database.py
--rw-r--r--   0     1001      123     2333 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/python/pyqrlew/io/postgresql.py
--rw-r--r--   0     1001      123    10104 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/src/lib.rs
--rw-r--r--   0     1001      123      136 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/tests/conftest.py
--rw-r--r--   0     1001      123     2481 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/tests/queries/sql_unlimited_queries.sql
--rw-r--r--   0     1001      123     7054 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/tests/queries/valid_queries.sql
--rw-r--r--   0     1001      123      178 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/tests/requirements.txt
--rw-r--r--   0     1001      123     1431 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/tests/test_extract_dataset.py
--rw-r--r--   0     1001      123    48628 2023-07-27 23:33:32.000000 pyqrlew-0.3.1/Cargo.lock
--rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pyqrlew-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 pyqrlew-0.3.2/Cargo.toml
+-rw-r--r--   0     1001      123     4542 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     3539 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/.gitignore
+-rw-r--r--   0     1001      123      818 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/.readthedocs.yaml
+-rw-r--r--   0     1001      123      839 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/CHANGELOG.md
+-rw-r--r--   0     1001      123    11357 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/LICENSE
+-rw-r--r--   0     1001      123     1466 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/README.md
+-rw-r--r--   0     1001      123      634 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/docs/Makefile
+-rw-r--r--   0     1001      123     1212 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/docs/conf.py
+-rw-r--r--   0     1001      123      224 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/docs/contributing.md
+-rw-r--r--   0     1001      123     1786 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/docs/index.md
+-rw-r--r--   0     1001      123      800 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/docs/make.bat
+-rw-r--r--   0     1001      123       61 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/docs/requirements.txt
+-rw-r--r--   0     1001      123   141874 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/examples/deprecated_demo.ipynb
+-rw-r--r--   0     1001      123      189 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/examples/expose_protobufs.py
+-rw-r--r--   0     1001      123    45574 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/examples/pyqrlew_display_relations.ipynb
+-rw-r--r--   0     1001      123    39156 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/examples/pyqrlew_retail_demo.ipynb
+-rw-r--r--   0     1001      123    77224 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/examples/range_propagation.ipynb
+-rw-r--r--   0     1001      123      133 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/examples/requirements.txt
+-rw-r--r--   0     1001      123      380 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/examples/simple.py
+-rw-r--r--   0     1001      123     1139 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/pyproject.toml
+-rw-r--r--   0     1001      123      130 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/python/pyqrlew/__init__.py
+-rw-r--r--   0     1001      123      112 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/python/pyqrlew/io/__init__.py
+-rw-r--r--   0     1001      123    12357 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/python/pyqrlew/io/database.py
+-rw-r--r--   0     1001      123     2712 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/python/pyqrlew/io/postgresql.py
+-rw-r--r--   0     1001      123     4780 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/python/pyqrlew/io/sqlite.py
+-rw-r--r--   0     1001      123     5589 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/python/pyqrlew/io/utils.py
+-rw-r--r--   0     1001      123     1115 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/python/pyqrlew/utils.py
+-rw-r--r--   0     1001      123    10104 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/src/lib.rs
+-rw-r--r--   0     1001      123      136 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/tests/conftest.py
+-rw-r--r--   0     1001      123     2481 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/tests/queries/sql_unlimited_queries.sql
+-rw-r--r--   0     1001      123     7054 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/tests/queries/valid_queries.sql
+-rw-r--r--   0     1001      123      178 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/tests/requirements.txt
+-rw-r--r--   0     1001      123     1431 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/tests/test_extract_dataset.py
+-rw-r--r--   0     1001      123    48628 2023-08-04 15:12:58.000000 pyqrlew-0.3.2/Cargo.lock
+-rw-r--r--   0        0        0     2527 1970-01-01 00:00:00.000000 pyqrlew-0.3.2/PKG-INFO
```

### Comparing `pyqrlew-0.3.1/.github/workflows/CI.yml` & `pyqrlew-0.3.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/.gitignore` & `pyqrlew-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/.readthedocs.yaml` & `pyqrlew-0.3.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/CHANGELOG.md` & `pyqrlew-0.3.2/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.3.2] - 2023-08-03
+### Added
+- support for SQLite
+### Added
+- retail Dataset + notebook `range_propagation.ipynb`
+
 ## [0.2.1] - 2023-07-18
 ### Changed
 - Updated `qrlew-datasets`
 
 ## [0.2.0] - 2023-07-18
 ### Changed
 - Remove data and db from pyqrlew. They are now in the qrlew-dataset package.
```

### Comparing `pyqrlew-0.3.1/LICENSE` & `pyqrlew-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/README.md` & `pyqrlew-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/docs/Makefile` & `pyqrlew-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/docs/conf.py` & `pyqrlew-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/docs/index.md` & `pyqrlew-0.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/docs/make.bat` & `pyqrlew-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/examples/pyqrlew_display_relations.ipynb` & `pyqrlew-0.3.2/examples/pyqrlew_display_relations.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/examples/pyqrlew_retail_demo.ipynb` & `pyqrlew-0.3.2/examples/pyqrlew_retail_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/pyproject.toml` & `pyqrlew-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = [
   "SQLAlchemy ~= 2.0",
   "psycopg[binary, pool] ~= 3.0",
   "pymysql ~= 1.0",
-  "qrlew-datasets ~= 0.3.0",
+  "qrlew-datasets ~= 0.3.2",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest ~= 7.0",
   "mypy ~= 1.0",
 ]
```

### Comparing `pyqrlew-0.3.1/python/pyqrlew/io/database.py` & `pyqrlew-0.3.2/python/pyqrlew/io/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import json
 from sqlalchemy import Engine, MetaData, Table, Column
 from sqlalchemy import types, select, func
 import pyqrlew as qrl
 
 def dataset(name: str, engine: Engine, schema_name: Optional[str]=None) -> qrl.Dataset:
     metadata = MetaData()
-    schema = schema_name or name
-    metadata.reflect(engine, schema=schema)
+    metadata.reflect(engine, schema=schema_name)
 
     def _dataset_schema_size() -> tuple[dict, dict, Optional[dict]]:
         """Return a (dataset, schema) pair or (dataset, schema, size) triplet """
         ds = _dataset()
         return (
             ds,
             _schema(ds),
@@ -34,42 +33,45 @@
                 },
             },
             'properties': {},
             'doc': 'This ia a demo dataset for testing purpose',
         }
 
     def _schema(dataset: dict) -> dict:
+        tables = {"fields": [_table(metadata.tables[name]) for name in metadata.tables]}
+
+        if schema_name is not None:
+            tables = {
+                "fields": [{
+                    'name': schema_name,
+                    'type': {
+                        'name': 'Union',
+                        'union': tables,
+                        'properties': {
+                            'public_fields': '[]'
+                        },
+                    }
+                }],
+            }
+
         return {
             '@type': 'sarus_data_spec/sarus_data_spec.Schema',
             'uuid': generate_uuid().hex,
             'dataset': dataset['uuid'],
             'name': name,
             'type': {
                 # Slugname
                 'name': name.lower(),
                 'struct': {
                     'fields': [
                         {
                             'name': 'sarus_data',
                             'type': {
                                 'name': 'Union',
-                                'union': {
-                                    "fields": [{
-                                        'name': schema,
-                                        'type': {
-                                            'name': 'Union',
-                                            'union': {
-                                                "fields": [_table(metadata.tables[name]) for name in metadata.tables]
-                                            },
-                                            'properties': {
-                                                'public_fields': '[]'
-                                            },
-                                        }
-                                    }],
-                                },
+                                'union': tables,
                                 'properties': {
                                     'public_fields': '[]',
                                 },
                             },
                         },
                         {
                             'name': 'sarus_weights',
@@ -200,36 +202,38 @@
                     'name': 'Type',
                     'type': {},
                     'properties': {},
                 },
             }
 
     def _size(dataset: dict) -> dict:
+        tables = {'fields': [_table_size(metadata.tables[name]) for name in metadata.tables]}
+        if schema_name is not None:
+            tables = {
+                'fields': [
+                    {
+                        'name': schema_name,
+                        'statistics': {
+                            'name': 'Union',
+                            'union': tables,
+                            'properties': {},
+                        },
+                        'properties': {},
+                    },
+                ],
+            }
+
         return {
             '@type': 'sarus_data_spec/sarus_data_spec.Size',
             'uuid': generate_uuid().hex,
             'dataset': dataset['uuid'],
             'name': f'{name}_sizes',
             'statistics': {
                 'name': 'Union',
-                'union': {
-                    'fields': [
-                        {
-                            'name': schema,
-                            'statistics': {
-                                'name': 'Union',
-                                'union': {
-                                    'fields': [_table_size(metadata.tables[name]) for name in metadata.tables]
-                                },
-                                'properties': {},
-                            },
-                            'properties': {},
-                        },
-                    ],
-                },
+                'union': tables,
                 'properties': {},
             },
             'properties': {},
         }
 
     def _table_size(tab: Table) -> dict:
         with engine.connect() as conn:
```

### Comparing `pyqrlew-0.3.1/python/pyqrlew/io/postgresql.py` & `pyqrlew-0.3.2/python/pyqrlew/io/postgresql.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,50 +13,60 @@
 USER: str = 'postgres'
 PASSWORD: str = 'pyqrlew-db'
 PORT: str = 5433
 
 class PostgreSQL(EmptyPostgreSQL):
     def __init__(self) -> None:
         super().__init__(NAME, USER, PASSWORD, PORT)
-    
+
     def load_resource(self, schema: str, src: Path) -> 'PostgreSQL':
         with self.engine().connect() as conn:
             res = list(conn.execute(select(column('schema_name')).select_from(table('schemata', schema='information_schema')).where(column('schema_name') == schema)))
             schema_exists = len(res)==1
         if not schema_exists:
             dst = Path('/tmp') / schema
             shutil.copyfile(src, dst)
             self.load(dst)
         return self
-    
+
     def load_extract(self) -> 'PostgreSQL':
         return self.load_resource('extract', pkg_resources.files(sources) / 'extract' / 'extract.sql')
 
     def load_financial(self) -> 'PostgreSQL':
         return self.load_resource('financial', pkg_resources.files(sources) / 'financial' / 'financial.sql')
 
     def load_hepatitis(self) -> 'PostgreSQL':
         return self.load_resource('hepatitis_std', pkg_resources.files(sources) / 'hepatitis' / 'Hepatitis_std.sql')
 
     def load_imdb(self) -> 'PostgreSQL':
         return self.load_resource('imdb_ijs', pkg_resources.files(sources) / 'imdb' / 'imdb_ijs.sql')
-    
+
+    def load_retail(self) -> 'PostgreSQL':
+        return self.load_resource('retail', pkg_resources.files(sources) / 'retail' / 'retail.sql')
+
     def extract(self) -> qrl.Dataset:
         self.load_extract()
-        return dataset('extract', self.engine())
-    
+        return dataset('extract', self.engine(), 'extract')
+
     def financial(self) -> qrl.Dataset:
         self.load_financial()
-        return dataset('financial', self.engine())
-    
+        return dataset('financial', self.engine(), 'financial')
+
     def hepatitis(self) -> qrl.Dataset:
         self.load_hepatitis()
-        return dataset('hepatitis_std', self.engine())
+        return dataset('hepatitis_std', self.engine(), 'hepatitis_std')
 
     def imdb(self) -> qrl.Dataset:
         self.load_imdb()
-        return dataset('imdb_ijs', self.engine())
+        return dataset('imdb_ijs', self.engine(), 'imdb_ijs')
+
+    def retail(self) -> qrl.Dataset:
+        self.load_retail()
+        return dataset('retail', self.engine(), 'retail')
 
     def eval(self, relation: qrl.Relation) -> list:
+        return self.execute(relation.render())
+
+    def execute(self, query: str) -> list:
         with self.engine().connect() as conn:
-            result = conn.execute(text(relation.render())).all()
+            result = conn.execute(text(query)).all()
         return result
```

### Comparing `pyqrlew-0.3.1/src/lib.rs` & `pyqrlew-0.3.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/tests/queries/sql_unlimited_queries.sql` & `pyqrlew-0.3.2/tests/queries/sql_unlimited_queries.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/tests/queries/valid_queries.sql` & `pyqrlew-0.3.2/tests/queries/valid_queries.sql`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/tests/test_extract_dataset.py` & `pyqrlew-0.3.2/tests/test_extract_dataset.py`

 * *Files identical despite different names*

### Comparing `pyqrlew-0.3.1/Cargo.lock` & `pyqrlew-0.3.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1018,15 +1018,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyqrlew"
-version = "0.3.1"
+version = "0.3.2"
 dependencies = [
  "pyo3",
  "qrlew",
  "qrlew-sarus",
  "serde_json",
 ]
```

### Comparing `pyqrlew-0.3.1/PKG-INFO` & `pyqrlew-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pyqrlew
-Version: 0.3.1
+Version: 0.3.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: SQLAlchemy ~= 2.0
 Requires-Dist: psycopg[binary, pool] ~= 3.0
 Requires-Dist: pymysql ~= 1.0
-Requires-Dist: qrlew-datasets ~= 0.3.0
+Requires-Dist: qrlew-datasets ~= 0.3.2
 Requires-Dist: pytest ~= 7.0; extra == 'test'
 Requires-Dist: mypy ~= 1.0; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: A library to manipulate SQL queries, designed with privacy application in mind.
 Keywords: SQL,Privecy,Differential Privacy,AST,Intermediate Representation,Rust
 Author-email: Nicolas Grislain <ng@sarus.tech>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: documentation, https://pyqrlew.readthedocs.io
-Project-URL: changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
 Project-URL: homepage, https://qrlew.github.io
+Project-URL: changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
 Project-URL: repository, https://github.com/Qrlew/pyqrlew
+Project-URL: documentation, https://pyqrlew.readthedocs.io
 
 # [Qrlew](https://qrlew.github.io/) framework (by [Sarus](https://www.sarus.tech/))
 Open source SQL manipulation framework written in Rust
 
 ## What is [Qrlew](https://qrlew.github.io/)?
 [Qrlew](https://qrlew.github.io/) is an open source library that aims to parse and compile SQL queries into an Intermediate Representation (IR) that is well-suited for various rewriting tasks. Although it was originally designed for privacy-focused applications, it can be utilized for a wide range of purposes.
```

