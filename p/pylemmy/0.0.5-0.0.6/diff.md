# Comparing `tmp/pylemmy-0.0.5.tar.gz` & `tmp/pylemmy-0.0.6.tar.gz`

## Comparing `pylemmy-0.0.5.tar` & `pylemmy-0.0.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pylemmy-0.0.5/mkdocs.yml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.github/workflows/integration.yml
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.github/workflows/run.yaml
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/index.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/api/lemmy.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/api/utils.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/api/models/comment.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/api/models/community.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylemmy-0.0.5/docs/api/models/post.md
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pylemmy-0.0.5/examples/lmgtfy.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/__about__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/__init__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/endpoints.py
--rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/lemmy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/py.typed
--rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/utils.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/auth.py
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/comment.py
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/community.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/listing.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/person.py
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/post.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/site.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/api/utils.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/models/__init__.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/models/comment.py
--rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/models/community.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pylemmy/models/post.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/integration/__init__.py
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/integration/docker-compose.yml
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/integration/lemmy.hjson
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/integration/test_api.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/integration/test_lemmy.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pylemmy-0.0.5/tests/unit/test_utils.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pylemmy-0.0.5/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pylemmy-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 pylemmy-0.0.5/README.md
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 pylemmy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pylemmy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 pylemmy-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pylemmy-0.0.6/mkdocs.yml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pylemmy-0.0.6/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 pylemmy-0.0.6/.github/workflows/integration.yml
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pylemmy-0.0.6/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 pylemmy-0.0.6/.github/workflows/run.yaml
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 pylemmy-0.0.6/docs/index.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.6/docs/api/lemmy.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pylemmy-0.0.6/docs/api/utils.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 pylemmy-0.0.6/docs/api/models/comment.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pylemmy-0.0.6/docs/api/models/community.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pylemmy-0.0.6/docs/api/models/post.md
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pylemmy-0.0.6/examples/lmgtfy.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/__about__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/__init__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/endpoints.py
+-rw-r--r--   0        0        0    10294 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/lemmy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/py.typed
+-rw-r--r--   0        0        0     9797 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/api/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/api/auth.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/api/comment.py
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/api/community.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/api/listing.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/api/person.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/api/post.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/api/site.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/api/utils.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/models/__init__.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/models/comment.py
+-rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/models/community.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pylemmy/models/post.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pylemmy-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 pylemmy-0.0.6/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 pylemmy-0.0.6/tests/integration/docker-compose.yml
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 pylemmy-0.0.6/tests/integration/lemmy.hjson
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 pylemmy-0.0.6/tests/integration/test_api.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 pylemmy-0.0.6/tests/integration/test_lemmy.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 pylemmy-0.0.6/tests/unit/test_utils.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pylemmy-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pylemmy-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 pylemmy-0.0.6/README.md
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 pylemmy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 pylemmy-0.0.6/PKG-INFO
```

### Comparing `pylemmy-0.0.5/mkdocs.yml` & `pylemmy-0.0.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/.github/workflows/docs.yaml` & `pylemmy-0.0.6/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/.github/workflows/publish.yaml` & `pylemmy-0.0.6/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/.github/workflows/run.yaml` & `pylemmy-0.0.6/.github/workflows/run.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 name: Run
 
-on: push
+on:
+  - push
+  - pull_request
 
 jobs:
   lint:
     name: Lint
     runs-on: ubuntu-latest
 
     steps:
```

### Comparing `pylemmy-0.0.5/docs/index.md` & `pylemmy-0.0.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/examples/lmgtfy.py` & `pylemmy-0.0.6/examples/lmgtfy.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/pylemmy/endpoints.py` & `pylemmy-0.0.6/pylemmy/endpoints.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/pylemmy/lemmy.py` & `pylemmy-0.0.6/pylemmy/lemmy.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,15 @@
         :param params: Parameters to send with the request (in the body).
         """
         response = self.session.post(
             self._get_url(path),
             json=params.dict() if params is not None else {},
             timeout=self.request_timeout,
         )
+        response.raise_for_status()
         return response.json()
 
     def get_request(
         self,
         path: LemmyAPI,
         params: Optional[BaseApiModel] = None,
     ):
@@ -231,14 +232,15 @@
         :param params: Parameters to send with the request (in the URL).
         """
         response = self.session.get(
             self._get_url(path),
             params=params.dict() if params is not None else {},
             timeout=self.request_timeout,
         )
+        response.raise_for_status()
         return response.json()
 
     def put_request(
         self,
         path: LemmyAPI,
         params: Optional[BaseApiModel] = None,
     ):
```

### Comparing `pylemmy-0.0.5/pylemmy/utils.py` & `pylemmy-0.0.6/pylemmy/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,123 +5,189 @@
     Any,
     AsyncGenerator,
     Callable,
     Generator,
     Iterable,
     Optional,
     Sequence,
+    Set,
     TypeVar,
 )
 
 from aiostream import stream
 from mypy_extensions import KwArg
 
 T = TypeVar("T")
 
 
+class StreamYielder:
+    """Helper class to manage a stream and keep track of previously seen results."""
+
+    def __init__(
+        self,
+        *,
+        skip_existing: bool,
+        filter_fn: Callable[[T], bool],
+        unique_key_fn: Callable[[T], str],
+        limit: Optional[int],
+        min_wait_time: int,
+        max_wait_time: int,
+    ):
+        """Initialize StreamYielder.
+
+        :param unique_key_fn: A function that takes an object and outputs a unique id.
+        This is used to keep track of what results were already yielded.
+        :param filter_fn: Ignore objects which return `True` for this function.
+        :param limit: Maximum number of objects to yield.
+        :param max_wait_time: If a function returns no new results, the time between
+        calls to it increases. This sets the maximum time (in seconds) to wait before
+        calling it again.
+        :param min_wait_time: Minimum time (in seconds) to wait before calling the
+        function again.
+        :param skip_existing: If `True`, skip existing results and return only future
+        ones.
+        In practice, this means the results from the first request are ignored.
+        """
+        self.skip_existing = skip_existing
+        self.filter_fn = filter_fn
+        self.unique_key_fn = unique_key_fn
+        self.limit = limit
+
+        self.results_count = 0
+        self.requests_count = 0
+        self.found_keys: Set[str] = set()
+        self.last_seen_key = ""
+
+        self.wait_time = min_wait_time
+        self.min_wait_time = min_wait_time
+        self.max_wait_time = max_wait_time
+
+    def yield_results(self, results: Iterable[T]) -> Generator[Optional[T], None, None]:
+        """Iterate through the results.
+
+        :param results: Results from one to the generator function.
+        """
+        skipping_yield = False
+        if self.requests_count == 1 and self.skip_existing:
+            skipping_yield = True
+        for r in filter(self.filter_fn, results):
+            unique_key = self.unique_key_fn(r)
+            if unique_key not in self.found_keys:
+                self.last_seen_key = unique_key
+                if not skipping_yield:
+                    yield r
+                    self.results_count += 1
+                if self.limit is not None and self.results_count >= self.limit:
+                    yield None
+                self.found_keys.add(unique_key)
+
+    def get_wait_time(self, first_key: str) -> int:
+        """Get how long we should wait.
+
+        :param first_key: First key seen in the previous iteration.
+        If this is the same as `self.last_seen_key` it means that no new content
+        was seen in the last request, and so wait time should increase.
+        """
+        if first_key == self.last_seen_key:  # no new results
+            self.wait_time = min(2 * self.wait_time, self.max_wait_time)
+        else:
+            self.wait_time = self.min_wait_time
+        return self.wait_time
+
+
 def stream_generator(
     results_fn: Callable[[KwArg(Any)], Iterable[T]],
     unique_key_fn: Callable[[T], str],
     *,
     filter_fn: Callable[[T], bool] = lambda _: True,
     limit: Optional[int] = None,
     max_wait_time: int = 300,
     min_wait_time: int = 1,
+    skip_existing: bool = False,
     **function_kwargs: Any,
 ) -> Generator[T, None, None]:
     """Helper function to generate streams.
 
     :param results_fn: A function to call repeatedly, which outputs a list of objects.
     :param unique_key_fn: A function that takes an object and outputs a unique id.
     This is used to keep track of what results were already yielded.
     :param filter_fn: Ignore objects which return `True` for this function.
     :param limit: Maximum number of objects to yield.
     :param max_wait_time: If a function returns no new results, the time between calls
     to it increases. This sets the maximum time (in seconds) to wait before calling it
     again.
     :param min_wait_time: Minimum time (in seconds) to wait before calling the function
     again.
+    :param skip_existing: If `True`, skip existing results and return only future ones.
+    In practice, this means the results from the first request are ignored.
     :param function_kwargs: Keyword parameters that are passed to the function.
     """
-    found_keys = set()
-    count = 0
-    last_key: str = ""
-
-    wait_time = min_wait_time
+    stream_obj = StreamYielder(
+        skip_existing=skip_existing,
+        filter_fn=filter_fn,
+        unique_key_fn=unique_key_fn,
+        limit=limit,
+        min_wait_time=min_wait_time,
+        max_wait_time=max_wait_time,
+    )
     while True:
-        # noinspection DuplicatedCode
-        first_key = last_key
+        first_key = stream_obj.last_seen_key
         results = results_fn(**function_kwargs)
-        for r in filter(filter_fn, results):
-            unique_key = unique_key_fn(r)
-            if unique_key not in found_keys:
-                last_key = unique_key
-                yield r
-                count += 1
-                if limit is not None and count >= limit:
-                    return
-                found_keys.add(unique_key)
+        for r in stream_obj.yield_results(results):
+            if r is None:
+                return
+            yield r
 
-        if first_key == last_key:  # no new results
-            wait_time = min(2 * wait_time, max_wait_time)
-        else:
-            wait_time = min_wait_time
-
-        time.sleep(wait_time)
+        time.sleep(stream_obj.get_wait_time(first_key))
 
 
 async def async_stream_generator(
     results_fn: Callable[[KwArg(Any)], Iterable[T]],
     unique_key_fn: Callable[[T], str],
     *,
     filter_fn: Callable[[T], bool] = lambda _: True,
     limit: Optional[int] = None,
     max_wait_time: int = 300,
     min_wait_time: int = 1,
+    skip_existing: bool = False,
     **function_kwargs: Any,
 ) -> AsyncGenerator[T, None]:
     """Helper function to generate streams.
 
     :param results_fn: A function to call repeatedly, which outputs a list of objects.
     :param unique_key_fn: A function that takes an object and outputs a unique id.
     This is used to keep track of what results were already yielded.
     :param filter_fn: Ignore objects which return `True` for this function.
     :param limit: Maximum number of objects to yield.
     :param max_wait_time: If a function returns no new results, the time between calls
     to it increases. This sets the maximum time (in seconds) to wait before calling it
     again.
     :param min_wait_time: Minimum time (in seconds) to wait before calling the function
     again.
+    :param skip_existing: If `True`, skip existing results and return only future ones.
+    In practice, this means the results from the first request are ignored.
     :param function_kwargs: Keyword parameters that are passed to the function.
     """
-    found_keys = set()
-    count = 0
-    last_key: str = ""
-
-    wait_time = min_wait_time
+    stream_obj = StreamYielder(
+        skip_existing=skip_existing,
+        filter_fn=filter_fn,
+        unique_key_fn=unique_key_fn,
+        limit=limit,
+        min_wait_time=min_wait_time,
+        max_wait_time=max_wait_time,
+    )
     while True:
-        # noinspection DuplicatedCode
-        first_key = last_key
+        first_key = stream_obj.last_seen_key
         results = results_fn(**function_kwargs)
-        for r in filter(filter_fn, results):
-            unique_key = unique_key_fn(r)
-            if unique_key not in found_keys:
-                last_key = unique_key
-                yield r
-                count += 1
-                if limit is not None and count >= limit:
-                    return
-                found_keys.add(unique_key)
-
-        if first_key == last_key:  # no new results
-            wait_time = min(2 * wait_time, max_wait_time)
-        else:
-            wait_time = min_wait_time
+        for r in stream_obj.yield_results(results):
+            if r is None:
+                return
+            yield r
 
-        await asyncio.sleep(wait_time)
+        await asyncio.sleep(stream_obj.get_wait_time(first_key))
 
 
 async def _merge_streams(
     results_fns: Sequence[Callable[[KwArg(Any)], Iterable[T]]],
     unique_key_fns: Sequence[Callable[[T], str]],
     callback: Callable[[T], Any],
     *,
```

### Comparing `pylemmy-0.0.5/pylemmy/api/comment.py` & `pylemmy-0.0.6/pylemmy/api/comment.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     comment_report: CommentReport
     community: Community
     counts: CommentAggregates
     creator: Person
     creator_banned_from_community: bool
     my_vote: Optional[int]
     post: Post
-    resolver: Person
+    resolver: Optional[Person]
 
 
 class CreateCommentReport(BaseApiModel):
     auth: str
     comment_id: int
     reason: str
```

### Comparing `pylemmy-0.0.5/pylemmy/api/community.py` & `pylemmy-0.0.6/pylemmy/api/community.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/pylemmy/api/post.py` & `pylemmy-0.0.6/pylemmy/api/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,21 +118,21 @@
     published: str
     updated: Optional[str]
 
 
 class PostReportView(BaseApiModel):
     post_report: PostReport
     post: Post
-    community: int
+    community: Community
     creator: Person
     post_creator: Person
     creator_banned_from_community: bool
     my_vote: Optional[int]
     counts: PostAggregates
-    resolve: Optional[Person]
+    resolver: Optional[Person]
 
 
 class CreatePostReport(BaseApiModel):
     auth: str
     post_id: int
     reason: str
```

### Comparing `pylemmy-0.0.5/pylemmy/models/comment.py` & `pylemmy-0.0.6/pylemmy/models/comment.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -89,12 +89,12 @@
         """
         payload = api.comment.CreateCommentReport(
             auth=self.lemmy.get_token(),
             comment_id=self.comment_view.comment.id,
             reason=reason,
         )
         result = self.lemmy.post_request(LemmyAPI.CreateCommentReport, params=payload)
-        parsed_result = api.comment.CommentReportResponse(**result)
 
+        parsed_result = api.comment.CommentReportResponse(**result)
         return CommentReport(
             lemmy=self.lemmy, report=parsed_result.comment_report_view, comment=self
         )
```

### Comparing `pylemmy-0.0.5/pylemmy/models/community.py` & `pylemmy-0.0.6/pylemmy/models/community.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/pylemmy/models/post.py` & `pylemmy-0.0.6/pylemmy/models/post.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -115,12 +115,12 @@
 
         :param reason: A reason for the report.
         """
         payload = api.post.CreatePostReport(
             auth=self.lemmy.get_token(), post_id=self.post_view.post.id, reason=reason
         )
         result = self.lemmy.post_request(LemmyAPI.CreatePostReport, params=payload)
-        parsed_result = api.post.PostReportResponse(**result)
 
+        parsed_result = api.post.PostReportResponse(**result)
         return PostReport(
             lemmy=self.lemmy, report=parsed_result.post_report_view, post=self
         )
```

### Comparing `pylemmy-0.0.5/tests/integration/docker-compose.yml` & `pylemmy-0.0.6/tests/integration/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/tests/integration/lemmy.hjson` & `pylemmy-0.0.6/tests/integration/lemmy.hjson`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/tests/integration/test_api.py` & `pylemmy-0.0.6/tests/integration/test_api.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/tests/integration/test_lemmy.py` & `pylemmy-0.0.6/tests/integration/test_lemmy.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/tests/unit/test_utils.py` & `pylemmy-0.0.6/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/.gitignore` & `pylemmy-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/LICENSE.txt` & `pylemmy-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/README.md` & `pylemmy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pylemmy-0.0.5/pyproject.toml` & `pylemmy-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-    "pydantic>=1.7",
+    "pydantic>=1.8,<2.0",
     "requests>=2.18",
     "loguru>=0.3",
     "aiostream~=0.4.5",
 ]
 
 [project.urls]
 Documentation = "https://dcferreira.com/pylemmy"
```

### Comparing `pylemmy-0.0.5/PKG-INFO` & `pylemmy-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylemmy
-Version: 0.0.5
+Version: 0.0.6
 Summary: pylemmy enables simple access to Lemmy's API with Python
 Project-URL: Documentation, https://dcferreira.com/pylemmy
 Project-URL: Issues, https://github.com/dcferreira/pylemmy/issues
 Project-URL: Source, https://github.com/dcferreira/pylemmy
 Author-email: Daniel Ferreira <daniel.ferreira.1@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Requires-Dist: aiostream~=0.4.5
 Requires-Dist: loguru>=0.3
-Requires-Dist: pydantic>=1.7
+Requires-Dist: pydantic<2.0,>=1.8
 Requires-Dist: requests>=2.18
 Description-Content-Type: text/markdown
 
 # pylemmy
 
 [![PyPI - Version](https://img.shields.io/pypi/v/pylemmy.svg)](https://pypi.org/project/pylemmy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pylemmy.svg)](https://pypi.org/project/pylemmy)
```

