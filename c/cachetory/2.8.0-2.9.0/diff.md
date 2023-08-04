# Comparing `tmp/cachetory-2.8.0.tar.gz` & `tmp/cachetory-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetory-2.8.0.tar", max compression
+gzip compressed data, was "cachetory-2.9.0.tar", max compression
```

## Comparing `cachetory-2.8.0.tar` & `cachetory-2.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11355 2023-07-17 14:32:17.842513 cachetory-2.8.0/LICENSE
--rw-r--r--   0        0        0    14352 2023-07-17 14:32:17.842513 cachetory-2.8.0/README.md
--rw-r--r--   0        0        0        0 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/__init__.py
--rw-r--r--   0        0        0       43 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/__init__.py
--rw-r--r--   0        0        0     1272 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/async_/__init__.py
--rw-r--r--   0        0        0     2385 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/async_/django.py
--rw-r--r--   0        0        0     1520 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/async_/dummy.py
--rw-r--r--   0        0        0     1718 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/async_/memory.py
--rw-r--r--   0        0        0     2476 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/async_/redis.py
--rw-r--r--   0        0        0     1266 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/sync/__init__.py
--rw-r--r--   0        0        0     2220 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/sync/django.py
--rw-r--r--   0        0        0     1408 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/sync/dummy.py
--rw-r--r--   0        0        0     2340 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/sync/memory.py
--rw-r--r--   0        0        0     2201 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/backends/sync/redis.py
--rw-r--r--   0        0        0       47 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/caches/__init__.py
--rw-r--r--   0        0        0     3631 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/caches/async_.py
--rw-r--r--   0        0        0      122 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/caches/private.py
--rw-r--r--   0        0        0     2978 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/caches/sync.py
--rw-r--r--   0        0        0        0 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/decorators/__init__.py
--rw-r--r--   0        0        0     4241 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/decorators/async_.py
--rw-r--r--   0        0        0      990 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/decorators/shared.py
--rw-r--r--   0        0        0     3665 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/decorators/sync.py
--rw-r--r--   0        0        0       41 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/backends/__init__.py
--rw-r--r--   0        0        0     3959 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/backends/async_.py
--rw-r--r--   0        0        0     1183 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/backends/private.py
--rw-r--r--   0        0        0     3489 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/backends/sync.py
--rw-r--r--   0        0        0     1598 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/interfaces/serializers.py
--rw-r--r--   0        0        0       67 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/private/__init__.py
--rw-r--r--   0        0        0      307 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/private/asyncio.py
--rw-r--r--   0        0        0      481 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/private/datetime.py
--rw-r--r--   0        0        0      909 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/private/functools.py
--rw-r--r--   0        0        0      205 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/private/typing.py
--rw-r--r--   0        0        0        0 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/py.typed
--rw-r--r--   0        0        0      402 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/__init__.py
--rw-r--r--   0        0        0     2718 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/chained.py
--rw-r--r--   0        0        0      326 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/compressors/__init__.py
--rw-r--r--   0        0        0     1026 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/compressors/zlib.py
--rw-r--r--   0        0        0     1248 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/compressors/zstd.py
--rw-r--r--   0        0        0      544 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/json.py
--rw-r--r--   0        0        0      608 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/msgpack.py
--rw-r--r--   0        0        0      538 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/noop.py
--rw-r--r--   0        0        0     1106 2023-07-17 14:32:17.846508 cachetory-2.8.0/cachetory/serializers/pickle.py
--rw-r--r--   0        0        0     3234 2023-07-17 14:32:30.802511 cachetory-2.8.0/pyproject.toml
--rw-r--r--   0        0        0    15890 1970-01-01 00:00:00.000000 cachetory-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-08-04 13:37:14.465255 cachetory-2.9.0/LICENSE
+-rw-r--r--   0        0        0     1337 2023-08-04 13:37:14.465255 cachetory-2.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-04 13:37:14.465255 cachetory-2.9.0/cachetory/__init__.py
+-rw-r--r--   0        0        0       43 2023-08-04 13:37:14.465255 cachetory-2.9.0/cachetory/backends/__init__.py
+-rw-r--r--   0        0        0     1272 2023-08-04 13:37:14.465255 cachetory-2.9.0/cachetory/backends/async_/__init__.py
+-rw-r--r--   0        0        0     2478 2023-08-04 13:37:14.465255 cachetory-2.9.0/cachetory/backends/async_/django.py
+-rw-r--r--   0        0        0     1520 2023-08-04 13:37:14.465255 cachetory-2.9.0/cachetory/backends/async_/dummy.py
+-rw-r--r--   0        0        0     1718 2023-08-04 13:37:14.465255 cachetory-2.9.0/cachetory/backends/async_/memory.py
+-rw-r--r--   0        0        0     2586 2023-08-04 13:37:14.465255 cachetory-2.9.0/cachetory/backends/async_/redis.py
+-rw-r--r--   0        0        0     1266 2023-08-04 13:37:14.465255 cachetory-2.9.0/cachetory/backends/sync/__init__.py
+-rw-r--r--   0        0        0     2312 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/backends/sync/django.py
+-rw-r--r--   0        0        0     1408 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/backends/sync/dummy.py
+-rw-r--r--   0        0        0     2340 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/backends/sync/memory.py
+-rw-r--r--   0        0        0     2311 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/backends/sync/redis.py
+-rw-r--r--   0        0        0       47 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/caches/__init__.py
+-rw-r--r--   0        0        0     3610 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/caches/async_.py
+-rw-r--r--   0        0        0      122 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/caches/private.py
+-rw-r--r--   0        0        0     4014 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/caches/sync.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/decorators/__init__.py
+-rw-r--r--   0        0        0     4241 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/decorators/async_.py
+-rw-r--r--   0        0        0     1096 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/decorators/shared.py
+-rw-r--r--   0        0        0     3665 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/decorators/sync.py
+-rw-r--r--   0        0        0       41 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/interfaces/backends/__init__.py
+-rw-r--r--   0        0        0     3959 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/interfaces/backends/async_.py
+-rw-r--r--   0        0        0     1183 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/interfaces/backends/private.py
+-rw-r--r--   0        0        0     3489 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/interfaces/backends/sync.py
+-rw-r--r--   0        0        0     1598 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/interfaces/serializers.py
+-rw-r--r--   0        0        0       67 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/private/__init__.py
+-rw-r--r--   0        0        0      307 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/private/asyncio.py
+-rw-r--r--   0        0        0      481 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/private/datetime.py
+-rw-r--r--   0        0        0      909 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/private/functools.py
+-rw-r--r--   0        0        0      205 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/private/typing.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/py.typed
+-rw-r--r--   0        0        0      776 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/serializers/__init__.py
+-rw-r--r--   0        0        0     3325 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/serializers/chained.py
+-rw-r--r--   0        0        0      326 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/serializers/compressors/__init__.py
+-rw-r--r--   0        0        0     1512 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/serializers/compressors/zlib.py
+-rw-r--r--   0        0        0     1999 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/serializers/compressors/zstd.py
+-rw-r--r--   0        0        0      731 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/serializers/json.py
+-rw-r--r--   0        0        0      846 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/serializers/msgpack.py
+-rw-r--r--   0        0        0      873 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/serializers/noop.py
+-rw-r--r--   0        0        0     1627 2023-08-04 13:37:14.469255 cachetory-2.9.0/cachetory/serializers/pickle.py
+-rw-r--r--   0        0        0     3539 2023-08-04 13:37:26.813354 cachetory-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2875 1970-01-01 00:00:00.000000 cachetory-2.9.0/PKG-INFO
```

### Comparing `cachetory-2.8.0/LICENSE` & `cachetory-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/backends/async_/__init__.py` & `cachetory-2.9.0/cachetory/backends/async_/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/backends/async_/django.py` & `cachetory-2.9.0/cachetory/backends/async_/django.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
 from typing import AsyncIterable, Generic, Iterable
 from urllib.parse import urlparse
 
-from django.core.cache import BaseCache, caches  # type: ignore[import]
+from django.core.cache import BaseCache, cache, caches  # type: ignore[import]
 from django.core.cache.backends.base import DEFAULT_TIMEOUT  # type: ignore[import]
 
 from cachetory.interfaces.backends.async_ import AsyncBackend
 from cachetory.interfaces.backends.private import WireT
 from cachetory.private.datetime import make_time_to_live
 
 _SENTINEL = object()
 
 
 class DjangoBackend(AsyncBackend[WireT], Generic[WireT]):
-    """Django cache adapter."""
+    """Asynchronous Django cache adapter."""
 
     __slots__ = ("_cache",)
 
     @classmethod
     def from_url(cls, url: str) -> DjangoBackend[WireT]:
         return DjangoBackend(caches[urlparse(url).hostname])
 
-    def __init__(self, cache: BaseCache) -> None:
+    def __init__(self, cache: BaseCache = cache) -> None:
+        """Initialize backend with the Django cache instance."""
         self._cache = cache
 
     async def get(self, key: str) -> WireT:
         if (value := await self._cache.aget(key, _SENTINEL)) is not _SENTINEL:
             return value
         raise KeyError(key)
```

### Comparing `cachetory-2.8.0/cachetory/backends/async_/dummy.py` & `cachetory-2.9.0/cachetory/backends/async_/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/backends/async_/memory.py` & `cachetory-2.9.0/cachetory/backends/async_/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/backends/async_/redis.py` & `cachetory-2.9.0/cachetory/backends/async_/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 class RedisBackend(AsyncBackend[bytes]):
     """Asynchronous Redis backend."""
 
     __slots__ = ("_client",)
 
     @classmethod
     def from_url(cls, url: str) -> RedisBackend:
+        """Instantiate a backend from the URL."""
         if url.startswith("redis+"):
             url = url[6:]
         return RedisBackend(Redis.from_url(url))
 
     def __init__(self, client: Redis) -> None:
+        """Instantiate a backend using the Redis client."""
         self._client = client
 
     async def get(self, key: str) -> bytes:
         data = await self._client.get(key)
         if data is not None:
             return data
         raise KeyError(key)
```

### Comparing `cachetory-2.8.0/cachetory/backends/sync/__init__.py` & `cachetory-2.9.0/cachetory/backends/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/backends/sync/django.py` & `cachetory-2.9.0/cachetory/backends/sync/django.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
 from typing import Generic, Iterable
 from urllib.parse import urlparse
 
-from django.core.cache import BaseCache, caches  # type: ignore[import]
+from django.core.cache import BaseCache, cache, caches  # type: ignore[import]
 from django.core.cache.backends.base import DEFAULT_TIMEOUT  # type: ignore[import]
 
 from cachetory.interfaces.backends.private import WireT
 from cachetory.interfaces.backends.sync import SyncBackend
 from cachetory.private.datetime import make_time_to_live
 
 _SENTINEL = object()
 
 
 class DjangoBackend(SyncBackend[WireT], Generic[WireT]):
-    """Django cache adapter."""
+    """Synchronous Django cache adapter."""
 
     __slots__ = ("_cache",)
 
     @classmethod
     def from_url(cls, url: str) -> DjangoBackend[WireT]:
         return DjangoBackend(caches[urlparse(url).hostname])
 
-    def __init__(self, cache: BaseCache) -> None:
+    def __init__(self, cache: BaseCache = cache) -> None:
+        """Initialize backend with the Django cache instance."""
         self._cache = cache
 
     def get(self, key: str) -> WireT:
         if (value := self._cache.get(key, _SENTINEL)) is not _SENTINEL:
             return value
         raise KeyError(key)
```

### Comparing `cachetory-2.8.0/cachetory/backends/sync/dummy.py` & `cachetory-2.9.0/cachetory/backends/sync/dummy.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/backends/sync/memory.py` & `cachetory-2.9.0/cachetory/backends/sync/memory.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/backends/sync/redis.py` & `cachetory-2.9.0/cachetory/backends/sync/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 class RedisBackend(SyncBackend[bytes]):
     """Synchronous Redis backend."""
 
     __slots__ = ("_client",)
 
     @classmethod
     def from_url(cls, url: str) -> RedisBackend:
+        """Instantiate a backend from the URL."""
         if url.startswith("redis+"):
             url = url[6:]
         return cls(Redis.from_url(url))
 
     def __init__(self, client: Redis) -> None:
+        """Instantiate a backend using the Redis client."""
         self._client = client
 
     def get(self, key: str) -> bytes:
         data = self._client.get(key)
         if data is not None:
             return data
         raise KeyError(key)
```

### Comparing `cachetory-2.8.0/cachetory/caches/async_.py` & `cachetory-2.9.0/cachetory/caches/async_.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ) -> None:
         """
         Instantiate a cache.
 
         Args:
             serialize_executor:
                 If specified, underlying serializing and deserializing will be performed
-                using the executor (for example, ``concurrent.futures.ProcessPoolExecutor``).
+                using the executor (for example, `ProcessPoolExecutor`).
                 This may be useful to better utilize CPU when caching large blobs.
                 If not specified, (de)serialization is performed in the current thread.
         """
         self._serializer = serializer
         self._backend = backend
         self._serialize_executor = serialize_executor
```

### Comparing `cachetory-2.8.0/cachetory/decorators/async_.py` & `cachetory-2.9.0/cachetory/decorators/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/decorators/shared.py` & `cachetory-2.9.0/cachetory/decorators/shared.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from hashlib import blake2s
 from typing import Any, Callable
 
 
 def make_default_key(callable_: Callable[..., Any], *args: Any, **kwargs: Any) -> str:
-    """Generate cache key given the callable and the arguments it's being called with."""
+    """
+    Generate a human-readable cache key out of decorated function fully-qualified name and stringified arguments.
+
+    The length of the key depends on the arguments.
+    """
 
     # noinspection PyUnresolvedReferences
     parts = (
         callable_.__module__,
         callable_.__qualname__,
         # Since we join with `:`, we need to «escape» `:`s with `::`.
         *(str(arg).replace(":", "::") for arg in args),
         *(f"{str(key).replace(':', '::')}={str(value).replace(':', '::')}" for key, value in sorted(kwargs.items())),
     )
     return ":".join(parts)
 
 
 def make_default_hashed_key(callable_: Callable[..., Any], *args: Any, **kwargs: Any) -> str:
     """
-    Generate a hashed cache key given the callable and the arguments it's being called with.
+    Generate a hashed fixed-length cache key given the callable and the arguments it's being called with.
 
     Uses `blake2s` as the fastest algorithm from `hashlib`.
     """
     return blake2s(make_default_key(callable_, *args, **kwargs).encode()).hexdigest()
```

### Comparing `cachetory-2.8.0/cachetory/decorators/sync.py` & `cachetory-2.9.0/cachetory/decorators/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/interfaces/backends/async_.py` & `cachetory-2.9.0/cachetory/interfaces/backends/async_.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/interfaces/backends/private.py` & `cachetory-2.9.0/cachetory/interfaces/backends/private.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/interfaces/backends/sync.py` & `cachetory-2.9.0/cachetory/interfaces/backends/sync.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/interfaces/serializers.py` & `cachetory-2.9.0/cachetory/interfaces/serializers.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/private/functools.py` & `cachetory-2.9.0/cachetory/private/functools.py`

 * *Files identical despite different names*

### Comparing `cachetory-2.8.0/cachetory/serializers/chained.py` & `cachetory-2.9.0/cachetory/serializers/chained.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,25 +24,43 @@
 except ImportError:
     _is_msgpack_available = False
 else:
     _is_msgpack_available = True
 
 
 class ChainedSerializer(Serializer[ValueT, WireT], Generic[ValueT, WireT]):
-    """Sequentially applies the chain of serializers. Allows defining multiple steps of serialization."""
+    """Sequentially applies the chain of serializers. It allows defining multiple steps of serialization."""
 
     __slots__ = ("_layers",)
 
     @classmethod
     def from_url(cls, url: str) -> ChainedSerializer[ValueT, WireT]:
+        """
+        Construct serializer from the URL.
+
+        This method parses the URL and constructs serializer layers based on the schema's
+        and query parameters.
+
+        Examples:
+            >>> serializer = ChainedSerializer.from_url(
+            >>>     # Serialize with Pickle and then compress with Zstandard:
+            >>>     "pickle+zstd://?pickle-protocol=4&compression-level=3",
+            >>> )
+        """
         parsed_url = urlparse(url)
         schemes = parsed_url.scheme.split("+")
         return cls(cls._make_layer(scheme, url) for scheme in schemes)
 
     def __init__(self, layers: Iterable[Serializer]) -> None:
+        """
+        Initialize the chained serializer.
+
+        Args:
+            layers: iterable of other serializers which are then applied sequentially
+        """
         self._layers = list(layers)
 
     def serialize(self, value: ValueT) -> WireT:
         value = cast(Any, value)
         for layer in self._layers:
             value = layer.serialize(value)
         return cast(WireT, value)
```

### Comparing `cachetory-2.8.0/cachetory/serializers/compressors/zlib.py` & `cachetory-2.9.0/cachetory/serializers/compressors/zlib.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,20 +5,33 @@
 
 from pydantic import BaseModel, Field, conint
 
 from cachetory.interfaces.serializers import Serializer
 
 
 class ZlibCompressor(Serializer[bytes, bytes]):
-    """Uses the built-in zlib compression."""
+    """Uses the built-in [zlib](https://docs.python.org/3/library/zlib.html) compression."""
 
     __slots__ = ("_level",)
 
     @classmethod
     def from_url(cls, url: str) -> ZlibCompressor:
+        """
+        Construct serializer from the URL.
+
+        # Supported schema's
+
+        - `zlib://`
+
+        # URL parameters
+
+        | Parameter           |                                                                 |
+        |---------------------|-----------------------------------------------------------------|
+        | `compression-level` | From `0` (no compression) to `9` (slowest and best compression) |
+        """
         params = _UrlParams.parse_obj(dict(parse_qsl(urlparse(url).query)))
         return cls(compression_level=params.compression_level)
 
     def __init__(self, *, compression_level: int = zlib.Z_DEFAULT_COMPRESSION) -> None:
         self._level = compression_level
 
     def serialize(self, value: bytes) -> bytes:
```

### Comparing `cachetory-2.8.0/cachetory/serializers/pickle.py` & `cachetory-2.9.0/cachetory/serializers/pickle.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,24 +6,47 @@
 
 from pydantic import BaseModel, Field, conint
 
 from cachetory.interfaces.serializers import Serializer, ValueT
 
 
 class PickleSerializer(Serializer[ValueT, bytes], Generic[ValueT]):
-    """Uses the standard built-in `pickle` serialization."""
+    """
+    Uses the standard built-in [`pickle`][1] serialization.
+
+    [1]: https://docs.python.org/3/library/pickle.html
+    """
 
     __slots__ = ("protocol",)
 
     @classmethod
     def from_url(cls, url: str) -> PickleSerializer[ValueT]:
+        """
+        Construct serializer from the URL.
+
+        # Supported schema's
+
+        - `pickle://`
+
+        # URL parameters
+
+        | Parameter         |                           |
+        |-------------------|---------------------------|
+        | `pickle-protocol` | `pickle` protocol version |
+        """
         params = _UrlParams.parse_obj(dict(parse_qsl(urlparse(url).query)))
         return cls(pickle_protocol=params.pickle_protocol)
 
     def __init__(self, pickle_protocol: int = pickle.HIGHEST_PROTOCOL) -> None:
+        """
+        Initialize the serializer.
+
+        Args:
+            pickle_protocol: `pickle` protocol version
+        """
         self.protocol = pickle_protocol
 
     def serialize(self, value: ValueT) -> bytes:
         return pickle.dumps(value, self.protocol)
 
     def deserialize(self, data: bytes) -> ValueT:
         return pickle.loads(data)
```

### Comparing `cachetory-2.8.0/pyproject.toml` & `cachetory-2.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 description = "Caching library with support for multiple cache backends"
 keywords = ["cache"]
 license = "Apache-2.0"
 name = "cachetory"
 readme = "README.md"
 repository = "https://github.com/kpn/cachetory"
-version = "2.8.0"
+version = "2.9.0"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -56,14 +56,26 @@
 mypy = "^1.3.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
 ruff = "^0.0.275"
 types-redis = "^4.4.0.4"
 
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs-material = "^9.0.12"
+pillow = "^9.4.0"
+cairosvg = "^2.6.0"
+mkdocs-git-revision-date-localized-plugin = "^1.1.0"
+mkdocstrings = { version = "^0.20.0", extras = ["python"] }
+mkdocs-autorefs = "^0.4.1"
+black = "^23.1.0"
+
 [tool.black]
 line-length = 120
 target_version = ["py37", "py38", "py39", "py310", "py311"]
 
 [tool.ruff]
 line-length = 120
 target-version = "py37"
```

