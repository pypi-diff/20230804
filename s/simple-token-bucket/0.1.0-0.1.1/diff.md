# Comparing `tmp/simple_token_bucket-0.1.0.tar.gz` & `tmp/simple_token_bucket-0.1.1.tar.gz`

## Comparing `simple_token_bucket-0.1.0.tar` & `simple_token_bucket-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/docs/api.rst
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/docs/contributing.rst
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/docs/index.rst
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/simple_token_bucket/__init__.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/simple_token_bucket/backends/__init__.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/simple_token_bucket/backends/redis.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/tests/test_redis_backend.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/.gitignore
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/README.md
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/docs/api.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/docs/conf.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/docs/contributing.rst
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/docs/index.rst
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/simple_token_bucket/__init__.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/simple_token_bucket/backends/__init__.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/simple_token_bucket/backends/redis.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/tests/test_redis_backend.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/README.md
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 simple_token_bucket-0.1.1/PKG-INFO
```

### Comparing `simple_token_bucket-0.1.0/.github/workflows/test.yml` & `simple_token_bucket-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.0/docs/conf.py` & `simple_token_bucket-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.0/docs/contributing.rst` & `simple_token_bucket-0.1.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.0/docs/index.rst` & `simple_token_bucket-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.0/simple_token_bucket/__init__.py` & `simple_token_bucket-0.1.1/simple_token_bucket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 
 from .backends import Backend
 
 
 class SimpleTokenBucket:
     def __init__(self, name: str, bucket_size: int, refresh_interval: int, backend: Backend):
```

### Comparing `simple_token_bucket-0.1.0/simple_token_bucket/backends/__init__.py` & `simple_token_bucket-0.1.1/simple_token_bucket/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.0/simple_token_bucket/backends/redis.py` & `simple_token_bucket-0.1.1/simple_token_bucket/backends/redis.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,8 +16,10 @@
         pipeline = self._client.pipeline()
         pipeline.set(bucket_name, bucket_size, nx=True, ex=refresh_interval)
         pipeline.ttl(bucket_name)
         pipeline.get(bucket_name)
         pipeline.decr(bucket_name)
         _, ttl, available_tokens, _ = pipeline.execute()
 
+        if ttl < 0:
+            return int(bucket_size), refresh_interval
         return int(available_tokens), ttl
```

### Comparing `simple_token_bucket-0.1.0/tests/test_redis_backend.py` & `simple_token_bucket-0.1.1/tests/test_redis_backend.py`

 * *Files identical despite different names*

### Comparing `simple_token_bucket-0.1.0/pyproject.toml` & `simple_token_bucket-0.1.1/pyproject.toml`

 * *Files identical despite different names*

