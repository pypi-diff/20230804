# Comparing `tmp/pytest_dogu_sdk-1.0.2.tar.gz` & `tmp/pytest_dogu_sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dogu_sdk-1.0.2.tar", max compression
+gzip compressed data, was "pytest_dogu_sdk-1.0.3.tar", max compression
```

## Comparing `pytest_dogu_sdk-1.0.2.tar` & `pytest_dogu_sdk-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      899 2023-07-21 06:19:11.695622 pytest_dogu_sdk-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1690 2023-07-20 16:33:36.015474 pytest_dogu_sdk-1.0.2/README.md
--rw-r--r--   0        0        0     1031 2023-07-21 04:07:57.199858 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/__init__.py
--rw-r--r--   0        0        0     3473 2023-07-21 06:13:11.583371 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/common.py
--rw-r--r--   0        0        0     1885 2023-07-20 16:33:36.020475 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu.config.schema.json
--rw-r--r--   0        0        0     3163 2023-07-20 16:33:36.021473 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu_config.py
--rw-r--r--   0        0        0       89 2023-07-21 06:08:38.134467 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu_hooks.py
--rw-r--r--   0        0        0     2875 2023-07-21 06:17:25.631796 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu_sdk.py
--rw-r--r--   0        0        0     2832 2023-07-20 16:33:36.023474 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/remote_dest_report_client.py
--rw-r--r--   0        0        0     9664 2023-07-21 04:07:57.201858 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/remote_dest_reporter.py
--rw-r--r--   0        0        0     3037 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/routine_dest_report_client.py
--rw-r--r--   0        0        0     9774 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/routine_dest_reporter.py
--rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 pytest_dogu_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      899 2023-08-04 09:52:40.945367 pytest_dogu_sdk-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1690 2023-07-20 16:33:36.015474 pytest_dogu_sdk-1.0.3/README.md
+-rw-r--r--   0        0        0     1549 2023-08-04 09:37:48.334239 pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/__init__.py
+-rw-r--r--   0        0        0     3473 2023-07-22 08:14:48.727156 pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/common.py
+-rw-r--r--   0        0        0     1885 2023-07-20 16:33:36.020475 pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/dogu.config.schema.json
+-rw-r--r--   0        0        0     3163 2023-07-20 16:33:36.021473 pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/dogu_config.py
+-rw-r--r--   0        0        0       89 2023-07-21 06:08:38.134467 pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/dogu_hooks.py
+-rw-r--r--   0        0        0     2879 2023-08-04 09:44:24.336230 pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/dogu_sdk.py
+-rw-r--r--   0        0        0     2832 2023-07-20 16:33:36.023474 pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/remote_dest_report_client.py
+-rw-r--r--   0        0        0     9664 2023-07-22 08:14:48.727975 pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/remote_dest_reporter.py
+-rw-r--r--   0        0        0     3037 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/routine_dest_report_client.py
+-rw-r--r--   0        0        0     9774 2023-07-20 16:33:36.024474 pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/routine_dest_reporter.py
+-rw-r--r--   0        0        0     2218 1970-01-01 00:00:00.000000 pytest_dogu_sdk-1.0.3/PKG-INFO
```

### Comparing `pytest_dogu_sdk-1.0.2/pyproject.toml` & `pytest_dogu_sdk-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-dogu-sdk"
-version = "1.0.2"
+version = "1.0.3"
 description = "pytest plugin for the Dogu"
 readme = "README.md"
 packages = [{include = "pytest_dogu_sdk", from = "src"}]
 authors = ["Dogu Technologies"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pytest_dogu_sdk-1.0.2/README.md` & `pytest_dogu_sdk-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/__init__.py` & `pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from pytest import Config, FixtureRequest, PytestPluginManager, fixture
 
 from .dogu_sdk import DoguSdk
+from .dogu_config import DoguConfig
+from .common import DoguClient
 from . import dogu_hooks
 
 
 def pytest_configure(config: Config):
     dogu_sdk = DoguSdk(config)
     config.pluginmanager.register(dogu_sdk, DoguSdk.name)
 
@@ -18,18 +20,31 @@
 
 
 def pytest_addhooks(pluginmanager: PytestPluginManager):
     pluginmanager.add_hookspecs(dogu_hooks)
 
 
 @fixture(scope="session")
-def dogu_client(request: FixtureRequest):
+def dogu_client(request: FixtureRequest) -> DoguClient:
     dogu_sdk = request.config.pluginmanager.get_plugin(DoguSdk.name)
     if dogu_sdk is None:
         raise Exception(
             "pytest_dogu_sdk is not registered. Please check your pytest configuration"
         )
 
     if not isinstance(dogu_sdk, DoguSdk):
         raise Exception("dogu_sdk is not an instance of DoguSdk")
 
     return dogu_sdk.client
+
+@fixture(scope="session")
+def dogu_config(request: FixtureRequest) -> DoguConfig:
+    dogu_sdk = request.config.pluginmanager.get_plugin(DoguSdk.name)
+    if dogu_sdk is None:
+        raise Exception(
+            "pytest_dogu_sdk is not registered. Please check your pytest configuration"
+        )
+
+    if not isinstance(dogu_sdk, DoguSdk):
+        raise Exception("dogu_sdk is not an instance of DoguSdk")
+
+    return dogu_sdk.config
```

### Comparing `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/common.py` & `pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/common.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu.config.schema.json` & `pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/dogu.config.schema.json`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu_config.py` & `pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/dogu_config.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/dogu_sdk.py` & `pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/dogu_sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from .dogu_config import DoguConfigFactory
 from .common import PyTestHandler, PyTestLocation, DoguClient
 
 
 class DoguSdk:
     name = "dogu_sdk"
 
-    def __init__(self, config: Config) -> None:
-        self._config = config
-        self._dogu_config = DoguConfigFactory().create()
+    def __init__(self, pytest_config: Config) -> None:
+        self._pytest_config = pytest_config
+        self.config = DoguConfigFactory().create()
 
-        (client,) = self._config.hook.pytest_dogu_create_client()
+        (client,) = self._pytest_config.hook.pytest_dogu_create_client()
         self.client: DoguClient = client
-        client_impl = self.client.on_setup(self._dogu_config)
+        client_impl = self.client.on_setup(self.config)
         if not client_impl:
             raise Exception("dogu client is not initialized on setup")
         self.client.impl = client_impl
 
         self._routine_dest_reporter = RoutineDestReporterFactory(
-            self._dogu_config
+            self.config
         ).create()
         self._remote_dest_reporter = RemoteDestReporterFactory(
-            self._dogu_config,
+            self.config,
             self.client,
         ).create()
         self._handlers: List[PyTestHandler] = [
             self._routine_dest_reporter,
             self._remote_dest_reporter,
         ]
```

### Comparing `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/remote_dest_report_client.py` & `pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/remote_dest_report_client.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/remote_dest_reporter.py` & `pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/remote_dest_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/routine_dest_report_client.py` & `pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/routine_dest_report_client.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.2/src/pytest_dogu_sdk/routine_dest_reporter.py` & `pytest_dogu_sdk-1.0.3/src/pytest_dogu_sdk/routine_dest_reporter.py`

 * *Files identical despite different names*

### Comparing `pytest_dogu_sdk-1.0.2/PKG-INFO` & `pytest_dogu_sdk-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-dogu-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: pytest plugin for the Dogu
 Author: Dogu Technologies
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

