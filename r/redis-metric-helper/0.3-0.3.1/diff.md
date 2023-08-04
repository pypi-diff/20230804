# Comparing `tmp/redis-metric-helper-0.3.tar.gz` & `tmp/redis-metric-helper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-metric-helper-0.3.tar", last modified: Thu Aug  3 16:04:12 2023, max compression
+gzip compressed data, was "redis-metric-helper-0.3.1.tar", last modified: Thu Aug  3 16:07:15 2023, max compression
```

## Comparing `redis-metric-helper-0.3.tar` & `redis-metric-helper-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 16:04:12.173353 redis-metric-helper-0.3/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.3/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1003 2023-08-03 16:04:12.173353 redis-metric-helper-0.3/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.3/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 16:04:12.173353 redis-metric-helper-0.3/metric_helper/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      800 2023-08-03 15:56:35.000000 redis-metric-helper-0.3/metric_helper/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      293 2023-08-03 15:42:28.000000 redis-metric-helper-0.3/metric_helper/apps.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7032 2023-08-01 14:40:40.000000 redis-metric-helper-0.3/metric_helper/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      653 2023-08-03 15:02:21.000000 redis-metric-helper-0.3/metric_helper/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2573 2023-08-03 15:56:41.000000 redis-metric-helper-0.3/metric_helper/connections.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.3/metric_helper/exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      185 2023-08-03 13:40:48.000000 redis-metric-helper-0.3/metric_helper/logging.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2528 2023-08-03 13:47:29.000000 redis-metric-helper-0.3/metric_helper/registry.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 16:04:12.173353 redis-metric-helper-0.3/redis_metric_helper.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1003 2023-08-03 16:04:12.000000 redis-metric-helper-0.3/redis_metric_helper.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      440 2023-08-03 16:04:12.000000 redis-metric-helper-0.3/redis_metric_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-08-03 16:04:12.000000 redis-metric-helper-0.3/redis_metric_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-08-03 16:04:12.000000 redis-metric-helper-0.3/redis_metric_helper.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-08-03 16:04:12.000000 redis-metric-helper-0.3/redis_metric_helper.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-08-03 16:04:12.173353 redis-metric-helper-0.3/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.3/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 16:07:15.650795 redis-metric-helper-0.3.1/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.3.1/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-08-03 16:07:15.646794 redis-metric-helper-0.3.1/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.3.1/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 16:07:15.646794 redis-metric-helper-0.3.1/metric_helper/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      802 2023-08-03 16:06:35.000000 redis-metric-helper-0.3.1/metric_helper/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      293 2023-08-03 15:42:28.000000 redis-metric-helper-0.3.1/metric_helper/apps.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7032 2023-08-01 14:40:40.000000 redis-metric-helper-0.3.1/metric_helper/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      653 2023-08-03 15:02:21.000000 redis-metric-helper-0.3.1/metric_helper/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2576 2023-08-03 16:06:16.000000 redis-metric-helper-0.3.1/metric_helper/connections.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.3.1/metric_helper/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      185 2023-08-03 13:40:48.000000 redis-metric-helper-0.3.1/metric_helper/logging.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2528 2023-08-03 13:47:29.000000 redis-metric-helper-0.3.1/metric_helper/registry.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 16:07:15.646794 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-08-03 16:07:15.000000 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      440 2023-08-03 16:07:15.000000 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-08-03 16:07:15.000000 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-08-03 16:07:15.000000 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-08-03 16:07:15.000000 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-08-03 16:07:15.650795 redis-metric-helper-0.3.1/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.3.1/setup.py
```

### Comparing `redis-metric-helper-0.3/LICENSE` & `redis-metric-helper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.3/PKG-INFO` & `redis-metric-helper-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.3
+Version: 0.3.1
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.3/metric_helper/__init__.py` & `redis-metric-helper-0.3.1/metric_helper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.3'
+__version__ = '0.3.1'
 
 
 
 
 def setup(connection_dict=None):
     """
     Example of ``connection_dict``::
```

### Comparing `redis-metric-helper-0.3/metric_helper/base.py` & `redis-metric-helper-0.3.1/metric_helper/base.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.3/metric_helper/conf.py` & `redis-metric-helper-0.3.1/metric_helper/conf.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.3/metric_helper/connections.py` & `redis-metric-helper-0.3.1/metric_helper/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,27 +66,27 @@
 
 _redis_proxy = _RedisProxy()
 
 
 
 
 def get_redis_connection(decode_responses=True):
-    return redis_proxy.connect()
+    return _redis_proxy.connect()
 
 
 
 
 def get_redis():
-    return redis_proxy.connect()
+    return _redis_proxy.connect()
 
 
 
 
 def get_redis_pipe():
-    redis = redis_proxy.connect()
+    redis = _redis_proxy.connect()
     return redis.pipeline()
 
 
 
 
 def get_redis_version():
     """
```

### Comparing `redis-metric-helper-0.3/metric_helper/registry.py` & `redis-metric-helper-0.3.1/metric_helper/registry.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.3/redis_metric_helper.egg-info/PKG-INFO` & `redis-metric-helper-0.3.1/redis_metric_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.3
+Version: 0.3.1
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.3/setup.py` & `redis-metric-helper-0.3.1/setup.py`

 * *Files identical despite different names*

