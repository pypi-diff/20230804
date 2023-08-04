# Comparing `tmp/bbat-0.2.1.tar.gz` & `tmp/bbat-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbat-0.2.1.tar", last modified: Fri Jul 28 01:14:06 2023, max compression
+gzip compressed data, was "bbat-0.2.2.tar", last modified: Fri Aug  4 03:30:41 2023, max compression
```

## Comparing `bbat-0.2.1.tar` & `bbat-0.2.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.562837 bbat-0.2.1/
--rw-rw-rw-   0        0        0      289 2023-07-28 01:14:06.561852 bbat-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-07-11 11:39:46.000000 bbat-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.413354 bbat-0.2.1/bbat/
--rw-rw-rw-   0        0        0        0 2023-07-09 13:29:18.000000 bbat-0.2.1/bbat/__init__.py
--rw-rw-rw-   0        0        0     1931 2023-07-18 01:38:19.000000 bbat-0.2.1/bbat/config.py
--rw-rw-rw-   0        0        0     3115 2023-07-17 07:29:02.000000 bbat-0.2.1/bbat/crypto.py
--rw-rw-rw-   0        0        0     1230 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/date.py
-drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.457235 bbat-0.2.1/bbat/db/
--rw-rw-rw-   0        0        0        0 2023-07-09 13:50:02.000000 bbat-0.2.1/bbat/db/__init__.py
--rw-rw-rw-   0        0        0     5722 2023-07-19 08:56:34.000000 bbat-0.2.1/bbat/db/aio_mysql.py
--rw-rw-rw-   0        0        0     2632 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/db/aio_sqlite.py
--rw-rw-rw-   0        0        0     2054 2023-07-15 12:58:24.000000 bbat-0.2.1/bbat/db/mysql.py
--rw-rw-rw-   0        0        0      491 2023-07-17 08:36:20.000000 bbat-0.2.1/bbat/document.py
--rw-rw-rw-   0        0        0       30 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/hi.py
--rw-rw-rw-   0        0        0     1978 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/image.py
-drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.465240 bbat-0.2.1/bbat/llm/
--rw-rw-rw-   0        0        0        0 2023-07-11 14:42:42.000000 bbat-0.2.1/bbat/llm/__init__.py
--rw-rw-rw-   0        0        0     2416 2023-07-12 14:36:12.000000 bbat-0.2.1/bbat/llm/chatgpt.py
--rw-rw-rw-   0        0        0      920 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/log.py
--rw-rw-rw-   0        0        0      828 2023-07-12 11:52:42.000000 bbat-0.2.1/bbat/machine.py
--rw-rw-rw-   0        0        0     1868 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/notice.py
--rw-rw-rw-   0        0        0     2497 2023-07-10 11:37:38.000000 bbat-0.2.1/bbat/np.py
--rw-rw-rw-   0        0        0     1764 2023-07-18 01:35:45.000000 bbat-0.2.1/bbat/path.py
--rw-rw-rw-   0        0        0     4198 2023-07-11 15:55:34.000000 bbat-0.2.1/bbat/text.py
-drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.499230 bbat-0.2.1/bbat/web/
--rw-rw-rw-   0        0        0        0 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/__init__.py
--rw-rw-rw-   0        0        0     1685 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/client.py
--rw-rw-rw-   0        0        0      504 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/cors.py
--rw-rw-rw-   0        0        0     4501 2023-07-27 07:39:54.000000 bbat-0.2.1/bbat/web/db_server.py
--rw-rw-rw-   0        0        0      177 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/flask_app.py
--rw-rw-rw-   0        0        0     1566 2023-07-13 12:06:02.000000 bbat-0.2.1/bbat/web/sanic_app.py
-drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.548850 bbat-0.2.1/bbat/web/url_to_sql/
--rw-rw-rw-   0        0        0        0 2023-07-10 11:37:38.000000 bbat-0.2.1/bbat/web/url_to_sql/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/url_to_sql/field.py
--rw-rw-rw-   0        0        0     7452 2023-07-27 07:40:43.000000 bbat-0.2.1/bbat/web/url_to_sql/query.py
--rw-rw-rw-   0        0        0     2256 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/url_to_sql/relation.py
--rw-rw-rw-   0        0        0      722 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/url_to_sql/test.py
--rw-rw-rw-   0        0        0      964 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/url_to_sql/util.py
--rw-rw-rw-   0        0        0     1473 2023-07-11 11:39:46.000000 bbat-0.2.1/bbat/web/url_to_sql/where.py
--rw-rw-rw-   0        0        0     1614 2023-07-12 11:52:42.000000 bbat-0.2.1/bbat/zcli.py
-drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.434731 bbat-0.2.1/bbat.egg-info/
--rw-rw-rw-   0        0        0      289 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      876 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      131 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-28 01:14:06.000000 bbat-0.2.1/bbat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 01:14:06.563838 bbat-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-07-28 01:13:39.000000 bbat-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 01:14:06.560838 bbat-0.2.1/test/
--rw-rw-rw-   0        0        0      209 2023-07-11 11:39:46.000000 bbat-0.2.1/test/test_config.py
--rw-rw-rw-   0        0        0      194 2023-07-11 11:39:46.000000 bbat-0.2.1/test/test_db_mysql.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:30:41.754098 bbat-0.2.2/
+-rw-rw-rw-   0        0        0      289 2023-08-04 03:30:41.753097 bbat-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-07-11 11:39:46.000000 bbat-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 03:30:41.604249 bbat-0.2.2/bbat/
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:29:18.000000 bbat-0.2.2/bbat/__init__.py
+-rw-rw-rw-   0        0        0     1931 2023-07-18 01:38:19.000000 bbat-0.2.2/bbat/config.py
+-rw-rw-rw-   0        0        0     3115 2023-07-17 07:29:02.000000 bbat-0.2.2/bbat/crypto.py
+-rw-rw-rw-   0        0        0     1230 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/date.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:30:41.668603 bbat-0.2.2/bbat/db/
+-rw-rw-rw-   0        0        0        0 2023-07-09 13:50:02.000000 bbat-0.2.2/bbat/db/__init__.py
+-rw-rw-rw-   0        0        0     5619 2023-08-04 03:28:52.000000 bbat-0.2.2/bbat/db/aio_mysql.py
+-rw-rw-rw-   0        0        0     2632 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/db/aio_sqlite.py
+-rw-rw-rw-   0        0        0     2020 2023-08-04 03:29:37.000000 bbat-0.2.2/bbat/db/mysql.py
+-rw-rw-rw-   0        0        0      491 2023-07-17 08:36:20.000000 bbat-0.2.2/bbat/document.py
+-rw-rw-rw-   0        0        0       30 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/hi.py
+-rw-rw-rw-   0        0        0     1978 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/image.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:30:41.679602 bbat-0.2.2/bbat/llm/
+-rw-rw-rw-   0        0        0        0 2023-07-11 14:42:42.000000 bbat-0.2.2/bbat/llm/__init__.py
+-rw-rw-rw-   0        0        0     2416 2023-07-12 14:36:12.000000 bbat-0.2.2/bbat/llm/chatgpt.py
+-rw-rw-rw-   0        0        0      920 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/log.py
+-rw-rw-rw-   0        0        0      828 2023-07-12 11:52:42.000000 bbat-0.2.2/bbat/machine.py
+-rw-rw-rw-   0        0        0     1868 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/notice.py
+-rw-rw-rw-   0        0        0     2497 2023-07-10 11:37:38.000000 bbat-0.2.2/bbat/np.py
+-rw-rw-rw-   0        0        0     1764 2023-07-18 01:35:45.000000 bbat-0.2.2/bbat/path.py
+-rw-rw-rw-   0        0        0     4198 2023-07-11 15:55:34.000000 bbat-0.2.2/bbat/text.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:30:41.723610 bbat-0.2.2/bbat/web/
+-rw-rw-rw-   0        0        0        0 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/web/__init__.py
+-rw-rw-rw-   0        0        0     1685 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/web/client.py
+-rw-rw-rw-   0        0        0      504 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/web/cors.py
+-rw-rw-rw-   0        0        0     4665 2023-08-04 02:58:55.000000 bbat-0.2.2/bbat/web/db_server.py
+-rw-rw-rw-   0        0        0      177 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/web/flask_app.py
+-rw-rw-rw-   0        0        0     1566 2023-07-13 12:06:02.000000 bbat-0.2.2/bbat/web/sanic_app.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:30:41.739098 bbat-0.2.2/bbat/web/url_to_sql/
+-rw-rw-rw-   0        0        0        0 2023-07-10 11:37:38.000000 bbat-0.2.2/bbat/web/url_to_sql/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/web/url_to_sql/field.py
+-rw-rw-rw-   0        0        0     7452 2023-07-27 07:40:43.000000 bbat-0.2.2/bbat/web/url_to_sql/query.py
+-rw-rw-rw-   0        0        0     2228 2023-07-28 01:27:46.000000 bbat-0.2.2/bbat/web/url_to_sql/relation.py
+-rw-rw-rw-   0        0        0      722 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/web/url_to_sql/test.py
+-rw-rw-rw-   0        0        0      964 2023-07-11 11:39:46.000000 bbat-0.2.2/bbat/web/url_to_sql/util.py
+-rw-rw-rw-   0        0        0     1473 2023-08-04 03:10:25.000000 bbat-0.2.2/bbat/web/url_to_sql/where.py
+-rw-rw-rw-   0        0        0     1614 2023-08-01 07:40:00.000000 bbat-0.2.2/bbat/zcli.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:30:41.652599 bbat-0.2.2/bbat.egg-info/
+-rw-rw-rw-   0        0        0      289 2023-08-04 03:30:41.000000 bbat-0.2.2/bbat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      876 2023-08-04 03:30:41.000000 bbat-0.2.2/bbat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 03:30:41.000000 bbat-0.2.2/bbat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-04 03:30:41.000000 bbat-0.2.2/bbat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-08-04 03:30:41.000000 bbat-0.2.2/bbat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-04 03:30:41.000000 bbat-0.2.2/bbat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 03:30:41.754098 bbat-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1027 2023-08-04 03:30:27.000000 bbat-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:30:41.752099 bbat-0.2.2/test/
+-rw-rw-rw-   0        0        0      209 2023-07-11 11:39:46.000000 bbat-0.2.2/test/test_config.py
+-rw-rw-rw-   0        0        0      194 2023-07-11 11:39:46.000000 bbat-0.2.2/test/test_db_mysql.py
```

### Comparing `bbat-0.2.1/bbat/config.py` & `bbat-0.2.2/bbat/config.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/crypto.py` & `bbat-0.2.2/bbat/crypto.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/date.py` & `bbat-0.2.2/bbat/date.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/db/aio_mysql.py` & `bbat-0.2.2/bbat/db/aio_mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,34 +69,34 @@
         """Returns the (singular) row returned by the given query.
         """
         if not self.pool:
             await self.init_pool()
         async with self.pool.acquire() as conn:
             async with conn.cursor() as cur:
                 try:
-                    await cur.execute(query, kwargs or args)
+                    await cur.execute(query)
                     ret = await cur.fetchone()
                 except pymysql.err.InternalError:
                     await conn.ping()
-                    await cur.execute(query, kwargs or args)
+                    await cur.execute(query)
                     ret = await cur.fetchone()
                 return ret
 
     async def execute(self, query, *args, **kwargs):
         """Executes the given query, returning the lastrowid from the query."""
         if not self.pool:
             await self.init_pool()
         async with self.pool.acquire() as conn:
             async with conn.cursor() as cur:
                 try:
-                    await cur.execute(query, kwargs or args)
+                    await cur.execute(query)
                 except Exception:
                     # https://github.com/aio-libs/aiomysql/issues/340
                     await conn.ping()
-                    await cur.execute(query, kwargs or args)
+                    await cur.execute(query)
                 return cur.lastrowid
             
     async def insert(self, table, data):
         keys = []
         values = []
         for k, v in data.items():
             if v is None: continue
@@ -104,15 +104,14 @@
             if isinstance(v, str):
                 v = v.replace("'", "\'")
             values.append(f"'{v}'")
             
         keys = ','.join(keys)
         values = ','.join(values)
         sql = f'INSERT INTO {table} ({keys}) VALUES ({values})'
-        print('>>> insert sql:', sql)
         res = await self.execute(sql)
         return res
 
     async def update(self, table, data, where=None):
         set_list = [f'`{k}`="{v}"' for k, v in data.items()]
         sql = f"update {table} set {','.join(set_list)}"
         if where:
```

### Comparing `bbat-0.2.1/bbat/db/aio_sqlite.py` & `bbat-0.2.2/bbat/db/aio_sqlite.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/db/mysql.py` & `bbat-0.2.2/bbat/db/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,13 +53,12 @@
 
     def insert(self, table=None, data_list: list = []):
         cur = self.conn.cursor()
         for data in data_list:
             field = ",".join([f"`{key}`" for key in data.keys()])
             value = ",".join([f'"{val}"' for val in data.values()])
             sql = f"insert into {table}({field}) values({value})"
-            print("sql>>>", sql)
             cur.execute(sql)
         self.conn.commit()
 
     def quit(self):
         self.conn.close()
```

### Comparing `bbat-0.2.1/bbat/image.py` & `bbat-0.2.2/bbat/image.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/llm/chatgpt.py` & `bbat-0.2.2/bbat/llm/chatgpt.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/log.py` & `bbat-0.2.2/bbat/log.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/machine.py` & `bbat-0.2.2/bbat/machine.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/notice.py` & `bbat-0.2.2/bbat/notice.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/np.py` & `bbat-0.2.2/bbat/np.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/path.py` & `bbat-0.2.2/bbat/path.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/text.py` & `bbat-0.2.2/bbat/text.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/web/client.py` & `bbat-0.2.2/bbat/web/client.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/web/db_server.py` & `bbat-0.2.2/bbat/web/db_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,18 @@
 
     sql = query.to_sql()
     # 1.主表查询
     data = await db.query(sql)
     # 根据field定义，做数据处理
     data = query.data_convert(query.fields, data)
     # 2.统计查询
-    info = await db.fetch(query.to_count_sql())
+    print('......', len(data))
+    count_sql = query.to_count_sql()
+    print(count_sql)
+    info = await db.fetch(count_sql)
     result["meta"] = {"total": info["cnt"]}
     # 3.子表查询
     for relation in query.relation:
         # master表外键所有id
         idhub = set([str(i[relation.master_key]) for i in data])
         if len(idhub) == 0:
             continue
@@ -67,20 +70,23 @@
     if not data:
         return error("ERROR: data is null")
     # 有query触发更新
     query = Query(table, query_string)
     if query_string:
         sql = query.to_update_sql(data)
         result = await db.execute(sql)
-        return success(result)
+        return success(data)
     else:
         # sql = query.to_insert_sql(data)
         # result = await db.execute(sql)
         result = await db.insert(table, data)
-        return success(result)
+        if not result:
+            return error(result)
+        data['id'] = result
+        return success(data)
 
 
 # delete data
 @router.delete("/hyper/{table}")
 async def delete(table, request: Request):
     db = router.db
     query_string = request.query_params
```

### Comparing `bbat-0.2.1/bbat/web/sanic_app.py` & `bbat-0.2.2/bbat/web/sanic_app.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/web/url_to_sql/field.py` & `bbat-0.2.2/bbat/web/url_to_sql/field.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/web/url_to_sql/query.py` & `bbat-0.2.2/bbat/web/url_to_sql/query.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/web/url_to_sql/relation.py` & `bbat-0.2.2/bbat/web/url_to_sql/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         jobs[project_id=id, name,created_at]
     '''
     def __init__(self, query):
         self.query = query
         if not self.check_query():
             return
         self.table, field_match = cutout(r"[\[\{].*?[\]\}]", query)
-        print(field_match)
         if field_match.startswith("["):
             self.type = 1
         elif field_match.startswith("{"):
             self.type = 0
         else: 
             raise ValueError("join格式错误")
         field_match = re.sub(r"[\[\]\{\}]", "", field_match)
```

### Comparing `bbat-0.2.1/bbat/web/url_to_sql/test.py` & `bbat-0.2.2/bbat/web/url_to_sql/test.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/web/url_to_sql/util.py` & `bbat-0.2.2/bbat/web/url_to_sql/util.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/web/url_to_sql/where.py` & `bbat-0.2.2/bbat/web/url_to_sql/where.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat/zcli.py` & `bbat-0.2.2/bbat/zcli.py`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/bbat.egg-info/SOURCES.txt` & `bbat-0.2.2/bbat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbat-0.2.1/setup.py` & `bbat-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import setuptools
 
 name = "bbat"
-version = "0.2.1"
+version = "0.2.2"
 
 def _process_requirements():
     packages = open('requirements.txt').read().strip().split('\n')
     requires = []
     for pkg in packages:
         if pkg.startswith('git+ssh'):
             return_code = os.system('pip install {}'.format(pkg))
```

