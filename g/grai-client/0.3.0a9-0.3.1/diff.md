# Comparing `tmp/grai_client-0.3.0a9.tar.gz` & `tmp/grai_client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_client-0.3.0a9.tar", max compression
+gzip compressed data, was "grai_client-0.3.1.tar", max compression
```

## Comparing `grai_client-0.3.0a9.tar` & `grai_client-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      168 2023-05-02 08:01:59.660150 grai_client-0.3.0a9/README.md
--rw-r--r--   0        0        0     1239 2023-06-30 16:51:39.153531 grai_client-0.3.0a9/pyproject.toml
--rw-r--r--   0        0        0      163 2023-06-30 16:51:42.790988 grai_client-0.3.0a9/src/grai_client/__init__.py
--rw-r--r--   0        0        0      643 2023-06-06 17:35:16.716176 grai_client-0.3.0a9/src/grai_client/authentication.py
--rw-r--r--   0        0        0      265 2023-06-06 17:35:16.716588 grai_client-0.3.0a9/src/grai_client/endpoints/__init__.py
--rw-r--r--   0        0        0    24172 2023-06-16 20:34:04.867796 grai_client-0.3.0a9/src/grai_client/endpoints/client.py
--rw-r--r--   0        0        0     1011 2023-06-29 08:12:22.777282 grai_client-0.3.0a9/src/grai_client/endpoints/rest.py
--rw-r--r--   0        0        0     7282 2023-06-29 08:12:22.777420 grai_client-0.3.0a9/src/grai_client/endpoints/utilities.py
--rw-r--r--   0        0        0       82 2023-02-14 12:06:39.058550 grai_client-0.3.0a9/src/grai_client/endpoints/v1/__init__.py
--rw-r--r--   0        0        0     3947 2023-06-29 08:12:22.777559 grai_client-0.3.0a9/src/grai_client/endpoints/v1/client.py
--rw-r--r--   0        0        0     5369 2023-06-29 08:12:22.777848 grai_client-0.3.0a9/src/grai_client/endpoints/v1/delete.py
--rw-r--r--   0        0        0      121 2023-06-29 08:12:22.777953 grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/__init__.py
--rw-r--r--   0        0        0     5904 2023-06-29 08:12:22.778062 grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/edge.py
--rw-r--r--   0        0        0     4895 2023-06-29 08:12:22.778126 grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/node.py
--rw-r--r--   0        0        0      838 2023-06-29 08:12:22.778210 grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/organisation.py
--rw-r--r--   0        0        0     2501 2023-06-29 08:12:22.778290 grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/source.py
--rw-r--r--   0        0        0     1953 2023-06-29 08:12:22.778367 grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/utils.py
--rw-r--r--   0        0        0     2622 2023-06-29 08:12:22.778433 grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/workspace.py
--rw-r--r--   0        0        0     6704 2023-06-29 08:12:22.778569 grai_client-0.3.0a9/src/grai_client/endpoints/v1/patch.py
--rw-r--r--   0        0        0     8301 2023-06-29 08:12:22.778680 grai_client-0.3.0a9/src/grai_client/endpoints/v1/post.py
--rw-r--r--   0        0        0     3167 2023-06-29 08:12:22.778795 grai_client-0.3.0a9/src/grai_client/endpoints/v1/url.py
--rw-r--r--   0        0        0     1102 2023-06-06 17:35:16.717987 grai_client-0.3.0a9/src/grai_client/endpoints/v1/utils.py
--rw-r--r--   0        0        0      307 2023-06-29 08:12:22.778860 grai_client-0.3.0a9/src/grai_client/errors.py
--rw-r--r--   0        0        0       42 2023-06-29 08:12:22.779159 grai_client-0.3.0a9/src/grai_client/integrations/__init__.py
--rw-r--r--   0        0        0     2736 2023-06-30 16:48:31.800558 grai_client-0.3.0a9/src/grai_client/integrations/base.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.059014 grai_client-0.3.0a9/src/grai_client/py.typed
--rw-r--r--   0        0        0       47 2023-06-29 08:12:22.779751 grai_client-0.3.0a9/src/grai_client/schemas/__init__.py
--rw-r--r--   0        0        0     1116 2023-06-29 08:12:22.779918 grai_client-0.3.0a9/src/grai_client/schemas/labels.py
--rw-r--r--   0        0        0      417 2023-06-06 17:35:16.718112 grai_client-0.3.0a9/src/grai_client/schemas/schema.py
--rw-r--r--   0        0        0       39 2023-02-14 12:06:39.059327 grai_client-0.3.0a9/src/grai_client/testing/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-16 16:15:18.411510 grai_client-0.3.0a9/src/grai_client/testing/schema.py
--rw-r--r--   0        0        0     3516 2023-06-29 08:12:22.780091 grai_client-0.3.0a9/src/grai_client/update.py
--rw-r--r--   0        0        0       40 2023-02-14 12:06:39.059522 grai_client-0.3.0a9/src/grai_client/utilities/__init__.py
--rw-r--r--   0        0        0      518 2023-06-06 17:35:16.718665 grai_client-0.3.0a9/src/grai_client/utilities/tests.py
--rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 grai_client-0.3.0a9/PKG-INFO
+-rw-r--r--   0        0        0      168 2023-05-02 08:01:59.660150 grai_client-0.3.1/README.md
+-rw-r--r--   0        0        0     1212 2023-08-04 09:47:34.138681 grai_client-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-08-04 09:47:41.891341 grai_client-0.3.1/src/grai_client/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-06 17:35:16.716176 grai_client-0.3.1/src/grai_client/authentication.py
+-rw-r--r--   0        0        0      265 2023-06-06 17:35:16.716588 grai_client-0.3.1/src/grai_client/endpoints/__init__.py
+-rw-r--r--   0        0        0    21729 2023-07-19 14:07:41.931050 grai_client-0.3.1/src/grai_client/endpoints/client.py
+-rw-r--r--   0        0        0     1011 2023-07-19 14:07:41.931417 grai_client-0.3.1/src/grai_client/endpoints/rest.py
+-rw-r--r--   0        0        0     7446 2023-07-19 14:07:41.931804 grai_client-0.3.1/src/grai_client/endpoints/utilities.py
+-rw-r--r--   0        0        0       82 2023-02-14 12:06:39.058550 grai_client-0.3.1/src/grai_client/endpoints/v1/__init__.py
+-rw-r--r--   0        0        0     7195 2023-07-19 14:07:41.931963 grai_client-0.3.1/src/grai_client/endpoints/v1/client.py
+-rw-r--r--   0        0        0     5369 2023-07-19 14:07:41.932077 grai_client-0.3.1/src/grai_client/endpoints/v1/delete.py
+-rw-r--r--   0        0        0      121 2023-07-19 14:07:41.932162 grai_client-0.3.1/src/grai_client/endpoints/v1/get/__init__.py
+-rw-r--r--   0        0        0     5904 2023-07-19 14:07:41.932257 grai_client-0.3.1/src/grai_client/endpoints/v1/get/edge.py
+-rw-r--r--   0        0        0     4943 2023-07-19 14:07:41.932335 grai_client-0.3.1/src/grai_client/endpoints/v1/get/node.py
+-rw-r--r--   0        0        0     1229 2023-07-19 14:07:41.932616 grai_client-0.3.1/src/grai_client/endpoints/v1/get/organisation.py
+-rw-r--r--   0        0        0     2521 2023-07-19 14:07:41.932710 grai_client-0.3.1/src/grai_client/endpoints/v1/get/source.py
+-rw-r--r--   0        0        0     1953 2023-07-19 14:07:41.932790 grai_client-0.3.1/src/grai_client/endpoints/v1/get/utils.py
+-rw-r--r--   0        0        0     3783 2023-07-19 14:07:41.932875 grai_client-0.3.1/src/grai_client/endpoints/v1/get/workspace.py
+-rw-r--r--   0        0        0     9739 2023-07-17 11:35:54.988484 grai_client-0.3.1/src/grai_client/endpoints/v1/get.py
+-rw-r--r--   0        0        0     6704 2023-07-19 14:07:41.933189 grai_client-0.3.1/src/grai_client/endpoints/v1/patch.py
+-rw-r--r--   0        0        0     8381 2023-07-19 14:07:41.933588 grai_client-0.3.1/src/grai_client/endpoints/v1/post.py
+-rw-r--r--   0        0        0     3167 2023-07-19 14:07:41.933868 grai_client-0.3.1/src/grai_client/endpoints/v1/url.py
+-rw-r--r--   0        0        0     1746 2023-07-19 14:07:41.934143 grai_client-0.3.1/src/grai_client/endpoints/v1/utils.py
+-rw-r--r--   0        0        0      307 2023-07-19 14:07:41.934625 grai_client-0.3.1/src/grai_client/errors.py
+-rw-r--r--   0        0        0       42 2023-07-19 14:07:41.934741 grai_client-0.3.1/src/grai_client/integrations/__init__.py
+-rw-r--r--   0        0        0     3850 2023-08-04 09:47:21.928736 grai_client-0.3.1/src/grai_client/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.059014 grai_client-0.3.1/src/grai_client/py.typed
+-rw-r--r--   0        0        0       47 2023-07-19 14:07:41.934956 grai_client-0.3.1/src/grai_client/schemas/__init__.py
+-rw-r--r--   0        0        0     1217 2023-07-19 14:07:41.935056 grai_client-0.3.1/src/grai_client/schemas/labels.py
+-rw-r--r--   0        0        0      417 2023-06-06 17:35:16.718112 grai_client-0.3.1/src/grai_client/schemas/schema.py
+-rw-r--r--   0        0        0       39 2023-02-14 12:06:39.059327 grai_client-0.3.1/src/grai_client/testing/__init__.py
+-rw-r--r--   0        0        0     3848 2023-07-17 11:35:54.988647 grai_client-0.3.1/src/grai_client/testing/schema.py
+-rw-r--r--   0        0        0     3168 2023-07-19 14:07:41.935162 grai_client-0.3.1/src/grai_client/update.py
+-rw-r--r--   0        0        0       40 2023-02-14 12:06:39.059522 grai_client-0.3.1/src/grai_client/utilities/__init__.py
+-rw-r--r--   0        0        0      518 2023-06-06 17:35:16.718665 grai_client-0.3.1/src/grai_client/utilities/tests.py
+-rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 grai_client-0.3.1/PKG-INFO
```

### Comparing `grai_client-0.3.0a9/pyproject.toml` & `grai_client-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-client"
-version = "0.3.0-alpha9"
+version = "0.3.1"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_client", from = "src" },
 ]
 readme = "README.md"
@@ -13,17 +13,16 @@
 documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 requests = "^2.28.1"
 multimethod = "^1.9"
-orjson = "^3.8.3"
 pyyaml = "^6.0"
-grai-schemas = "^0.2.0a1"
+grai-schemas = "^0.2.0"
 httpx = {extras = ["http2"], version = "^0.24.0"}
 brotli = "^1.0.9"
 tqdm = "^4.65.0"
 more-itertools = "^9.1.0"
 furl = "^2.1.3"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `grai_client-0.3.0a9/src/grai_client/authentication.py` & `grai_client-0.3.1/src/grai_client/authentication.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/client.py` & `grai_client-0.3.1/src/grai_client/endpoints/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import json
 import sys
 import warnings
 from functools import wraps
 from typing import (
     Any,
     Callable,
-    Coroutine,
     Dict,
     Generator,
     Iterable,
     List,
     Literal,
     Optional,
     Sequence,
@@ -19,26 +18,21 @@
     TypeVar,
     Union,
 )
 
 import httpx
 from furl import furl
 from grai_schemas.base import Edge, Node
-from httpx import Auth, BasicAuth, QueryParams, Request, Response
+from httpx import Auth, BasicAuth, QueryParams, Response
 from multimethod import multimethod
 from pydantic import BaseModel, SecretStr
 from tqdm.autonotebook import tqdm
 
 from grai_client.authentication import APIKeyAuth
 from grai_client.endpoints.rest import delete, get, patch, post
-from grai_client.endpoints.utilities import (
-    add_query_params,
-    response_status_check,
-    serialize_obj,
-)
 from grai_client.schemas.schema import GraiType
 
 if sys.version_info < (3, 10):
     from typing_extensions import ParamSpec
 else:
     from typing import ParamSpec
 
@@ -811,109 +805,7 @@
     """
     segmented_patch = segmented_caller(patch)
     result = segmented_patch(client, objs, options)
     return result
 
 
 # -------------------------------------------- #
-
-
-@get.register
-def client_get_url(client: BaseClient, url: str, options: ClientOptions = ClientOptions()) -> Response:
-    """
-
-    Args:
-        client (BaseClient):
-        url (str):
-        options (ClientOptions, optional):  (Default value = ClientOptions())
-
-    Returns:
-
-    Raises:
-
-    """
-    if options.query_args:
-        url = add_query_params(url, options.query_args)
-
-    response = client.session.get(url, headers=options.headers, **options.request_args)
-    response_status_check(response)
-    return response
-
-
-@delete.register
-def client_delete_url(client: BaseClient, url: str, options: ClientOptions = ClientOptions()) -> Response:
-    """
-
-    Args:
-        client (BaseClient):
-        url (str):
-        options (ClientOptions, optional):  (Default value = ClientOptions())
-
-    Returns:
-
-    Raises:
-
-    """
-    response = client.session.delete(url, headers=options.headers, **options.request_args)
-    response_status_check(response)
-    return response
-
-
-@post.register
-def client_post_url(
-    client: BaseClient,
-    url: str,
-    payload: Dict,
-    options: ClientOptions = ClientOptions(),
-) -> Response:
-    """
-
-    Args:
-        client (BaseClient):
-        url (str):
-        payload (Dict):
-        options (ClientOptions, optional):  (Default value = ClientOptions())
-
-    Returns:
-
-    Raises:
-
-    """
-    headers = {
-        "Content-Type": "application/json",
-        **options.headers,
-    }
-    payload = {**payload, **options.payload}
-
-    response = client.session.post(url, content=serialize_obj(payload), headers=headers, **options.request_args)
-
-    response_status_check(response)
-    return response
-
-
-@patch.register
-def client_patch_url(
-    client: BaseClient,
-    url: str,
-    payload: Dict,
-    options: ClientOptions = ClientOptions(),
-) -> Response:
-    """
-
-    Args:
-        client (BaseClient):
-        url (str):
-        payload (Dict):
-        options (ClientOptions, optional):  (Default value = ClientOptions())
-
-    Returns:
-
-    Raises:
-
-    """
-    headers = {"Content-Type": "application/json", **options.headers}
-    payload = {**payload, **options.payload}
-
-    response = client.session.patch(url, content=serialize_obj(payload), headers=headers, **options.request_args)
-
-    response_status_check(response)
-    return response
```

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/rest.py` & `grai_client-0.3.1/src/grai_client/endpoints/rest.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/utilities.py` & `grai_client-0.3.1/src/grai_client/endpoints/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,23 +92,25 @@
     Returns:
 
     Raises:
 
     """
     if resp.status_code in {200, 201, 204}:
         return resp
+    elif resp.status_code == 404:
+        raise ObjectNotFoundError(f"Object not found: {resp.url}")
+    else:
+        message = f"Error: {resp.status_code}. {resp.reason_phrase}. {resp.content.decode()}"
 
-    message = f"Error: {resp.status_code}. {resp.reason_phrase}. {resp.content.decode()}"
     if resp.status_code == 500:
         message = (
             f"{message}"
             "If you think this should not be the case it might be a bug, you can "
             "submit a bug report at https://github.com/grai-io/grai-core/issues"
         )
-
     raise RequestException(message)
 
 
 def orjson_defaults(obj: Any) -> Any:
     """
 
     Args:
@@ -119,15 +121,17 @@
     Raises:
 
     """
     if isinstance(obj, set):
         return list(obj)
     elif isinstance(obj, (pathlib.PosixPath, pathlib.WindowsPath)):
         return str(obj)
-    elif isinstance(obj, (GraiBaseModel, BaseModel)):
+    elif isinstance(obj, GraiBaseModel):
+        return obj.json()
+    elif isinstance(obj, BaseModel):
         return obj.dict()
     else:
         raise Exception(f"No supported JSON serialization format for objects of type {type(obj)}")
 
 
 class GraiEncoder(json.JSONEncoder):
     """Needed for the base python json implementation"""
@@ -295,15 +299,15 @@
     """"""
 
     @wraps(fn)
     def wrapper(*args, **kwargs) -> T:
         result = fn(*args, **kwargs)
         if (num_results := len(result)) == 0:
             missing_message = (
-                f"A request to `{fn.__name__}{tuple(args)}` was marked as expecting a single unique response ."
+                f"A request to `{fn.__name__}{tuple(args)}` was marked as expecting a single unique response. "
                 f"However, no results were returned by the server"
             )
             raise ObjectNotFoundError(missing_message)
         elif num_results == 1:
             return result[0]
         else:
             invalid_message = (
```

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/v1/delete.py` & `grai_client-0.3.1/src/grai_client/endpoints/v1/delete.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/edge.py` & `grai_client-0.3.1/src/grai_client/endpoints/v1/get/edge.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/node.py` & `grai_client-0.3.1/src/grai_client/endpoints/v1/get/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,17 @@
 
 
 # ----- SourcedNode ----- #
 
 
 @get.register
 def get_source_node_by_label_v1(
-    client: ClientV1, grai_type: SourceNodeLabels, options: ClientOptions = ClientOptions()
+    client: ClientV1,
+    grai_type: SourceNodeLabels,
+    options: ClientOptions = ClientOptions(),
 ):
     """
 
     Args:
         client:
         grai_type:
         options:  (Default value = ClientOptions())
@@ -135,15 +137,18 @@
 
     """
     raise NotSupportedError("It's not possible to query for lineage sources without a source id.")
 
 
 @get.register
 def get_source_node_by_label_and_id_v1(
-    client: ClientV1, grai_type: SourceNodeLabels, source_id: Union[str, UUID], options: ClientOptions = ClientOptions()
+    client: ClientV1,
+    grai_type: SourceNodeLabels,
+    source_id: Union[str, UUID],
+    options: ClientOptions = ClientOptions(),
 ) -> List[SourcedNodeV1]:
     """
 
     Args:
         client:
         grai_type:
         source_id:
@@ -154,15 +159,15 @@
     Raises:
 
     """
     if (source_id := validated_uuid(source_id)) is None:
         source: SourceV1 = get_is_unique(client, "Source", name=source_id)
         source_id = source.spec.id
     else:
-        source = get(client, "Source", source_id)
+        source = get(client, "Source", source_id, options=options)
 
     url = client.get_url(grai_type, source_id)
     resp = paginated_get(client, url, options)
 
     for item in resp:
         item["data_source"] = source.spec
     return [source_node_builder(obj) for obj in resp]
@@ -185,15 +190,17 @@
 
     """
     return get(client, grai_type.spec, options)
 
 
 @get.register
 def get_source_node_by_source_node_spec(
-    client: ClientV1, grai_type: SourcedNodeSpec, options: ClientOptions = ClientOptions()
+    client: ClientV1,
+    grai_type: SourcedNodeSpec,
+    options: ClientOptions = ClientOptions(),
 ) -> SourcedNodeV1:
     """
 
     Args:
         client:
         grai_type:
         options:  (Default value = ClientOptions())
```

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/source.py` & `grai_client-0.3.1/src/grai_client/endpoints/v1/get/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,8 +106,8 @@
 
     url = client.get_url(grai_type)
     options = options.copy()
     options.query_args["name"] = grai_type.name
 
     validated_query = expects_unique_query(paginated_get)
     result = validated_query(client, url, options=options)
-    return result
+    return SourceV1.from_spec(result)
```

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/v1/get/utils.py` & `grai_client-0.3.1/src/grai_client/endpoints/v1/get/utils.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/v1/patch.py` & `grai_client-0.3.1/src/grai_client/endpoints/v1/patch.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/v1/post.py` & `grai_client-0.3.1/src/grai_client/endpoints/v1/post.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     """
     result = []
     for source in data_sources:
         if isinstance(source, UUID):
             source_obj = {"id": source}
         elif isinstance(source, SourceSpec):
-            source_obj = source
+            source_obj = {"id": source.id} if source.id else {"name": source.name}
         else:
             raise NotSupportedError(f"Only UUIDs and SourceSpecs are supported not {type(source)}")
 
         result.append(source_obj)
 
     return result
 
@@ -70,15 +70,16 @@
 
     Raises:
 
     """
     url = client.get_url(grai_type)
     payload = grai_type.dict(exclude_none=True)
     payload["data_sources"] = collect_data_sources(grai_type.data_sources)
-    response = post(client, url, payload, options=options)
+    response = post(client, url, payload, options)
+
     return NodeV1.from_spec(response.json())
 
 
 @post.register
 def post_sourced_node_v1(
     client: ClientV1, grai_type: SourcedNodeV1, options: ClientOptions = ClientOptions()
 ) -> SourcedNodeV1:
@@ -280,14 +281,16 @@
             message = (
                 f"The workspace id provided in the source {grai_type} does not match the client's "
                 f"workspace id {client.workspace}."
             )
             raise ValueError(message)
 
     payload = grai_type.dict(exclude_none=True)
+    payload.pop("workspace", None)
+
     response = post(client, url, payload, options=options).json()
     response["workspace"] = client.workspace
     return SourceV1.from_spec(response)
 
 
 @post.register
 def post_source_v1(client: ClientV1, grai_type: SourceV1, options: ClientOptions = ClientOptions()) -> SourceV1:
```

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/v1/url.py` & `grai_client-0.3.1/src/grai_client/endpoints/v1/url.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a9/src/grai_client/endpoints/v1/utils.py` & `grai_client-0.3.1/src/grai_client/endpoints/v1/get/organisation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,54 @@
-from grai_schemas.v1.node import NodeIdTypes
+from typing import Union
+
+from grai_schemas.v1 import OrganisationV1
+from grai_schemas.v1.organization import OrganisationSpec
 
 from grai_client.endpoints.client import ClientOptions
 from grai_client.endpoints.rest import get
 from grai_client.endpoints.v1.client import ClientV1
+from grai_client.errors import NotSupportedError
+from grai_client.schemas.labels import OrganisationLabels
 
 
-def process_node_id(client: ClientV1, grai_type: NodeIdTypes, options: ClientOptions = ClientOptions()) -> NodeIdTypes:
-    """Process a NodeID object, either by returning if it has a known id, or by getting
-    the id from the server.
+@get.register
+def get_organisation_v1(
+    client: ClientV1,
+    grai_type: OrganisationLabels,
+    options: ClientOptions = ClientOptions(),
+):
+    """
 
     Args:
-        client (ClientV1):
-        grai_type (NodeIdTypes):
-        options (ClientOptions, optional):  (Default value = ClientOptions())
+        client:
+        grai_type:
+        options:  (Default value = ClientOptions())
 
     Returns:
 
     Raises:
 
     """
-    if grai_type.id is not None:
-        return grai_type
+    message = "The get organisation endpoint is not supported through the REST API."
+    raise NotSupportedError(message)
+
+
+@get.register
+def get_organisation_v1(
+    client: ClientV1,
+    grai_type: Union[OrganisationV1, OrganisationSpec],
+    options: ClientOptions = ClientOptions(),
+):
+    """
 
-    server_node = get(client, grai_type, options=options)
-    if server_node is None:
-        if grai_type.id is None:
-            message = (
-                f"Could not find node with namespace=`{grai_type.namespace} " f"and name=`{grai_type.name}` on server"
-            )
-        else:
-            message = f"Could not find node with id=`{grai_type.id}`"
-        raise ValueError(message)
+    Args:
+        client:
+        grai_type:
+        options:  (Default value = ClientOptions())
 
-    return server_node.spec
+    Returns:
+
+    Raises:
+
+    """
+    message = "The get organisation endpoint is not supported through the REST API."
+    raise NotSupportedError(message)
```

### Comparing `grai_client-0.3.0a9/src/grai_client/integrations/base.py` & `grai_client-0.3.1/src/grai_client/integrations/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+import sys
 from abc import ABC, abstractmethod
-from typing import List, Optional, ParamSpec, Tuple, Union
+from typing import List, Optional, Tuple, Union
+from uuid import UUID
 
 from grai_schemas.base import Event, SourcedEdge, SourcedNode
 from grai_schemas.v1.source import SourceSpec, SourceV1
 
 from grai_client.endpoints.client import BaseClient
 from grai_client.update import update
 
+if sys.version_info < (3, 10):
+    from typing_extensions import ParamSpec
+else:
+    from typing import ParamSpec
 
-class EventMixin(ABC):
-    def __init__(self):
-        raise NotImplementedError(
-            "The EventMixin is not yet stable or ready for production use."
-        )
 
+class EventMixin(ABC):
     @abstractmethod
     def events(self) -> List[Event]:
         pass
 
     def update(self):
         super().update()
         update(self.client, self.events())
@@ -48,33 +50,64 @@
     def edges(self) -> List[SourcedEdge]:
         pass
 
     @abstractmethod
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
         pass
 
+    @abstractmethod
+    def ready(self) -> bool:
+        pass
+
     @classmethod
     def from_client(
-        cls, client: BaseClient, source_name: str, *args: P.args, **kwargs: P.kwargs
+        cls,
+        client: BaseClient,
+        source: Union[SourceV1, SourceSpec, str, UUID] = None,
+        *args: P.args,
+        **kwargs: P.kwargs,
     ):
         class WithClient(cls):
             client: BaseClient
 
-            def __init__(self, client: BaseClient, *args: P.args, **kwargs: P.kwargs):
+            def __init__(
+                self,
+                client: BaseClient,
+                source: SourceV1,
+                version: str,
+                *args: P.args,
+                **kwargs: P.kwargs,
+            ):
                 self.client = client
-                super().__init__(*args, **kwargs)
+                super().__init__(source=source, version=version, *args, **kwargs)
 
             def update(self):
-                update(self.client, self.nodes())
-                update(self.client, self.edges())
+                nodes, edges = self.get_nodes_and_edges()
+
+                update(self.client, nodes)
+                update(self.client, edges)
 
-        source = client.get("Source", name=source_name)
+        if isinstance(source, str):
+            sources = client.get("Source", name=source)
+            assert len(sources) == 1, f"Expected 1 source, got {len(sources)}"
+            source = sources[0]
+        elif isinstance(source, UUID):
+            source = client.get("Source", source)
+
+        if (kwargs_version := kwargs.pop("version", None)) is not None:
+            if kwargs_version != client.id:
+                raise Exception(
+                    f"Client version mismatch, the user provided version=`{kwargs_version}` does not match the "
+                    f"client id=`{client.id}`. Either leave `version` empty or set it to the client id."
+                )
         version = client.id
 
-        return WithClient(source=source, version=version, *args, **kwargs)
+        return WithClient(
+            client=client, source=source, version=version, *args, **kwargs
+        )
 
 
 class SeparateNodesAndEdgesMixin:
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
         return self.nodes(), self.edges()
 
 
@@ -92,7 +125,12 @@
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
         with self.connector.connect() as conn:
             nodes, edges = conn.get_nodes_and_edges()
 
         nodes = self.adapt_to_client(nodes)
         edges = self.adapt_to_client(edges)
         return nodes, edges
+
+    def ready(self) -> bool:
+        with self.connector.connect() as _:
+            pass
+        return True
```

### Comparing `grai_client-0.3.0a9/src/grai_client/schemas/labels.py` & `grai_client-0.3.1/src/grai_client/schemas/labels.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,8 +40,17 @@
     "Sourcednode",
     "Sourcednodes",
     "SourcedNode",
     "SourcedNodes",
 ]
 WorkspaceLabels = Literal["workspace", "workspaces", "Workspace", "Workspaces"]
 SourceLabels = Literal["source", "sources", "Source", "Sources"]
-OrganisationLabels = Literal["organisation", "organisations", "Organisation", "Organisations"]
+OrganisationLabels = Literal[
+    "organisation",
+    "organisations",
+    "Organisation",
+    "Organisations",
+    "organization",
+    "organizations",
+    "Organization",
+    "Organizations",
+]
```

### Comparing `grai_client-0.3.0a9/src/grai_client/testing/schema.py` & `grai_client-0.3.1/src/grai_client/testing/schema.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a9/src/grai_client/update.py` & `grai_client-0.3.1/src/grai_client/update.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from typing import Any, Dict, List, Optional, Tuple, TypeVar, Union
+from typing import Dict, List, Optional, Tuple, TypeVar, Union
 
-from grai_schemas.base import Edge, Node
-from grai_schemas.utilities import merge, merge_models
 from grai_schemas.v1.edge import EdgeV1, SourcedEdgeV1
 from grai_schemas.v1.node import NodeV1, SourcedNodeV1
-from grai_schemas.v1.source import SourceSpec
-from multimethod import multimethod
+from grai_schemas.v1.source import SourceSpec, SourceV1
 
 from grai_client.endpoints.client import BaseClient
 
 T = TypeVar("T", SourcedNodeV1, SourcedEdgeV1)
 
 
 def compute_graph_changes(items: List[T], active_items: List[T]) -> Tuple[List[T], List[T], List[T]]:
@@ -35,51 +32,19 @@
 
     new_items: List[T] = [item_map[k] for k in new_item_keys]
     updated_items = [item_map[k] for k in updated_item_keys if item_map[k] != active_item_map[k]]
 
     return new_items, updated_items, deleted_from_sources
 
 
-@multimethod
-def update(*args, **kwargs):
-    """
-
-    Args:
-        client:
-        items:
-        active_items:  (Default value = None)
-    """
-    raise NotImplementedError(f"Updated is not implemented for arguments of typ {[type(arg) for arg in args]}")
-
-
-@multimethod
-def update(client: BaseClient, items: List[Union[NodeV1, EdgeV1]], active_items: Any = None, source: Any = None):
-    """
-
-    Args:
-        client:
-        items:
-        active_items:  (Default value = None)
-
-    Returns:
-
-    Raises:
-
-    """
-    if not items:
-        return
-
-    raise NotImplementedError(
-        f"Update is not supported for NodeV1 or EdgeV1. Please use SourcedNodeV1 or SourcedEdgeV1 instead."
-    )
-
-
-@update.register
 def update(
-    client: BaseClient, items: List[T], active_items: Optional[List[T]] = None, source: Optional[SourceSpec] = None
+    client: BaseClient,
+    items: List[Union[SourcedNodeV1, SourcedEdgeV1]],
+    active_items: Optional[List[T]] = None,
+    source: Optional[Union[SourceV1, SourceSpec]] = None,
 ):
     """
 
     Args:
         client:
         items:
         active_items:  (Default value = None)
@@ -94,30 +59,40 @@
         return
     else:
         item_types = {type(item) for item in items}
         if len(item_types) != 1:
             raise ValueError(
                 f"All items provided to `update` must be of the same type. Instead got a mix of types:" f" {item_types}"
             )
+    if any(isinstance(item, Union[NodeV1, EdgeV1]) for item in items):
+        raise NotImplementedError(
+            f"Update is not supported for NodeV1 or EdgeV1. Please use SourcedNodeV1 or SourcedEdgeV1 instead."
+        )
     if source is None:
-        source = items[0].spec.data_source
+        source_spec = items[0].spec.data_source
+    elif isinstance(source, SourceV1):
+        source_spec = source.spec
+    else:
+        source_spec = source
+
+    if source_spec.id is None:
+        source_spec = client.get(source_spec).spec
 
     sources = {item.spec.data_source for item in items}
     if len(sources) != 1:
         raise ValueError(
             f"All items provided to `update` must be from the same source. Instead got items from sources:"
             f" {sources}"
         )
 
     if active_items is None:
-        active_items = client.get(items[0].type, source.id)
+        active_items = client.get(items[0].type, source_spec.id)
 
     new_items, updated_items, deleted_items = compute_graph_changes(items, active_items)
 
     # Going to need to deal with invalid deactivated nodes.
     # new_items are valid by virtue of being created by the caller
     # updated_items should be valid by virtue of merge logic and the caller providing a valid object.
     # However, deactivated_items may be invalid if the server provided an invalid object.
-
     client.post(new_items)
     client.patch(updated_items)
     client.delete(deleted_items)
```

### Comparing `grai_client-0.3.0a9/src/grai_client/utilities/tests.py` & `grai_client-0.3.1/src/grai_client/utilities/tests.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a9/PKG-INFO` & `grai_client-0.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: grai-client
-Version: 0.3.0a9
+Version: 0.3.1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: brotli (>=1.0.9,<2.0.0)
 Requires-Dist: furl (>=2.1.3,<3.0.0)
-Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
+Requires-Dist: grai-schemas (>=0.2.0,<0.3.0)
 Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: multimethod (>=1.9,<2.0)
-Requires-Dist: orjson (>=3.8.3,<4.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-client
 Description-Content-Type: text/markdown
```

