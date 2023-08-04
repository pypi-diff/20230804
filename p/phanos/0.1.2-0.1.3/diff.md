# Comparing `tmp/phanos-0.1.2.tar.gz` & `tmp/phanos-0.1.3.tar.gz`

## Comparing `phanos-0.1.2.tar` & `phanos-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 phanos-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.1.2/Pipfile
--rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.1.2/Pipfile.lock
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 phanos-0.1.2/requirements.txt
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/pyvenv.cfg
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/Activate.ps1
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/activate
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/activate.csh
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/activate.fish
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/pip
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/pip3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/pip3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/pip3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/python -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/python3 -> python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.2/deactivate/bin/python3.11 -> /usr/bin/python3.11
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/__init__.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/config.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/log.py
--rw-r--r--   0        0        0    17132 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/metrics.py
--rw-r--r--   0        0        0    20338 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/publisher.py
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 phanos-0.1.2/src/phanos/tree.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 phanos-0.1.2/test/__init__.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 phanos-0.1.2/test/dummy_api.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 phanos-0.1.2/test/requirements.txt
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 phanos-0.1.2/test/run_tests.py
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 phanos-0.1.2/test/test_config.py
--rw-r--r--   0        0        0    26021 2020-02-02 00:00:00.000000 phanos-0.1.2/test/test_metric.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 phanos-0.1.2/test/testing_data.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.1.2/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.1.2/LICENSE
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 phanos-0.1.2/README.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 phanos-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 phanos-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 phanos-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 phanos-0.1.3/Pipfile
+-rw-r--r--   0        0        0    22933 2020-02-02 00:00:00.000000 phanos-0.1.3/Pipfile.lock
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 phanos-0.1.3/requirements-dev.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 phanos-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/pyvenv.cfg
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/Activate.ps1
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/activate
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/activate.csh
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/activate.fish
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/pip
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/pip3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/pip3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/pip3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/python -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/python3 -> python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 phanos-0.1.3/deactivate/bin/python3.11 -> /usr/bin/python3.11
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 phanos-0.1.3/src/phanos/__init__.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 phanos-0.1.3/src/phanos/config.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 phanos-0.1.3/src/phanos/log.py
+-rw-r--r--   0        0        0     5988 2020-02-02 00:00:00.000000 phanos-0.1.3/src/phanos/messaging.py
+-rw-r--r--   0        0        0    17129 2020-02-02 00:00:00.000000 phanos-0.1.3/src/phanos/metrics.py
+-rw-r--r--   0        0        0    21603 2020-02-02 00:00:00.000000 phanos-0.1.3/src/phanos/publisher.py
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 phanos-0.1.3/src/phanos/tree.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 phanos-0.1.3/src/phanos/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 phanos-0.1.3/test/__init__.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 phanos-0.1.3/test/dummy_api.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 phanos-0.1.3/test/requirements.txt
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 phanos-0.1.3/test/run_tests.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 phanos-0.1.3/test/test_config.py
+-rw-r--r--   0        0        0    26021 2020-02-02 00:00:00.000000 phanos-0.1.3/test/test_metric.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 phanos-0.1.3/test/testing_data.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 phanos-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 phanos-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 phanos-0.1.3/README.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 phanos-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 phanos-0.1.3/PKG-INFO
```

### Comparing `phanos-0.1.2/Pipfile.lock` & `phanos-0.1.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/deactivate/bin/Activate.ps1` & `phanos-0.1.3/deactivate/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/deactivate/bin/activate` & `phanos-0.1.3/deactivate/bin/activate`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/deactivate/bin/activate.csh` & `phanos-0.1.3/deactivate/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/deactivate/bin/activate.fish` & `phanos-0.1.3/deactivate/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/src/phanos/config.py` & `phanos-0.1.3/src/phanos/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 import copy
 import importlib
 import typing
+
 from . import (
     publisher,
 )
 
 """
-example_config = {
-    "handlers": {
-        "stdout_handler": {
-            "class": "phanos.publisher.StreamHandler",
-            "handler_name": "stdout_handler",
-            "output": "ext://sys.stdout",
-        }
-    },
-}
+res
 """
 
 EXTERNAL_PREFIX = "ext://"
 
 
 def import_external(full_name: str) -> typing.Any:
     """
```

### Comparing `phanos-0.1.2/src/phanos/log.py` & `phanos-0.1.3/src/phanos/log.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import logging
 import typing
 
-LoggerLike = typing.Union[logging.Logger, logging.LoggerAdapter]
+from .types import LoggerLike
 
 
 class InstanceLoggerMixin:
     """Adds method for instance logging"""
+
     __slots__ = (
         "logger",
         "logged_name",
     )
     logger: LoggerLike
     logged_name: str
 
     def __init__(
-            self,
-            *args,
-            logged_name: typing.Optional[str] = None,
-            logger: typing.Optional[LoggerLike] = None,
-            logger_name: typing.Optional[str] = None,
-            **kwargs,
+        self,
+        *args,
+        logged_name: typing.Optional[str] = None,
+        logger: typing.Optional[LoggerLike] = None,
+        logger_name: typing.Optional[str] = None,
+        **kwargs,
     ) -> None:
         """
         Bind logger to class logger.
 
         :param logged_name: log messages are formatted as "{name} - {message}"
         :param logger: logger to use for logging
         :param logger_name: only if no logger object is given, get named logger from
```

### Comparing `phanos-0.1.2/src/phanos/metrics.py` & `phanos-0.1.3/src/phanos/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from __future__ import annotations
 
 import logging
 import sys
 import typing
 from datetime import datetime as dt
 
-from imp_prof import Record
-
 from . import log
+from .types import Record
 
 
 class MetricWrapper(log.InstanceLoggerMixin):
     """Wrapper around all Prometheus metric types"""
 
     name: str
     item: typing.List[str]
```

### Comparing `phanos-0.1.2/src/phanos/publisher.py` & `phanos-0.1.3/src/phanos/publisher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """ """
 from __future__ import annotations
+
 import inspect
 import logging
 import sys
 import threading
 import typing
 from abc import abstractmethod
 
-import imp_prof.messaging.publisher
-from imp_prof.messaging.publisher import BlockingPublisher
+from . import (
+    log,
+    types,
+    messaging,
+)
 from .metrics import MetricWrapper, TimeProfiler, ResponseSize
 from .tree import MethodTreeNode
-from . import log
 
 TIME_PROFILER = "time_profiler"
 RESPONSE_SIZE = "response_size"
 
 
 class OutputFormatter:
     """class for converting Record type into profiling string"""
 
     @staticmethod
-    def record_to_str(name: str, record: imp_prof.Record) -> str:
+    def record_to_str(name: str, record: types.Record) -> str:
         """converts Record type into profiling string
 
         :param name: name of profiler
         :param record: metric record which to convert
         """
         value = record["value"][1]
         if not record.get("labels"):
@@ -49,30 +52,30 @@
         """
         :param handler_name: name of handler. used for managing handlers"""
         self.handler_name = handler_name
 
     @abstractmethod
     def handle(
         self,
-        records: typing.List[imp_prof.Record],
+        records: typing.List[types.Record],
         profiler_name: str = "profiler",
     ) -> None:
         """
         method for handling records
 
         :param profiler_name: name of profiler
         :param records: list of records to handle
         """
         raise NotImplementedError
 
 
 class ImpProfHandler(BaseHandler):
     """RabbitMQ record handler"""
 
-    publisher: BlockingPublisher
+    publisher: messaging.BlockingPublisher
     logger: typing.Optional[log.LoggerLike]
 
     def __init__(
         self,
         handler_name: str,
         host: str = "127.0.0.1",
         port: int = 5672,
@@ -83,15 +86,15 @@
         retry_delay: float = 0.137,
         retry: int = 3,
         exchange_name: str = "profiling",
         exchange_type: str = "fanout",
         logger: typing.Optional[log.LoggerLike] = None,
         **kwargs,
     ) -> None:
-        """Creates BlockingPublisher instance (connection not established yet),
+        """Creates `messaging.BlockingPublisher` instance (connection not established yet),
          sets logger and create time profiler and response size profiler
 
         :param handler_name: name of handler. used for managing handlers
         :param host: rabbitMQ server host
         :param port: rabbitMQ server port
         :param user: rabbitMQ login username
         :param password: rabbitMQ user password
@@ -110,15 +113,15 @@
             `reason_code` of `InternalCloseReasons.BLOCKED_CONNECTION_TIMEOUT`.
         :param kwargs: other connection params, like `timeout goes here`
         :param logger: logger
         """
         super().__init__(handler_name)
 
         self.logger = logger or logging.getLogger(__name__)
-        self.publisher = BlockingPublisher(
+        self.publisher = messaging.BlockingPublisher(
             host=host,
             port=port,
             user=user,
             password=password,
             heartbeat=heartbeat,
             timeout=timeout,
             retry_delay=retry_delay,
@@ -126,24 +129,24 @@
             exchange_name=exchange_name,
             exchange_type=exchange_type,
             logger=logger,
             **kwargs,
         )
         try:
             self.publisher.connect()
-        except imp_prof.messaging.publisher.NETWORK_ERRORS as err:
+        except messaging.NETWORK_ERRORS as err:
             self.logger.error(f"ImpProfHandler cannot connect to RabbitMQ because of {err}")
             raise RuntimeError("Cannot connect to RabbitMQ") from err
 
         self.logger.info("ImpProfHandler created successfully")
         self.publisher.close()
 
     def handle(
         self,
-        records: typing.List[imp_prof.Record],
+        records: typing.List[types.Record],
         profiler_name: str = "profiler",
     ) -> None:
         """Sends list of records to rabitMq queue
 
         :param profiler_name: name of profiler (not used)
         :param records: list of records to publish
         """
@@ -180,15 +183,50 @@
             self.logger.setLevel(10)
             handler = logging.StreamHandler(sys.stdout)
             handler.setLevel(10)
             self.logger.addHandler(handler)
         self.level = level
         self.formatter = OutputFormatter()
 
-    def handle(self, records: typing.List[imp_prof.Record], profiler_name: str = "profiler") -> None:
+    def handle(self, records: typing.List[types.Record], profiler_name: str = "profiler") -> None:
+        """logs list of records
+
+        :param profiler_name: name of profiler
+        :param records: list of records
+        """
+        for record in records:
+            self.logger.log(self.level, self.formatter.record_to_str(profiler_name, record))
+
+
+class NamedLoggerHandler(BaseHandler):
+    """Logger handler initialised with name of logger rather than passing object"""
+
+    logger: log.LoggerLike
+    formatter: OutputFormatter
+    level: int
+
+    def __init__(
+        self,
+        handler_name: str,
+        logger_name: str,
+        level: int = logging.DEBUG,
+    ) -> None:
+        """
+        Initialise handler and find logger by name.
+
+        :param handler_name: name of handler. used for managing handlers
+        :param logger_name: find this logger `logging.getLogger(logger_name)`
+        :param level: level of logger in which prints records. default is DEBUG
+        """
+        super().__init__(handler_name)
+        self.logger = logging.getLogger(logger_name)
+        self.level = level
+        self.formatter = OutputFormatter()
+
+    def handle(self, records: typing.List[types.Record], profiler_name: str = "profiler") -> None:
         """logs list of records
 
         :param profiler_name: name of profiler
         :param records: list of records
         """
         for record in records:
             self.logger.log(self.level, self.formatter.record_to_str(profiler_name, record))
@@ -208,15 +246,15 @@
         :param output: stream output. Default 'sys.stdout'
         """
         super().__init__(handler_name)
         self.output = output
         self.formatter = OutputFormatter()
         self._lock = threading.Lock()
 
-    def handle(self, records: typing.List[imp_prof.Record], profiler_name: str = "profiler") -> None:
+    def handle(self, records: typing.List[types.Record], profiler_name: str = "profiler") -> None:
         """logs list of records
 
         :param profiler_name: name of profiler
         :param records: list of records
         """
         for record in records:
             with self._lock:
@@ -263,14 +301,15 @@
         self.resp_size_profile = None
         self.time_profile = None
 
         self.before_func = None
         self.after_func = None
         self.before_root_func = None
         self.after_root_func = None
+
         super().__init__(logged_name="phanos")
 
     def config(
         self,
         logger=None,
         job: str = "",
         time_profile: bool = True,
@@ -319,24 +358,29 @@
 
         :param settings: dictionary of desired profiling set up
         """
         from . import config as phanos_config
 
         if "logger" in settings:
             self.logger = logging.getLogger(settings["logger"])
+        else:
+            self.logger = logging.getLogger(__name__)
         if "job" in settings:
             self.job = settings["job"]
         if settings.get("time_profile"):
             self.create_time_profiler()
         self.handle_records = settings.get("handle_records", True)
         if "handlers" in settings:
             named_handlers = phanos_config.create_handlers(settings["handlers"])
             for handler in named_handlers.values():
                 self.add_handler(handler)
 
+        self._root = MethodTreeNode(None, self.logger)
+        self.current_node = self._root
+
     def create_time_profiler(self) -> None:
         """Create time profiling metric"""
         self.time_profile = TimeProfiler(TIME_PROFILER, job=self.job, logger=self.logger)
         self.add_metric(self.time_profile)
         self.debug("Phanos - time profiler created")
 
     def create_response_size_profiler(self) -> None:
```

### Comparing `phanos-0.1.2/src/phanos/tree.py` & `phanos-0.1.3/src/phanos/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import inspect
 import typing
+
 from . import log
 
 
 class MethodTreeNode(log.InstanceLoggerMixin):
     """
     Tree for storing method calls context
     """
```

### Comparing `phanos-0.1.2/test/dummy_api.py` & `phanos-0.1.3/test/dummy_api.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/test/run_tests.py` & `phanos-0.1.3/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/test/test_config.py` & `phanos-0.1.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/test/test_metric.py` & `phanos-0.1.3/test/test_metric.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/test/testing_data.py` & `phanos-0.1.3/test/testing_data.py`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/.gitignore` & `phanos-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/LICENSE` & `phanos-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/README.md` & `phanos-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `phanos-0.1.2/pyproject.toml` & `phanos-0.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "phanos"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Miroslav Bulička", email="bulickamiroslav@gmail.com" },
 ]
 description = "Python client to gather data for Prometheus logging in server with multiple instances and workers."
 readme = "README.md"
 requires-python = ">=3.10.6"
 classifiers = [
@@ -19,13 +19,14 @@
     "Topic :: System :: Monitoring",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pip>=23.1.2",
     "pika>=1.3.2",
-    "imp_prof>=0.1.2",
+    "aio_pika>=9.2",
+    "orjson>=3.9",
     ]
 
 [project.urls]
 "Homepage" = "https://github.com/kajotgames/phanos"
 "Bug Tracker" = "https://github.com/kajotgames/phanos/issues"
```

### Comparing `phanos-0.1.2/PKG-INFO` & `phanos-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: phanos
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python client to gather data for Prometheus logging in server with multiple instances and workers.
 Project-URL: Homepage, https://github.com/kajotgames/phanos
 Project-URL: Bug Tracker, https://github.com/kajotgames/phanos/issues
 Author-email: Miroslav Bulička <bulickamiroslav@gmail.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.10.6
-Requires-Dist: imp-prof>=0.1.2
+Requires-Dist: aio-pika>=9.2
+Requires-Dist: orjson>=3.9
 Requires-Dist: pika>=1.3.2
 Requires-Dist: pip>=23.1.2
 Description-Content-Type: text/markdown
 
 # PHANOS
 
 Python client to gather data for Prometheus logging in server with multiple instances and workers.
```

