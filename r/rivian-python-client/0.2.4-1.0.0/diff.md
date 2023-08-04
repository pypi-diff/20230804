# Comparing `tmp/rivian_python_client-0.2.4.tar.gz` & `tmp/rivian_python_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivian_python_client-0.2.4.tar", max compression
+gzip compressed data, was "rivian_python_client-1.0.0.tar", max compression
```

## Comparing `rivian_python_client-0.2.4.tar` & `rivian_python_client-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      325 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/README.md
--rw-r--r--   0        0        0      555 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      102 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/src/rivian/__init__.py
--rw-r--r--   0        0        0     3242 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/src/rivian/const.py
--rw-r--r--   0        0        0      779 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/src/rivian/exceptions.py
--rw-r--r--   0        0        0    23190 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/src/rivian/rivian.py
--rw-r--r--   0        0        0     7383 2023-07-30 01:43:46.885077 rivian_python_client-0.2.4/src/rivian/ws_monitor.py
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 rivian_python_client-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      325 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/README.md
+-rw-r--r--   0        0        0      775 2023-08-04 16:02:00.061496 rivian_python_client-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      155 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/__init__.py
+-rw-r--r--   0        0        0     5766 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/const.py
+-rw-r--r--   0        0        0      969 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/py.typed
+-rw-r--r--   0        0        0    26126 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/rivian.py
+-rw-r--r--   0        0        0     3031 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/utils.py
+-rw-r--r--   0        0        0     7509 2023-08-04 16:01:43.321081 rivian_python_client-1.0.0/src/rivian/ws_monitor.py
+-rw-r--r--   0        0        0      976 1970-01-01 00:00:00.000000 rivian_python_client-1.0.0/PKG-INFO
```

### Comparing `rivian_python_client-0.2.4/pyproject.toml` & `rivian_python_client-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [tool.poetry]
 name = "rivian-python-client"
-version = "0.2.4"
+version = "1.0.0"
 description = "Rivian API Client (Unofficial)"
 readme = "README.md"
 authors = ["Brian Retterer <bretterer@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "rivian", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = ">=3.0.0"
-yarl = ">=1.6.0"
+cryptography = "^41.0.1"
+backports-strenum = { version = "^1.2.4", python = "<3.11" } 
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.18.3"
 python-dotenv = "^0.20.0"
 aresponses = "^2.1.5"
 
+[tool.poetry-dynamic-versioning]
+enable = true
+vcs = "git"
+style = "semver"
+pattern = "default-unprefixed"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `rivian_python_client-0.2.4/src/rivian/exceptions.py` & `rivian_python_client-1.0.0/src/rivian/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,7 +27,15 @@
 
 class RivianTemporarilyLockedError(RivianApiException):
     """Rivian User Temporarily Locked Error"""
 
 
 class RivianApiRateLimitError(RivianApiException):
     """Rivian API is being rate limited."""
+
+
+class RivianPhoneLimitReachedError(RivianApiException):
+    """Rivian phone limit has been reached."""
+
+
+class RivianBadRequestError(RivianApiException):
+    """Rivian API bad request."""
```

### Comparing `rivian_python_client-0.2.4/src/rivian/ws_monitor.py` & `rivian_python_client-1.0.0/src/rivian/ws_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime, timezone
 from json import loads
 from random import uniform
 from typing import TYPE_CHECKING, Any
 from uuid import uuid4
 
 import async_timeout
-from aiohttp import ClientWebSocketResponse, WSMsgType
+from aiohttp import ClientWebSocketResponse, WSMessage, WSMsgType
 
 if TYPE_CHECKING:
     from .rivian import Rivian
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -77,43 +77,46 @@
         return self._monitor_task
 
     async def new_connection(self, start_monitor: bool = False) -> None:
         """Create a new connection and, optionally, start the monitor."""
         await cancel_task(self._receiver_task)
         self._disconnect = False
         # pylint: disable=protected-access
+        assert self._account._session
         self._ws = await self._account._session.ws_connect(
             url=self._url, headers={"sec-websocket-protocol": "graphql-transport-ws"}
         )
         await self._connection_init(self._ws)
         self._receiver_task = asyncio.ensure_future(self._receiver())
         if start_monitor:
             await self.start_monitor()
 
     async def start_subscription(
         self, payload: dict[str, Any], callback: Callable[[dict[str, Any]], None]
     ) -> Callable[[], Awaitable[None]] | None:
         """Start a subscription."""
         if not self.connected:
-            return
+            return None
         _id = str(uuid4())
         self._subscriptions[_id] = (callback, payload)
         await self._subscribe(_id, payload)
 
         async def unsubscribe() -> None:
             """Unsubscribe."""
             if _id in self._subscriptions:
                 del self._subscriptions[_id]
                 if self.connected:
+                    assert self._ws
                     await self._ws.send_json({"id": _id, "type": "complete"})
 
         return unsubscribe
 
     async def _subscribe(self, _id: str, payload: dict[str, Any]) -> None:
         """Send a subscribe request."""
+        assert self._ws
         await self._ws.send_json({"id": _id, "payload": payload, "type": "subscribe"})
 
     async def _resubscribe_all(self) -> None:
         """Resubscribe all subscriptions."""
         try:
             async with async_timeout.timeout(self._account.request_timeout):
                 await self.connection_ack.wait()
@@ -138,16 +141,15 @@
                 self._last_received = datetime.now(timezone.utc)
                 if msg.type == WSMsgType.TEXT:
                     data = loads(msg.data)
                     if (data_type := data.get("type")) == "connection_ack":
                         self._connection_ack.set()
                     elif data_type == "next":
                         if (_id := data.get("id")) in self._subscriptions:
-                            if callback := self._subscriptions[_id][0]:
-                                callback(data)
+                            self._subscriptions[_id][0](data)
                     else:
                         self._log_message(msg)
                 elif msg.type == WSMsgType.ERROR:
                     self._log_message(msg, True)
                     continue
             except asyncio.TimeoutError:
                 await self._resubscribe_all()
@@ -155,15 +157,16 @@
         self._log_message("web socket stopped")
 
     async def _monitor(self) -> None:
         """Monitor a web socket connection."""
         attempt = 0
         while not self._disconnect:
             while self.connected:
-                if self._receiver_task.done():  # Need to restart the receiver
+                if self._receiver_task and self._receiver_task.done():
+                    # Need to restart the receiver
                     self._receiver_task = asyncio.ensure_future(self._receiver())
                 await asyncio.sleep(1)
             if not self._disconnect:
                 try:
                     await self.new_connection()
                 except Exception as ex:  # pylint: disable=broad-except
                     self._log_message(ex, True)
@@ -187,11 +190,13 @@
     async def close(self) -> None:
         """Close the web socket."""
         self._disconnect = True
         if self._ws:
             await self._ws.close()
         await cancel_task(self._monitor_task, self._receiver_task)
 
-    def _log_message(self, message: str | Exception, is_error: bool = False) -> None:
+    def _log_message(
+        self, message: str | Exception | WSMessage, is_error: bool = False
+    ) -> None:
         """Log a message."""
         log_method = _LOGGER.error if is_error else _LOGGER.debug
         log_method(message)
```

### Comparing `rivian_python_client-0.2.4/PKG-INFO` & `rivian_python_client-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: rivian-python-client
-Version: 0.2.4
+Version: 1.0.0
 Summary: Rivian API Client (Unofficial)
 License: MIT
 Author: Brian Retterer
 Author-email: bretterer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.0.0)
-Requires-Dist: yarl (>=1.6.0)
+Requires-Dist: backports-strenum (>=1.2.4,<2.0.0) ; python_version < "3.11"
+Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Description-Content-Type: text/markdown
 
 # Python: Rivian API Client
 
 Currently a Work In Progress
 
 ## Dependencies
```

