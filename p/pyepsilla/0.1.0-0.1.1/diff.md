# Comparing `tmp/pyepsilla-0.1.0.tar.gz` & `tmp/pyepsilla-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyepsilla-0.1.0.tar", last modified: Sun Jul 30 14:40:26 2023, max compression
+gzip compressed data, was "pyepsilla-0.1.1.tar", last modified: Thu Aug  3 22:52:24 2023, max compression
```

## Comparing `pyepsilla-0.1.0.tar` & `pyepsilla-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/pyepsilla/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/pyepsilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/pyepsilla/simple_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/pyepsilla/vectordb/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/pyepsilla/vectordb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/pyepsilla/vectordb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/pyepsilla/vectordb/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/pyepsilla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-30 14:40:26.000000 pyepsilla-0.1.0/pyepsilla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-30 14:40:26.000000 pyepsilla-0.1.0/pyepsilla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 14:40:26.000000 pyepsilla-0.1.0/pyepsilla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 14:40:26.000000 pyepsilla-0.1.0/pyepsilla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 14:40:26.000000 pyepsilla-0.1.0/pyepsilla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 14:40:26.231106 pyepsilla-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-30 14:40:10.000000 pyepsilla-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:52:24.188443 pyepsilla-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-03 22:52:09.000000 pyepsilla-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 22:52:09.000000 pyepsilla-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-03 22:52:24.188443 pyepsilla-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-03 22:52:09.000000 pyepsilla-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:52:24.188443 pyepsilla-0.1.1/pyepsilla/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-03 22:52:09.000000 pyepsilla-0.1.1/pyepsilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-08-03 22:52:09.000000 pyepsilla-0.1.1/pyepsilla/simple_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:52:24.188443 pyepsilla-0.1.1/pyepsilla/vectordb/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-03 22:52:09.000000 pyepsilla-0.1.1/pyepsilla/vectordb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-08-03 22:52:09.000000 pyepsilla-0.1.1/pyepsilla/vectordb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-03 22:52:09.000000 pyepsilla-0.1.1/pyepsilla/vectordb/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 22:52:24.188443 pyepsilla-0.1.1/pyepsilla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-03 22:52:24.000000 pyepsilla-0.1.1/pyepsilla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-03 22:52:24.000000 pyepsilla-0.1.1/pyepsilla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 22:52:24.000000 pyepsilla-0.1.1/pyepsilla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-03 22:52:24.000000 pyepsilla-0.1.1/pyepsilla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 22:52:24.000000 pyepsilla-0.1.1/pyepsilla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 22:52:24.188443 pyepsilla-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-03 22:52:09.000000 pyepsilla-0.1.1/setup.py
```

### Comparing `pyepsilla-0.1.0/LICENSE` & `pyepsilla-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.1.0/README.md` & `pyepsilla-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.1.0/pyepsilla/simple_example.py` & `pyepsilla-0.1.1/pyepsilla/simple_example.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.1.0/pyepsilla/vectordb/client.py` & `pyepsilla-0.1.1/pyepsilla/vectordb/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,19 +39,21 @@
         status_code = res.status_code
         body = res.json()
         return status_code, body
 
     def use_db(self, db_name):
         self._db = db_name
 
-    def load_db(self, db_name, db_path, vector_scale=None):
+    def load_db(self, db_name, db_path, vector_scale=None, wal_enabled=None):
         req_url = "{}/api/load".format(self._baseurl)
         req_data= {"name": db_name, "path": db_path}
         if vector_scale is not None:
             req_data["vectorScale"] = vector_scale
+        if wal_enabled is not None:
+            req_data["walEnabled"] = wal_enabled
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
         return status_code, body
 
     def unload_db(self, db_name):
         req_url = "{}/api/{}/unload".format(self._baseurl, db_name)
@@ -88,14 +90,23 @@
         req_url = "{}/api/{}/data/query".format(self._baseurl, self._db)
         req_data= {"table": table_name, "queryField": query_field, "queryVector": query_vector, "response": response_fields, "limit": limit}
         res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
         status_code = res.status_code
         body = res.json()
         return status_code, body
 
+    def get(self, table_name="MyTable", response_fields=[]):
+        if self._db is None:
+            raise Exception("[ERROR] Please use_db() first!")
+        req_url = "{}/api/{}/data/get".format(self._baseurl, self._db)
+        req_data= {"table": table_name, "response": response_fields}
+        res = requests.post(url=req_url, data=json.dumps(req_data), headers=self._header)
+        status_code = res.status_code
+        body = res.json()
+        return status_code, body
 
     def drop_table(self, table_name="MyTable"):
         if self._db is None:
             raise Exception("[ERROR] Please use_db() first!")
         req_url = "{}/api/{}/schema/tables/{}".format(self._baseurl, self._db, table_name)
         req_data= None
         res = requests.delete(url=req_url, data=json.dumps(req_data), headers=self._header)
```

### Comparing `pyepsilla-0.1.0/pyepsilla/vectordb/field.py` & `pyepsilla-0.1.1/pyepsilla/vectordb/field.py`

 * *Files identical despite different names*

### Comparing `pyepsilla-0.1.0/setup.py` & `pyepsilla-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='pyepsilla',
-    version= '0.1.0',
+    version= '0.1.1',
     keywords='epsilla',
     author= 'Epsilla Team',
     description='Epsilla Python SDK',
     long_description='Epsilla Python SDK',
     license='Apache License',
     packages=find_packages(),
     include_package_data=True,
```

