# Comparing `tmp/onestep-0.1.81.tar.gz` & `tmp/onestep-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onestep-0.1.81.tar", max compression
+gzip compressed data, was "onestep-0.2.0.tar", max compression
```

## Comparing `onestep-0.1.81.tar` & `onestep-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
--rw-r--r--   0        0        0     1362 2023-04-28 02:40:02.210281 onestep-0.1.81/README.md
--rw-r--r--   0        0        0      704 2023-04-28 02:40:02.210281 onestep-0.1.81/pyproject.toml
--rw-r--r--   0        0        0     1390 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/__init__.py
--rw-r--r--   0        0        0      414 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/_utils.py
--rw-r--r--   0        0        0      221 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/__init__.py
--rw-r--r--   0        0        0     4543 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/base.py
--rw-r--r--   0        0        0      957 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/cron.py
--rw-r--r--   0        0        0      151 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/memory.py
--rw-r--r--   0        0        0     2271 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/rabbitmq.py
--rw-r--r--   0        0        0     2144 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/webhook.py
--rw-r--r--   0        0        0      610 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/exception.py
--rw-r--r--   0        0        0     4543 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/message.py
--rw-r--r--   0        0        0      286 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/middleware/__init__.py
--rw-r--r--   0        0        0      521 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/middleware/base.py
--rw-r--r--   0        0        0     2438 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/middleware/config.py
--rw-r--r--   0        0        0     6350 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/onestep.py
--rw-r--r--   0        0        0     2699 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/retry.py
--rw-r--r--   0        0        0      293 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/signal.py
--rw-r--r--   0        0        0      618 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/state.py
--rw-r--r--   0        0        0       86 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/store/__init__.py
--rw-r--r--   0        0        0     4466 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/store/rabbitmq.py
--rw-r--r--   0        0        0     3516 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/worker.py
--rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.81/PKG-INFO
+-rw-r--r--   0        0        0     1362 2023-08-04 08:01:22.636207 onestep-0.2.0/README.md
+-rw-r--r--   0        0        0      726 2023-08-04 08:01:22.636207 onestep-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1390 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/__init__.py
+-rw-r--r--   0        0        0      414 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/_utils.py
+-rw-r--r--   0        0        0      221 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/broker/__init__.py
+-rw-r--r--   0        0        0     4543 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/broker/base.py
+-rw-r--r--   0        0        0      957 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/broker/cron.py
+-rw-r--r--   0        0        0      151 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/broker/memory.py
+-rw-r--r--   0        0        0     2291 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/broker/rabbitmq.py
+-rw-r--r--   0        0        0     2144 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/broker/webhook.py
+-rw-r--r--   0        0        0      610 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/exception.py
+-rw-r--r--   0        0        0     4543 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/message.py
+-rw-r--r--   0        0        0      286 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/middleware/__init__.py
+-rw-r--r--   0        0        0      521 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/middleware/base.py
+-rw-r--r--   0        0        0     2438 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/middleware/config.py
+-rw-r--r--   0        0        0     6350 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/onestep.py
+-rw-r--r--   0        0        0     2699 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/retry.py
+-rw-r--r--   0        0        0      293 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/signal.py
+-rw-r--r--   0        0        0      618 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/state.py
+-rw-r--r--   0        0        0     3516 2023-08-04 08:01:22.636207 onestep-0.2.0/src/onestep/worker.py
+-rw-r--r--   0        0        0     2003 1970-01-01 00:00:00.000000 onestep-0.2.0/PKG-INFO
```

### Comparing `onestep-0.1.81/README.md` & `onestep-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/pyproject.toml` & `onestep-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "onestep"
-version = "0.1.81"
+version = "0.2.0"
 description = ""
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'onestep', from = 'src' }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-amqpstorm = { version = "^2.10.6", optional = true }
 asgiref = "^3.6.0"
 blinker = "^1.5"
 croniter = "^1.3.8"
+usepy-plugin-rabbitmq = { version = "^0.1.0", optional = true }
 
 [tool.poetry.extras]
-rabbitmq = ["amqpstorm"]
+rabbitmq = ["usepy-plugin-rabbitmq"]
 
 [tool.poetry.group.dev.dependencies]
 nacos-sdk-python = "^0.1.12"
 redis = "^4.5.1"
 autopep8 = "^2.0.2"
 loguru = "^0.6.0"
```

### Comparing `onestep-0.1.81/src/onestep/__init__.py` & `onestep-0.2.0/src/onestep/__init__.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/broker/base.py` & `onestep-0.2.0/src/onestep/broker/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/broker/cron.py` & `onestep-0.2.0/src/onestep/broker/cron.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/broker/rabbitmq.py` & `onestep-0.2.0/src/onestep/broker/rabbitmq.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import threading
 from queue import Queue
 from typing import Optional, Dict, Any
 
 import amqpstorm
 
 from .base import BaseBroker, BaseConsumer
-from ..store.rabbitmq import RabbitMQStore
+from usepy_plugin_rabbitmq import useRabbitMQ as RabbitMQStore
 from ..message import Message
 
 
 class RabbitMQBroker(BaseBroker):
 
     def __init__(self, queue_name, params: Optional[Dict] = None, prefetch: Optional[int] = 1, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `onestep-0.1.81/src/onestep/broker/webhook.py` & `onestep-0.2.0/src/onestep/broker/webhook.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/exception.py` & `onestep-0.2.0/src/onestep/exception.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/message.py` & `onestep-0.2.0/src/onestep/message.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/middleware/base.py` & `onestep-0.2.0/src/onestep/middleware/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/middleware/config.py` & `onestep-0.2.0/src/onestep/middleware/config.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/onestep.py` & `onestep-0.2.0/src/onestep/onestep.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/retry.py` & `onestep-0.2.0/src/onestep/retry.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/state.py` & `onestep-0.2.0/src/onestep/state.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/src/onestep/worker.py` & `onestep-0.2.0/src/onestep/worker.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.81/PKG-INFO` & `onestep-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: onestep
-Version: 0.1.81
+Version: 0.2.0
 Summary: 
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: rabbitmq
-Requires-Dist: amqpstorm (>=2.10.6,<3.0.0) ; extra == "rabbitmq"
 Requires-Dist: asgiref (>=3.6.0,<4.0.0)
 Requires-Dist: blinker (>=1.5,<2.0)
 Requires-Dist: croniter (>=1.3.8,<2.0.0)
+Requires-Dist: usepy-plugin-rabbitmq (>=0.1.0,<0.2.0) ; extra == "rabbitmq"
 Description-Content-Type: text/markdown
 
 # OneStep
 
 <a href="https://github.com/mic1on/onestep/actions/workflows/test.yml?query=event%3Apush+branch%3Amain" target="_blank">
     <img src="https://github.com/mic1on/onestep/workflows/test%20suite/badge.svg?branch=main&event=push" alt="Test">
 </a>
```

