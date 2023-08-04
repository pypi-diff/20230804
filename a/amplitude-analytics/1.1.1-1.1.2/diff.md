# Comparing `tmp/amplitude-analytics-1.1.1.tar.gz` & `tmp/amplitude-analytics-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Amplitude-Python/Amplitude-Python/dist/.tmp-3y10g5kn/amplitude-analytics-1.1.1.tar", last modified: Wed Jan 11 05:49:53 2023, max compression
+gzip compressed data, was "/home/runner/work/Amplitude-Python/Amplitude-Python/dist/.tmp-izfr8g94/amplitude-analytics-1.1.2.tar", last modified: Fri Aug  4 19:28:52 2023, max compression
```

## Comparing `amplitude-analytics-1.1.1.tar` & `amplitude-analytics-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 05:49:53.000000 amplitude-analytics-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-01-11 05:49:53.000000 amplitude-analytics-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 05:49:53.000000 amplitude-analytics-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 05:49:53.000000 amplitude-analytics-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 05:49:53.000000 amplitude-analytics-1.1.1/src/amplitude/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-01-11 05:49:43.000000 amplitude-analytics-1.1.1/src/amplitude/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    62087 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-01-11 05:49:11.000000 amplitude-analytics-1.1.1/src/amplitude/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 05:49:53.000000 amplitude-analytics-1.1.1/src/amplitude_analytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-01-11 05:49:53.000000 amplitude-analytics-1.1.1/src/amplitude_analytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-01-11 05:49:53.000000 amplitude-analytics-1.1.1/src/amplitude_analytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 05:49:53.000000 amplitude-analytics-1.1.1/src/amplitude_analytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-11 05:49:53.000000 amplitude-analytics-1.1.1/src/amplitude_analytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:28:52.000000 amplitude-analytics-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-04 19:28:52.000000 amplitude-analytics-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:28:52.000000 amplitude-analytics-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:28:52.000000 amplitude-analytics-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:28:52.000000 amplitude-analytics-1.1.2/src/amplitude/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-04 19:28:43.000000 amplitude-analytics-1.1.2/src/amplitude/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62087 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-08-04 19:28:20.000000 amplitude-analytics-1.1.2/src/amplitude/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:28:52.000000 amplitude-analytics-1.1.2/src/amplitude_analytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-04 19:28:52.000000 amplitude-analytics-1.1.2/src/amplitude_analytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-04 19:28:52.000000 amplitude-analytics-1.1.2/src/amplitude_analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:28:52.000000 amplitude-analytics-1.1.2/src/amplitude_analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 19:28:52.000000 amplitude-analytics-1.1.2/src/amplitude_analytics.egg-info/top_level.txt
```

### Comparing `amplitude-analytics-1.1.1/LICENSE` & `amplitude-analytics-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/PKG-INFO` & `amplitude-analytics-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplitude-analytics
-Version: 1.1.1
+Version: 1.1.2
 Summary: The official Amplitude backend Python SDK for server-side instrumentation.
 Home-page: https://github.com/amplitude/Amplitude-Python
 Author: Amplitude Inc.
 Author-email: sdk.dev@amplitude.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/amplitude/Amplitude-Python/issues
 Project-URL: Source, https://github.com/amplitude/Amplitude-Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amplitude-analytics Version: 1.1.1 Summary: The
+Metadata-Version: 2.1 Name: amplitude-analytics Version: 1.1.2 Summary: The
 official Amplitude backend Python SDK for server-side instrumentation. Home-
 page: https://github.com/amplitude/Amplitude-Python Author: Amplitude Inc.
 Author-email: sdk.dev@amplitude.com License: MIT License Project-URL: Bug
 Reports, https://github.com/amplitude/Amplitude-Python/issues Project-URL:
 Source, https://github.com/amplitude/Amplitude-Python Project-URL: Developer
 Doc, https://docs.developers.amplitude.com/data/sdks/python/ Keywords:
 amplitude,python,backend Classifier: Development Status :: 5 - Production/
```

### Comparing `amplitude-analytics-1.1.1/README.md` & `amplitude-analytics-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/setup.py` & `amplitude-analytics-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/src/amplitude/client.py` & `amplitude-analytics-1.1.2/src/amplitude/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,23 @@
         revenue(revenue_obj, event_options): Send a revenue event with revenue info in event_properties
         flush(): Flush all event waiting to be sent in the buffer
         add(plugin): Add the plugin object to client instance.
         remove(plugin): Remove the plugin object from client instance
         shutdown(): Shutdown the client instance
     """
 
-    def __init__(self, api_key: str, configuration: Config = Config()):
+    def __init__(self, api_key: str, configuration: Optional[Config] = None):
         """The constructor for the Amplitude class
 
         Args:
             api_key (str): The api key of amplitude project. Must be set properly before tracking events.
             configuration (amplitude.config.Config, optional): The configuration of client instance. A new instance
                 with default config value will be used by default.
         """
-        self.configuration: Config = configuration
+        self.configuration: Config = configuration or Config()
         self.configuration.api_key = api_key
         self.__timeline = Timeline()
         self.__timeline.setup(self)
         self._register_on_exit()
         self.add(AmplitudeDestinationPlugin())
         self.add(ContextPlugin())
```

### Comparing `amplitude-analytics-1.1.1/src/amplitude/config.py` & `amplitude-analytics-1.1.2/src/amplitude/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,30 +51,30 @@
                  flush_max_retries: int = constants.FLUSH_MAX_RETRIES,
                  logger=logging.getLogger(constants.LOGGER_NAME),
                  min_id_length: Optional[int] = None,
                  callback: Optional[Callable[[BaseEvent, int, Optional[str]], None]] = None,
                  server_zone: str = constants.DEFAULT_ZONE,
                  use_batch: bool = False,
                  server_url: Optional[str] = None,
-                 storage_provider: StorageProvider = InMemoryStorageProvider(),
+                 storage_provider: Optional[StorageProvider] = None,
                  plan: Plan = None,
                  ingestion_metadata: IngestionMetadata = None):
         """The constructor of Config class"""
         self.api_key: str = api_key
         self._flush_queue_size: int = flush_queue_size
         self._flush_size_divider: int = 1
         self.flush_interval_millis: int = flush_interval_millis
         self.flush_max_retries: int = flush_max_retries
         self.logger = logger
         self.min_id_length: Optional[int] = min_id_length
         self.callback: Optional[Callable[[BaseEvent, int, Optional[str]], None]] = callback
         self.server_zone: str = server_zone
         self.use_batch: bool = use_batch
         self._url: Optional[str] = server_url
-        self.storage_provider: StorageProvider = storage_provider
+        self.storage_provider: StorageProvider = storage_provider or InMemoryStorageProvider()
         self.opt_out: bool = False
         self.plan: Plan = plan
         self.ingestion_metadata: IngestionMetadata = ingestion_metadata
 
     def get_storage(self) -> Storage:
         """Use configured StorageProvider to create a Storage instance then return.
```

### Comparing `amplitude-analytics-1.1.1/src/amplitude/constants.py` & `amplitude-analytics-1.1.2/src/amplitude/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import Enum
 
 SDK_LIBRARY = "amplitude-python"
-SDK_VERSION = "1.1.1"
+SDK_VERSION = "1.1.2"
 
 EU_ZONE = "EU"
 DEFAULT_ZONE = "US"
 BATCH = 'batch'
 HTTP_V2 = 'v2'
 SERVER_URL = {
     EU_ZONE: {
```

### Comparing `amplitude-analytics-1.1.1/src/amplitude/event.py` & `amplitude-analytics-1.1.2/src/amplitude/event.py`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/src/amplitude/http_client.py` & `amplitude-analytics-1.1.2/src/amplitude/http_client.py`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/src/amplitude/plugin.py` & `amplitude-analytics-1.1.2/src/amplitude/plugin.py`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/src/amplitude/processor.py` & `amplitude-analytics-1.1.2/src/amplitude/processor.py`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/src/amplitude/storage.py` & `amplitude-analytics-1.1.2/src/amplitude/storage.py`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/src/amplitude/timeline.py` & `amplitude-analytics-1.1.2/src/amplitude/timeline.py`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/src/amplitude/utils.py` & `amplitude-analytics-1.1.2/src/amplitude/utils.py`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/src/amplitude/worker.py` & `amplitude-analytics-1.1.2/src/amplitude/worker.py`

 * *Files identical despite different names*

### Comparing `amplitude-analytics-1.1.1/src/amplitude_analytics.egg-info/PKG-INFO` & `amplitude-analytics-1.1.2/src/amplitude_analytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amplitude-analytics
-Version: 1.1.1
+Version: 1.1.2
 Summary: The official Amplitude backend Python SDK for server-side instrumentation.
 Home-page: https://github.com/amplitude/Amplitude-Python
 Author: Amplitude Inc.
 Author-email: sdk.dev@amplitude.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/amplitude/Amplitude-Python/issues
 Project-URL: Source, https://github.com/amplitude/Amplitude-Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: amplitude-analytics Version: 1.1.1 Summary: The
+Metadata-Version: 2.1 Name: amplitude-analytics Version: 1.1.2 Summary: The
 official Amplitude backend Python SDK for server-side instrumentation. Home-
 page: https://github.com/amplitude/Amplitude-Python Author: Amplitude Inc.
 Author-email: sdk.dev@amplitude.com License: MIT License Project-URL: Bug
 Reports, https://github.com/amplitude/Amplitude-Python/issues Project-URL:
 Source, https://github.com/amplitude/Amplitude-Python Project-URL: Developer
 Doc, https://docs.developers.amplitude.com/data/sdks/python/ Keywords:
 amplitude,python,backend Classifier: Development Status :: 5 - Production/
```

### Comparing `amplitude-analytics-1.1.1/src/amplitude_analytics.egg-info/SOURCES.txt` & `amplitude-analytics-1.1.2/src/amplitude_analytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

