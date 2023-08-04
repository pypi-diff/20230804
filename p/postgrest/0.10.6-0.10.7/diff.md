# Comparing `tmp/postgrest-0.10.6.tar.gz` & `tmp/postgrest-0.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgrest-0.10.6.tar", max compression
+gzip compressed data, was "postgrest-0.10.7.tar", max compression
```

## Comparing `postgrest-0.10.6.tar` & `postgrest-0.10.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1077 2022-10-10 16:43:48.419108 postgrest-0.10.6/LICENSE
--rw-r--r--   0        0        0     4078 2023-01-23 01:50:04.944224 postgrest-0.10.6/README.md
--rw-r--r--   0        0        0      742 2023-02-26 14:47:40.278305 postgrest-0.10.6/postgrest/__init__.py
--rw-r--r--   0        0        0       35 2022-10-10 16:43:48.421467 postgrest-0.10.6/postgrest/_async/__init__.py
--rw-r--r--   0        0        0     3077 2022-10-10 16:43:48.421653 postgrest-0.10.6/postgrest/_async/client.py
--rw-r--r--   0        0        0    11662 2023-02-19 11:39:08.772028 postgrest-0.10.6/postgrest/_async/request_builder.py
--rw-r--r--   0        0        0       35 2023-02-19 11:04:33.000000 postgrest-0.10.6/postgrest/_sync/__init__.py
--rw-r--r--   0        0        0     3025 2023-02-19 11:39:08.772136 postgrest-0.10.6/postgrest/_sync/client.py
--rw-r--r--   0        0        0    11593 2023-02-19 11:39:08.772430 postgrest-0.10.6/postgrest/_sync/request_builder.py
--rw-r--r--   0        0        0     1918 2022-10-10 16:43:48.422100 postgrest-0.10.6/postgrest/base_client.py
--rw-r--r--   0        0        0    15329 2023-02-19 11:39:08.772617 postgrest-0.10.6/postgrest/base_request_builder.py
--rw-r--r--   0        0        0      151 2022-10-10 16:43:48.422290 postgrest-0.10.6/postgrest/constants.py
--rw-r--r--   0        0        0      409 2022-10-10 16:43:48.422359 postgrest-0.10.6/postgrest/deprecated_client.py
--rw-r--r--   0        0        0      422 2022-10-10 16:43:48.422431 postgrest-0.10.6/postgrest/deprecated_get_request_builder.py
--rw-r--r--   0        0        0     1510 2023-02-19 11:39:08.772778 postgrest-0.10.6/postgrest/exceptions.py
--rw-r--r--   0        0        0      874 2023-01-26 01:37:52.113883 postgrest-0.10.6/postgrest/types.py
--rw-r--r--   0        0        0      551 2023-02-26 14:47:14.689338 postgrest-0.10.6/postgrest/utils.py
--rw-r--r--   0        0        0     1701 2023-02-26 14:47:28.287476 postgrest-0.10.6/pyproject.toml
--rw-r--r--   0        0        0     5058 1970-01-01 00:00:00.000000 postgrest-0.10.6/setup.py
--rw-r--r--   0        0        0     5132 1970-01-01 00:00:00.000000 postgrest-0.10.6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-08-04 08:05:21.633151 postgrest-0.10.7/LICENSE
+-rw-r--r--   0        0        0     4078 2023-08-04 08:05:21.633343 postgrest-0.10.7/README.md
+-rw-r--r--   0        0        0      742 2023-08-04 08:05:48.500205 postgrest-0.10.7/postgrest/__init__.py
+-rw-r--r--   0        0        0       35 2023-08-04 08:05:21.635697 postgrest-0.10.7/postgrest/_async/__init__.py
+-rw-r--r--   0        0        0     3077 2023-08-04 08:05:21.635798 postgrest-0.10.7/postgrest/_async/client.py
+-rw-r--r--   0        0        0    11429 2023-08-04 08:05:21.635882 postgrest-0.10.7/postgrest/_async/request_builder.py
+-rw-r--r--   0        0        0       35 2023-08-04 08:05:21.635982 postgrest-0.10.7/postgrest/_sync/__init__.py
+-rw-r--r--   0        0        0     3025 2023-08-04 08:05:21.636061 postgrest-0.10.7/postgrest/_sync/client.py
+-rw-r--r--   0        0        0    11360 2023-08-04 08:05:21.636127 postgrest-0.10.7/postgrest/_sync/request_builder.py
+-rw-r--r--   0        0        0     1918 2023-08-04 08:05:21.636200 postgrest-0.10.7/postgrest/base_client.py
+-rw-r--r--   0        0        0    15948 2023-08-04 08:05:21.636400 postgrest-0.10.7/postgrest/base_request_builder.py
+-rw-r--r--   0        0        0      151 2023-08-04 08:05:21.636462 postgrest-0.10.7/postgrest/constants.py
+-rw-r--r--   0        0        0      409 2023-08-04 08:05:21.636522 postgrest-0.10.7/postgrest/deprecated_client.py
+-rw-r--r--   0        0        0      422 2023-08-04 08:05:21.636621 postgrest-0.10.7/postgrest/deprecated_get_request_builder.py
+-rw-r--r--   0        0        0     1510 2023-08-04 08:05:21.636685 postgrest-0.10.7/postgrest/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:05:21.636708 postgrest-0.10.7/postgrest/py.typed
+-rw-r--r--   0        0        0      874 2023-08-04 08:05:21.636797 postgrest-0.10.7/postgrest/types.py
+-rw-r--r--   0        0        0      551 2023-08-04 08:05:21.636855 postgrest-0.10.7/postgrest/utils.py
+-rw-r--r--   0        0        0     1707 2023-08-04 08:05:54.794117 postgrest-0.10.7/pyproject.toml
+-rw-r--r--   0        0        0     5082 1970-01-01 00:00:00.000000 postgrest-0.10.7/PKG-INFO
```

### Comparing `postgrest-0.10.6/LICENSE` & `postgrest-0.10.7/LICENSE`

 * *Files identical despite different names*

### Comparing `postgrest-0.10.6/README.md` & `postgrest-0.10.7/README.md`

 * *Files identical despite different names*

### Comparing `postgrest-0.10.6/postgrest/__init__.py` & `postgrest-0.10.7/postgrest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "0.10.6"
+__version__ = "0.10.7"
 
 from httpx import Timeout
 
 from ._async.client import AsyncPostgrestClient
 from ._async.request_builder import (
     AsyncFilterRequestBuilder,
     AsyncQueryRequestBuilder,
```

### Comparing `postgrest-0.10.6/postgrest/_async/client.py` & `postgrest-0.10.7/postgrest/_async/client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.10.6/postgrest/_async/request_builder.py` & `postgrest-0.10.7/postgrest/_sync/request_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,47 +16,47 @@
     pre_insert,
     pre_select,
     pre_update,
     pre_upsert,
 )
 from ..exceptions import APIError, generate_default_error_message
 from ..types import ReturnMethod
-from ..utils import AsyncClient
+from ..utils import SyncClient
 
 
-class AsyncQueryRequestBuilder:
+class SyncQueryRequestBuilder:
     def __init__(
         self,
-        session: AsyncClient,
+        session: SyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         self.session = session
         self.path = path
         self.http_method = http_method
         self.headers = headers
         self.params = params
         self.json = json
 
-    async def execute(self) -> APIResponse:
+    def execute(self) -> APIResponse:
         """Execute the query.
 
         .. tip::
             This is the last method called, after the query is built.
 
         Returns:
             :class:`APIResponse`
 
         Raises:
             :class:`APIError` If the API raised an error.
         """
-        r = await self.session.request(
+        r = self.session.request(
             self.http_method,
             self.path,
             json=self.json,
             params=self.params,
             headers=self.headers,
         )
         try:
@@ -68,44 +68,44 @@
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
         except JSONDecodeError as e:
             raise APIError(generate_default_error_message(r))
 
 
-class AsyncSingleRequestBuilder:
+class SyncSingleRequestBuilder:
     def __init__(
         self,
-        session: AsyncClient,
+        session: SyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         self.session = session
         self.path = path
         self.http_method = http_method
         self.headers = headers
         self.params = params
         self.json = json
 
-    async def execute(self) -> SingleAPIResponse:
+    def execute(self) -> SingleAPIResponse:
         """Execute the query.
 
         .. tip::
             This is the last method called, after the query is built.
 
         Returns:
             :class:`SingleAPIResponse`
 
         Raises:
             :class:`APIError` If the API raised an error.
         """
-        r = await self.session.request(
+        r = self.session.request(
             self.http_method,
             self.path,
             json=self.json,
             params=self.params,
             headers=self.headers,
         )
         try:
@@ -117,156 +117,150 @@
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
         except JSONDecodeError as e:
             raise APIError(generate_default_error_message(r))
 
 
-class AsyncMaybeSingleRequestBuilder(AsyncSingleRequestBuilder):
-    async def execute(self) -> SingleAPIResponse:
+class SyncMaybeSingleRequestBuilder(SyncSingleRequestBuilder):
+    def execute(self) -> Optional[SingleAPIResponse]:
         r = None
         try:
-            r = await super().execute()
+            r = super().execute()
         except APIError as e:
             if e.details and "Results contain 0 rows" in e.details:
-                return SingleAPIResponse.from_dict(
-                    {
-                        "data": None,
-                        "error": None,
-                        "count": 0,  # NOTE: needs to take value from res.count
-                    }
-                )
+                return None
         if not r:
             raise APIError(
                 {
                     "message": "Missing response",
                     "code": "204",
                     "hint": "Please check traceback of the code",
                     "details": "Postgrest couldn't retrieve response, please check traceback of the code. Please create an issue in `supabase-community/postgrest-py` if needed.",
                 }
             )
         return r
 
 
 # ignoring type checking as a workaround for https://github.com/python/mypy/issues/9319
-class AsyncFilterRequestBuilder(BaseFilterRequestBuilder, AsyncQueryRequestBuilder):  # type: ignore
+class SyncFilterRequestBuilder(BaseFilterRequestBuilder, SyncQueryRequestBuilder):  # type: ignore
     def __init__(
         self,
-        session: AsyncClient,
+        session: SyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         BaseFilterRequestBuilder.__init__(self, session, headers, params)
-        AsyncQueryRequestBuilder.__init__(
+        SyncQueryRequestBuilder.__init__(
             self, session, path, http_method, headers, params, json
         )
 
 
 # ignoring type checking as a workaround for https://github.com/python/mypy/issues/9319
-class AsyncSelectRequestBuilder(BaseSelectRequestBuilder, AsyncQueryRequestBuilder):  # type: ignore
+class SyncSelectRequestBuilder(BaseSelectRequestBuilder, SyncQueryRequestBuilder):  # type: ignore
     def __init__(
         self,
-        session: AsyncClient,
+        session: SyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         BaseSelectRequestBuilder.__init__(self, session, headers, params)
-        AsyncQueryRequestBuilder.__init__(
+        SyncQueryRequestBuilder.__init__(
             self, session, path, http_method, headers, params, json
         )
 
-    def single(self) -> AsyncSingleRequestBuilder:
+    def single(self) -> SyncSingleRequestBuilder:
         """Specify that the query will only return a single row in response.
 
         .. caution::
             The API will raise an error if the query returned more than one row.
         """
         self.headers["Accept"] = "application/vnd.pgrst.object+json"
-        return AsyncSingleRequestBuilder(
+        return SyncSingleRequestBuilder(
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
-    def maybe_single(self) -> AsyncMaybeSingleRequestBuilder:
+    def maybe_single(self) -> SyncMaybeSingleRequestBuilder:
         """Retrieves at most one row from the result. Result must be at most one row (e.g. using `eq` on a UNIQUE column), otherwise this will result in an error."""
         self.headers["Accept"] = "application/vnd.pgrst.object+json"
-        return AsyncMaybeSingleRequestBuilder(
+        return SyncMaybeSingleRequestBuilder(
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
     def text_search(
         self, column: str, query: str, options: Dict[str, any] = {}
-    ) -> AsyncFilterRequestBuilder:
+    ) -> SyncFilterRequestBuilder:
         type_ = options.get("type")
         type_part = ""
         if type_ == "plain":
             type_part = "pl"
         elif type_ == "phrase":
             type_part = "ph"
         elif type_ == "web_search":
             type_part = "w"
         config_part = f"({options.get('config')})" if options.get("config") else ""
         self.params = self.params.add(column, f"{type_part}fts{config_part}.{query}")
 
-        return AsyncQueryRequestBuilder(
+        return SyncQueryRequestBuilder(
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
 
-class AsyncRequestBuilder:
-    def __init__(self, session: AsyncClient, path: str) -> None:
+class SyncRequestBuilder:
+    def __init__(self, session: SyncClient, path: str) -> None:
         self.session = session
         self.path = path
 
     def select(
         self,
         *columns: str,
         count: Optional[CountMethod] = None,
-    ) -> AsyncSelectRequestBuilder:
+    ) -> SyncSelectRequestBuilder:
         """Run a SELECT query.
 
         Args:
             *columns: The names of the columns to fetch.
             count: The method to use to get the count of rows returned.
         Returns:
             :class:`AsyncSelectRequestBuilder`
         """
         method, params, headers, json = pre_select(*columns, count=count)
-        return AsyncSelectRequestBuilder(
+        return SyncSelectRequestBuilder(
             self.session, self.path, method, headers, params, json
         )
 
     def insert(
         self,
         json: Union[dict, list],
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
         upsert: bool = False,
-    ) -> AsyncQueryRequestBuilder:
+    ) -> SyncQueryRequestBuilder:
         """Run an INSERT query.
 
         Args:
             json: The row to be inserted.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
             upsert: Whether the query should be an upsert.
@@ -275,27 +269,27 @@
         """
         method, params, headers, json = pre_insert(
             json,
             count=count,
             returning=returning,
             upsert=upsert,
         )
-        return AsyncQueryRequestBuilder(
+        return SyncQueryRequestBuilder(
             self.session, self.path, method, headers, params, json
         )
 
     def upsert(
         self,
         json: dict,
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
         ignore_duplicates: bool = False,
         on_conflict: str = "",
-    ) -> AsyncQueryRequestBuilder:
+    ) -> SyncQueryRequestBuilder:
         """Run an upsert (INSERT ... ON CONFLICT DO UPDATE) query.
 
         Args:
             json: The row to be inserted.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
             ignore_duplicates: Whether duplicate rows should be ignored.
@@ -306,60 +300,60 @@
         method, params, headers, json = pre_upsert(
             json,
             count=count,
             returning=returning,
             ignore_duplicates=ignore_duplicates,
             on_conflict=on_conflict,
         )
-        return AsyncQueryRequestBuilder(
+        return SyncQueryRequestBuilder(
             self.session, self.path, method, headers, params, json
         )
 
     def update(
         self,
         json: dict,
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
-    ) -> AsyncFilterRequestBuilder:
+    ) -> SyncFilterRequestBuilder:
         """Run an UPDATE query.
 
         Args:
             json: The updated fields.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
         Returns:
             :class:`AsyncFilterRequestBuilder`
         """
         method, params, headers, json = pre_update(
             json,
             count=count,
             returning=returning,
         )
-        return AsyncFilterRequestBuilder(
+        return SyncFilterRequestBuilder(
             self.session, self.path, method, headers, params, json
         )
 
     def delete(
         self,
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
-    ) -> AsyncFilterRequestBuilder:
+    ) -> SyncFilterRequestBuilder:
         """Run a DELETE query.
 
         Args:
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
         Returns:
             :class:`AsyncFilterRequestBuilder`
         """
         method, params, headers, json = pre_delete(
             count=count,
             returning=returning,
         )
-        return AsyncFilterRequestBuilder(
+        return SyncFilterRequestBuilder(
             self.session, self.path, method, headers, params, json
         )
 
     def stub(self):
         return None
```

### Comparing `postgrest-0.10.6/postgrest/_sync/client.py` & `postgrest-0.10.7/postgrest/_sync/client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.10.6/postgrest/_sync/request_builder.py` & `postgrest-0.10.7/postgrest/_async/request_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,47 +16,47 @@
     pre_insert,
     pre_select,
     pre_update,
     pre_upsert,
 )
 from ..exceptions import APIError, generate_default_error_message
 from ..types import ReturnMethod
-from ..utils import SyncClient
+from ..utils import AsyncClient
 
 
-class SyncQueryRequestBuilder:
+class AsyncQueryRequestBuilder:
     def __init__(
         self,
-        session: SyncClient,
+        session: AsyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         self.session = session
         self.path = path
         self.http_method = http_method
         self.headers = headers
         self.params = params
         self.json = json
 
-    def execute(self) -> APIResponse:
+    async def execute(self) -> APIResponse:
         """Execute the query.
 
         .. tip::
             This is the last method called, after the query is built.
 
         Returns:
             :class:`APIResponse`
 
         Raises:
             :class:`APIError` If the API raised an error.
         """
-        r = self.session.request(
+        r = await self.session.request(
             self.http_method,
             self.path,
             json=self.json,
             params=self.params,
             headers=self.headers,
         )
         try:
@@ -68,44 +68,44 @@
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
         except JSONDecodeError as e:
             raise APIError(generate_default_error_message(r))
 
 
-class SyncSingleRequestBuilder:
+class AsyncSingleRequestBuilder:
     def __init__(
         self,
-        session: SyncClient,
+        session: AsyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         self.session = session
         self.path = path
         self.http_method = http_method
         self.headers = headers
         self.params = params
         self.json = json
 
-    def execute(self) -> SingleAPIResponse:
+    async def execute(self) -> SingleAPIResponse:
         """Execute the query.
 
         .. tip::
             This is the last method called, after the query is built.
 
         Returns:
             :class:`SingleAPIResponse`
 
         Raises:
             :class:`APIError` If the API raised an error.
         """
-        r = self.session.request(
+        r = await self.session.request(
             self.http_method,
             self.path,
             json=self.json,
             params=self.params,
             headers=self.headers,
         )
         try:
@@ -117,156 +117,150 @@
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
         except JSONDecodeError as e:
             raise APIError(generate_default_error_message(r))
 
 
-class SyncMaybeSingleRequestBuilder(SyncSingleRequestBuilder):
-    def execute(self) -> SingleAPIResponse:
+class AsyncMaybeSingleRequestBuilder(AsyncSingleRequestBuilder):
+    async def execute(self) -> Optional[SingleAPIResponse]:
         r = None
         try:
-            r = super().execute()
+            r = await super().execute()
         except APIError as e:
             if e.details and "Results contain 0 rows" in e.details:
-                return SingleAPIResponse.from_dict(
-                    {
-                        "data": None,
-                        "error": None,
-                        "count": 0,  # NOTE: needs to take value from res.count
-                    }
-                )
+                return None
         if not r:
             raise APIError(
                 {
                     "message": "Missing response",
                     "code": "204",
                     "hint": "Please check traceback of the code",
                     "details": "Postgrest couldn't retrieve response, please check traceback of the code. Please create an issue in `supabase-community/postgrest-py` if needed.",
                 }
             )
         return r
 
 
 # ignoring type checking as a workaround for https://github.com/python/mypy/issues/9319
-class SyncFilterRequestBuilder(BaseFilterRequestBuilder, SyncQueryRequestBuilder):  # type: ignore
+class AsyncFilterRequestBuilder(BaseFilterRequestBuilder, AsyncQueryRequestBuilder):  # type: ignore
     def __init__(
         self,
-        session: SyncClient,
+        session: AsyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         BaseFilterRequestBuilder.__init__(self, session, headers, params)
-        SyncQueryRequestBuilder.__init__(
+        AsyncQueryRequestBuilder.__init__(
             self, session, path, http_method, headers, params, json
         )
 
 
 # ignoring type checking as a workaround for https://github.com/python/mypy/issues/9319
-class SyncSelectRequestBuilder(BaseSelectRequestBuilder, SyncQueryRequestBuilder):  # type: ignore
+class AsyncSelectRequestBuilder(BaseSelectRequestBuilder, AsyncQueryRequestBuilder):  # type: ignore
     def __init__(
         self,
-        session: SyncClient,
+        session: AsyncClient,
         path: str,
         http_method: str,
         headers: Headers,
         params: QueryParams,
         json: dict,
     ) -> None:
         BaseSelectRequestBuilder.__init__(self, session, headers, params)
-        SyncQueryRequestBuilder.__init__(
+        AsyncQueryRequestBuilder.__init__(
             self, session, path, http_method, headers, params, json
         )
 
-    def single(self) -> SyncSingleRequestBuilder:
+    def single(self) -> AsyncSingleRequestBuilder:
         """Specify that the query will only return a single row in response.
 
         .. caution::
             The API will raise an error if the query returned more than one row.
         """
         self.headers["Accept"] = "application/vnd.pgrst.object+json"
-        return SyncSingleRequestBuilder(
+        return AsyncSingleRequestBuilder(
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
-    def maybe_single(self) -> SyncMaybeSingleRequestBuilder:
+    def maybe_single(self) -> AsyncMaybeSingleRequestBuilder:
         """Retrieves at most one row from the result. Result must be at most one row (e.g. using `eq` on a UNIQUE column), otherwise this will result in an error."""
         self.headers["Accept"] = "application/vnd.pgrst.object+json"
-        return SyncMaybeSingleRequestBuilder(
+        return AsyncMaybeSingleRequestBuilder(
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
     def text_search(
         self, column: str, query: str, options: Dict[str, any] = {}
-    ) -> SyncFilterRequestBuilder:
+    ) -> AsyncFilterRequestBuilder:
         type_ = options.get("type")
         type_part = ""
         if type_ == "plain":
             type_part = "pl"
         elif type_ == "phrase":
             type_part = "ph"
         elif type_ == "web_search":
             type_part = "w"
         config_part = f"({options.get('config')})" if options.get("config") else ""
         self.params = self.params.add(column, f"{type_part}fts{config_part}.{query}")
 
-        return SyncQueryRequestBuilder(
+        return AsyncQueryRequestBuilder(
             headers=self.headers,
             http_method=self.http_method,
             json=self.json,
             params=self.params,
             path=self.path,
             session=self.session,  # type: ignore
         )
 
 
-class SyncRequestBuilder:
-    def __init__(self, session: SyncClient, path: str) -> None:
+class AsyncRequestBuilder:
+    def __init__(self, session: AsyncClient, path: str) -> None:
         self.session = session
         self.path = path
 
     def select(
         self,
         *columns: str,
         count: Optional[CountMethod] = None,
-    ) -> SyncSelectRequestBuilder:
+    ) -> AsyncSelectRequestBuilder:
         """Run a SELECT query.
 
         Args:
             *columns: The names of the columns to fetch.
             count: The method to use to get the count of rows returned.
         Returns:
             :class:`AsyncSelectRequestBuilder`
         """
         method, params, headers, json = pre_select(*columns, count=count)
-        return SyncSelectRequestBuilder(
+        return AsyncSelectRequestBuilder(
             self.session, self.path, method, headers, params, json
         )
 
     def insert(
         self,
         json: Union[dict, list],
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
         upsert: bool = False,
-    ) -> SyncQueryRequestBuilder:
+    ) -> AsyncQueryRequestBuilder:
         """Run an INSERT query.
 
         Args:
             json: The row to be inserted.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
             upsert: Whether the query should be an upsert.
@@ -275,27 +269,27 @@
         """
         method, params, headers, json = pre_insert(
             json,
             count=count,
             returning=returning,
             upsert=upsert,
         )
-        return SyncQueryRequestBuilder(
+        return AsyncQueryRequestBuilder(
             self.session, self.path, method, headers, params, json
         )
 
     def upsert(
         self,
         json: dict,
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
         ignore_duplicates: bool = False,
         on_conflict: str = "",
-    ) -> SyncQueryRequestBuilder:
+    ) -> AsyncQueryRequestBuilder:
         """Run an upsert (INSERT ... ON CONFLICT DO UPDATE) query.
 
         Args:
             json: The row to be inserted.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
             ignore_duplicates: Whether duplicate rows should be ignored.
@@ -306,60 +300,60 @@
         method, params, headers, json = pre_upsert(
             json,
             count=count,
             returning=returning,
             ignore_duplicates=ignore_duplicates,
             on_conflict=on_conflict,
         )
-        return SyncQueryRequestBuilder(
+        return AsyncQueryRequestBuilder(
             self.session, self.path, method, headers, params, json
         )
 
     def update(
         self,
         json: dict,
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
-    ) -> SyncFilterRequestBuilder:
+    ) -> AsyncFilterRequestBuilder:
         """Run an UPDATE query.
 
         Args:
             json: The updated fields.
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
         Returns:
             :class:`AsyncFilterRequestBuilder`
         """
         method, params, headers, json = pre_update(
             json,
             count=count,
             returning=returning,
         )
-        return SyncFilterRequestBuilder(
+        return AsyncFilterRequestBuilder(
             self.session, self.path, method, headers, params, json
         )
 
     def delete(
         self,
         *,
         count: Optional[CountMethod] = None,
         returning: ReturnMethod = ReturnMethod.representation,
-    ) -> SyncFilterRequestBuilder:
+    ) -> AsyncFilterRequestBuilder:
         """Run a DELETE query.
 
         Args:
             count: The method to use to get the count of rows returned.
             returning: Either 'minimal' or 'representation'
         Returns:
             :class:`AsyncFilterRequestBuilder`
         """
         method, params, headers, json = pre_delete(
             count=count,
             returning=returning,
         )
-        return SyncFilterRequestBuilder(
+        return AsyncFilterRequestBuilder(
             self.session, self.path, method, headers, params, json
         )
 
     def stub(self):
         return None
```

### Comparing `postgrest-0.10.6/postgrest/base_client.py` & `postgrest-0.10.7/postgrest/base_client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.10.6/postgrest/base_request_builder.py` & `postgrest-0.10.7/postgrest/base_request_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Type,
     TypeVar,
     Union,
 )
 
 from httpx import Headers, QueryParams
 from httpx import Response as RequestResponse
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 
 from .types import CountMethod, Filters, RequestMethod, ReturnMethod
 from .utils import AsyncClient, SyncClient, sanitize_param
 
 
 class QueryArgs(NamedTuple):
     # groups the method, json, headers and params for a query in a single object
@@ -109,15 +109,15 @@
 
 class APIResponse(BaseModel):
     data: List[Dict[str, Any]]
     """The data returned by the query."""
     count: Optional[int] = None
     """The number of rows returned."""
 
-    @validator("data")
+    @field_validator("data")
     @classmethod
     def raise_when_api_error(cls: Type[APIResponse], value: Any) -> Any:
         if isinstance(value, dict) and value.get("message"):
             raise ValueError("You are passing an API error to the data field.")
         return value
 
     @staticmethod
@@ -398,14 +398,33 @@
         self,
         session: Union[AsyncClient, SyncClient],
         headers: Headers,
         params: QueryParams,
     ) -> None:
         BaseFilterRequestBuilder.__init__(self, session, headers, params)
 
+    def explain(
+        self: _FilterT,
+        analyze: bool = False,
+        verbose: bool = False,
+        settings: bool = False,
+        buffers: bool = False,
+        wal: bool = False,
+        format: str = "",
+    ) -> _FilterT:
+        options = [
+            key
+            for key, value in locals().items()
+            if key not in ["self", "format"] and value
+        ]
+        options_str = "|".join(options)
+        options_str = f'options="{options_str};"' if options_str else ""
+        self.headers["Accept"] = f"application/vnd.pgrst.plan+{format}; {options_str}"
+        return self
+
     def order(
         self: _FilterT,
         column: str,
         *,
         desc: bool = False,
         nullsfirst: bool = False,
         foreign_table: Optional[str] = None,
```

### Comparing `postgrest-0.10.6/postgrest/exceptions.py` & `postgrest-0.10.7/postgrest/exceptions.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.10.6/postgrest/types.py` & `postgrest-0.10.7/postgrest/types.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.10.6/postgrest/utils.py` & `postgrest-0.10.7/postgrest/utils.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.10.6/pyproject.toml` & `postgrest-0.10.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgrest"
-version = "0.10.6"
+version = "0.10.7"
 description = "PostgREST client for Python. This library provides an ORM interface to PostgREST."
 authors = ["Lương Quang Mạnh <luongquangmanh85@gmail.com>", "Joel Lee <joel@joellee.org>", "Anand"]
 homepage = "https://github.com/supabase-community/postgrest-py"
 repository = "https://github.com/supabase-community/postgrest-py"
 documentation = "https://postgrest-py.rtfd.io"
 readme = "README.md"
 license = "MIT"
@@ -17,30 +17,30 @@
     { include = "postgrest" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = "^0.23.0"
 deprecation = "^2.1.0"
-pydantic = "^1.9.0"
+pydantic = ">=2.1.0,<3.0"
 strenum = "^0.4.9"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.3"
-Sphinx = "^6.1.3"
+pytest = "^7.3.2"
+Sphinx = "^7.1.2"
 flake8 = "^5.0.4"
-black = "^23.1"
+black = "^23.3"
 isort = "^5.12.0"
-pre-commit = "^3.1.0"
+pre-commit = "^3.3.3"
 pytest-cov = "^4.0.0"
 pytest-depends = "^1.0.1"
 pytest-asyncio = "^0.18.3"
 unasync-cli = "^0.0.9"
-python-semantic-release = "^7.32.1"
-furo = "^2022.12.7"
+python-semantic-release = "^7.34.6"
+furo = "^2023.5.20"
 
 [tool.semantic_release]
 version_variable = "postgrest/__init__.py:__version__"
 version_toml = "pyproject.toml:tool.poetry.version"
 major_on_zero = false
 commit_subject = "chore(release): bump version to v{version}"
 build_command = "curl -sSL https://install.python-poetry.org | python - && export PATH=\"/github/home/.local/bin:$PATH\" && poetry install && poetry build"
```

### Comparing `postgrest-0.10.6/setup.py` & `postgrest-0.10.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,148 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: postgrest
+Version: 0.10.7
+Summary: PostgREST client for Python. This library provides an ORM interface to PostgREST.
+Home-page: https://github.com/supabase-community/postgrest-py
+License: MIT
+Author: Lương Quang Mạnh
+Author-email: luongquangmanh85@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: deprecation (>=2.1.0,<3.0.0)
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: pydantic (>=2.1.0,<3.0)
+Requires-Dist: strenum (>=0.4.9,<0.5.0)
+Project-URL: Documentation, https://postgrest-py.rtfd.io
+Project-URL: Repository, https://github.com/supabase-community/postgrest-py
+Description-Content-Type: text/markdown
 
-packages = \
-['postgrest', 'postgrest._async', 'postgrest._sync']
+# postgrest-py
 
-package_data = \
-{'': ['*']}
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?label=license)](https://opensource.org/licenses/MIT)
+[![CI](https://github.com/supabase-community/postgrest-py/actions/workflows/ci.yml/badge.svg)](https://github.com/supabase-community/postgrest-py/actions/workflows/ci.yml)
+[![Python](https://img.shields.io/pypi/pyversions/postgrest-py)](https://pypi.org/project/postgrest-py)
+[![Version](https://img.shields.io/pypi/v/postgrest-py?color=%2334D058)](https://pypi.org/project/postgrest-py)
+[![Codecov](https://codecov.io/gh/supabase-community/postgrest-py/branch/master/graph/badge.svg)](https://codecov.io/gh/supabase-community/postgrest-py)
+[![Last commit](https://img.shields.io/github/last-commit/supabase-community/postgrest-py.svg?style=flat)](https://github.com/supabase-community/postgrest-py/commits)
+[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/supabase-community/postgrest-py)](https://github.com/supabase-community/postgrest-py/commits)
+[![Github Stars](https://img.shields.io/github/stars/supabase-community/postgrest-py?style=flat&logo=github)](https://github.com/supabase-community/postgrest-py/stargazers)
+[![Github Forks](https://img.shields.io/github/forks/supabase-community/postgrest-py?style=flat&logo=github)](https://github.com/supabase-community/postgrest-py/network/members)
+[![Github Watchers](https://img.shields.io/github/watchers/supabase-community/postgrest-py?style=flat&logo=github)](https://github.com/supabase-community/postgrest-py)
+[![GitHub contributors](https://img.shields.io/github/contributors/supabase-community/postgrest-py)](https://github.com/supabase-community/postgrest-py/graphs/contributors)
 
-install_requires = \
-['deprecation>=2.1.0,<3.0.0',
- 'httpx>=0.23.0,<0.24.0',
- 'pydantic>=1.9.0,<2.0.0',
- 'strenum>=0.4.9,<0.5.0']
-
-setup_kwargs = {
-    'name': 'postgrest',
-    'version': '0.10.6',
-    'description': 'PostgREST client for Python. This library provides an ORM interface to PostgREST.',
-    'long_description': '# postgrest-py\n\n[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?label=license)](https://opensource.org/licenses/MIT)\n[![CI](https://github.com/supabase-community/postgrest-py/actions/workflows/ci.yml/badge.svg)](https://github.com/supabase-community/postgrest-py/actions/workflows/ci.yml)\n[![Python](https://img.shields.io/pypi/pyversions/postgrest-py)](https://pypi.org/project/postgrest-py)\n[![Version](https://img.shields.io/pypi/v/postgrest-py?color=%2334D058)](https://pypi.org/project/postgrest-py)\n[![Codecov](https://codecov.io/gh/supabase-community/postgrest-py/branch/master/graph/badge.svg)](https://codecov.io/gh/supabase-community/postgrest-py)\n[![Last commit](https://img.shields.io/github/last-commit/supabase-community/postgrest-py.svg?style=flat)](https://github.com/supabase-community/postgrest-py/commits)\n[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/supabase-community/postgrest-py)](https://github.com/supabase-community/postgrest-py/commits)\n[![Github Stars](https://img.shields.io/github/stars/supabase-community/postgrest-py?style=flat&logo=github)](https://github.com/supabase-community/postgrest-py/stargazers)\n[![Github Forks](https://img.shields.io/github/forks/supabase-community/postgrest-py?style=flat&logo=github)](https://github.com/supabase-community/postgrest-py/network/members)\n[![Github Watchers](https://img.shields.io/github/watchers/supabase-community/postgrest-py?style=flat&logo=github)](https://github.com/supabase-community/postgrest-py)\n[![GitHub contributors](https://img.shields.io/github/contributors/supabase-community/postgrest-py)](https://github.com/supabase-community/postgrest-py/graphs/contributors)\n\nPostgREST client for Python. This library provides an ORM interface to PostgREST.\n\nStatus: **Unstable**\n\n## INSTALLATION\n\n### Requirements\n\n- Python >= 3.7\n- PostgreSQL >= 12\n- PostgREST >= 7\n\n### Local PostgREST server\n\nIf you want to use a local PostgREST server for development, you can use our preconfigured instance via Docker Compose.\n\n```sh\ndocker-compose up\n```\n\nOnce Docker Compose started, PostgREST is accessible at <http://localhost:3000>.\n\n### Instructions\n\n#### With Poetry (recommended)\n\n```sh\npoetry add postgrest\n```\n\n#### With Pip\n\n```sh\npip install postgrest\n```\n\n## USAGE\n\n### Getting started\n\n```py\nimport asyncio\nfrom postgrest import AsyncPostgrestClient\n\nasync def main():\n    async with AsyncPostgrestClient("http://localhost:3000") as client:\n        r = await client.from_("countries").select("*").execute()\n        countries = r.data\n\nasyncio.run(main())\n```\n\n### Create\n\n```py\nawait client.from_("countries").insert({ "name": "Việt Nam", "capital": "Hà Nội" }).execute()\n```\n\n### Read\n\n```py\nr = await client.from_("countries").select("id", "name").execute()\ncountries = r.data\n```\n\n### Update\n\n```py\nawait client.from_("countries").update({"capital": "Hà Nội"}).eq("name", "Việt Nam").execute()\n```\n\n### Delete\n\n```py\nawait client.from_("countries").delete().eq("name", "Việt Nam").execute()\n```\n\n### General filters\n\n### Stored procedures (RPC)\n```py\nawait client.rpc("foobar", {"arg1": "value1", "arg2": "value2"}).execute()\n```\n\n## DEVELOPMENT\n\n```sh\ngit clone https://github.com/supabase/postgrest-py.git\ncd postgrest-py\npoetry install\npoetry run pre-commit install\n```\n\n### Testing\n\n```sh\npoetry run pytest\n```\n\n## CHANGELOG\n\nRead more [here](https://github.com/supabase/postgrest-py/blob/master/CHANGELOG.md).\n\n## SPONSORS\n\nWe are building the features of Firebase using enterprise-grade, open source products. We support existing communities wherever possible, and if the products don’t exist we build them and open source them ourselves. Thanks to these sponsors who are making the OSS ecosystem better for everyone.\n\n[![Worklife VC](https://user-images.githubusercontent.com/10214025/90451355-34d71200-e11e-11ea-81f9-1592fd1e9146.png)](https://www.worklife.vc)\n[![New Sponsor](https://user-images.githubusercontent.com/10214025/90518111-e74bbb00-e198-11ea-8f88-c9e3c1aa4b5b.png)](https://github.com/sponsors/supabase)\n',
-    'author': 'Lương Quang Mạnh',
-    'author_email': 'luongquangmanh85@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/supabase-community/postgrest-py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+PostgREST client for Python. This library provides an ORM interface to PostgREST.
 
+Status: **Unstable**
+
+## INSTALLATION
+
+### Requirements
+
+- Python >= 3.7
+- PostgreSQL >= 12
+- PostgREST >= 7
+
+### Local PostgREST server
+
+If you want to use a local PostgREST server for development, you can use our preconfigured instance via Docker Compose.
+
+```sh
+docker-compose up
+```
+
+Once Docker Compose started, PostgREST is accessible at <http://localhost:3000>.
+
+### Instructions
+
+#### With Poetry (recommended)
+
+```sh
+poetry add postgrest
+```
+
+#### With Pip
+
+```sh
+pip install postgrest
+```
+
+## USAGE
+
+### Getting started
+
+```py
+import asyncio
+from postgrest import AsyncPostgrestClient
+
+async def main():
+    async with AsyncPostgrestClient("http://localhost:3000") as client:
+        r = await client.from_("countries").select("*").execute()
+        countries = r.data
+
+asyncio.run(main())
+```
+
+### Create
+
+```py
+await client.from_("countries").insert({ "name": "Việt Nam", "capital": "Hà Nội" }).execute()
+```
+
+### Read
+
+```py
+r = await client.from_("countries").select("id", "name").execute()
+countries = r.data
+```
+
+### Update
+
+```py
+await client.from_("countries").update({"capital": "Hà Nội"}).eq("name", "Việt Nam").execute()
+```
+
+### Delete
+
+```py
+await client.from_("countries").delete().eq("name", "Việt Nam").execute()
+```
+
+### General filters
+
+### Stored procedures (RPC)
+```py
+await client.rpc("foobar", {"arg1": "value1", "arg2": "value2"}).execute()
+```
+
+## DEVELOPMENT
+
+```sh
+git clone https://github.com/supabase/postgrest-py.git
+cd postgrest-py
+poetry install
+poetry run pre-commit install
+```
+
+### Testing
+
+```sh
+poetry run pytest
+```
+
+## CHANGELOG
+
+Read more [here](https://github.com/supabase/postgrest-py/blob/master/CHANGELOG.md).
+
+## SPONSORS
+
+We are building the features of Firebase using enterprise-grade, open source products. We support existing communities wherever possible, and if the products don’t exist we build them and open source them ourselves. Thanks to these sponsors who are making the OSS ecosystem better for everyone.
+
+[![Worklife VC](https://user-images.githubusercontent.com/10214025/90451355-34d71200-e11e-11ea-81f9-1592fd1e9146.png)](https://www.worklife.vc)
+[![New Sponsor](https://user-images.githubusercontent.com/10214025/90518111-e74bbb00-e198-11ea-8f88-c9e3c1aa4b5b.png)](https://github.com/sponsors/supabase)
 
-setup(**setup_kwargs)
```

