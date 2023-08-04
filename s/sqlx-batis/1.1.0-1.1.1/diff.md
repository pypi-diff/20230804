# Comparing `tmp/sqlx-batis-1.1.0.tar.gz` & `tmp/sqlx-batis-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-1.1.0.tar", last modified: Wed Aug  2 12:44:53 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-1.1.1.tar", last modified: Fri Aug  4 01:52:22 2023, max compression
```

## Comparing `sqlx-batis-1.1.0.tar` & `sqlx-batis-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 12:44:53.000000 sqlx-batis-1.1.0/
--rw-rw-rw-   0        0        0     5701 2023-08-02 12:44:53.000000 sqlx-batis-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-1.1.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-02 12:44:53.000000 sqlx-batis-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1352 2023-08-02 12:44:29.000000 sqlx-batis-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:44:53.000000 sqlx-batis-1.1.0/sqlbatis/
--rw-rw-rw-   0        0        0      927 2023-08-01 15:24:17.000000 sqlx-batis-1.1.0/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     6719 2023-08-01 15:51:50.000000 sqlx-batis-1.1.0/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-1.1.0/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     6724 2023-07-30 16:13:17.000000 sqlx-batis-1.1.0/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     3731 2023-08-01 15:34:15.000000 sqlx-batis-1.1.0/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    35069 2023-08-02 00:35:05.000000 sqlx-batis-1.1.0/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     4089 2023-08-02 00:22:16.000000 sqlx-batis-1.1.0/sqlbatis/orm_support.py
--rw-rw-rw-   0        0        0     2540 2023-08-02 03:13:03.000000 sqlx-batis-1.1.0/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7063 2023-08-02 12:41:34.000000 sqlx-batis-1.1.0/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-1.1.0/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1216 2023-08-01 15:23:13.000000 sqlx-batis-1.1.0/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-1.1.0/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1662 2023-08-01 10:18:34.000000 sqlx-batis-1.1.0/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:44:53.000000 sqlx-batis-1.1.0/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-02 12:44:53.000000 sqlx-batis-1.1.0/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-1.1.0/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5701 2023-08-02 12:44:53.000000 sqlx-batis-1.1.0/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-08-02 12:44:53.000000 sqlx-batis-1.1.0/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      489 2023-08-02 12:44:53.000000 sqlx-batis-1.1.0/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 12:44:53.000000 sqlx-batis-1.1.0/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/
+-rw-rw-rw-   0        0        0     5701 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-1.1.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2023-08-04 01:51:46.000000 sqlx-batis-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlbatis/
+-rw-rw-rw-   0        0        0      927 2023-08-01 15:24:17.000000 sqlx-batis-1.1.1/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     6719 2023-08-01 15:51:50.000000 sqlx-batis-1.1.1/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-1.1.1/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     6732 2023-08-03 03:29:50.000000 sqlx-batis-1.1.1/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     3731 2023-08-01 15:34:15.000000 sqlx-batis-1.1.1/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    35069 2023-08-02 00:35:05.000000 sqlx-batis-1.1.1/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     4089 2023-08-02 00:22:16.000000 sqlx-batis-1.1.1/sqlbatis/orm_support.py
+-rw-rw-rw-   0        0        0     2672 2023-08-04 01:49:10.000000 sqlx-batis-1.1.1/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7278 2023-08-04 01:47:15.000000 sqlx-batis-1.1.1/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-1.1.1/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1216 2023-08-01 15:23:13.000000 sqlx-batis-1.1.1/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-1.1.1/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1662 2023-08-01 10:18:34.000000 sqlx-batis-1.1.1/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5701 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      489 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-08-04 01:52:22.000000 sqlx-batis-1.1.1/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-1.1.0/PKG-INFO` & `sqlx-batis-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 1.1.0
+Version: 1.1.1
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-1.1.0/README.rst` & `sqlx-batis-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.0/setup.py` & `sqlx-batis-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.4.5',
+        'sqlx-exec>=1.4.6',
     ],
-    version='1.1.0',
+    version='1.1.1',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-1.1.0/sqlbatis/constant.py` & `sqlx-batis-1.1.1/sqlbatis/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.0/sqlbatis/db.py` & `sqlx-batis-1.1.1/sqlbatis/db.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.0/sqlbatis/dbx.py` & `sqlx-batis-1.1.1/sqlbatis/dbx.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.0/sqlbatis/engine.py` & `sqlx-batis-1.1.1/sqlbatis/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,16 @@
         elif Engine.current_engine() == POSTGRESQL:
             return PostgresEngine.get_table_columns(table)
         elif Engine.current_engine() == SQLITE:
             return SQLiteEngine.get_table_columns(table)
         raise "*"
 
 
-class BaseEngine(Engine):
+class BaseEngine(SupperEngine):
+
     @staticmethod
     def get_page_sql_args(sql: str, page_num: int, page_size: int, *args):
         start = get_page_start(page_num, page_size)
         if require_limit(sql):
             sql = '{} LIMIT ? OFFSET ?'.format(sql)
         args = [*args, page_size, start]
         return sql, args
```

### Comparing `sqlx-batis-1.1.0/sqlbatis/log_support.py` & `sqlx-batis-1.1.1/sqlbatis/log_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.0/sqlbatis/orm.py` & `sqlx-batis-1.1.1/sqlbatis/orm.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.0/sqlbatis/orm_support.py` & `sqlx-batis-1.1.1/sqlbatis/orm_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.0/sqlbatis/snowflake.py` & `sqlx-batis-1.1.1/sqlbatis/snowflake.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-"""
+__doc__ = """
 默认worker_bits=3, sequence_bits=6。
-不区分数据中心，机器id最多2^3=8 台，每秒最大并发为2^6*1000=64000，超过40年id长度还是15位，javascript可以直接使用，不需转化为string
+不区分数据中心，机器id最多2^3=8 台，每秒最大并发为2^6*1000=64000，使用超过40年id的长度也不超过15位，javascript可以直接使用，不需转化为string
 """
 
 import time
 from threading import RLock
 
 _SNOWFLAKE = None
 # _SEQUENCE_MASK = 4095
-_SNOWFLAKE_LOCK = RLock()
+
+
+class SnowflakeError(Exception):
+    pass
 
 def init_snowflake(epoch=1688140800000, machine_id=0, worker_bits=3, sequence_bits=6):
     global _SNOWFLAKE
-    with _SNOWFLAKE_LOCK:
-        _SNOWFLAKE = Snowflake(machine_id, epoch, worker_bits, sequence_bits)
+    if _SNOWFLAKE is not None:
+        SnowflakeError("Snowflake was already initialized.")
+    _SNOWFLAKE = Snowflake(machine_id, epoch, worker_bits, sequence_bits)
 
 
 def get_snowflake_id():
     global _SNOWFLAKE
     try:
         return _SNOWFLAKE.generate_id()
     except AttributeError:
@@ -40,21 +44,22 @@
         self.machine_id = machine_id
         self.epoch = epoch
         self.sequence = 0
         self.last_timestamp = -1
         self.worker_shift = sequence_bits
         self.sequence_mask = -1 ^ (-1 << sequence_bits)
         self.timestamp_left_shift = worker_bits + sequence_bits
+        self.lock = RLock()
 
         maxWorkerId = -1 ^ (-1 << worker_bits);
         assert 0 <= machine_id < maxWorkerId, 'machine_id must ge 0 and lt %d, but it is %d' % (maxWorkerId, machine_id)
         # assert 10 <= self.timestamp_left_shift <= 22, 'worker_bits add sequence_bits must between 10 and 20, but it is %d' % self.timestamp_left_shift
 
     def generate_id(self):
-        with _SNOWFLAKE_LOCK:
+        with self.lock:
             timestamp = _get_timestamp()
             if timestamp < self.last_timestamp:
                 raise Exception("Clock moved backwards")
             if timestamp == self.last_timestamp:
                 self.sequence = (self.sequence + 1) & self.sequence_mask
                 if self.sequence == 0:
                     timestamp = _wait_next_millis(self.last_timestamp)
```

### Comparing `sqlx-batis-1.1.0/sqlbatis/sql_holder.py` & `sqlx-batis-1.1.1/sqlbatis/sql_holder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-import os
 import re
-import asyncio
-import pathlib
 from typing import List
+from pathlib import Path
 from typing import Mapping
 from jinja2 import Template
 from .log_support import logger
 from .support import MapperError, SqlAction
 from .sql_support import is_dynamic_sql, get_named_sql_args
 
 try:
     import xml.etree.cElementTree as ET
 except ImportError:
     import xml.etree.ElementTree as ET
 
+_IS_LOADED = False
 _SQL_CONTAINER = dict()
 _valid_sql_actions = (SqlAction.INSERT.value, SqlAction.UPDATE.value, SqlAction.DELETE.value, SqlAction.SELECT.value)
 
 
 class SqlModel:
     def __init__(self, sql: str, action: str, namespace: str, dynamic=False, includes: List[str] = None, key_seq: str = None, select_key: str=None):
         self.sql = sql
@@ -72,27 +71,35 @@
 def get_sql_model(sql_id: str):
     global _SQL_CONTAINER
     return _SQL_CONTAINER[sql_id]
 
 
 # ----------------------------------------------------------Load mapper--------------------------------------------------------------------
 def load_mapper(path: str):
-    path = pathlib.Path(path)
+    global _IS_LOADED
+    if _IS_LOADED:
+        raise MapperError("Don't repeat load mapper files.")
+
+    _IS_LOADED = True
+    path = Path(path)
     if path.is_file() and path.suffix ==".xml":
-        tasks = [_parse_mapper_file(path)]
+        _parse_mapper_file(path)
     elif path.is_dir():
-        tasks = [_parse_mapper_file(file) for file in path.rglob('*.xml')]
+        import asyncio
+        tasks = map(_async_parse_mapper_file, path.rglob('*.xml'))
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(asyncio.wait(tasks))
+        loop.close()
 
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(asyncio.wait(tasks))
-    loop.close()
 
+async def _async_parse_mapper_file(file: str):
+    _parse_mapper_file(file)
 
 
-async def _parse_mapper_file(file: str):
+def _parse_mapper_file(file: str):
     global _SQL_CONTAINER
     tree = ET.parse(file)
     root = tree.getroot()
     namespace = root.attrib.get('namespace', '')
     results = list(map(lambda child: _load_sql(namespace, child, file), root))
     sql_ids, file_all_includes = zip(*results)
     for i, includes in enumerate(file_all_includes):
```

### Comparing `sqlx-batis-1.1.0/sqlbatis/sql_mapper.py` & `sqlx-batis-1.1.1/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.0/sqlbatis/sql_support.py` & `sqlx-batis-1.1.1/sqlbatis/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.0/sqlbatis/__init__.py` & `sqlx-batis-1.1.1/sqlbatis/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-1.1.0/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-1.1.1/sqlx_batis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 1.1.0
+Version: 1.1.1
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

