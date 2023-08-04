# Comparing `tmp/tonconnect-0.1.2.tar.gz` & `tmp/tonconnect-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonconnect-0.1.2.tar", last modified: Fri May 26 12:46:35 2023, max compression
+gzip compressed data, was "tonconnect-0.1.3.tar", last modified: Fri Aug  4 21:04:15 2023, max compression
```

## Comparing `tonconnect-0.1.2.tar` & `tonconnect-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       34 2023-04-14 20:07:11.801816 tonconnect-0.1.2/.gitignore
--rw-r--r--   0        0        0    11350 2023-04-14 20:08:17.432870 tonconnect-0.1.2/LICENSE.md
--rw-r--r--   0        0        0     2501 2023-05-26 12:46:02.932893 tonconnect-0.1.2/README.md
--rw-r--r--   0        0        0      288 2023-05-26 09:22:35.528472 tonconnect-0.1.2/examples/address.py
--rw-r--r--   0        0        0      324 2023-05-15 14:11:06.445617 tonconnect-0.1.2/examples/all_versions_support.py
--rw-r--r--   0        0        0      464 2023-05-26 12:33:52.390794 tonconnect-0.1.2/examples/async_address.py
--rw-r--r--   0        0        0      782 2023-04-21 11:32:11.563469 tonconnect-0.1.2/examples/transactions.py
--rw-r--r--   0        0        0      556 2023-05-26 12:46:07.691963 tonconnect-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 07:29:33.705331 tonconnect-0.1.2/tonconnect/__init__.py
--rw-r--r--   0        0        0      261 2023-05-26 12:32:45.875304 tonconnect-0.1.2/tonconnect/apps.py
--rw-r--r--   0        0        0     3759 2023-04-25 18:07:17.059721 tonconnect-0.1.2/tonconnect/bridge.py
--rw-r--r--   0        0        0     4081 2023-05-26 12:44:26.568017 tonconnect-0.1.2/tonconnect/connector.py
--rw-r--r--   0        0        0     1202 2023-04-12 07:19:51.920373 tonconnect-0.1.2/tonconnect/crypto.py
--rw-r--r--   0        0        0     3442 2023-05-26 12:30:59.031168 tonconnect-0.1.2/tonconnect/events.py
--rw-r--r--   0        0        0      162 2023-04-12 09:29:00.652526 tonconnect-0.1.2/tonconnect/exceptions.py
--rw-r--r--   0        0        0     2930 2023-04-25 18:02:37.265076 tonconnect-0.1.2/tonconnect/httpbridge.py
--rw-r--r--   0        0        0      472 2023-04-12 09:30:53.246514 tonconnect-0.1.2/tonconnect/options.py
--rw-r--r--   0        0        0     1733 2023-04-24 10:38:25.387486 tonconnect-0.1.2/tonconnect/requests.py
--rw-r--r--   0        0        0      320 2023-04-12 07:22:22.791632 tonconnect-0.1.2/tonconnect/static.py
--rw-r--r--   0        0        0      330 2023-05-12 16:46:40.731106 tonconnect-0.1.2/tonconnect/url.py
--rw-r--r--   0        0        0      225 2023-04-12 07:24:37.312579 tonconnect-0.1.2/tonconnect/utils.py
--rw-r--r--   0        0        0      416 2023-04-25 17:06:44.302885 tonconnect-0.1.2/tonconnect/wallet.py
--rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 tonconnect-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-04-14 20:07:11.801816 tonconnect-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1076 2023-08-04 20:53:36.689907 tonconnect-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0     2602 2023-08-04 21:02:51.546308 tonconnect-0.1.3/README.md
+-rw-r--r--   0        0        0      288 2023-05-26 09:22:35.528472 tonconnect-0.1.3/examples/address.py
+-rw-r--r--   0        0        0      324 2023-05-15 14:11:06.445617 tonconnect-0.1.3/examples/all_versions_support.py
+-rw-r--r--   0        0        0      497 2023-08-04 21:00:06.882018 tonconnect-0.1.3/examples/async_address.py
+-rw-r--r--   0        0        0      782 2023-04-21 11:32:11.563469 tonconnect-0.1.3/examples/transactions.py
+-rw-r--r--   0        0        0      556 2023-08-04 20:55:33.523855 tonconnect-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 07:29:33.705331 tonconnect-0.1.3/tonconnect/__init__.py
+-rw-r--r--   0        0        0      261 2023-05-26 12:32:45.875304 tonconnect-0.1.3/tonconnect/apps.py
+-rw-r--r--   0        0        0     3702 2023-06-13 11:38:49.793230 tonconnect-0.1.3/tonconnect/bridge.py
+-rw-r--r--   0        0        0     4169 2023-08-04 20:57:48.654371 tonconnect-0.1.3/tonconnect/connector.py
+-rw-r--r--   0        0        0     1186 2023-08-04 20:54:38.603473 tonconnect-0.1.3/tonconnect/crypto.py
+-rw-r--r--   0        0        0     3442 2023-05-26 12:30:59.031168 tonconnect-0.1.3/tonconnect/events.py
+-rw-r--r--   0        0        0      162 2023-04-12 09:29:00.652526 tonconnect-0.1.3/tonconnect/exceptions.py
+-rw-r--r--   0        0        0     2943 2023-06-13 11:04:29.136264 tonconnect-0.1.3/tonconnect/httpbridge.py
+-rw-r--r--   0        0        0      472 2023-04-12 09:30:53.246514 tonconnect-0.1.3/tonconnect/options.py
+-rw-r--r--   0        0        0     1733 2023-04-24 10:38:25.387486 tonconnect-0.1.3/tonconnect/requests.py
+-rw-r--r--   0        0        0      320 2023-04-12 07:22:22.791632 tonconnect-0.1.3/tonconnect/static.py
+-rw-r--r--   0        0        0      330 2023-05-12 16:46:40.731106 tonconnect-0.1.3/tonconnect/url.py
+-rw-r--r--   0        0        0      225 2023-04-12 07:24:37.312579 tonconnect-0.1.3/tonconnect/utils.py
+-rw-r--r--   0        0        0      416 2023-04-25 17:06:44.302885 tonconnect-0.1.3/tonconnect/wallet.py
+-rw-r--r--   0        0        0     3098 1970-01-01 00:00:00.000000 tonconnect-0.1.3/PKG-INFO
```

### Comparing `tonconnect-0.1.2/README.md` & `tonconnect-0.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -70,38 +70,43 @@
     print(f'Universal connect url for Tonkeeper: {url}')
 
     address = await connector.get_address()
     print(f'Successfuly connected {address}.')
 
 
 if __name__ == '__main__':
-    loop = asyncio.get_event_loop()
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
     loop.run_until_complete(main())
 ```
 
 ## Authors
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
+* 0.1.3
+    * License change
+    * Python 3.11 support
+    * Small changes
 * 0.1.2
     * Bug fix
 * 0.1.1
     * Added tonapi.io support
 * 0.1.0
     * Async wrapper
 * 0.0.2 & 0.0.3
     * pyproject.toml fix
 * 0.0.1
     * Initial Beta
 
 ## License
 
-This project is licensed under the Apache License 2.0 - see the LICENSE.md file for details
+This project is licensed under the MIT License - see the LICENSE.md file for details
 
 ## Donate
 
 If you like the library, I will be glad to accept donations.
 
 * TON: EQCgphx8rTI0PukwmgpVqiPgqguTujhQscg2h7jgc4U0t347
```

### Comparing `tonconnect-0.1.2/examples/transactions.py` & `tonconnect-0.1.3/examples/transactions.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.2/pyproject.toml` & `tonconnect-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "tonconnect"
 description = "TON Connect - Python library for using TON Connect 2."
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "Vlad100"}
 ]
 dependencies = [
     "pynacl",
     "requests",
     "tonsdk",
```

### Comparing `tonconnect-0.1.2/tonconnect/bridge.py` & `tonconnect-0.1.3/tonconnect/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,51 +55,52 @@
         return data
 
     def form_request(self, message: Request) -> tuple[str, str]:
         if self.session is None:
             raise BridgeException('Sending request on non-connected bridge.')
         
         message = message.to_dict()
-        # print(json.dumps(message))
         encrypted_message = self.session.encrypt(json.dumps(message))
-        # print(encrypted_message)
         concatenated_message = b''.join([bytes(i) for i in encrypted_message])
         body = base64.b64encode(concatenated_message).decode()
-        # print(body)
         
-        url = f'https://{self.url}{self.slash_url}/message?client_id={self.session.to_hex()}&to={public_key_to_hex(self.session.app_public_key)}&ttl={self.ttl}&topic={message["method"]}'
+        url = f'{self.slash_url}/message?client_id={self.session.to_hex()}&to={public_key_to_hex(self.session.app_public_key)}&ttl={self.ttl}&topic={message["method"]}'
         
         return url, body
 
     def get_event(self) -> dict:
         return {}
 
     def send_request(self, message: Request) -> dict:
         return {}
 
+
 class Bridge(BaseBridge):
     def get_event(self):
         url = self.get_events_url()
         
         client = SyncClient(self.url, url)
         data, id = client.get(self.timeout)
         
         return self.encode_event(data, id)
     
     def send_request(self, message: Request) -> dict:
         # WIP
         
         url, body = self.form_request(message)
         
+        # print(self.url, url)
         client = SyncClient(self.url, url)
         answer = client.send(body)
+        # print(body)
         # print(answer.text, 'sended')
         
         return self.get_event()
 
+
 class AsyncBridge(BaseBridge):
     async def get_event(self):
         url = self.get_events_url()
         
         client = AsyncClient(self.url, url)
         data, id = await client.get(self.timeout)
```

### Comparing `tonconnect-0.1.2/tonconnect/connector.py` & `tonconnect-0.1.3/tonconnect/connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,21 +59,24 @@
         
         if not event.proof.check(event.address.raw_address, verify_key):
             raise ConnectorException('Invalid proof.')
         
         return event.address.address
 
 class AsyncConnector(Connector):
-    async def connect(self, wallet: str, payload: str):
+    async def connect(self, wallet: Wallet, payload: str):
         metadata = Metadata(self.metadata_url, [AddressRequestOption(), ProofRequestOption(payload)])
         
-        if wallet not in APPS:
-            raise ConnectorException(f'Unknown wallet {wallet}.')
+        if isinstance(wallet, str):
+            if wallet not in APPS:
+                raise ConnectorException(f'Unknown wallet {wallet}.')
+            
+            wallet = APPS[wallet]
         
-        self.wallet = APPS[wallet](bridge_client=AsyncBridge)
+        self.wallet = wallet(bridge_client=AsyncBridge)
         self.bridge: AsyncBridge = self.wallet.bridge
         
         self.bridge.connect(self.session)
         return self.wallet.get_url(metadata)
     
     async def get_address(self):
         event = await self.bridge.get_event()
```

### Comparing `tonconnect-0.1.2/tonconnect/events.py` & `tonconnect-0.1.3/tonconnect/events.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.2/tonconnect/httpbridge.py` & `tonconnect-0.1.3/tonconnect/httpbridge.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                             break
                         elif key == 'id':
                             id = value
 
         return data, id
     
     def send(self, body):
-        return requests.post(self.base_url + self.url, data=body)
+        return requests.post('https://' + self.base_url + self.url, json=body)
 
 class AsyncClient():
     def __init__(self, base_url, url):
         self.base_url = base_url
         self.url = url
     
     async def get(self, timeout=60):
```

### Comparing `tonconnect-0.1.2/tonconnect/requests.py` & `tonconnect-0.1.3/tonconnect/requests.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.2/PKG-INFO` & `tonconnect-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonconnect
-Version: 0.1.2
+Version: 0.1.3
 Summary: TON Connect - Python library for using TON Connect 2.
 Author: Vlad100
 Description-Content-Type: text/markdown
 Requires-Dist: pynacl
 Requires-Dist: requests
 Requires-Dist: tonsdk
 Requires-Dist: aiohttp
@@ -84,38 +84,43 @@
     print(f'Universal connect url for Tonkeeper: {url}')
 
     address = await connector.get_address()
     print(f'Successfuly connected {address}.')
 
 
 if __name__ == '__main__':
-    loop = asyncio.get_event_loop()
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
     loop.run_until_complete(main())
 ```
 
 ## Authors
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
+* 0.1.3
+    * License change
+    * Python 3.11 support
+    * Small changes
 * 0.1.2
     * Bug fix
 * 0.1.1
     * Added tonapi.io support
 * 0.1.0
     * Async wrapper
 * 0.0.2 & 0.0.3
     * pyproject.toml fix
 * 0.0.1
     * Initial Beta
 
 ## License
 
-This project is licensed under the Apache License 2.0 - see the LICENSE.md file for details
+This project is licensed under the MIT License - see the LICENSE.md file for details
 
 ## Donate
 
 If you like the library, I will be glad to accept donations.
 
 * TON: EQCgphx8rTI0PukwmgpVqiPgqguTujhQscg2h7jgc4U0t347
```

