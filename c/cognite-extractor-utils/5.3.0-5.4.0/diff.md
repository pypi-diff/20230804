# Comparing `tmp/cognite_extractor_utils-5.3.0.tar.gz` & `tmp/cognite_extractor_utils-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-5.3.0.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-5.4.0.tar", max compression
```

## Comparing `cognite_extractor_utils-5.3.0.tar` & `cognite_extractor_utils-5.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10173 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/LICENSE
--rw-r--r--   0        0        0     4090 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/README.md
--rw-r--r--   0        0        0      739 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1558 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0    15974 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/cognite/extractorutils/base.py
--rw-r--r--   0        0        0     2861 2023-07-14 13:10:37.889018 cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/__init__.py
--rw-r--r--   0        0        0     4739 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/_util.py
--rw-r--r--   0        0        0    19910 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/elements.py
--rw-r--r--   0        0        0     9545 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/loaders.py
--rw-r--r--   0        0        0     1061 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0    14929 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0     1108 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/middleware.py
--rw-r--r--   0        0        0        0 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0    17829 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     3091 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/__init__.py
--rw-r--r--   0        0        0     5169 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/_base.py
--rw-r--r--   0        0        0     4300 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/_metrics.py
--rw-r--r--   0        0        0     5814 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/assets.py
--rw-r--r--   0        0        0     5895 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/events.py
--rw-r--r--   0        0        0    11674 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/files.py
--rw-r--r--   0        0        0     7021 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/raw.py
--rw-r--r--   0        0        0    26582 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/time_series.py
--rw-r--r--   0        0        0     7476 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1146 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0    14284 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     2067 2023-07-14 13:10:37.893018 cognite_extractor_utils-5.3.0/pyproject.toml
--rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 cognite_extractor_utils-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-08-04 07:31:06.603920 cognite_extractor_utils-5.4.0/LICENSE
+-rw-r--r--   0        0        0     4090 2023-08-04 07:31:06.603920 cognite_extractor_utils-5.4.0/README.md
+-rw-r--r--   0        0        0      739 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1558 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0    15974 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0     2861 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/configtools/__init__.py
+-rw-r--r--   0        0        0     4739 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/configtools/_util.py
+-rw-r--r--   0        0        0    19910 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/configtools/elements.py
+-rw-r--r--   0        0        0     9699 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/configtools/loaders.py
+-rw-r--r--   0        0        0     1061 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0    14929 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0     1108 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/middleware.py
+-rw-r--r--   0        0        0        0 2023-08-04 07:31:06.607920 cognite_extractor_utils-5.4.0/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0    18070 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/statestore.py
+-rw-r--r--   0        0        0     3091 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/__init__.py
+-rw-r--r--   0        0        0     5169 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/_base.py
+-rw-r--r--   0        0        0     3247 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/_metrics.py
+-rw-r--r--   0        0        0     5441 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/assets.py
+-rw-r--r--   0        0        0     5502 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/events.py
+-rw-r--r--   0        0        0    10907 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/files.py
+-rw-r--r--   0        0        0     6732 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/raw.py
+-rw-r--r--   0        0        0    26097 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/time_series.py
+-rw-r--r--   0        0        0     7476 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1146 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0    14230 2023-08-04 07:31:06.611920 cognite_extractor_utils-5.4.0/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     2067 2023-08-04 07:31:06.615920 cognite_extractor_utils-5.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 cognite_extractor_utils-5.4.0/PKG-INFO
```

### Comparing `cognite_extractor_utils-5.3.0/LICENSE` & `cognite_extractor_utils-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/README.md` & `cognite_extractor_utils-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "5.3.0"
+__version__ = "5.4.0"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/base.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/__init__.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/configtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/_util.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/configtools/_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/elements.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/configtools/elements.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/configtools/loaders.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/configtools/loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,14 +219,18 @@
             _logger.debug("Loading remote config file")
             tmp_config: _BaseConfig = load_yaml(self._config_text, _BaseConfig)  # type: ignore
             client = tmp_config.cognite.get_cognite_client("config_resolver")
             response = client.extraction_pipelines.config.retrieve(
                 tmp_config.cognite.get_extraction_pipeline(client).external_id  # type: ignore  # ignoring extpipe None
             )
 
+            if response.config is None:
+                _logger.error("No config included in response from extraction pipelines")
+                return
+
             self._next_config = _load_yaml(
                 source=response.config,
                 config_type=self.config_type,
                 dict_manipulator=lambda d: self._inject_cognite(tmp_config, d),
             )
 
         else:
```

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/middleware.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/middleware.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/statestore.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,14 +381,18 @@
 
         # ignore type since list _is_ optional, sdk types are wrong
         rows = self._cdf_client.raw.rows.list(db_name=self.database, table_name=self.table, limit=None)  # type: ignore
 
         with self.lock:
             self._local_state.clear()
             for row in rows:
+                if row.key is None or row.columns is None:
+                    self.logger.warning(f"None encountered in row: {str(row)}")
+                    # should never happen, but type from sdk is optional
+                    continue
                 self._local_state[row.key] = row.columns
 
         self._initialized = True
 
     def synchronize(self) -> None:
         self._synchronize_implementation()
```

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/__init__.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/_base.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/assets.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/assets.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,29 +11,25 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from threading import Event
 from typing import Any, Callable, List, Optional, Type
 
-import arrow
-from arrow.arrow import Arrow
-
 from cognite.client import CogniteClient
 from cognite.client.data_classes.assets import Asset
 from cognite.client.exceptions import CogniteAPIError, CogniteDuplicatedError
 from cognite.extractorutils.uploader._base import (
     RETRIES,
     RETRY_BACKOFF_FACTOR,
     RETRY_DELAY,
     RETRY_MAX_DELAY,
     AbstractUploadQueue,
 )
 from cognite.extractorutils.uploader._metrics import (
-    ASSETS_UPLOADER_LATENCY,
     ASSETS_UPLOADER_QUEUE_SIZE,
     ASSETS_UPLOADER_QUEUED,
     ASSETS_UPLOADER_WRITTEN,
 )
 from cognite.extractorutils.util import retry
 
 
@@ -72,28 +68,23 @@
             thread_name,
             cancellation_token,
         )
         self.upload_queue: List[Asset] = []
         self.assets_queued = ASSETS_UPLOADER_QUEUED
         self.assets_written = ASSETS_UPLOADER_WRITTEN
         self.queue_size = ASSETS_UPLOADER_QUEUE_SIZE
-        self.latency = ASSETS_UPLOADER_LATENCY
-        self.latency_zero_point: Arrow = arrow.utcnow()
 
     def add_to_upload_queue(self, asset: Asset) -> None:
         """
         Add asset to upload queue. The queue will be uploaded if the queue size is larger than the threshold
         specified in the __init__.
 
         Args:
             asset: Asset to add
         """
-        if self.upload_queue_size == 0:
-            self.latency_zero_point = arrow.utcnow()
-
         with self.lock:
             self.upload_queue.append(asset)
             self.assets_queued.inc()
             self.upload_queue_size += 1
             self.queue_size.set(self.upload_queue_size)
             self._check_triggers()
 
@@ -101,16 +92,14 @@
         """
         Trigger an upload of the queue, clears queue afterwards
         """
         if len(self.upload_queue) > 0:
             with self.lock:
                 self._upload_batch()
 
-                self.latency.observe((arrow.utcnow() - self.latency_zero_point).total_seconds() / 60)
-
                 try:
                     self._post_upload(self.upload_queue)
                 except Exception as e:
                     self.logger.error("Error in upload callback: %s", str(e))
 
                 self.assets_written.inc(self.upload_queue_size)
                 self.logger.info(f"Uploaded {self.upload_queue_size} assets")
```

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/events.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,28 +12,25 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import threading
 from types import TracebackType
 from typing import Callable, List, Optional, Type
 
-import arrow
-
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Event
 from cognite.client.exceptions import CogniteAPIError, CogniteDuplicatedError
 from cognite.extractorutils.uploader._base import (
     RETRIES,
     RETRY_BACKOFF_FACTOR,
     RETRY_DELAY,
     RETRY_MAX_DELAY,
     AbstractUploadQueue,
 )
 from cognite.extractorutils.uploader._metrics import (
-    EVENTS_UPLOADER_LATENCY,
     EVENTS_UPLOADER_QUEUE_SIZE,
     EVENTS_UPLOADER_QUEUED,
     EVENTS_UPLOADER_WRITTEN,
 )
 from cognite.extractorutils.util import retry
 
 
@@ -74,29 +71,24 @@
         )
 
         self.upload_queue: List[Event] = []
 
         self.events_queued = EVENTS_UPLOADER_QUEUED
         self.events_written = EVENTS_UPLOADER_WRITTEN
         self.queue_size = EVENTS_UPLOADER_QUEUE_SIZE
-        self.latency = EVENTS_UPLOADER_LATENCY
-        self.latency_zero_point = arrow.utcnow()
 
     def add_to_upload_queue(self, event: Event) -> None:
         """
         Add event to upload queue. The queue will be uploaded if the queue size is larger than the threshold
         specified in the __init__.
 
         Args:
             event: Event to add
         """
         with self.lock:
-            if self.upload_queue_size == 0:
-                self.latency_zero_point = arrow.utcnow()
-
             self.upload_queue.append(event)
             self.events_queued.inc()
             self.upload_queue_size += 1
             self.queue_size.set(self.upload_queue_size)
 
             self._check_triggers()
 
@@ -106,17 +98,14 @@
         """
         if len(self.upload_queue) == 0:
             return
 
         with self.lock:
             self._upload_batch()
 
-            self.latency.observe(
-                (arrow.utcnow() - self.latency_zero_point).total_seconds() / 60
-            )  # show data in minutes
             self.events_written.inc(self.upload_queue_size)
 
             try:
                 self._post_upload(self.upload_queue)
             except Exception as e:
                 self.logger.error("Error in upload callback: %s", str(e))
             self.upload_queue.clear()
```

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/files.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,33 +14,30 @@
 
 import threading
 from concurrent.futures import ThreadPoolExecutor
 from os import PathLike
 from types import TracebackType
 from typing import Any, Callable, List, Optional, Tuple, Type, Union
 
-import arrow
 from requests import ConnectionError
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Event, FileMetadata
 from cognite.client.exceptions import CogniteAPIError
 from cognite.extractorutils.uploader._base import (
     RETRIES,
     RETRY_BACKOFF_FACTOR,
     RETRY_DELAY,
     RETRY_MAX_DELAY,
     AbstractUploadQueue,
 )
 from cognite.extractorutils.uploader._metrics import (
-    BYTES_UPLOADER_LATENCY,
     BYTES_UPLOADER_QUEUE_SIZE,
     BYTES_UPLOADER_QUEUED,
     BYTES_UPLOADER_WRITTEN,
-    FILES_UPLOADER_LATENCY,
     FILES_UPLOADER_QUEUE_SIZE,
     FILES_UPLOADER_QUEUED,
     FILES_UPLOADER_WRITTEN,
 )
 from cognite.extractorutils.util import retry
 
 
@@ -83,31 +80,26 @@
 
         self.upload_queue: List[Tuple[FileMetadata, Union[str, PathLike]]] = []
         self.overwrite_existing = overwrite_existing
 
         self.files_queued = FILES_UPLOADER_QUEUED
         self.files_written = FILES_UPLOADER_WRITTEN
         self.queue_size = FILES_UPLOADER_QUEUE_SIZE
-        self.latency = FILES_UPLOADER_LATENCY
-        self.latency_zero_point = arrow.utcnow()
 
     def add_to_upload_queue(self, file_meta: FileMetadata, file_name: Union[str, PathLike]) -> None:
         """
         Add file to upload queue. The queue will be uploaded if the queue size is larger than the threshold
         specified in the __init__.
 
         Args:
             file_meta: File metadata-object
             file_name: Path to file to be uploaded.
                 If none, the file object will still be created, but no data is uploaded
         """
         with self.lock:
-            if self.upload_queue_size == 0:
-                self.latency_zero_point = arrow.utcnow()
-
             self.upload_queue.append((file_meta, file_name))
             self.upload_queue_size += 1
             self.files_queued.inc()
             self.queue_size.set(self.upload_queue_size)
 
             self._check_triggers()
 
@@ -117,17 +109,14 @@
         """
         if len(self.upload_queue) == 0:
             return
 
         with self.lock:
             self._upload_batch()
 
-            self.latency.observe(
-                (arrow.utcnow() - self.latency_zero_point).total_seconds() / 60
-            )  # show data in minutes
             self.files_written.inc(self.upload_queue_size)
 
             try:
                 self._post_upload(self.upload_queue)
             except Exception as e:
                 self.logger.error("Error in upload callback: %s", str(e))
             self.upload_queue.clear()
@@ -224,33 +213,28 @@
             trigger_log_level,
             thread_name,
             cancellation_token,
         )
         self.upload_queue: List[Tuple[bytes, FileMetadata]] = []
         self.overwrite_existing = overwrite_existing
         self.upload_queue_size = 0
-        self.latency_zero_point = arrow.utcnow()
 
         self.bytes_queued = BYTES_UPLOADER_QUEUED
         self.queue_size = BYTES_UPLOADER_QUEUE_SIZE
-        self.latency = BYTES_UPLOADER_LATENCY
         self.bytes_written = BYTES_UPLOADER_WRITTEN
 
     def add_to_upload_queue(self, content: bytes, metadata: FileMetadata) -> None:
         """
         Add object to upload queue. The queue will be uploaded if the queue size is larger than the threshold
         specified in the __init__.
         Args:
             content: bytes object to upload
             metadata: metadata for the given bytes object
         """
         with self.lock:
-            if self.upload_queue_size == 0:
-                self.latency_zero_point = arrow.utcnow()
-
             self.upload_queue.append((content, metadata))
             self.upload_queue_size += 1
             self.bytes_queued.inc()
             self.queue_size.set(self.upload_queue_size)
 
     def upload(self) -> None:
         """
@@ -260,17 +244,14 @@
             return
 
         with self.lock:
             # Upload frames in batches
             self._upload_batch()
 
             # Log stats
-            self.latency.observe(
-                (arrow.utcnow() - self.latency_zero_point).total_seconds() / 60
-            )  # show data in minutes
             self.bytes_written.inc(self.upload_queue_size)
 
             try:
                 self._post_upload(self.upload_queue)
             except Exception as e:
                 self.logger.error("Error in upload callback: %s", str(e))
```

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/raw.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/raw.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     RETRY_BACKOFF_FACTOR,
     RETRY_DELAY,
     RETRY_MAX_DELAY,
     AbstractUploadQueue,
     TimestampedObject,
 )
 from cognite.extractorutils.uploader._metrics import (
-    RAW_UPLOADER_LATENCY,
     RAW_UPLOADER_QUEUE_SIZE,
     RAW_UPLOADER_ROWS_DUPLICATES,
     RAW_UPLOADER_ROWS_QUEUED,
     RAW_UPLOADER_ROWS_WRITTEN,
 )
 from cognite.extractorutils.util import retry
 
@@ -79,15 +78,14 @@
         self.upload_queue: Dict[str, Dict[str, List[TimestampedObject]]] = {}
 
         # It is a hack since Prometheus client registers metrics on object creation, so object has to be created once
         self.rows_queued = RAW_UPLOADER_ROWS_QUEUED
         self.rows_written = RAW_UPLOADER_ROWS_WRITTEN
         self.rows_duplicates = RAW_UPLOADER_ROWS_DUPLICATES
         self.queue_size = RAW_UPLOADER_QUEUE_SIZE
-        self.latency = RAW_UPLOADER_LATENCY
 
     def add_to_upload_queue(self, database: str, table: str, raw_row: Row) -> None:
         """
         Adds a row to the upload queue. The queue will be uploaded if the queue size is larger than the threshold
         specified in the __init__.
 
         Args:
@@ -126,18 +124,14 @@
                     # In case of duplicate keys, the first key is preserved, and the last value is preserved.
                     patch: Dict[str, Row] = {r.payload.key: r.payload for r in rows}
                     self.rows_duplicates.labels(_labels).inc(len(rows) - len(patch))
 
                     self._upload_batch(database=database, table=table, patch=list(patch.values()))
                     self.rows_written.labels(_labels).inc(len(patch))
                     _written: Arrow = arrow.utcnow()
-                    for r in rows:
-                        self.latency.labels(_labels).observe(
-                            (_written - r.created).total_seconds() / 60
-                        )  # show data in minutes
 
                     # Perform post-upload logic if applicable
                     try:
                         self._post_upload(rows)
                     except Exception as e:
                         self.logger.error("Error in upload callback: %s", str(e))
```

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader/time_series.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader/time_series.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,33 +14,30 @@
 
 import math
 import threading
 from datetime import datetime
 from types import TracebackType
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
-import arrow
 from requests import ConnectionError
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Sequence, SequenceData, TimeSeries
 from cognite.client.exceptions import CogniteAPIError, CogniteDuplicatedError, CogniteNotFoundError
 from cognite.extractorutils.uploader._base import (
     RETRIES,
     RETRY_BACKOFF_FACTOR,
     RETRY_DELAY,
     RETRY_MAX_DELAY,
     AbstractUploadQueue,
 )
 from cognite.extractorutils.uploader._metrics import (
-    SEQUENCES_UPLOADER_LATENCY,
     SEQUENCES_UPLOADER_POINTS_QUEUED,
     SEQUENCES_UPLOADER_POINTS_WRITTEN,
     SEQUENCES_UPLOADER_QUEUE_SIZE,
-    TIMESERIES_UPLOADER_LATENCY,
     TIMESERIES_UPLOADER_POINTS_DISCARDED,
     TIMESERIES_UPLOADER_POINTS_QUEUED,
     TIMESERIES_UPLOADER_POINTS_WRITTEN,
     TIMESERIES_UPLOADER_QUEUE_SIZE,
 )
 from cognite.extractorutils.util import EitherId, retry
 
@@ -127,16 +124,14 @@
             self.missing_factory = create_missing
 
         self.upload_queue: Dict[EitherId, DataPointList] = {}
 
         self.points_queued = TIMESERIES_UPLOADER_POINTS_QUEUED
         self.points_written = TIMESERIES_UPLOADER_POINTS_WRITTEN
         self.queue_size = TIMESERIES_UPLOADER_QUEUE_SIZE
-        self.latency = TIMESERIES_UPLOADER_LATENCY
-        self.latency_zero_point = arrow.utcnow()
         self.data_set_id = data_set_id
 
     def _verify_datapoint_time(self, time: Union[int, float, datetime, str]) -> bool:
         if isinstance(time, int) or isinstance(time, float):
             return not math.isnan(time) and time >= MIN_DATAPOINT_TIMESTAMP
         elif isinstance(time, str):
             return False
@@ -190,22 +185,16 @@
 
         either_id = EitherId(id=id, external_id=external_id)
 
         with self.lock:
             if either_id not in self.upload_queue:
                 self.upload_queue[either_id] = []
 
-            if self.upload_queue_size == 0:
-                self.latency_zero_point = arrow.utcnow()
-
             self.upload_queue[either_id].extend(datapoints)
             self.points_queued.inc(len(datapoints))
-            self.latency.observe(
-                (arrow.utcnow() - self.latency_zero_point).total_seconds() / 60
-            )  # show data in minutes
             self.upload_queue_size += len(datapoints)
             self.queue_size.set(self.upload_queue_size)
 
             self._check_triggers()
 
     def upload(self) -> None:
         """
@@ -380,16 +369,14 @@
         self.asset_ids: Dict[str, int] = {}
         self.dataset_ids: Dict[str, int] = {}
         self.create_missing = create_missing
 
         self.points_queued = SEQUENCES_UPLOADER_POINTS_QUEUED
         self.points_written = SEQUENCES_UPLOADER_POINTS_WRITTEN
         self.queue_size = SEQUENCES_UPLOADER_QUEUE_SIZE
-        self.latency = SEQUENCES_UPLOADER_LATENCY
-        self.latency_zero_point = arrow.utcnow()
 
     def set_sequence_metadata(
         self,
         metadata: Dict[str, Union[str, int, float]],
         id: Optional[int] = None,
         external_id: Optional[str] = None,
         asset_external_id: Optional[str] = None,
@@ -492,15 +479,15 @@
                 # Update sequence
                 seq.values.extend(rows.values)  # type: ignore  # type is list, mypy is wrong
                 seq.row_numbers.extend(rows.row_numbers)  # type: ignore
 
                 self.upload_queue[either_id] = seq
             else:
                 self.upload_queue[either_id] = rows
-            self.upload_queue_size = len(self.upload_queue)
+            self.upload_queue_size = sum([len(rows) for rows in self.upload_queue.values()])
             self.queue_size.set(self.upload_queue_size)
             self.points_queued.inc()
 
     def upload(self) -> None:
         """
         Trigger an upload of the queue, clears queue afterwards
         """
@@ -511,31 +498,28 @@
             if self.create_missing:
                 self._resolve_asset_ids()
                 self._resolve_dataset_ids()
 
             for either_id, upload_this in self.upload_queue.items():
                 _labels = str(either_id.content())
                 self._upload_single(either_id, upload_this)
-                self.latency.observe(
-                    (arrow.utcnow() - self.latency_zero_point).total_seconds() / 60
-                )  # show data in minutes
                 self.points_written.inc()
 
             try:
                 self._post_upload([seqdata for _, seqdata in self.upload_queue.items()])
             except Exception as e:
                 self.logger.error("Error in upload callback: %s", str(e))
 
+            self.logger.info(f"Uploaded {self.upload_queue_size} sequence rows")
             self.upload_queue.clear()
             self.upload_queue_size = 0
-            self.logger.info(f"Uploaded {self.upload_queue_size} sequence rows")
             self.queue_size.set(self.upload_queue_size)
 
     @retry(
-        exceptions=[CogniteAPIError],
+        exceptions=(CogniteAPIError, ConnectionError),
         tries=RETRIES,
         delay=RETRY_DELAY,
         max_delay=RETRY_MAX_DELAY,
         backoff=RETRY_BACKOFF_FACTOR,
     )
     def _upload_single(self, either_id: EitherId, upload_this: SequenceData) -> SequenceData:
         self.logger.debug("Writing {} rows to sequence {}".format(len(upload_this.values), either_id))
@@ -611,14 +595,15 @@
         if len(assets) > 0:
             try:
                 self.asset_ids = {
                     asset.external_id: asset.id
                     for asset in self.cdf_client.assets.retrieve_multiple(
                         external_ids=list(assets), ignore_unknown_ids=True
                     )
+                    if asset.id is not None and asset.external_id is not None
                 }
             except Exception as e:
                 self.logger.error("Error in resolving asset id: %s", str(e))
                 self.asset_ids = {}
 
     def _resolve_dataset_ids(self) -> None:
         """
@@ -630,14 +615,15 @@
         if len(datasets) > 0:
             try:
                 self.dataset_ids = {
                     dataset.external_id: dataset.id
                     for dataset in self.cdf_client.data_sets.retrieve_multiple(
                         external_ids=list(datasets), ignore_unknown_ids=True
                     )
+                    if dataset.id is not None and dataset.external_id is not None
                 }
             except Exception as e:
                 self.logger.error("Error in resolving dataset id: %s", str(e))
                 self.dataset_ids = {}
 
     def __enter__(self) -> "SequenceUploadQueue":
         """
```

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-5.3.0/cognite/extractorutils/util.py` & `cognite_extractor_utils-5.4.0/cognite/extractorutils/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,27 +326,27 @@
 
 _T2 = TypeVar("_T2")
 
 
 def _retry_internal(
     f: Callable[..., _T2],
     cancellation_token: threading.Event = threading.Event(),
-    exceptions: Iterable[Type[Exception]] = [Exception],
+    exceptions: Tuple[Type[Exception], ...] = (Exception,),
     tries: int = -1,
     delay: float = 0,
     max_delay: Optional[float] = None,
     backoff: float = 1,
     jitter: Union[float, Tuple[float, float]] = 0,
 ) -> _T2:
     logger = logging.getLogger(__name__)
 
     while tries and not cancellation_token.is_set():
         try:
             return f()
-        except exceptions as e:  # type: ignore  # Exception is an exception type, smh mypy
+        except exceptions as e:
             tries -= 1
             if not tries:
                 raise e
 
             if logger is not None:
                 logger.warning("%s, retrying in %s seconds...", e, delay)
 
@@ -362,15 +362,15 @@
                 delay = min(delay, max_delay)
 
     return None  # type: ignore  # unreachable, we will have raised an exception before this
 
 
 def retry(
     cancellation_token: threading.Event = threading.Event(),
-    exceptions: Iterable[Type[Exception]] = [Exception],
+    exceptions: Tuple[Type[Exception], ...] = (Exception,),
     tries: int = -1,
     delay: float = 0,
     max_delay: Optional[float] = None,
     backoff: float = 1,
     jitter: Union[float, Tuple[float, float]] = 0,
 ) -> Callable[[Callable[..., _T2]], Callable[..., _T2]]:
     """
```

### Comparing `cognite_extractor_utils-5.3.0/pyproject.toml` & `cognite_extractor_utils-5.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "5.3.0"
+version = "5.4.0"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
```

### Comparing `cognite_extractor_utils-5.3.0/PKG-INFO` & `cognite_extractor_utils-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 5.3.0
+Version: 5.4.0
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 5.3.0 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 5.4.0 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

