# Comparing `tmp/slxjsonrpc-0.8.1.tar.gz` & `tmp/slxjsonrpc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slxjsonrpc-0.8.1.tar", last modified: Thu Nov 25 14:30:09 2021, max compression
+gzip compressed data, was "slxjsonrpc-0.9.0.tar", last modified: Fri Aug  4 08:32:01 2023, max compression
```

## Comparing `slxjsonrpc-0.8.1.tar` & `slxjsonrpc-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxrwxr-x   0 bach      (1000) bach      (1000)        0 2021-11-25 14:30:09.218181 slxjsonrpc-0.8.1/
--rw-rw-r--   0 bach      (1000) bach      (1000)     5246 2021-11-25 14:30:09.218181 slxjsonrpc-0.8.1/PKG-INFO
--rw-rw-r--   0 bach      (1000) bach      (1000)     3576 2021-11-25 14:27:43.000000 slxjsonrpc-0.8.1/README.md
--rw-rw-r--   0 bach      (1000) bach      (1000)       38 2021-11-25 14:30:09.218181 slxjsonrpc-0.8.1/setup.cfg
--rw-rw-r--   0 bach      (1000) bach      (1000)     1431 2021-11-12 13:31:51.000000 slxjsonrpc-0.8.1/setup.py
-drwxrwxr-x   0 bach      (1000) bach      (1000)        0 2021-11-25 14:30:09.218181 slxjsonrpc-0.8.1/slxjsonrpc/
--rw-rw-r--   0 bach      (1000) bach      (1000)      543 2021-11-25 14:28:00.000000 slxjsonrpc-0.8.1/slxjsonrpc/__init__.py
--rw-rw-r--   0 bach      (1000) bach      (1000)    18870 2021-11-25 14:28:00.000000 slxjsonrpc-0.8.1/slxjsonrpc/jsonrpc.py
--rw-rw-r--   0 bach      (1000) bach      (1000)     2172 2021-11-25 14:28:00.000000 slxjsonrpc-0.8.1/slxjsonrpc/jsonrpc.pyi
-drwxrwxr-x   0 bach      (1000) bach      (1000)        0 2021-11-25 14:30:09.218181 slxjsonrpc-0.8.1/slxjsonrpc/schema/
--rw-rw-r--   0 bach      (1000) bach      (1000)        8 2021-11-12 13:31:51.000000 slxjsonrpc-0.8.1/slxjsonrpc/schema/__init__.py
--rw-rw-r--   0 bach      (1000) bach      (1000)    11076 2021-11-25 14:27:43.000000 slxjsonrpc-0.8.1/slxjsonrpc/schema/jsonrpc.py
-drwxrwxr-x   0 bach      (1000) bach      (1000)        0 2021-11-25 14:30:09.218181 slxjsonrpc-0.8.1/slxjsonrpc.egg-info/
--rw-rw-r--   0 bach      (1000) bach      (1000)     5246 2021-11-25 14:30:09.000000 slxjsonrpc-0.8.1/slxjsonrpc.egg-info/PKG-INFO
--rw-rw-r--   0 bach      (1000) bach      (1000)      314 2021-11-25 14:30:09.000000 slxjsonrpc-0.8.1/slxjsonrpc.egg-info/SOURCES.txt
--rw-rw-r--   0 bach      (1000) bach      (1000)        1 2021-11-25 14:30:09.000000 slxjsonrpc-0.8.1/slxjsonrpc.egg-info/dependency_links.txt
--rw-rw-r--   0 bach      (1000) bach      (1000)       16 2021-11-25 14:30:09.000000 slxjsonrpc-0.8.1/slxjsonrpc.egg-info/requires.txt
--rw-rw-r--   0 bach      (1000) bach      (1000)       11 2021-11-25 14:30:09.000000 slxjsonrpc-0.8.1/slxjsonrpc.egg-info/top_level.txt
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 08:32:01.287698 slxjsonrpc-0.9.0/
+-rw-r--r--   0 bach      (1000) bach      (1000)      762 2023-08-03 13:25:00.000000 slxjsonrpc-0.9.0/CHANGELOG.md
+-rw-rw-r--   0 bach      (1000) bach      (1000)    11357 2022-03-14 08:12:47.000000 slxjsonrpc-0.9.0/LICENSE
+-rw-r--r--   0 bach      (1000) bach      (1000)      115 2023-08-02 09:50:26.000000 slxjsonrpc-0.9.0/MANIFEST.in
+-rw-r--r--   0 bach      (1000) bach      (1000)    10862 2023-08-04 08:32:01.286698 slxjsonrpc-0.9.0/PKG-INFO
+-rw-r--r--   0 bach      (1000) bach      (1000)     9676 2023-08-03 12:47:55.000000 slxjsonrpc-0.9.0/README.md
+-rw-r--r--   0 bach      (1000) bach      (1000)       38 2023-08-04 08:32:01.287698 slxjsonrpc-0.9.0/setup.cfg
+-rw-r--r--   0 bach      (1000) bach      (1000)     2323 2023-08-03 13:22:29.000000 slxjsonrpc-0.9.0/setup.py
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 08:32:01.282698 slxjsonrpc-0.9.0/slxjsonrpc/
+-rw-r--r--   0 bach      (1000) bach      (1000)      570 2023-08-03 13:28:39.000000 slxjsonrpc-0.9.0/slxjsonrpc/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      267 2023-08-04 07:52:18.000000 slxjsonrpc-0.9.0/slxjsonrpc/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    19840 2023-08-04 07:49:27.000000 slxjsonrpc-0.9.0/slxjsonrpc/jsonrpc.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     2036 2023-08-04 07:52:18.000000 slxjsonrpc-0.9.0/slxjsonrpc/jsonrpc.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)       62 2023-08-02 09:50:26.000000 slxjsonrpc-0.9.0/slxjsonrpc/py.typed
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 08:32:01.285698 slxjsonrpc-0.9.0/slxjsonrpc/schema/
+-rw-rw-r--   0 bach      (1000) bach      (1000)        8 2022-03-14 08:12:47.000000 slxjsonrpc-0.9.0/slxjsonrpc/schema/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-08-04 07:52:18.000000 slxjsonrpc-0.9.0/slxjsonrpc/schema/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    12516 2023-08-04 07:45:19.000000 slxjsonrpc-0.9.0/slxjsonrpc/schema/jsonrpc.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     2703 2023-08-04 08:29:15.000000 slxjsonrpc-0.9.0/slxjsonrpc/schema/jsonrpc.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 08:32:01.284698 slxjsonrpc-0.9.0/slxjsonrpc.egg-info/
+-rw-r--r--   0 bach      (1000) bach      (1000)    10862 2023-08-04 08:32:01.000000 slxjsonrpc-0.9.0/slxjsonrpc.egg-info/PKG-INFO
+-rw-r--r--   0 bach      (1000) bach      (1000)      452 2023-08-04 08:32:01.000000 slxjsonrpc-0.9.0/slxjsonrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)        1 2023-08-04 08:32:01.000000 slxjsonrpc-0.9.0/slxjsonrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)       16 2023-08-04 08:32:01.000000 slxjsonrpc-0.9.0/slxjsonrpc.egg-info/requires.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)       11 2023-08-04 08:32:01.000000 slxjsonrpc-0.9.0/slxjsonrpc.egg-info/top_level.txt
```

### Comparing `slxjsonrpc-0.8.1/setup.py` & `slxjsonrpc-0.9.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,85 @@
 from setuptools import find_packages
 from setuptools import setup
 
+import pathlib
 import codecs
 import os
 import re
 
 
-with open("README.md", "r") as file:
-    long_description = file.read()
-
+readme_file = pathlib.Path('README.md')
+changelog_file = pathlib.Path('CHANGELOG.md')
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 
+def get_long_description():
+    long_description = ""
+
+    if not readme_file.exists():
+        return ""
+
+    with readme_file.open("r") as file:
+        long_description += file.read()
+
+    long_description += "\n\n"
+
+    if not changelog_file.exists():
+        return long_description
+
+    with changelog_file.open("r") as file:
+        long_description += file.read()
+
+    return long_description
+
+
 def find_version(*file_paths):
     path = os.path.join(here, *file_paths)
     with codecs.open(path, 'r') as fp:
         version_file = fp.read()
         version_match = re.search(r"__version__ = ['\"]([^'\"]*)['\"]",
                                   version_file, re.M)
         if version_match:
             return version_match.group(1)
         raise RuntimeError("Unable to find version string.")
 
 
+def find_auther(*file_paths):
+    path = os.path.join(here, *file_paths)
+    with codecs.open(path, 'r') as fp:
+        auther_file = fp.read()
+        auther_match = re.search(r"__auther__ = ['\"]([^'\"]*)['\"]",
+                                 auther_file, re.M)
+        if auther_match:
+            return auther_match.group(1)
+        raise RuntimeError("Unable to find auther string.")
+
+
 setup(
     name="slxjsonrpc",
     version=find_version("slxjsonrpc", "__init__.py"),
-    author="Seluxit A/S",
+    author=find_auther("slxjsonrpc", "__init__.py"),
     author_email="support@seluxit.com",
     license="Apache-2.0",
     description="SlxJsonRpc JsonRpc helper class, that uses pydantic.",
-    long_description=long_description,
+    long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/Wappsto/slxjsonrpc",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent"
     ],
     packages=find_packages(),
     package_data={
-        'slxjsonrpc': ['jsonrpc.pyi'],
-        'slxjsonrpc/schema': ['schema/jsonrpc.pyi'],
+        'slxjsonrpc': ["py.typed", "*.pyi", "**/*.pyi"],
     },
     tests_require=[
         'pytest',
         'tox'
     ],
+    data_files=[('info', [readme_file.name, changelog_file.name])],
     install_requires=[
-       'pydantic>=1.6.1'
+       'pydantic>=2.1.1'
     ],
-    python_requires='>3.6.0',
+    python_requires='>3.6.15',
 )
```

### Comparing `slxjsonrpc-0.8.1/slxjsonrpc/__init__.py` & `slxjsonrpc-0.9.0/slxjsonrpc/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,8 +14,9 @@
     'RpcBatch',
     'RpcError',
     'RpcNotification',
     'RpcRequest',
     'RpcResponse',
 ]
 
-__version__ = "v0.8.1"
+__version__ = "v0.9.0"
+__auther__ = "Seluxit A/S"
```

### Comparing `slxjsonrpc-0.8.1/slxjsonrpc/jsonrpc.py` & `slxjsonrpc-0.9.0/slxjsonrpc/jsonrpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,39 +3,42 @@
 import json
 import logging
 
 from contextlib import contextmanager
 
 from typing import Any
 from typing import Callable
+from typing import Generator
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import overload
 from typing import Type
 from typing import Union
 
 from enum import Enum
 
-from pydantic import parse_obj_as
+from pydantic import TypeAdapter
 from pydantic import ValidationError
+from pydantic_core import ErrorDetails
 
 from slxjsonrpc.schema.jsonrpc import RpcBatch
 from slxjsonrpc.schema.jsonrpc import RpcError
 from slxjsonrpc.schema.jsonrpc import RpcNotification
 from slxjsonrpc.schema.jsonrpc import RpcRequest
 from slxjsonrpc.schema.jsonrpc import RpcResponse
 
 from slxjsonrpc.schema.jsonrpc import ErrorModel
+from slxjsonrpc.schema.jsonrpc import MethodError
+from slxjsonrpc.schema.jsonrpc import rpc_set_name
 from slxjsonrpc.schema.jsonrpc import RpcErrorCode
 from slxjsonrpc.schema.jsonrpc import RpcErrorMsg
-from slxjsonrpc.schema.jsonrpc import rpc_set_name
+from slxjsonrpc.schema.jsonrpc import set_id_mapping
 from slxjsonrpc.schema.jsonrpc import set_params_map
 from slxjsonrpc.schema.jsonrpc import set_result_map
-from slxjsonrpc.schema.jsonrpc import set_id_mapping
 
 RpcSchemas = Union[
     RpcError,
     RpcNotification,
     RpcRequest,
     RpcResponse
 ]
@@ -62,17 +65,17 @@
 
         Args:
             code: The Rpc Error code, within the range of -32000 to -32099
             msg: The Rpc Error message, that shortly describe the error for given code.
             data: (Optional) The Rpc Extended error message.
         """
         super().__init__()
-        self.code = code
-        self.msg = msg
-        self.data = data
+        self.code: Union[int, RpcErrorCode] = code
+        self.msg: str = msg
+        self.data: Optional[Any] = data
 
     def get_rpc_model(self, id: Union[str, int, None]) -> RpcError:
         """
         Returns a RpcError Response, for this given exception.
 
         The returned RpcError Model are used to send back to server,
         as a JsonRpc Error package.
@@ -119,39 +122,41 @@
         # noqa: D417
 
         Args:
             method: (Optional) A String-Enum, with all the acceptable methods.
                     If not given, will there not be make checks for any wrong methods.
             method_cb: The mapping for each given method to a function call. (Server only)
                         callback: The function to be call when data is received.
-                                  The Callback gets the params definded in as args,
+                                  The Callback gets the params defined in as args,
                                   & should return the Result defined.
                                   If an error happens, and custom error code
                                   are needed, to send back, raise the RpcErrorException
                                   in the callback.
             result: (Optional) The method & 'result' mapping.
                     If not given, will there not be make checks for any wrong 'result'.
             params: (Optional) The Parser method & 'params' mapping.
                     If not given, will there not be make checks for any wrong 'params'.
         """
-        self.log = logging.getLogger(__name__)
+        self.log: logging.Logger = logging.getLogger(__name__)
         self.log.addHandler(logging.NullHandler())
 
         rpc_set_name(None)
         if methods:
             RpcRequest.update_method(methods)
             RpcNotification.update_method(methods)
         if params:
             set_params_map(params)
         if result:
             set_result_map(result)
 
         self.__batch_lock: int = 0
         self.__batched_list: List[RpcSchemas] = []
 
+        self.__parse_as_rpc_obj: TypeAdapter = TypeAdapter(RpcSchemas)  # type: ignore
+
         self._method_cb: Dict[Union[Enum, str], Callable[[Any], Any]] = method_cb if method_cb else {}
 
         self._id_cb: Dict[Union[str, int, None], Callable[[Any], None]] = {}
         self._id_error_cb: Dict[Union[str, int, None], Callable[[Any], None]] = {}
         self._id_method: Dict[Union[str, int, None], Union[Enum, str]] = {}
 
         set_id_mapping(self._id_method)
@@ -171,15 +176,15 @@
         for the given request are received (through the parser-method),
         it will be passed on to the callback.
 
         Args:
             method: Should be a apart of the given Method Enum, given on init,
                     or if not given, a string.
             callback: The function to be called when data is received.
-                      The Callback gets the Result datamodel (if set)
+                      The Callback gets the Result data model (if set)
                       else a Dict/List back as argument.
             error_callback: (Optional) The function to be called, when an error
                             have happened.
                             The callback gets an ErrorModel object as parameter.
             params: (Optional) Should be fitting the a DataModel,
                     if given on init, else a valid Dictionary or List.
 
@@ -190,21 +195,36 @@
             ValidationError, if the given data do not fit the given Schema.
         """
         r_data = RpcRequest(
             method=method,
             params=params
         )
 
-        self._id_cb[r_data.id] = callback
-        if error_callback:
-            self._id_error_cb[r_data.id] = error_callback
-        self._id_method[r_data.id] = method
+        self._add_result_handling(
+            method=method,
+            _id=r_data.id,
+            callback=callback,
+            error_callback=error_callback
+        )
 
         return self._batch_filter(r_data)
 
+    def _add_result_handling(
+        self,
+        method: Union[Enum, str],
+        _id: Union[str, int, None],
+        callback: Callable[[Any], None],
+        error_callback: Optional[Callable[[ErrorModel], None]] = None,
+    ) -> None:
+        """Added handling for when a result comes back."""
+        self._id_cb[_id] = callback
+        if error_callback:
+            self._id_error_cb[_id] = error_callback
+        self._id_method[_id] = method
+
     def create_notification(
         self,
         method: Union[Enum, str],
         params: Optional[Any] = None,
     ) -> Optional[RpcNotification]:
         """
         Create a JsonRpc Notification, with given method & params.
@@ -233,15 +253,15 @@
         return self._batch_filter(r_data)
 
     # -------------------------------------------------------------------------
     #                          Batching Functions
     # -------------------------------------------------------------------------
 
     @contextmanager
-    def batch(self):
+    def batch(self) -> Generator[None, None, None]:
         """Batch RPC's within the context manager, into one RPC-Batch-List."""
         self.__batch_lock += 1
         try:
             yield
         finally:
             self.__batch_lock -= 1
 
@@ -267,19 +287,19 @@
             RpcBatch, if there was batch anything.
             None, if nothing was batch.
         """
         if len(self.__batched_list) < 1:
             return None
         if data:
             self.__batched_list.append(data)
-        sdata = self.__batched_list.copy()
+        batched_data = self.__batched_list.copy()
         self.__batched_list.clear()
-        if len(sdata) == 1:
-            return sdata[0]
-        return parse_obj_as(RpcBatch, sdata)
+        if len(batched_data) == 1:
+            return batched_data[0]
+        return RpcBatch.model_validate(batched_data)
 
     @overload
     def _batch_filter(self, data: RpcError) -> Optional[RpcError]: ...  # noqa: E704
 
     @overload
     def _batch_filter(self, data: RpcNotification) -> Optional[RpcNotification]: ...  # noqa: E704
 
@@ -311,15 +331,15 @@
 
     # -------------------------------------------------------------------------
     #                          Parsing Functions
     # -------------------------------------------------------------------------
 
     def parser(
         self,
-        data: Union[bytes, str, dict, list]
+        data: Union[bytes, str, Dict[str, Any], List[Dict[str, Any]]]
     ) -> Optional[Union[RpcError, RpcResponse, RpcBatch]]:
         """
         Parse raw JsonRpc data, & returns the Response or Error.
 
         For the Parsed data, there will be make a check for any method
         callbacks, if found, the callback(s) will be called for the given data,
         and the return value from the callback will be packed into, a jsonrpc
@@ -332,15 +352,15 @@
             data: The Raw data to be parsed.
 
         Returns:
             The fitting JsonRpc reply to the given data.
             None, if no reply are needed.
         """
         try:
-            j_data: Union[dict, list]
+            j_data: Union[Dict[str, Any], List[Dict[str, Any]]]
             if isinstance(data, dict) or isinstance(data, list):
                 j_data = data
             else:
                 j_data = json.loads(data)
 
         except json.decoder.JSONDecodeError as err:
             return self._batch_filter(RpcError(
@@ -371,30 +391,30 @@
                         id=f_data['id'] if 'id' in f_data else None,
                     ))
                     continue
                 if temp:
                     r_data = self.__reply_logic(temp)
                     if r_data:
                         b_data.append(r_data)
-                # UNSURE: Is it requerid to return a batch of 1, if it was received as batch of 1?
+                # UNSURE: Is it required to return a batch of 1, if it was received as batch of 1?
 
-            return parse_obj_as(RpcBatch, b_data) if b_data else None
+            return RpcBatch.model_validate(b_data) if b_data else None
 
         try:
             p_data = self._parse_data(j_data)
         except RpcErrorException as err:
             return self._batch_filter(err.get_rpc_model(
                 id=j_data['id'] if 'id' in j_data else None,
             ))
         return self.__reply_logic(p_data)
 
     def __reply_logic(
         self,
         p_data: RpcSchemas
-    ) -> Union[RpcError, RpcResponse, None]:
+    ) -> Optional[Union[RpcResponse, RpcError]]:
         try:
             if isinstance(p_data, RpcError):
                 return self._error_reply_logic(data=p_data)
 
             elif isinstance(p_data, RpcNotification):
                 return self._notification_reply_logic(data=p_data)
 
@@ -418,43 +438,45 @@
                     message=RpcErrorMsg.InternalError,
                     data=err.args[0]
                 )
             ))
 
         return None
 
-    def _error_reply_logic(self, data):
+    def _error_reply_logic(self, data: RpcError) -> Optional[RpcError]:
         if data.id not in self._id_cb.keys():
             # NOTE: Triggers only if it was an error that we generated.
             return data
         self._id_cb.pop(data.id)
         if data.id not in self._id_error_cb.keys():
             self.log.warning(f"Unhanded error: {data}")
         else:
             with self._except_handler():
                 cb = self._id_error_cb.pop(data.id)
                 self.log.debug(f"Exec Error CB: {cb}")
                 cb(data.error)
+        return None
 
-    def _notification_reply_logic(self, data):
+    def _notification_reply_logic(self, data: RpcNotification) -> Optional[RpcError]:
         if data.method not in self._method_cb.keys():
             return self._batch_filter(RpcError(
                 id=None,
                 error=ErrorModel(
                     code=RpcErrorCode.MethodNotFound,
                     message=RpcErrorMsg.MethodNotFound,
                     data=data.method
                 )
             ))
         with self._except_handler():
             cb = self._method_cb[data.method]
             self.log.debug(f"Exec Notification CB: {cb}")
             cb(data.params)
+        return None
 
-    def _request_reply_logic(self, data):
+    def _request_reply_logic(self, data: RpcRequest) -> Optional[Union[RpcResponse, RpcError]]:
         if data.method in self._method_cb.keys():
             with self._except_handler():
                 cb = self._method_cb[data.method]
                 self.log.debug(f"Request CB: {cb}")
                 result = cb(data.params)
             return self._batch_filter(RpcResponse(
                 id=data.id,
@@ -465,53 +487,48 @@
             error=ErrorModel(
                 code=RpcErrorCode.MethodNotFound,
                 message=RpcErrorMsg.MethodNotFound,
                 data=data.method
             )
         ))
 
-    def _response_reply_logic(self, data):
+    def _response_reply_logic(self, data: RpcResponse) -> Optional[RpcResponse]:
         if data.id not in self._id_cb.keys():
             self.log.warning(f"Received an unknown RpcResponse: {data}")
         else:
             self._id_error_cb.pop(data.id, None)
             with self._except_handler():
                 cb = self._id_cb.pop(data.id)
                 self.log.debug(f"Exec Response CB: {cb}")
                 cb(data.result)
+        return None
 
     @contextmanager
-    def _except_handler(self):
+    def _except_handler(self) -> Generator[None, None, None]:
         try:
             yield
         except RpcErrorException:
             raise
         except Exception as err:
-            # NOTE: Only trickered from user given function, or if it was not a function
+            # NOTE: Only triggered from user given function, or if it was not a function
+            self.log.exception("An error happened doing execution of a callback.")
             raise RpcErrorException(
                 code=RpcErrorCode.ServerError,
                 msg=RpcErrorMsg.ServerError,
                 data=err.args[0]
             ).with_traceback(err.__traceback__)
 
     def __ValidationError2ErrorModel(
         self,
-        errors: List[Dict[str, Union[List[str], str, Dict[str, List[str]]]]]
+        errors: List[ErrorDetails]
     ) -> Optional[ErrorModel]:
         # TODO (MBK): Find a faster/better way to do this!
-        method_error = list(filter(lambda x: x.get('type') == "type_error.enum", errors))
-        params_error = list(filter(lambda x: x.get('loc') == ('__root__', 'params', '__root__'), errors))
-        type_error = list(filter(lambda x: x.get('type') in ["value_error.missing", "value_error.extra"], errors))
-        if method_error:
-            raise RpcErrorException(
-                code=RpcErrorCode.MethodNotFound,
-                msg=RpcErrorMsg.MethodNotFound,
-                data=method_error[0]
-            )
-        elif params_error:
+        params_error = list(filter(lambda x: x['loc'][1] == 'params', errors))
+        type_error = list(filter(lambda x: x['type'] in ["missing", "extra_forbidden"], errors))
+        if params_error:
             raise RpcErrorException(
                 code=RpcErrorCode.InvalidParams,
                 msg=RpcErrorMsg.InvalidParams,
                 data=params_error[0]
             )
         elif type_error:
             raise RpcErrorException(
@@ -520,20 +537,23 @@
                 data=type_error[0]
             )
 
         return None
 
     def _parse_data(
         self,
-        data: dict
+        data: Dict[str, Any]
     ) -> RpcSchemas:
         try:
-            p_data: RpcSchemas = parse_obj_as(
-                RpcSchemas,  # type: ignore
-                data
+            p_data: RpcSchemas = self.__parse_as_rpc_obj.validate_python(data)
+        except MethodError as error:
+            raise RpcErrorException(
+                code=RpcErrorCode.MethodNotFound,
+                msg=RpcErrorMsg.MethodNotFound,
+                data=error.args[0]
             )
         except ValidationError as error:
             error_package = self.__ValidationError2ErrorModel(
                 errors=error.errors()
             )
 
             if not error_package:
```

### Comparing `slxjsonrpc-0.8.1/slxjsonrpc/schema/jsonrpc.py` & `slxjsonrpc-0.9.0/slxjsonrpc/schema/jsonrpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 The slxJsonRpc are build with the specification in mind, listed here:
     https://www.jsonrpc.org/specification
 """
 import random
 import string
 
 from enum import Enum
+from enum import IntEnum
 
 from pydantic import BaseModel
-from pydantic import Extra
+from pydantic import ConfigDict
 from pydantic import Field
-from pydantic import validator
-from pydantic import parse_obj_as
-from pydantic.fields import ModelField
+from pydantic import field_validator
+from pydantic import FieldValidationInfo
+from pydantic import RootModel
+from pydantic import TypeAdapter
+from pydantic.fields import FieldInfo
 
 
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
@@ -51,14 +54,19 @@
     global _session_id
     global _RpcName
     rpc_name = name if name else _RpcName
     _session_count += 1
     return f"{_session_id}_{rpc_name}_{_session_count}"
 
 
+class MethodError(Exception):
+    """Exception to track if the Method is wrong."""
+    pass
+
+
 class RpcVersion(str, Enum):
     """The supported JsonRpc versions."""
     v2_0 = "2.0"
 
 
 ###############################################################################
 #                             JsonRpc Request Object
@@ -75,59 +83,63 @@
 
 class RpcRequest(BaseModel):
     """
     The Standard JsonRpc Request Schema, used to do a request of the server.
 
     Attributes:
         jsonrpc: The JsonRpc version this schema is using. (Default v2.0)
-        id: A identifier set by the client. (Is emitted it will be auto generated)
+        id: A identifier set by the client. (If emitted it will be auto generated)
         method: The name of the method to be invoked.
         params: (Optional) The input parameters for the invoked method.
     """
     jsonrpc: Optional[RpcVersion] = RpcVersion.v2_0
     method: str
-    id: Optional[Union[str, int]] = None
-    params: Optional[Any]
+    id: Optional[Union[str, int]] = Field(default=None, validate_default=True)
+    params: Optional[Any] = Field(default=None, validate_default=True)
 
-    class Config:
-        """Enforce that there can not be added extra keys to the BaseModel."""
-        extra = Extra.forbid
+    """Enforce that there can not be added extra keys to the BaseModel."""
+    model_config: ConfigDict = ConfigDict(extra='forbid')  # type: ignore
 
-    @validator('id', pre=True, always=True)
-    def id_autofill(cls, v, values, **kwargs) -> str:
+    @field_validator('id', mode='before')
+    def id_autofill(cls, v: Optional[Union[str, int]], info: FieldValidationInfo) -> Union[str, int]:
         """Validate the id, and auto-fill it is not set."""
-        return v or _id_gen(name=rpc_get_name() or values.get('method'))
+        return v or _id_gen(name=rpc_get_name() or info.data.get('method'))
 
     @classmethod
     def update_method(cls, new_type: Enum) -> None:
         """Update the Method schema, to fit the new one."""
-        new_fields = ModelField.infer(
-            name="method",
-            value=...,
+        cls.model_fields['method'] = FieldInfo(
             annotation=new_type,
-            class_validators=None,
-            config=cls.__config__
         )
-        cls.__fields__['method'] = new_fields
         cls.__annotations__['method'] = new_type
 
-    @validator("params", pre=True, always=True)
-    def method_params_mapper(cls, v, values, **kwargs) -> Any:
+    @field_validator("params")
+    def method_params_mapper(cls, v: Optional[Any], info: FieldValidationInfo) -> Any:
         """Check & enforce the params schema, depended on the method value."""
         global params_mapping
 
         if not params_mapping.keys():
             return v
 
-        if values.get('method') not in params_mapping.keys():
-            raise ValueError(f"Not valid params fro method: {values.get('method')}.")
+        if info.data.get('method') is None:
+            # UNSURE: Why is this needed, when MethodError is use instead of ValueError? o.0
+            return v
+
+        if info.data.get('method') not in params_mapping.keys():
+            raise MethodError(f"Unknown method: {info.data.get('method')}.")
+
+        model = params_mapping[str(info.data.get('method'))]
+
+        if isinstance(model, BaseModel):
+            return model.model_validate(v)
 
-        model = params_mapping[values.get('method')]
         if model is not None:
-            return parse_obj_as(model, v)
+            model_converter: TypeAdapter = TypeAdapter(model)  # type: ignore
+            return model_converter.validate_python(v)
+
         if v:
             raise ValueError("params should not be set.")
 
 
 class RpcNotification(BaseModel):
     """
     The Standard JsonRpc Notification Schema, to Notifies the server of change.
@@ -137,47 +149,51 @@
     Attributes:
         jsonrpc: The JsonRpc version this schema is using. (Default v2.0)
         method: The name of the method to be invoked.
         params: (Optional) The input parameters for the invoked method.
     """
     jsonrpc: Optional[RpcVersion] = RpcVersion.v2_0
     method: str
-    params: Optional[Any]
+    params: Optional[Any] = Field(default=None, validate_default=True)
 
-    class Config:
-        """Enforce that there can not be added extra keys to the BaseModel."""
-        extra = Extra.forbid
+    """Enforce that there can not be added extra keys to the BaseModel."""
+    model_config: ConfigDict = ConfigDict(extra='forbid')  # type: ignore
 
     @classmethod
     def update_method(cls, new_type: Enum) -> Any:
         """Update the Method schema, to fit the new one."""
-        new_fields = ModelField.infer(
-            name="method",
-            value=...,
+        cls.model_fields['method'] = FieldInfo(
             annotation=new_type,
-            class_validators=None,
-            config=cls.__config__
         )
-        cls.__fields__['method'] = new_fields
         cls.__annotations__['method'] = new_type
 
-    @validator("params", pre=True, always=True)
-    def method_params_mapper(cls, v, values, **kwargs) -> Any:
+    @field_validator("params")
+    def method_params_mapper(cls, v: Optional[Any], info: FieldValidationInfo) -> Any:
         """Check & enforce the params schema, depended on the method value."""
         global params_mapping
 
         if not params_mapping.keys():
             return v
 
-        if values.get('method') not in params_mapping.keys():
-            raise ValueError(f"Not valid params fro method: {values.get('method')}.")
+        if info.data.get('method') is None:
+            # UNSURE: Why is this needed, when MethodError is use instead of ValueError? o.0
+            return v
+
+        if info.data.get('method') not in params_mapping.keys():
+            raise MethodError(f"Unknown method: {info.data.get('method')}.")
+
+        model = params_mapping[str(info.data.get('method'))]
+
+        if isinstance(model, BaseModel):
+            return model.model_validate(v)
 
-        model = params_mapping[values.get('method')]
         if model is not None:
-            return parse_obj_as(model, v)
+            model_converter: TypeAdapter = TypeAdapter(model)  # type: ignore
+            return model_converter.validate_python(v)
+
         if v:
             raise ValueError("params should not be set.")
 
 
 ###############################################################################
 #                          JsonRpc Response Object
 ###############################################################################
@@ -196,63 +212,66 @@
 def set_result_map(mapping: Dict[Union[Enum, str], Union[type, Type[Any]]]) -> None:
     """Set the method to params schema mapping."""
     global result_mapping
     result_mapping = mapping
 
 
 class RpcResponse(BaseModel):
-    """
-    The Standard JsonRpc Response Schema, that is responded with.
+    """The Standard JsonRpc Response Schema, that is responded with.
 
     Attributes:
         jsonrpc: The JsonRpc version this schema is using. (Default v2.0)
         id: Must be the same value as the object this is a response to.
         result: The result of the Request object, if it did not fail.
     """
     jsonrpc: Optional[RpcVersion] = RpcVersion.v2_0
     id: Union[str, int]
-    result: Any
+    result: Any = Field(validate_default=True)
 
-    class Config:
-        """Enforce that there can not be added extra keys to the BaseModel."""
-        extra = Extra.forbid
+    """Enforce that there can not be added extra keys to the BaseModel."""
+    model_config: ConfigDict = ConfigDict(extra='forbid')  # type: ignore
 
-    @validator("result", pre=True, always=True)
-    def method_params_mapper(cls, v, values, **kwargs) -> Any:
+    @field_validator("result", mode='before')
+    def method_params_mapper(cls, v: Any, info: FieldValidationInfo) -> Any:
         """Check & enforce the params schema, depended on the method value."""
         global result_mapping
         global method_id_mapping
 
         if not result_mapping.keys():
             return v
 
-        the_id = values.get('id')
+        the_id = info.data.get('id')
 
         if the_id not in id_mapping:
-            # UNSURE (MBK): What should done, when it was not ment for this receiver?
+            # UNSURE (MBK): What should done, when it was not meant for this receiver?
             return v
 
         the_method = id_mapping[the_id]
 
         if the_method not in result_mapping.keys():
-            raise ValueError(f"Not valid params for method: {values.get('method')}.")
+            raise ValueError(f"Not valid params for method: {info.data.get('method')}.")
 
         model = result_mapping[the_method]
+
+        if isinstance(model, BaseModel):
+            return model.model_validate(v)
+
         if model is not None:
-            return parse_obj_as(model, v)
+            model_converter: TypeAdapter = TypeAdapter(model)  # type: ignore
+            return model_converter.validate_python(v)
 
         if v:
             raise ValueError("result should not be set.")
 
 
 ###############################################################################
 #                             JsonRpc Error Object
 ###############################################################################
 
-class RpcErrorCode(Enum):
+class RpcErrorCode(IntEnum):
     """
     JsonRpc Standard Error Codes.
 
     Error Codes:    Error code:         Message Description:
     ---
         -32700      Parse error         Invalid JSON was received by the server.
                                         An error occurred on the server while parsing the JSON text.
@@ -303,21 +322,34 @@
     The Default JsonRpc Error message, that is responded with on error.
 
     Attributes:
         code: The error code.
         message: A short describing of the error.
         data: (Optional), a Additional information of the error.
     """
-    code: Union[RpcErrorCode, int] = Field(None, le=-32001, ge=-32099)
+    code: Union[int, RpcErrorCode]
     message: str
-    data: Optional[Any]
+    data: Optional[Any] = None
+
+    """Enforce that there can not be added extra keys to the BaseModel."""
+    model_config: ConfigDict = ConfigDict(extra='forbid')  # type: ignore
+
+    @field_validator("code")
+    def method_code_parser(
+        cls,
+        v: Union[str, bytes, int, float],
+        info: FieldValidationInfo
+    ) -> Union[int, RpcErrorCode]:
+        """Error code parser."""
+        value = int(v)
+
+        if -32100 < value < -32000:
+            return value
 
-    class Config:
-        """Enforce that there can not be added extra keys to the BaseModel."""
-        extra = Extra.forbid
+        return RpcErrorCode(value)
 
 
 class RpcError(BaseModel):
     """
     The default JsonRpc Error Reply Schema.
 
     Attributes:
@@ -330,15 +362,15 @@
     error: ErrorModel
 
 
 ###############################################################################
 #                             JsonRpc Batch Object
 ###############################################################################
 
-class RpcBatch(BaseModel):
+class RpcBatch(RootModel[List[Union[RpcRequest, RpcNotification, RpcResponse, RpcError]]]):
     """The Default JsonRpc Batch Schema."""
-    __root__: List[Union[
+    root: List[Union[
         RpcRequest,
         RpcNotification,
         RpcResponse,
         RpcError,
-    ]] = Field(..., min_items=1)
+    ]] = Field(..., min_length=1)
```

