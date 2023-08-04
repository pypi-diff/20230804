# Comparing `tmp/redis-metric-helper-0.3.1.tar.gz` & `tmp/redis-metric-helper-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-metric-helper-0.3.1.tar", last modified: Thu Aug  3 16:07:15 2023, max compression
+gzip compressed data, was "redis-metric-helper-0.3.2.tar", last modified: Fri Aug  4 08:26:19 2023, max compression
```

## Comparing `redis-metric-helper-0.3.1.tar` & `redis-metric-helper-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 16:07:15.650795 redis-metric-helper-0.3.1/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.3.1/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-08-03 16:07:15.646794 redis-metric-helper-0.3.1/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.3.1/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 16:07:15.646794 redis-metric-helper-0.3.1/metric_helper/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      802 2023-08-03 16:06:35.000000 redis-metric-helper-0.3.1/metric_helper/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      293 2023-08-03 15:42:28.000000 redis-metric-helper-0.3.1/metric_helper/apps.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7032 2023-08-01 14:40:40.000000 redis-metric-helper-0.3.1/metric_helper/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      653 2023-08-03 15:02:21.000000 redis-metric-helper-0.3.1/metric_helper/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2576 2023-08-03 16:06:16.000000 redis-metric-helper-0.3.1/metric_helper/connections.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.3.1/metric_helper/exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      185 2023-08-03 13:40:48.000000 redis-metric-helper-0.3.1/metric_helper/logging.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2528 2023-08-03 13:47:29.000000 redis-metric-helper-0.3.1/metric_helper/registry.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-03 16:07:15.646794 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-08-03 16:07:15.000000 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      440 2023-08-03 16:07:15.000000 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-08-03 16:07:15.000000 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-08-03 16:07:15.000000 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-08-03 16:07:15.000000 redis-metric-helper-0.3.1/redis_metric_helper.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-08-03 16:07:15.650795 redis-metric-helper-0.3.1/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.3.1/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-04 08:26:18.999874 redis-metric-helper-0.3.2/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.3.2/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-08-04 08:26:18.999874 redis-metric-helper-0.3.2/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.3.2/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-04 08:26:18.999874 redis-metric-helper-0.3.2/metric_helper/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      802 2023-08-04 08:25:44.000000 redis-metric-helper-0.3.2/metric_helper/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      293 2023-08-03 15:42:28.000000 redis-metric-helper-0.3.2/metric_helper/apps.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7032 2023-08-01 14:40:40.000000 redis-metric-helper-0.3.2/metric_helper/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      653 2023-08-03 15:02:21.000000 redis-metric-helper-0.3.2/metric_helper/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2674 2023-08-04 08:24:11.000000 redis-metric-helper-0.3.2/metric_helper/connections.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.3.2/metric_helper/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      185 2023-08-03 13:40:48.000000 redis-metric-helper-0.3.2/metric_helper/logging.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2523 2023-08-03 16:12:00.000000 redis-metric-helper-0.3.2/metric_helper/registry.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-08-04 08:26:18.999874 redis-metric-helper-0.3.2/redis_metric_helper.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-08-04 08:26:18.000000 redis-metric-helper-0.3.2/redis_metric_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      440 2023-08-04 08:26:18.000000 redis-metric-helper-0.3.2/redis_metric_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-08-04 08:26:18.000000 redis-metric-helper-0.3.2/redis_metric_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-08-04 08:26:18.000000 redis-metric-helper-0.3.2/redis_metric_helper.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-08-04 08:26:18.000000 redis-metric-helper-0.3.2/redis_metric_helper.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-08-04 08:26:18.999874 redis-metric-helper-0.3.2/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.3.2/setup.py
```

### Comparing `redis-metric-helper-0.3.1/LICENSE` & `redis-metric-helper-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.3.1/PKG-INFO` & `redis-metric-helper-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.3.1
+Version: 0.3.2
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.3.1/metric_helper/__init__.py` & `redis-metric-helper-0.3.2/metric_helper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 
 
 
 def setup(connection_dict=None):
     """
     Example of ``connection_dict``::
```

### Comparing `redis-metric-helper-0.3.1/metric_helper/base.py` & `redis-metric-helper-0.3.2/metric_helper/base.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.3.1/metric_helper/conf.py` & `redis-metric-helper-0.3.2/metric_helper/conf.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.3.1/metric_helper/connections.py` & `redis-metric-helper-0.3.2/metric_helper/connections.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,19 @@
         host = config.get('host', 'localhost')
         port = config.get('port', 6379)
         password = config.get('password', '')
         decode_responses = config.get('decode_responses', True)
         socket_connect_timeout = config.get('socket_connect_timeout', 5)
         health_check_interval = config.get('health_check_interval', 30)
 
+        if not host:
+            host = 'localhost'
+        if not port:
+            port = 6379
+
         port = int(port)
         decode_responses = bool(decode_responses)
         socket_connect_timeout = int(socket_connect_timeout)
         health_check_interval = int(health_check_interval)
 
         self.redis = StrictRedis(
             host=host,
```

### Comparing `redis-metric-helper-0.3.1/metric_helper/registry.py` & `redis-metric-helper-0.3.2/metric_helper/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from metric_helper.conf import settings
 from metric_helper.base import Timeseries, Counter, Gauge, PositiveGauge
 from metric_helper.connections import get_redis_connection
 from metric_helper.exceptions import MetricNotFound
 
+# These strings may not change unless extreme caution is used
+# and the consequences are understood.
 TIMESERIES = 'timeseries'
 COUNTER = 'counter'
 GAUGE = 'gauge'
 POS_GAUGE = 'positive_gauge'
 
 metric_classes = [
     Timeseries,
     Counter,
     Gauge,
     PositiveGauge,
 ]
-# These string names may not change unless extreme caution is used
-# and the consequences are understood.
 mapping = {
     TIMESERIES: Timeseries,
     COUNTER: Counter,
     GAUGE: Gauge,
     POS_GAUGE: PositiveGauge,
 }
 reverse_mapping = {
```

### Comparing `redis-metric-helper-0.3.1/redis_metric_helper.egg-info/PKG-INFO` & `redis-metric-helper-0.3.2/redis_metric_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.3.1
+Version: 0.3.2
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.3.1/setup.py` & `redis-metric-helper-0.3.2/setup.py`

 * *Files identical despite different names*

