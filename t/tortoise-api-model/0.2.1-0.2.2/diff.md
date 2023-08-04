# Comparing `tmp/tortoise_api_model-0.2.1.tar.gz` & `tmp/tortoise_api_model-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_api_model-0.2.1.tar", last modified: Thu Aug  3 08:03:16 2023, max compression
+gzip compressed data, was "tortoise_api_model-0.2.2.tar", last modified: Thu Aug  3 17:57:36 2023, max compression
```

## Comparing `tortoise_api_model-0.2.1.tar` & `tortoise_api_model-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 08:03:16.949791 tortoise_api_model-0.2.1/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-08-03 08:03:16.949575 tortoise_api_model-0.2.1/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-08-03 08:03:16.949845 tortoise_api_model-0.2.1/setup.cfg
--rw-r--r--   0 sol        (501) staff       (20)      819 2023-08-03 06:39:10.000000 tortoise_api_model-0.2.1/setup.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 08:03:16.948372 tortoise_api_model-0.2.1/tortoise_api_model/
--rw-r--r--   0 sol        (501) staff       (20)      140 2023-08-01 16:56:50.000000 tortoise_api_model-0.2.1/tortoise_api_model/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)      280 2023-07-30 18:24:21.000000 tortoise_api_model-0.2.1/tortoise_api_model/consts.py
--rw-r--r--   0 sol        (501) staff       (20)     1538 2023-08-02 10:01:54.000000 tortoise_api_model-0.2.1/tortoise_api_model/fields.py
--rw-r--r--   0 sol        (501) staff       (20)     6436 2023-08-03 06:28:34.000000 tortoise_api_model-0.2.1/tortoise_api_model/model.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 08:03:16.949335 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-08-03 08:03:16.000000 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      334 2023-08-03 08:03:16.000000 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-08-03 08:03:16.000000 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-08-03 08:03:16.000000 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       19 2023-08-03 08:03:16.000000 tortoise_api_model-0.2.1/tortoise_api_model.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 17:57:36.085681 tortoise_api_model-0.2.2/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-08-03 17:57:36.085469 tortoise_api_model-0.2.2/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-08-03 17:57:36.085733 tortoise_api_model-0.2.2/setup.cfg
+-rw-r--r--   0 sol        (501) staff       (20)      819 2023-08-03 17:56:43.000000 tortoise_api_model-0.2.2/setup.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 17:57:36.082996 tortoise_api_model-0.2.2/tortoise_api_model/
+-rw-r--r--   0 sol        (501) staff       (20)      140 2023-08-01 16:56:50.000000 tortoise_api_model-0.2.2/tortoise_api_model/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)      280 2023-07-30 18:24:21.000000 tortoise_api_model-0.2.2/tortoise_api_model/consts.py
+-rw-r--r--   0 sol        (501) staff       (20)     1538 2023-08-02 10:01:54.000000 tortoise_api_model-0.2.2/tortoise_api_model/fields.py
+-rw-r--r--   0 sol        (501) staff       (20)     6563 2023-08-03 08:13:34.000000 tortoise_api_model-0.2.2/tortoise_api_model/model.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-08-03 17:57:36.085220 tortoise_api_model-0.2.2/tortoise_api_model.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-08-03 17:57:36.000000 tortoise_api_model-0.2.2/tortoise_api_model.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      334 2023-08-03 17:57:36.000000 tortoise_api_model-0.2.2/tortoise_api_model.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-08-03 17:57:36.000000 tortoise_api_model-0.2.2/tortoise_api_model.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-08-03 17:57:36.000000 tortoise_api_model-0.2.2/tortoise_api_model.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       19 2023-08-03 17:57:36.000000 tortoise_api_model-0.2.2/tortoise_api_model.egg-info/top_level.txt
```

### Comparing `tortoise_api_model-0.2.1/setup.py` & `tortoise_api_model-0.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'Base model for tortoise-api'
 LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="tortoise_api_model",
     version=VERSION,
```

### Comparing `tortoise_api_model-0.2.1/tortoise_api_model/fields.py` & `tortoise_api_model-0.2.2/tortoise_api_model/fields.py`

 * *Files identical despite different names*

### Comparing `tortoise_api_model-0.2.1/tortoise_api_model/model.py` & `tortoise_api_model-0.2.2/tortoise_api_model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,29 +30,31 @@
         for fk in cls._meta.fetch_fields:
             field: RelationalField = cls._meta.fields_map[fk]
             first: {str: str} = {'': 'Empty'} if field.null else {}
             res[fk] = {**first, **{x.pk: x.repr() for x in await field.related_model.all()}}
         cls._options = res
 
     @classmethod
-    async def upsert(cls, data: dict):
+    async def upsert(cls, data: dict, oid = None):
         meta: MetaInfo = cls._meta
 
         # pop fields for relations from general data dict
-        m2ms = {k: data.pop(k) for k in cls._meta.m2m_fields if k in data}
-        bfks = {k: data.pop(k) for k in cls._meta.backward_fk_fields if k in data}
-        bo2os = {k: data.pop(k) for k in cls._meta.backward_o2o_fields if k in data}
+        m2ms = {k: data.pop(k) for k in meta.m2m_fields if k in data}
+        bfks = {k: data.pop(k) for k in meta.backward_fk_fields if k in data}
+        bo2os = {k: data.pop(k) for k in meta.backward_o2o_fields if k in data}
 
         # save general model
-        if pk := meta.pk_attr in data.keys():
-            unq = {pk: data.pop(pk)}
-        else:
-            unq = {key: data.pop(key) for key, ft in meta.fields_map.items() if ft.unique and key in data.keys()}
-        # unq = meta.unique_together
-        obj, is_created = await cls.update_or_create(data, **unq)
+
+        # if pk := meta.pk_attr in data.keys():
+        #     unq = {pk: data.pop(pk)}
+        # else:
+        #     unq = {key: data.pop(key) for key, ft in meta.fields_map.items() if ft.unique and key in data.keys()}
+        # # unq = meta.unique_together
+        # obj, is_created = await cls.update_or_create(data, **unq)
+        obj, cr = await cls.create(**data), True if oid else await cls.update_or_create(data, **{meta.pk_attr: oid})
 
         # save relations
         for k, ids in m2ms.items():
             m2m_rel: ManyToManyRelation = getattr(obj, k)
             items = [await m2m_rel.remote_model[i] for i in ids]
             await m2m_rel.add(*items)
         for k, ids in bfks.items():
```

