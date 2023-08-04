# Comparing `tmp/gama_client-1.1.3.tar.gz` & `tmp/gama_client-1.1.4.tar.gz`

## Comparing `gama_client-1.1.3.tar` & `gama_client-1.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gama_client-1.1.3/gama_client/__init__.py
--rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 gama_client-1.1.3/gama_client/base_client.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 gama_client-1.1.3/gama_client/command_types.py
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 gama_client-1.1.3/gama_client/message_types.py
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 gama_client-1.1.3/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 gama_client-1.1.3/LICENSE
--rw-r--r--   0        0        0     8998 2020-02-02 00:00:00.000000 gama_client-1.1.3/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 gama_client-1.1.3/pyproject.toml
--rw-r--r--   0        0        0    10663 2020-02-02 00:00:00.000000 gama_client-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gama_client-1.1.4/gama_client/__init__.py
+-rw-r--r--   0        0        0    18335 2020-02-02 00:00:00.000000 gama_client-1.1.4/gama_client/base_client.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 gama_client-1.1.4/gama_client/command_types.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 gama_client-1.1.4/gama_client/message_types.py
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 gama_client-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 gama_client-1.1.4/LICENSE
+-rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 gama_client-1.1.4/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 gama_client-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 gama_client-1.1.4/PKG-INFO
```

### Comparing `gama_client-1.1.3/gama_client/base_client.py` & `gama_client-1.1.4/gama_client/base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         message_handler function
 
         :param handle_connection_message: If set to true, the function checks for messages of type ConnectionSuccessful
             and will set its content field as the result of connection_future that is used in connect to wait for the socket_id
         :param timeout: timeout for reading the next message
         :return: Never returns
         """
-        while True:
+        while self.socket.open:
             try:
                 mess = await asyncio.wait_for(self.socket.recv(), timeout=timeout)
                 try:
                     js = json.loads(mess)
                     if handle_connection_message \
                         and "type" in js \
                         and "content" in js \
@@ -76,16 +76,17 @@
 
                         self.connection_future.set_result(js["content"])
                     else:
                         await self.message_handler(js)
                 except Exception as js_ex:
                     print("Unable to unpack gama-server messages as a json. Error:", js_ex, "Message received:", mess)
             except Exception as sock_ex:
-                print("Error while waiting for a message from gama-server. Exiting", sock_ex)
-                sys.exit(-1)
+                if self.socket.open:
+                    print("Error while waiting for a message from gama-server. Exiting", sock_ex)
+                    sys.exit(-1)
 
     async def load(self, file_path: str, experiment_name: str, console: bool = None, status: bool = None,
                    dialog: bool = None, runtime: bool = None, parameters: List[Dict] = None, until: str = "", socket_id: str = "",
                    additional_data: Dict = None):
         """Sends a command to load the experiment **experiment_name** from the file **file_path** (on the server side).
 
         **Note**
@@ -148,14 +149,49 @@
         :return: Nothing
         """
         cmd = {
             "type": CommandTypes.Exit.value
         }
         await self.socket.send(json.dumps(cmd))
 
+    async def download(self, file_path: str):
+        """
+        Downloads a file from gama server file system
+        :type file_path: the path of the file to download on gama-server's file system
+        :return: if everything goes well, gama-server will send back an object containing the entirety
+        of the file as a string
+        """
+        cmd = {
+            "type": CommandTypes.Download.value,
+            "file": file_path,
+        }
+        await self.socket.send(json.dumps(cmd))
+
+    async def upload(self, file_path: str, content: str):
+        """
+        Uploads a file to gama-server's file-system
+        :param file_path: the path on gama-server file-system where the content is going to be saved
+        :param content: the content of the file to be uploaded
+        """
+        cmd = {
+            "type": CommandTypes.Upload.value,
+            "file": file_path,
+            "content": content
+        }
+        await self.socket.send(json.dumps(cmd))
+
+    async def close_connection(self, close_code=1000, reason=""):
+        """
+        Closes the connection
+        :param close_code: the close code, 1000 by default
+        :param reason: a human-readable reason for closing.
+        :return:
+        """
+        await self.socket.close(close_code, reason)
+
     async def play(self, exp_id: str, sync: bool = None, socket_id: str = "", additional_data: Dict = None):
         """
         Sends a command to run the experiment **exp_id**
 
         :param exp_id: The id of the experiment on which the command applies
             (sent by gama-server after the load command)
         :param socket_id: The socket_id that is linked to the experiment, if empty gama will use current connection
```

### Comparing `gama_client-1.1.3/gama_client/message_types.py` & `gama_client-1.1.4/gama_client/message_types.py`

 * *Files identical despite different names*

### Comparing `gama_client-1.1.3/.gitignore` & `gama_client-1.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gama_client-1.1.3/LICENSE` & `gama_client-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gama_client-1.1.3/README.md` & `gama_client-1.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Gama client
- Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the modeling and simulation platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.1.
+ Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the modeling and simulation platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.2.
 This wrapper will take care of the connection with gama-server and of sending properly formatted requests to gama-server. It is made to fit the asynchronous nature of gama-server and thus makes it possible to handle multiple simulations at the same time, but the counterpart is that the users will still have to manage what to do with the received messages (command confirmation, simulation output, errors etc.) by themselves. We provide a working example that shows the architecture you can deploy if you still want to have a sequential execution.
 
 # Installation
 In your python environment, install the gama-client package with the command:
 
 ```
 pip install gama-client
@@ -66,14 +66,20 @@
 ```
 or
 ```python
 await client.connect()
 ```
 And the client will take care of handling this first message and setting the `socket_id` by itself.
 
+To explicitly disconnect from gama-server, simply use the `close_connection` function:
+```python
+await client.close_connection()
+```
+you can later reconnect with the same `client` object the same way you did the first time, with the `connect` function.
+
 ### Running commands
 Once connected you will want to run commands, the principle is pretty simple: all commands can be run your `client` variable through functions. For example if you want to run the [load command](https://gama-platform.org/wiki/next/HeadlessServer#the-load-command) you just have to call the `load` function with the proper parameters.
 ```python
 await client.load("path/to/gaml/file", "my_experiment_name")
 ```
 
 ### Message handling
```

### Comparing `gama_client-1.1.3/pyproject.toml` & `gama_client-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "gama_client"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Baptiste Lesquoy", email="baptistelesquoy@protonmail.com" },
 ]
 description = "A python library to interact with Gama server"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `gama_client-1.1.3/PKG-INFO` & `gama_client-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gama_client
-Version: 1.1.3
+Version: 1.1.4
 Summary: A python library to interact with Gama server
 Project-URL: Homepage, https://github.com/gama-platform/Gama-client-python
 Project-URL: Bug Tracker, https://github.com/gama-platform/Gama-client-python/issues
 Author-email: Baptiste Lesquoy <baptistelesquoy@protonmail.com>
 License: MIT License
         
         Copyright (c) 2022 Baptiste Lesquoy
@@ -31,15 +31,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: websockets~=10.3
 Description-Content-Type: text/markdown
 
 # Gama client
- Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the modeling and simulation platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.1.
+ Gama-client is a python wrapper for interacting with the headless mode (called gama-server) of the modeling and simulation platform [gama](https://gama-platform.org/). The latest release is compatible with gama 1.9.2.
 This wrapper will take care of the connection with gama-server and of sending properly formatted requests to gama-server. It is made to fit the asynchronous nature of gama-server and thus makes it possible to handle multiple simulations at the same time, but the counterpart is that the users will still have to manage what to do with the received messages (command confirmation, simulation output, errors etc.) by themselves. We provide a working example that shows the architecture you can deploy if you still want to have a sequential execution.
 
 # Installation
 In your python environment, install the gama-client package with the command:
 
 ```
 pip install gama-client
@@ -102,14 +102,20 @@
 ```
 or
 ```python
 await client.connect()
 ```
 And the client will take care of handling this first message and setting the `socket_id` by itself.
 
+To explicitly disconnect from gama-server, simply use the `close_connection` function:
+```python
+await client.close_connection()
+```
+you can later reconnect with the same `client` object the same way you did the first time, with the `connect` function.
+
 ### Running commands
 Once connected you will want to run commands, the principle is pretty simple: all commands can be run your `client` variable through functions. For example if you want to run the [load command](https://gama-platform.org/wiki/next/HeadlessServer#the-load-command) you just have to call the `load` function with the proper parameters.
 ```python
 await client.load("path/to/gaml/file", "my_experiment_name")
 ```
 
 ### Message handling
```

