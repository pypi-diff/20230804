# Comparing `tmp/highlight_io-0.5.4.tar.gz` & `tmp/highlight_io-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "highlight_io-0.5.4.tar", max compression
+gzip compressed data, was "highlight_io-0.5.5.tar", max compression
```

## Comparing `highlight_io-0.5.4.tar` & `highlight_io-0.5.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      542 2023-08-04 17:06:55.462439 highlight_io-0.5.4/README.md
--rw-r--r--   0        0        0       64 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/__init__.py
--rw-r--r--   0        0        0      155 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/__init__.py
--rw-r--r--   0        0        0      717 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/aws.py
--rw-r--r--   0        0        0      740 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/azure.py
--rw-r--r--   0        0        0     1631 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/django.py
--rw-r--r--   0        0        0     1799 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/fastapi.py
--rw-r--r--   0        0        0     1519 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/flask.py
--rw-r--r--   0        0        0      747 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/gcp.py
--rw-r--r--   0        0        0     1072 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/integrations/serverless.py
--rw-r--r--   0        0        0    11999 2023-08-04 17:06:55.466439 highlight_io-0.5.4/highlight_io/sdk.py
--rw-r--r--   0        0        0     1687 2023-08-04 17:06:55.466439 highlight_io-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     2248 1970-01-01 00:00:00.000000 highlight_io-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      867 2023-08-04 21:53:02.985756 highlight_io-0.5.5/README.md
+-rw-r--r--   0        0        0       64 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/__init__.py
+-rw-r--r--   0        0        0      155 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/__init__.py
+-rw-r--r--   0        0        0      717 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/aws.py
+-rw-r--r--   0        0        0      740 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/azure.py
+-rw-r--r--   0        0        0     1631 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/django.py
+-rw-r--r--   0        0        0     1799 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/fastapi.py
+-rw-r--r--   0        0        0     1519 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/flask.py
+-rw-r--r--   0        0        0      747 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/gcp.py
+-rw-r--r--   0        0        0     1072 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/integrations/serverless.py
+-rw-r--r--   0        0        0    12453 2023-08-04 21:53:02.985756 highlight_io-0.5.5/highlight_io/sdk.py
+-rw-r--r--   0        0        0     1688 2023-08-04 21:53:02.985756 highlight_io-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 highlight_io-0.5.5/PKG-INFO
```

### Comparing `highlight_io-0.5.4/README.md` & `highlight_io-0.5.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,16 +7,38 @@
 The `e2e` directory contains supported Python frameworks integrated with our SDK for local development and testing.
 Do not use the snippets verbatim as they are configured for local development and will not work in production without changes.
 
 
 ## Install
 
 * Install [poetry](https://python-poetry.org/docs/#installing-with-the-official-installer)
-* `poetry install`
+* `poetry install --all-extras`
+
+## Run e2e apps
+
+### Django
+
+* `cd e2e/highlight_django`
+* `poetry run python manage.py runserver`
+
+### Flask
+
+* `cd e2e/highlight_flask`
+* `poetry run flask run`
+
+### Fastapi
+
+* `cd e2e/highlight_fastapi`
+* `poetry run uvicorn main:app`
+
+### Loguru
+
+* `cd e2e/highlight_loguru`
+* `poetry run python main.py`
 
 ## Run tests
 
 * `poetry run pytest`
 
 ## Lint
 
-* poetry run black  .
+* `poetry run black  .`
```

### Comparing `highlight_io-0.5.4/highlight_io/integrations/aws.py` & `highlight_io-0.5.5/highlight_io/integrations/aws.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.4/highlight_io/integrations/azure.py` & `highlight_io-0.5.5/highlight_io/integrations/azure.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.4/highlight_io/integrations/django.py` & `highlight_io-0.5.5/highlight_io/integrations/django.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.4/highlight_io/integrations/fastapi.py` & `highlight_io-0.5.5/highlight_io/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.4/highlight_io/integrations/flask.py` & `highlight_io-0.5.5/highlight_io/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.4/highlight_io/integrations/gcp.py` & `highlight_io-0.5.5/highlight_io/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.4/highlight_io/integrations/serverless.py` & `highlight_io-0.5.5/highlight_io/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `highlight_io-0.5.4/highlight_io/sdk.py` & `highlight_io-0.5.5/highlight_io/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     def __init__(self, highlight: "H", level=logging.NOTSET):
         self.highlight = highlight
         super(LogHandler, self).__init__(level=level)
 
     def emit(self, record: logging.LogRecord):
         ctx = contextlib.nullcontext
         span = trace.get_current_span()
+
         if span is None or not span.is_recording():
             ctx = self.highlight.trace
 
         with ctx():
             self.highlight.log_hook(trace.get_current_span(), record)
 
 
@@ -280,22 +281,36 @@
             ts = int(record.created * 1000.0 * 1000.0 * 1000.0)
             attributes = span.attributes.copy()
             attributes["code.function"] = record.funcName
             attributes["code.namespace"] = record.module
             attributes["code.filepath"] = record.pathname
             attributes["code.lineno"] = record.lineno
             attributes.update(record.args or {})
+
+            message = record.getMessage()
+            try:
+                # Handle loguru's serialize=True format
+                # See: https://loguru.readthedocs.io/en/stable/api/logger.html#record
+                obj = json.loads(message)
+                extra = obj["record"]["extra"]
+                message = obj["text"]
+
+                for key, value in extra.items():
+                    attributes[key] = value
+            except:
+                pass
+
             r = LogRecord(
                 timestamp=ts,
                 trace_id=ctx.trace_id,
                 span_id=ctx.span_id,
                 trace_flags=ctx.trace_flags,
                 severity_text=record.levelname,
                 severity_number=std_to_otel(record.levelno),
-                body=record.getMessage(),
+                body=message,
                 resource=span.resource,
                 attributes=attributes,
             )
             self.log.emit(r)
 
     def _instrument_logging(self):
         if H._logging_instrumented:
```

### Comparing `highlight_io-0.5.4/pyproject.toml` & `highlight_io-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "highlight-io"
-version = "0.5.4"
+version = "0.5.5"
 description = "Session replay and error monitoring: stop guessing why bugs happen!"
 license = "Apache-2.0"
 authors = [
     "Vadim Korolik <vadim@highlight.io>",
     "Jay Khatri <jay@highlight.io>",
 ]
 readme = "README.md"
@@ -25,15 +25,15 @@
 packages = [{ include = "highlight_io" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 blinker = { version = "^1.5", optional = true }
 django = { version = "^4.1", optional = true }
 flask = { version = "^2.2", optional = true }
-fastapi = { version = "^0.92", optional = true }
+fastapi = { version = ">=0.92", optional = true }
 uvicorn = {version = "^0.20", extras = ["standard"], optional = true }
 opentelemetry-api = "1.19.0"
 opentelemetry-distro = { extras = ["otlp"], version = "0.40b0" }
 opentelemetry-exporter-otlp-proto-http = "1.19.0"
 opentelemetry-instrumentation = "0.40b0"
 opentelemetry-instrumentation-logging = "0.40b0"
 opentelemetry-proto = "1.19.0"
```

### Comparing `highlight_io-0.5.4/PKG-INFO` & `highlight_io-0.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highlight-io
-Version: 0.5.4
+Version: 0.5.5
 Summary: Session replay and error monitoring: stop guessing why bugs happen!
 Home-page: https://www.highlight.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Vadim Korolik
 Author-email: vadim@highlight.io
 Requires-Python: >=3.8,<4.0
@@ -20,15 +20,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Monitoring
 Provides-Extra: django
 Provides-Extra: fastapi
 Provides-Extra: flask
 Requires-Dist: blinker (>=1.5,<2.0) ; extra == "flask"
 Requires-Dist: django (>=4.1,<5.0) ; extra == "django"
-Requires-Dist: fastapi (>=0.92,<0.93) ; extra == "fastapi"
+Requires-Dist: fastapi (>=0.92) ; extra == "fastapi"
 Requires-Dist: flask (>=2.2,<3.0) ; extra == "flask"
 Requires-Dist: opentelemetry-api (==1.19.0)
 Requires-Dist: opentelemetry-distro[otlp] (==0.40b0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.19.0)
 Requires-Dist: opentelemetry-instrumentation (==0.40b0)
 Requires-Dist: opentelemetry-instrumentation-logging (==0.40b0)
 Requires-Dist: opentelemetry-proto (==1.19.0)
@@ -47,16 +47,38 @@
 The `e2e` directory contains supported Python frameworks integrated with our SDK for local development and testing.
 Do not use the snippets verbatim as they are configured for local development and will not work in production without changes.
 
 
 ## Install
 
 * Install [poetry](https://python-poetry.org/docs/#installing-with-the-official-installer)
-* `poetry install`
+* `poetry install --all-extras`
+
+## Run e2e apps
+
+### Django
+
+* `cd e2e/highlight_django`
+* `poetry run python manage.py runserver`
+
+### Flask
+
+* `cd e2e/highlight_flask`
+* `poetry run flask run`
+
+### Fastapi
+
+* `cd e2e/highlight_fastapi`
+* `poetry run uvicorn main:app`
+
+### Loguru
+
+* `cd e2e/highlight_loguru`
+* `poetry run python main.py`
 
 ## Run tests
 
 * `poetry run pytest`
 
 ## Lint
 
-* poetry run black  .
+* `poetry run black  .`
```

