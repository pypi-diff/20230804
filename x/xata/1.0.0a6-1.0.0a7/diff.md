# Comparing `tmp/xata-1.0.0a6.tar.gz` & `tmp/xata-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-1.0.0a6.tar", max compression
+gzip compressed data, was "xata-1.0.0a7.tar", max compression
```

## Comparing `xata-1.0.0a6.tar` & `xata-1.0.0a7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2023-08-03 14:00:46.126982 xata-1.0.0a6/LICENSE
--rw-r--r--   0        0        0     1083 2023-08-03 14:00:46.126982 xata-1.0.0a6/README.md
--rw-r--r--   0        0        0      822 2023-08-03 14:00:46.154984 xata-1.0.0a6/pyproject.toml
--rw-r--r--   0        0        0      873 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/__init__.py
--rw-r--r--   0        0        0      769 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/__init__.py
--rw-r--r--   0        0        0     2995 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/authentication.py
--rw-r--r--   0        0        0    13898 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/branch.py
--rw-r--r--   0        0        0     8389 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/databases.py
--rw-r--r--   0        0        0     8962 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/files.py
--rw-r--r--   0        0        0     6742 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/invites.py
--rw-r--r--   0        0        0    13228 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/migrations.py
--rw-r--r--   0        0        0    13684 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/records.py
--rw-r--r--   0        0        0    33149 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/search_and_filter.py
--rw-r--r--   0        0        0    13796 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/table.py
--rw-r--r--   0        0        0     2771 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/users.py
--rw-r--r--   0        0        0     8262 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api/workspaces.py
--rw-r--r--   0        0        0     3080 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api_request.py
--rw-r--r--   0        0        0     3186 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/api_response.py
--rw-r--r--   0        0        0    13444 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/client.py
--rw-r--r--   0        0        0     1188 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/errors.py
--rw-r--r--   0        0        0    15894 2023-08-03 14:00:46.186986 xata-1.0.0a6/xata/helpers.py
--rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 xata-1.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-04 10:18:33.336464 xata-1.0.0a7/LICENSE
+-rw-r--r--   0        0        0     1083 2023-08-04 10:18:33.336464 xata-1.0.0a7/README.md
+-rw-r--r--   0        0        0      822 2023-08-04 10:18:33.360465 xata-1.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0      873 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/__init__.py
+-rw-r--r--   0        0        0      769 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/__init__.py
+-rw-r--r--   0        0        0     3634 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/authentication.py
+-rw-r--r--   0        0        0    13898 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/branch.py
+-rw-r--r--   0        0        0     8389 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/databases.py
+-rw-r--r--   0        0        0     8962 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/files.py
+-rw-r--r--   0        0        0     6742 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/invites.py
+-rw-r--r--   0        0        0    13228 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/migrations.py
+-rw-r--r--   0        0        0    13684 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/records.py
+-rw-r--r--   0        0        0    33213 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/search_and_filter.py
+-rw-r--r--   0        0        0    13796 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/table.py
+-rw-r--r--   0        0        0     2771 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/users.py
+-rw-r--r--   0        0        0     8262 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api/workspaces.py
+-rw-r--r--   0        0        0     3823 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api_request.py
+-rw-r--r--   0        0        0     3186 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/api_response.py
+-rw-r--r--   0        0        0    13444 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/client.py
+-rw-r--r--   0        0        0     1188 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/errors.py
+-rw-r--r--   0        0        0    15894 2023-08-04 10:18:33.392466 xata-1.0.0a7/xata/helpers.py
+-rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 xata-1.0.0a7/PKG-INFO
```

### Comparing `xata-1.0.0a6/LICENSE` & `xata-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/README.md` & `xata-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/pyproject.toml` & `xata-1.0.0a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xata"
-version = "1.0.0a6"
+version = "1.0.0a7"
 description = "Python client for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
```

### Comparing `xata-1.0.0a6/xata/__init__.py` & `xata-1.0.0a7/xata/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api/__init__.py` & `xata-1.0.0a7/xata/api/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api/authentication.py` & `xata-1.0.0a7/xata/api/authentication.py`

 * *Files 20% similar despite different names*

```diff
@@ -90,7 +90,28 @@
 
         :param key_name: str API Key name
 
         :returns ApiResponse
         """
         url_path = f"/user/keys/{key_name}"
         return self.request("DELETE", url_path)
+
+    def get_oauth_user_clients(self) -> ApiResponse:
+        """
+        Retrieve the list of OAuth Clients that a user has authorized
+
+        Reference: https://xata.io/docs/api-reference/user/oauth/clients#get-the-list-of-user-oauth-clients
+        Path: /user/oauth/clients
+        Method: GET
+        Response status codes:
+        - 200: OK
+        - 400: Bad Request
+        - 401: Authentication Error
+        - 404: Example response
+        - 5XX: Unexpected Error
+        Response: application/json
+
+
+        :returns ApiResponse
+        """
+        url_path = "/user/oauth/clients"
+        return self.request("GET", url_path)
```

### Comparing `xata-1.0.0a6/xata/api/branch.py` & `xata-1.0.0a7/xata/api/branch.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api/databases.py` & `xata-1.0.0a7/xata/api/databases.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api/files.py` & `xata-1.0.0a7/xata/api/files.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api/invites.py` & `xata-1.0.0a7/xata/api/invites.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api/migrations.py` & `xata-1.0.0a7/xata/api/migrations.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api/records.py` & `xata-1.0.0a7/xata/api/records.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api/search_and_filter.py` & `xata-1.0.0a7/xata/api/search_and_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,15 @@
         payload = {
             "question": question,
         }
         headers = {
             "content-type": "application/json",
             "accept": "text/event-stream" if streaming_results else "application/json",
         }
-        return self.request("POST", url_path, headers, payload)
+        return self.request("POST", url_path, headers, payload, is_streaming=streaming_results)
 
     def ask_follow_up(
         self,
         table_name: str,
         session_id: str,
         question: str,
         streaming_results: bool = False,
@@ -415,15 +415,15 @@
         payload = {
             "message": question,
         }
         headers = {
             "content-type": "application/json",
             "accept": "text/event-stream" if streaming_results else "application/json",
         }
-        return self.request("POST", url_path, headers, payload)
+        return self.request("POST", url_path, headers, payload, is_streaming=streaming_results)
 
     def summarize(self, table_name: str, payload: dict, db_name: str = None, branch_name: str = None) -> ApiResponse:
         """
         This endpoint allows you to (optionally) define groups, and then to run calculations on
         the values in each group.  This is most helpful when  you'd like to understand the data
         you have in your database.  A group is a combination of unique values.  If you create a
         group for  `sold_by`, `product_name`, we will return one row for every combination  of
```

### Comparing `xata-1.0.0a6/xata/api/table.py` & `xata-1.0.0a7/xata/api/table.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api/users.py` & `xata-1.0.0a7/xata/api/users.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api/workspaces.py` & `xata-1.0.0a7/xata/api/workspaces.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/api_request.py` & `xata-1.0.0a7/xata/api_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,27 +15,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 
 import logging
 
-from requests import request
+from requests import Session, request
 
 from xata.api_response import ApiResponse
 
 from .errors import RateLimitError, UnauthorizedError, XataServerError
 
 
 class ApiRequest:
-    """
-    Parent class for API requests
-    """
-
     def __init__(self, client):
+        self.session = Session()
         self.client = client
         self.logger = logging.getLogger(self.__class__.__name__)
 
     def get_scope(self) -> str:
         return self.scope
 
     def is_control_plane(self) -> bool:
@@ -45,40 +42,56 @@
         if self.is_control_plane():
             return "https://" + self.client.get_config()["domain_core"]
         # Base URL must be build on the fly as the region & workspace Id can change
         cfg = self.client.get_config()
         return "https://%s.%s.%s" % (cfg["workspaceId"], cfg["region"], cfg["domain_workspace"])
 
     def request(
-        self, http_method: str, url_path: str, headers: dict = {}, payload: dict = None, data: bytes = None
+        self,
+        http_method: str,
+        url_path: str,
+        headers: dict = {},
+        payload: dict = None,
+        data: bytes = None,
+        is_streaming: bool = False,
     ) -> ApiResponse:
         """
         :param http_method: str
         :param url_path: str
         :headers: dict = {}
         :param payload: dict = None
         :param data: bytes = None
+        :param is_streaming: bool = False
 
         :returns ApiResponse
 
         :raises RateLimitError
         :raises UnauthorizedError
         :raises ServerError
         """
-        # TODO use "|" when client py min version >= 3.9
         headers = {**headers, **self.client.get_headers()}
-
-        # build url
         url = "%s/%s" % (self.get_base_url(), url_path.lstrip("/"))
-        if payload is None and data is None:
-            resp = request(http_method, url, headers=headers)
-        elif data is not None:
-            resp = request(http_method, url, headers=headers, data=data)
+
+        # In order not exhaust the connection pool with open connections from unread streams
+        # we opt for Session usage on all non-stream requests
+        # https://requests.readthedocs.io/en/latest/user/advanced/#body-content-workflow
+        if is_streaming:
+            if payload is None and data is None:
+                resp = request(http_method, url, headers=headers, stream=True)
+            elif data is not None:
+                resp = request(http_method, url, headers=headers, data=data, stream=True)
+            else:
+                resp = request(http_method, url, headers=headers, json=payload, stream=True)
         else:
-            resp = request(http_method, url, headers=headers, json=payload)
+            if payload is None and data is None:
+                resp = self.session.request(http_method, url, headers=headers)
+            elif data is not None:
+                resp = self.session.request(http_method, url, headers=headers, data=data)
+            else:
+                resp = self.session.request(http_method, url, headers=headers, json=payload)
 
         # Any special status code we can raise an exception for ?
         if resp.status_code == 429:
             raise RateLimitError(f"code: {resp.status_code}, rate limited: {resp.json()}")
         if resp.status_code == 401:
             raise UnauthorizedError(f"code: {resp.status_code}, unauthorized: {resp.json()}")
         elif resp.status_code >= 500:
```

### Comparing `xata-1.0.0a6/xata/api_response.py` & `xata-1.0.0a7/xata/api_response.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/client.py` & `xata-1.0.0a7/xata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .api.search_and_filter import SearchAndFilter
 from .api.table import Table
 from .api.users import Users
 from .api.workspaces import Workspaces
 
 # TODO this is a manual task, to keep in sync with pyproject.toml
 # could/should be automated to keep in sync
-__version__ = "1.0.0a6"
+__version__ = "1.0.0a7"
 
 PERSONAL_API_KEY_LOCATION = "~/.config/xata/key"
 DEFAULT_DATA_PLANE_DOMAIN = "xata.sh"
 DEFAULT_CONTROL_PLANE_DOMAIN = "api.xata.io"
 DEFAULT_REGION = "us-east-1"
 DEFAULT_BRANCH_NAME = "main"
 CONFIG_LOCATION = ".xatarc"
```

### Comparing `xata-1.0.0a6/xata/errors.py` & `xata-1.0.0a7/xata/errors.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/xata/helpers.py` & `xata-1.0.0a7/xata/helpers.py`

 * *Files identical despite different names*

### Comparing `xata-1.0.0a6/PKG-INFO` & `xata-1.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Python client for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

