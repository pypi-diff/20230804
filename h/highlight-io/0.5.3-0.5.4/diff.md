# Comparing `tmp/highlight_io-0.5.3.tar.gz` & `tmp/highlight_io-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.5.3.tar", max compression
+gzip compressed data, was "highlight_io-0.5.4.tar", max compression
```

## Comparing `highlight_io-0.5.3.tar` & `highlight_io-0.5.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      350 2023-03-06 07:22:47.581214 highlight_io-0.5.3/README.md
--rw-r--r--   0        0        0       64 2023-03-06 07:22:47.585934 highlight_io-0.5.3/highlight_io/__init__.py
--rw-r--r--   0        0        0      155 2023-03-06 07:22:47.586006 highlight_io-0.5.3/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0      717 2023-04-11 23:45:03.063104 highlight_io-0.5.3/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2023-04-11 23:45:03.063208 highlight_io-0.5.3/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0     1631 2023-03-06 07:22:47.586615 highlight_io-0.5.3/highlight_io/integrations/django.py
--rw-r--r--   0        0        0     1799 2023-06-29 15:32:09.529959 highlight_io-0.5.3/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1519 2023-03-06 07:22:47.586917 highlight_io-0.5.3/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2023-04-11 23:45:03.063318 highlight_io-0.5.3/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0     1072 2023-04-11 23:45:03.063459 highlight_io-0.5.3/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0    11253 2023-06-29 15:32:09.530463 highlight_io-0.5.3/highlight_io/sdk.py
--rw-r--r--   0        0        0     1687 2023-07-13 21:54:33.791784 highlight_io-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2056 1970-01-01 00:00:00.000000 highlight_io-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0      542 2023-08-04 17:06:55.462439 highlight_io-0.5.4/README.md
+-rw-r--r--   0        0        0       64 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/__init__.py
+-rw-r--r--   0        0        0      155 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0      717 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0     1631 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0     1799 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1519 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0     1072 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0    11999 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/sdk.py
+-rw-r--r--   0        0        0     1687 2023-08-04 17:06:55.466439 highlight_io-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 highlight_io-0.5.4/PKG-INFO
```

### Comparing `highlight_io-0.5.3/highlight_io/integrations/aws.py` & `highlight_io-0.5.4/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.3/highlight_io/integrations/azure.py` & `highlight_io-0.5.4/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.3/highlight_io/integrations/django.py` & `highlight_io-0.5.4/highlight_io/integrations/django.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.3/highlight_io/integrations/fastapi.py` & `highlight_io-0.5.4/highlight_io/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.3/highlight_io/integrations/flask.py` & `highlight_io-0.5.4/highlight_io/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.3/highlight_io/integrations/gcp.py` & `highlight_io-0.5.4/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.3/highlight_io/integrations/serverless.py` & `highlight_io-0.5.4/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.3/highlight_io/sdk.py` & `highlight_io-0.5.4/highlight_io/sdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
 from opentelemetry.sdk._logs import LoggerProvider, LogRecord
 from opentelemetry.sdk._logs.export import BatchLogRecordProcessor
 from opentelemetry.sdk.trace import TracerProvider, Span
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 from opentelemetry.trace import INVALID_SPAN
+from opentelemetry.sdk.resources import Attributes, Resource
 
 from highlight_io.integrations import Integration
 
 
 class LogHandler(logging.Handler):
     def __init__(self, highlight: "H", level=logging.NOTSET):
         self.highlight = highlight
@@ -52,51 +53,61 @@
     def __init__(
         self,
         project_id: str,
         integrations: typing.List[Integration] = None,
         otlp_endpoint: str = "",
         instrument_logging: bool = True,
         log_level=logging.DEBUG,
+        service_name: str = "",
+        service_version: str = "",
     ):
         """
         Setup Highlight backend instrumentation.
 
         Example:
             import highlight_io
             H = highlight_io.H('project_id', ...)
 
 
         :param project_id: a string that corresponds to the verbose id of your project from app.highlight.io/setup
         :param integrations: a list of Integrations that allow connecting with your framework, like Flask or Django.
         :param instrument_logging: defaults to True. set False to disable auto-instrumentation of python `logging` methods.
         :param otlp_endpoint: set to a custom otlp destination
+        :param service_name: a string to name this app
+        :param service_version: a string to set this app's version (typically a Git deploy sha).
         :return: a configured H instance
         """
         H._instance = self
         self._project_id = project_id
         self._integrations = integrations or []
         self._otlp_endpoint = otlp_endpoint or H.OTLP_HTTP
         self._log_handler = LogHandler(self, level=log_level)
         if instrument_logging:
             self._instrument_logging()
 
-        self._trace_provider = TracerProvider()
+        resource = _build_resource(
+            service_name=service_name,
+            service_version=service_version,
+        )
+        self._trace_provider = TracerProvider(resource=resource)
         self._trace_provider.add_span_processor(
             BatchSpanProcessor(
                 OTLPSpanExporter(
                     f"{self._otlp_endpoint}/v1/traces", compression=Compression.Gzip
                 ),
                 schedule_delay_millis=1000,
                 export_timeout_millis=5000,
             )
         )
         trace.set_tracer_provider(self._trace_provider)
         self.tracer = trace.get_tracer(__name__)
 
-        self._log_provider = LoggerProvider()
+        self._log_provider = LoggerProvider(
+            resource=resource,
+        )
         self._log_provider.add_log_record_processor(
             BatchLogRecordProcessor(
                 OTLPLogExporter(
                     f"{self._otlp_endpoint}/v1/logs", compression=Compression.Gzip
                 ),
                 schedule_delay_millis=1000,
                 export_timeout_millis=5000,
@@ -302,13 +313,27 @@
             else:
                 manager = self.trace()
 
             try:
                 with manager:
                     return otel_factory(*args, **kwargs)
             except RecursionError:
-                # in case we are hitting a recusrive log from the `self.trace()` invocation
+                # in case we are hitting a recursive log from the `self.trace()` invocation
                 # (happens when we exceed the otel log queue depth)
                 return otel_factory(*args, **kwargs)
 
         logging.setLogRecordFactory(factory)
         H._logging_instrumented = True
+
+
+def _build_resource(
+    service_name: str,
+    service_version: str,
+) -> Resource:
+    attrs = {}
+
+    if service_name:
+        attrs["service.name"] = service_name
+    if service_version:
+        attrs["service.version"] = service_version
+
+    return Resource.create(attrs)
```

### Comparing `highlight_io-0.5.3/pyproject.toml` & `highlight_io-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highlight-io"
-version = "0.5.3"
+version = "0.5.4"
 description = "Session replay and error monitoring: stop guessing why bugs happen!"
 license = "Apache-2.0"
 authors = [
     "Vadim Korolik <vadim@highlight.io>",
     "Jay Khatri <jay@highlight.io>",
 ]
 readme = "README.md"
```

### Comparing `highlight_io-0.5.3/PKG-INFO` & `highlight_io-0.5.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlight-io
-Version: 0.5.3
+Version: 0.5.4
 Summary: Session replay and error monitoring: stop guessing why bugs happen!
 Home-page: https://www.highlight.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Vadim Korolik
 Author-email: vadim@highlight.io
 Requires-Python: >=3.8,<4.0
@@ -43,7 +43,20 @@
 This directory contains the source code for the Highlight Python SDK.
 
 ### E2E
 
 The `e2e` directory contains supported Python frameworks integrated with our SDK for local development and testing.
 Do not use the snippets verbatim as they are configured for local development and will not work in production without changes.
 
+
+## Install
+
+* Install [poetry](https://python-poetry.org/docs/#installing-with-the-official-installer)
+* `poetry install`
+
+## Run tests
+
+* `poetry run pytest`
+
+## Lint
+
+* poetry run black  .
```

