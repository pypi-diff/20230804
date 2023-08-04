# Comparing `tmp/sqlx-exec-1.4.5.tar.gz` & `tmp/sqlx-exec-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.4.5.tar", last modified: Wed Aug  2 02:16:32 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.4.6.tar", last modified: Fri Aug  4 01:37:03 2023, max compression
```

## Comparing `sqlx-exec-1.4.5.tar` & `sqlx-exec-1.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.5/LICENSE
--rw-rw-rw-   0        0        0     3750 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     3163 2023-08-01 10:41:13.000000 sqlx-exec-1.4.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-08-02 02:15:55.000000 sqlx-exec-1.4.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlexec/
--rw-rw-rw-   0        0        0      977 2023-08-01 15:23:57.000000 sqlx-exec-1.4.5/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.4.5/sqlexec/engine.py
--rw-rw-rw-   0        0        0    13769 2023-08-01 16:09:28.000000 sqlx-exec-1.4.5/sqlexec/exec.py
--rw-rw-rw-   0        0        0     2025 2023-08-01 10:12:06.000000 sqlx-exec-1.4.5/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      984 2023-08-01 15:30:49.000000 sqlx-exec-1.4.5/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.4.5/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     2174 2023-08-01 15:23:57.000000 sqlx-exec-1.4.5/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.4.5/sqlexec/support.py
--rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.5/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3750 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 01:37:03.000000 sqlx-exec-1.4.6/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.6/LICENSE
+-rw-rw-rw-   0        0        0     3750 2023-08-04 01:37:03.000000 sqlx-exec-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3163 2023-08-01 10:41:13.000000 sqlx-exec-1.4.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-04 01:37:03.000000 sqlx-exec-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-08-04 01:36:33.000000 sqlx-exec-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:37:03.000000 sqlx-exec-1.4.6/sqlexec/
+-rw-rw-rw-   0        0        0      977 2023-08-01 15:23:57.000000 sqlx-exec-1.4.6/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2511 2023-08-03 03:26:25.000000 sqlx-exec-1.4.6/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    13604 2023-08-03 03:26:25.000000 sqlx-exec-1.4.6/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     2025 2023-08-01 10:12:06.000000 sqlx-exec-1.4.6/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0     1002 2023-08-02 04:09:46.000000 sqlx-exec-1.4.6/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0      764 2023-08-04 01:32:48.000000 sqlx-exec-1.4.6/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     2174 2023-08-01 15:23:57.000000 sqlx-exec-1.4.6/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-08-02 04:09:24.000000 sqlx-exec-1.4.6/sqlexec/support.py
+-rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.6/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:37:03.000000 sqlx-exec-1.4.6/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-04 01:37:03.000000 sqlx-exec-1.4.6/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.6/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3750 2023-08-04 01:37:03.000000 sqlx-exec-1.4.6/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-08-04 01:37:03.000000 sqlx-exec-1.4.6/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-08-04 01:37:03.000000 sqlx-exec-1.4.6/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.4.5/LICENSE` & `sqlx-exec-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.5/PKG-INFO` & `sqlx-exec-1.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.4.5
+Version: 1.4.6
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.4.5/README.rst` & `sqlx-exec-1.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.5/setup.py` & `sqlx-exec-1.4.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.4.5',
+    version='1.4.6',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.4.5/sqlexec/constant.py` & `sqlx-exec-1.4.6/sqlexec/constant.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.5/sqlexec/engine.py` & `sqlx-exec-1.4.6/sqlexec/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     def __init__(self, name, trans_placeholder, show_sql = False):
         self.name = name
         self.show_sql = show_sql
         self.trans_placeholder = trans_placeholder
 
     @classmethod
     def init(cls, name=UNKNOW, trans_placeholder=None):
-        cls.init0(name, trans_placeholder, show_sql=False)
+        cls.do_init(name, trans_placeholder, show_sql=False)
 
     @classmethod
-    def init0(cls, name, trans_placeholder, show_sql):
+    def do_init(cls, name, trans_placeholder, show_sql):
         global _ENGINE
         if _ENGINE:
             _ENGINE.show_sql = show_sql
             if _ENGINE.name is None or _ENGINE.name == UNKNOW:
                 _ENGINE.name = name
             if _ENGINE.trans_placeholder is None:
                 _ENGINE.trans_placeholder = trans_placeholder
```

### Comparing `sqlx-exec-1.4.5/sqlexec/exec.py` & `sqlx-exec-1.4.6/sqlexec/exec.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
         _DB_CTX = DBCtx(connect=connect, prepared=prepared)
 
     if SQLITE == engine:
         trans_placeholder = False
-    Engine.init0(engine, trans_placeholder, show_sql)
+    Engine.do_init(engine, trans_placeholder, show_sql)
     if pool_size > 0:
         logger.info("Inited db engine <%s> of %s with driver: '%s' and pool size: %d." % (hex(id(_DB_CTX)), engine, driver, pool_size))
     else:
         logger.info("Inited db engine <%s> of %s with driver: '%s'." % (hex(id(_DB_CTX)), engine, driver))
 
 
 def connection():
@@ -168,52 +168,14 @@
     :return: Primary key
     """
     logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t sql: %s \n\t args: %s \n\t kwargs: %s" % ('save_sql', select_key, sql, args, kwargs))
     sql, args = sql_support.get_mapping_sql_args(sql, *args, **kwargs)
     return do_save_sql(select_key, sql, *args)
 
 
-def batch_insert(table: str, *args):
-    """
-    Batch insert
-    :param table: table name
-    :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
-    :return: Effect row count
-    """
-    logger.debug("Exec func 'sqlexec.%s' \n\t Table: '%s', args: %s" % ('batch_insert', table, args))
-    sql, args = sql_support.batch_insert_sql_args(table, *args)
-    return batch_execute(sql, *args)
-
-
-@with_connection
-def batch_execute(sql: str, *args):
-    """
-    Batch execute sql return effect rowcount
-    :param sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
-    :param args: All number must have same size.
-    :return: Effect rowcount
-    """
-    global _DB_CTX
-    cursor = None
-    assert args, "*args must not be empty."
-    if isinstance(args[0], dict):
-        sql, args = sql_support.batch_named_sql_args(sql, *args)
-    sql = Engine.before_execute_intf('batch_execute', sql.strip(), *args)
-    args = sql_support.get_batch_args(*args)
-    try:
-        cursor = _DB_CTX.cursor()
-        cursor.executemany(sql, args)
-        effect_rowcount = cursor.rowcount
-        try_commit(_DB_CTX)
-        return effect_rowcount
-    finally:
-        if cursor:
-            cursor.close()
-
-
 def get(sql: str, *args, **kwargs):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     sql, args = try_mapping('sqlexec.get', sql, *args, **kwargs)
@@ -252,57 +214,31 @@
     execute select SQL and return unique result(dict), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
     sql, args = try_mapping('sqlexec.query_one', sql, *args, **kwargs)
     return do_query_one(sql, *args)
 
 
-@with_connection
 def do_execute(sql: str, *args):
     """
     Execute sql return effect rowcount
     sql: insert into person(name, age) values(?, ?)  -->  args: ('张三', 20)
     """
-    global _DB_CTX
-    cursor = None
-    sql = Engine.before_execute_intf('do_execute', sql.strip(), *args)
-    try:
-        cursor = _DB_CTX.connection.cursor()
-        cursor.execute(sql, args)
-        effect_rowcount = cursor.rowcount
-        try_commit(_DB_CTX)
-        return effect_rowcount
-    finally:
-        if cursor:
-            cursor.close()
+    return _execute(None, sql, *args)
 
 
-@with_connection
 def do_save_sql(select_key: str, sql: str, *args):
     """
     Insert data into table, return primary key.
     :param select_key: sql for select primary key
     :param sql: table
     :param args:
     :return: Primary key
     """
-    global _DB_CTX
-    cursor = None
-    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s" % ('do_save_sql', select_key))
-    sql = Engine.before_execute_intf('save_sql', sql, *args)
-    try:
-        cursor = _DB_CTX.connection.cursor()
-        cursor.execute(sql, args)
-        cursor.execute(select_key)
-        result = cursor.fetchone()
-        try_commit(_DB_CTX)
-        return result[0]
-    finally:
-        if cursor:
-            cursor.close()
+    return _execute(select_key, sql, *args)
 
 
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
@@ -356,14 +292,79 @@
     result, description = _select_one(sql, *args)
     if result and description:
         names = list(map(lambda x: x[0], description))
         return Dict(names, result)
     return result
 
 
+def batch_insert(table: str, *args):
+    """
+    Batch insert
+    :param table: table name
+    :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
+    :return: Effect row count
+    """
+    logger.debug("Exec func 'sqlexec.%s' \n\t Table: '%s', args: %s" % ('batch_insert', table, args))
+    sql, args = sql_support.batch_insert_sql_args(table, *args)
+    return batch_execute(sql, *args)
+
+
+@with_connection
+def batch_execute(sql: str, *args):
+    """
+    Batch execute sql return effect rowcount
+    :param sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
+    :param args: All number must have same size.
+    :return: Effect rowcount
+    """
+    global _DB_CTX
+    cursor = None
+    assert args, "*args must not be empty."
+    if isinstance(args[0], dict):
+        sql, args = sql_support.batch_named_sql_args(sql, *args)
+    sql = Engine.before_execute_intf('batch_execute', sql.strip(), *args)
+    args = sql_support.get_batch_args(*args)
+    try:
+        cursor = _DB_CTX.cursor()
+        cursor.executemany(sql, args)
+        effect_rowcount = cursor.rowcount
+        try_commit(_DB_CTX)
+        return effect_rowcount
+    finally:
+        if cursor:
+            cursor.close()
+
+
+def get_connection():
+    global _DB_CTX
+    _DB_CTX.try_init()
+    return _DB_CTX.connection
+
+
+@with_connection
+def _execute(select_key: str, sql: str, *args):
+    global _DB_CTX
+    cursor = None
+    logger.debug("Exec func 'sqlexec.%s', 'select_key': %s" % ('_execute', select_key))
+    sql = Engine.before_execute_intf('_execute', sql, *args)
+    try:
+        cursor = _DB_CTX.connection.cursor()
+        cursor.execute(sql, args)
+        if select_key:
+            cursor.execute(select_key)
+            result = cursor.fetchone()[0]
+        else:
+            result = cursor.rowcount
+        try_commit(_DB_CTX)
+        return result
+    finally:
+        if cursor:
+            cursor.close()
+
+
 @with_connection
 def _select(sql: str, *args):
     global _DB_CTX
     cursor = None
     sql = Engine.before_execute_intf('do_select', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
@@ -385,20 +386,14 @@
         cursor.execute(sql, args)
         return cursor.fetchone(), cursor.description
     finally:
         if cursor:
             cursor.close()
 
 
-def get_connection():
-    global _DB_CTX
-    _DB_CTX.try_init()
-    return _DB_CTX.connection
-
-
 def try_mapping(function, sql, *args, **kwargs):
     sql_log(function, sql, *args, **kwargs)
     return sql_support.get_mapping_sql_args(sql, *args, **kwargs)
 
 
 def _do_limit_sql_args(function, sql, *args):
     do_sql_log(function, sql, *args)
```

### Comparing `sqlx-exec-1.4.5/sqlexec/init_import.py` & `sqlx-exec-1.4.6/sqlexec/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.5/sqlexec/log_support.py` & `sqlx-exec-1.4.6/sqlexec/log_support.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import threading
 from logging import basicConfig, INFO, getLogger
 
 logger = getLogger(__name__)
 basicConfig(level=INFO, format='[%(levelname)s]: %(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
 
 def insert_log(function: str, table: str, **kwargs):
@@ -17,9 +18,9 @@
 
 
 def do_sql_log(function: str, sql: str, *args):
     logger.debug("Exec func '%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
 
 
 def db_ctx_log(action, connection):
-    logger.debug('%s connection <%s>...' % (action, hex(id(connection))))
+    logger.debug("%s connection <%s>..." % (action, hex(id(connection))))
```

### Comparing `sqlx-exec-1.4.5/sqlexec/sql_support.py` & `sqlx-exec-1.4.6/sqlexec/sql_support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.5/sqlexec/support.py` & `sqlx-exec-1.4.6/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.5/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.4.6/sqlx_exec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.4.5
+Version: 1.4.6
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
```

