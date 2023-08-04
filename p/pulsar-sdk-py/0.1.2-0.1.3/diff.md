# Comparing `tmp/pulsar_sdk_py-0.1.2.tar.gz` & `tmp/pulsar_sdk_py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsar_sdk_py-0.1.2.tar", max compression
+gzip compressed data, was "pulsar_sdk_py-0.1.3.tar", max compression
```

## Comparing `pulsar_sdk_py-0.1.2.tar` & `pulsar_sdk_py-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-08-01 12:08:43.850947 pulsar_sdk_py-0.1.2/README.md
--rw-r--r--   0        0        0       34 2023-07-31 15:53:29.875987 pulsar_sdk_py-0.1.2/pulsar_sdk_py/__init__.py
--rw-r--r--   0        0        0     6326 2023-07-31 15:18:34.164193 pulsar_sdk_py-0.1.2/pulsar_sdk_py/enums.py
--rw-r--r--   0        0        0      140 2023-07-26 10:51:45.846061 pulsar_sdk_py-0.1.2/pulsar_sdk_py/exceptions.py
--rw-r--r--   0        0        0      634 2023-07-26 10:51:45.846131 pulsar_sdk_py-0.1.2/pulsar_sdk_py/helpers.py
--rw-r--r--   0        0        0    25965 2023-08-01 12:11:48.834609 pulsar_sdk_py-0.1.2/pulsar_sdk_py/pulsar_sdk.py
--rw-r--r--   0        0        0        0 2023-07-26 10:51:45.846396 pulsar_sdk_py-0.1.2/pulsar_sdk_py/schemas/__init__.py
--rw-r--r--   0        0        0    10286 2023-08-01 12:12:00.824832 pulsar_sdk_py-0.1.2/pulsar_sdk_py/schemas/schemas.py
--rw-r--r--   0        0        0     1283 2023-07-31 15:21:39.102392 pulsar_sdk_py-0.1.2/pulsar_sdk_py/schemas/serializer.py
--rw-r--r--   0        0        0      572 2023-08-02 17:59:50.429845 pulsar_sdk_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 pulsar_sdk_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1140 2023-08-04 13:35:13.009608 pulsar_sdk_py-0.1.3/README.md
+-rw-r--r--   0        0        0       34 2023-07-31 15:53:29.875987 pulsar_sdk_py-0.1.3/pulsar_sdk_py/__init__.py
+-rw-r--r--   0        0        0     6326 2023-07-31 15:18:34.164193 pulsar_sdk_py-0.1.3/pulsar_sdk_py/enums.py
+-rw-r--r--   0        0        0      140 2023-07-26 10:51:45.846061 pulsar_sdk_py-0.1.3/pulsar_sdk_py/exceptions.py
+-rw-r--r--   0        0        0      634 2023-07-26 10:51:45.846131 pulsar_sdk_py-0.1.3/pulsar_sdk_py/helpers.py
+-rw-r--r--   0        0        0    25944 2023-08-04 13:33:42.148688 pulsar_sdk_py-0.1.3/pulsar_sdk_py/pulsar_sdk.py
+-rw-r--r--   0        0        0        0 2023-07-26 10:51:45.846396 pulsar_sdk_py-0.1.3/pulsar_sdk_py/schemas/__init__.py
+-rw-r--r--   0        0        0    10327 2023-08-04 13:29:47.942380 pulsar_sdk_py-0.1.3/pulsar_sdk_py/schemas/schemas.py
+-rw-r--r--   0        0        0     1283 2023-07-31 15:21:39.102392 pulsar_sdk_py-0.1.3/pulsar_sdk_py/schemas/serializer.py
+-rw-r--r--   0        0        0      572 2023-08-04 13:34:36.604042 pulsar_sdk_py-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 pulsar_sdk_py-0.1.3/PKG-INFO
```

### Comparing `pulsar_sdk_py-0.1.2/README.md` & `pulsar_sdk_py-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -25,13 +25,14 @@
 ````
 
 Which will fetch you all the wallet balances for your wallet, provided the Chain is active in our environment.
 
 For more information, check out our [documentation](http://pulsar.readme.io/).
 
 ## Changelog
-
+### v0.1.2/3:
+- Changing names of dataclasses to match return from API.
 ### v0.1.1: 
 - Fixed issue where balances and timeseries would come duplicated. 
 - Fixed wallet timeseries schema.
 ### v0.1.0:
 - Beta launch.
```

### Comparing `pulsar_sdk_py-0.1.2/pulsar_sdk_py/enums.py` & `pulsar_sdk_py-0.1.3/pulsar_sdk_py/enums.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-0.1.2/pulsar_sdk_py/helpers.py` & `pulsar_sdk_py-0.1.3/pulsar_sdk_py/helpers.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-0.1.2/pulsar_sdk_py/pulsar_sdk.py` & `pulsar_sdk_py-0.1.3/pulsar_sdk_py/pulsar_sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import re
-import time
 import uuid
 import json
 import logging
-import asyncio
 import requests
 import websockets
 
+
 from typing import AsyncGenerator
 from pulsar_sdk_py.helpers import filter_non_empty_params
 from pulsar_sdk_py.schemas.serializer import serialize_to_dataclass
 from pulsar_sdk_py.exceptions import (
     WebSocketClosed,
     SerializationError,
     WrongResponseFormat,
@@ -31,23 +30,28 @@
     ResolvedName,
     ProtocolData,
     NFTCollection,
     ExtendedToken,
     ResolvedAddress,
     NFTTraitsFilter,
     PaginatedNFTItem,
-    WalletTokenErrors,
     ProtocolTimeseries,
     TokenPriceTimeseries,
     PaginatedNFTCollection,
-    WalletIntegrationErrors,
     PaginatedTokenWithStats,
     PaginatedProtocolWithStats,
+    AggregateWalletIntegrations,
+    AggregateWalletTokens,
 )
 
+API_URL = "https://dev-api.pulsar.finance"
+BASE_URL = "%s/v1/thirdparty" % API_URL
+WS_API_URL = "wss://dev-api.pulsar.finance"
+WS_URL = "%s/v1/thirdparty/ws" % WS_API_URL
+
 
 class PulsarSDK:
     """
     A client for interacting with the Pulsar Third Party API.
 
     This class provides a high-level interface for interacting with the API, including the ability to
     retrieve data about tokens, domain names, NFTs, protocols, and wallet balances. The class serves typified ways to
@@ -79,15 +83,14 @@
         Attributes: headers (dict): A dictionary of headers to include in WebSocket connection requests sent by
         instances of this class. uri (str): The URI for the WebSocket connection. websocket_conn: The WebSocket
         connection object.
 
         """
 
         headers = {}
-        uri = "wss://dev-api.pulsar.finance/v1/thirdparty/ws"
         websocket_conn = None
 
         def __init__(self, api_key):
             self.headers = {"Authorization": api_key}
 
         async def __connect_websocket(self):
             """
@@ -101,15 +104,15 @@
 
             """
             if self.websocket_conn is not None and self.websocket_conn.open:
                 # WebSocket connection is already open, return the existing connection
                 return self.websocket_conn
 
             # Create a new WebSocket connection
-            self.websocket_conn = await websockets.connect(self.uri, extra_headers=self.headers)
+            self.websocket_conn = await websockets.connect(WS_URL, extra_headers=self.headers)
             return self.websocket_conn
 
         async def response_generator(self, msg):
             """
             Generate responses from a WebSocket connection.
 
             This method sends a message to the WebSocket connection, and then waits for responses to be received from
@@ -196,20 +199,20 @@
             Raises:
                 SerializationError: If an error occurs during serialization of the payload data.
 
             """
             try:
                 if payload_type.startswith("Timeseries"):
                     yield serialize_to_dataclass(payload_data[0], Timeseries)
-                elif payload_type.startswith("WalletIntegrationErrors"):
-                    yield serialize_to_dataclass(payload_data, WalletIntegrationErrors)
+                elif payload_type.startswith("AggregateWalletIntegrations"):
+                    yield serialize_to_dataclass(payload_data, AggregateWalletIntegrations)
                 elif payload_type.startswith("NFTItem"):
                     yield [serialize_to_dataclass(item, NFTItem) for item in payload_data["items"]]
-                elif payload_type.startswith("WalletTokenErrors"):
-                    yield serialize_to_dataclass(payload_data, WalletTokenErrors)
+                elif payload_type.startswith("AggregateWalletTokens"):
+                    yield serialize_to_dataclass(payload_data, AggregateWalletTokens)
             except Exception as e:
                 # Handle serialization error
                 raise SerializationError(
                     f"An error occurred during serialization: {str(e)}\nSerializing {payload_type}."
                 ) from e
 
         @staticmethod
@@ -254,15 +257,15 @@
 
         def __init__(self, ws_client):
             self.__ws_client = ws_client
 
         @replace_enums_with_values
         async def get_wallet_balances(
             self, wallet_addr: str, chain: ChainKeys
-        ) -> AsyncGenerator[WalletIntegrationErrors | list[NFTItem] | WalletTokenErrors | None, None]:
+        ) -> AsyncGenerator[AggregateWalletIntegrations | list[NFTItem] | AggregateWalletTokens | None, None]:
             request_id = str(uuid.uuid4())
             msg = {
                 "method": "COMMAND",
                 "command": {
                     "key": f"{self.__KEYS['WALLET_BALANCES']['COMMAND']}",
                     "data": {"address": f"{wallet_addr}", "chain": f"{chain}"},
                 },
@@ -309,20 +312,18 @@
         This class provides several methods for sending HTTP requests to Pulsar REST API endpoints.
         It includes a static method for filtering out any key-value pairs from a dictionary where the value is None,
         as well as a method for sending an HTTP request to a Pulsar REST API endpoint and returning the JSON
         response body.
 
         Attributes:
             headers (dict): A dictionary of headers to include in HTTP requests sent by instances of this class.
-            base_url (str): The base URL for the REST API.
 
         """
 
         headers = {}
-        base_url = "https://dev-api.pulsar.finance/v1/thirdparty"
 
         def __init__(self, headers):
             self.headers = headers
 
         @replace_enums_with_values
         def __get_request_on_endpoint(self, func_name, request_type, request_body=None, **kwargs):
             """
@@ -344,23 +345,23 @@
             if request_body is None:
                 request_body = {}
             endpoint_url = self.endpoints[func_name]
 
             # This code extracts named parameters from a string (endpoint_url) using regular expressions,
             # and populates them with corresponding values from a dictionary (kwargs).The resulting string is formed
             # by substituting the named parameters with their corresponding values, and concatenating the result with
-            # another string (self.base_url).
+            # another string (BASE_URL).
             param_names = re.findall(r"\{([^{}]*)\}", endpoint_url)
             params = {}
             for param_name in param_names:
                 if param_name in kwargs:
                     param_value = kwargs.pop(param_name)
                     params[param_name] = param_value
             formatted_url = endpoint_url.format(**params)
-            endpoint_url = self.base_url + formatted_url
+            endpoint_url = BASE_URL + formatted_url
 
             if kwargs:
                 # If there are any remaining kwargs, construct them as query parameters for the endpoint URL
                 query_params = []
                 for key, value in kwargs.items():
                     if isinstance(value, list):
                         query_params.extend(f"{key}={item}" for item in value)
```

### Comparing `pulsar_sdk_py-0.1.2/pulsar_sdk_py/schemas/schemas.py` & `pulsar_sdk_py-0.1.3/pulsar_sdk_py/schemas/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     volume: str | None = None
     average_price: str | None = None
     floor_price: str | None = None
     market_cap: str | None = None
     stats: NFTCollectionStats | None = None
     low_volume: bool = False
     unknown_volume: bool = False
+    is_fully_index: bool = False
 
 
 @dataclass
 class NFTItem:
     name: str
     id: str
     token_id: str
@@ -196,15 +197,15 @@
 @dataclass
 class TokenError:
     token: SimpleToken
     chain: ChainKeys
 
 
 @dataclass
-class WalletTokenErrors:
+class AggregateWalletTokens:
     stats: list[WalletTokenStats]
     errors: list[TokenError]
 
 
 @dataclass
 class ProtocolTimeseries:
     tier: str
@@ -457,15 +458,15 @@
 @dataclass
 class RecipeError:
     recipe: Recipe
     chain: ChainKeys
 
 
 @dataclass
-class WalletIntegrationErrors:
+class AggregateWalletIntegrations:
     stats: list[WalletIntegration]
     errors: list[RecipeError]
 
 
 @dataclass
 class PaginatedTokenWithStats:
     response: list[TokenWithStats]
```

### Comparing `pulsar_sdk_py-0.1.2/pulsar_sdk_py/schemas/serializer.py` & `pulsar_sdk_py-0.1.3/pulsar_sdk_py/schemas/serializer.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-0.1.2/pyproject.toml` & `pulsar_sdk_py-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pulsar-sdk-py"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = [ "Pulsar <admin@pulsar.finance>",]
 readme = "README.md"
 packages = [
     {include = "pulsar_sdk_py"},
 ]
```

### Comparing `pulsar_sdk_py-0.1.2/PKG-INFO` & `pulsar_sdk_py-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsar-sdk-py
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Pulsar
 Author-email: admin@pulsar.finance
 Requires-Python: >=3.11.0,<3.12.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
@@ -41,13 +41,14 @@
 ````
 
 Which will fetch you all the wallet balances for your wallet, provided the Chain is active in our environment.
 
 For more information, check out our [documentation](http://pulsar.readme.io/).
 
 ## Changelog
-
+### v0.1.2/3:
+- Changing names of dataclasses to match return from API.
 ### v0.1.1: 
 - Fixed issue where balances and timeseries would come duplicated. 
 - Fixed wallet timeseries schema.
 ### v0.1.0:
 - Beta launch.
```

