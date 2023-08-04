# Comparing `tmp/pih-1.48033.tar.gz` & `tmp/pih-1.48034.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48033.tar", last modified: Fri Aug  4 01:29:21 2023, max compression
+gzip compressed data, was "pih-1.48034.tar", last modified: Fri Aug  4 01:33:29 2023, max compression
```

## Comparing `pih-1.48033.tar` & `pih-1.48034.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 01:29:21.702361 pih-1.48033/
--rw-rw-rw-   0        0        0      261 2023-08-04 01:29:21.686739 pih-1.48033/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 01:29:19.556405 pih-1.48033/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48033/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48033/pih/collection.py
--rw-rw-rw-   0        0        0    60753 2023-08-04 00:59:36.000000 pih-1.48033/pih/console_api.py
--rw-rw-rw-   0        0        0   109574 2023-08-04 01:03:56.000000 pih-1.48033/pih/const.py
--rw-rw-rw-   0        0        0   320963 2023-08-04 01:28:43.000000 pih-1.48033/pih/pih.py
--rw-rw-rw-   0        0        0    25242 2023-08-03 08:55:57.000000 pih-1.48033/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48033/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48033/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2528 2023-08-03 23:30:35.000000 pih-1.48033/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48033/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48033/pih/service_example.py
--rw-rw-rw-   0        0        0    38314 2023-08-04 01:09:15.000000 pih-1.48033/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48033/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-04 01:29:20.745554 pih-1.48033/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-04 01:29:12.000000 pih-1.48033/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-04 01:29:14.000000 pih-1.48033/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 01:29:12.000000 pih-1.48033/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-04 01:29:13.000000 pih-1.48033/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-04 01:29:13.000000 pih-1.48033/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48033/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-04 01:29:21.749281 pih-1.48033/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 01:33:17.897314 pih-1.48034/
+-rw-rw-rw-   0        0        0      261 2023-08-04 01:33:29.763343 pih-1.48034/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 01:33:27.368146 pih-1.48034/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48034/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48034/pih/collection.py
+-rw-rw-rw-   0        0        0    60753 2023-08-04 00:59:36.000000 pih-1.48034/pih/console_api.py
+-rw-rw-rw-   0        0        0   109574 2023-08-04 01:03:56.000000 pih-1.48034/pih/const.py
+-rw-rw-rw-   0        0        0   320963 2023-08-04 01:32:24.000000 pih-1.48034/pih/pih.py
+-rw-rw-rw-   0        0        0    25242 2023-08-03 08:55:57.000000 pih-1.48034/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48034/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48034/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2528 2023-08-03 23:30:35.000000 pih-1.48034/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6492 2023-08-03 06:51:54.000000 pih-1.48034/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48034/pih/service_example.py
+-rw-rw-rw-   0        0        0    38338 2023-08-04 01:31:31.000000 pih-1.48034/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48034/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-04 01:33:29.482095 pih-1.48034/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-04 01:33:16.000000 pih-1.48034/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-04 01:33:17.000000 pih-1.48034/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 01:33:16.000000 pih-1.48034/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-04 01:33:16.000000 pih-1.48034/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-04 01:33:16.000000 pih-1.48034/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2007 2023-08-03 07:28:58.000000 pih-1.48034/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-04 01:33:29.810218 pih-1.48034/setup.cfg
```

### Comparing `pih-1.48033/pih/collection.py` & `pih-1.48034/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48033/pih/console_api.py` & `pih-1.48034/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.48033/pih/const.py` & `pih-1.48034/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48033/pih/pih.py` & `pih-1.48034/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1648,15 +1648,15 @@
                     handler(message, close_handler)  
             PIH.EVENT.waiting_for_mobile_helper_message_input(
                 recipient, internal_handler)
             return PIH.MIO.ANSWER[recipient][-1] 
 
     class VERSION:
 
-        value: str = "1.48033"
+        value: str = "1.48034"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.value < PIH.VERSION.remote()
     
     class INPUT_WAIT:
```

### Comparing `pih-1.48033/pih/rpc.py` & `pih-1.48034/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48033/pih/rpcCommandCall_pb2.py` & `pih-1.48034/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48033/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48034/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48033/pih/rpc_collection.py` & `pih-1.48034/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48033/pih/rpc_const.py` & `pih-1.48034/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48033/pih/service_example.py` & `pih-1.48034/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48033/pih/tools.py` & `pih-1.48034/pih/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import socket
 from typing import Any
 import inspect
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
-from pih.const import PASSWORD_GENERATION_ORDER, CONST
+from pih.const import PASSWORD_GENERATION_ORDER, CONST, FieldCollectionAliases
 from pih.collection import R, T, FieldItem, FieldItemList, FullName, Result, User, PolibasePerson
 
 def if_else(check_value: bool, true_value: Callable[[None], Any | None] | Any, false_value: Callable[[None], Any | None] | Any = None) -> Any | None:
     return (true_value() if callable(true_value) else true_value) if check_value else (false_value() if not DataTool.is_none(false_value) and callable(false_value) else false_value)
 
 
 def i(value: str) -> str:
@@ -112,15 +112,15 @@
             if DataTool.is_empty(class_type_holder):
                 return item
             return class_type_holder(item) if callable(class_type_holder) and not inspect.isclass(class_type_holder) else DataTool.fill_data_from_source(
                 class_type_holder() if inspect.isclass(class_type_holder) else class_type_holder, item)
         def obtain_data() -> Any | None:
             return list(map(fill_data_with, data)) if isinstance(data, list) else fill_data_with(data)
         if "fields_alias" in result_object:
-            return Result(FieldItemList(EnumTool.get(FIELD_COLLECTION_ALIAS, result_object["fields_alias"]).value), obtain_data())
+            return Result(FieldItemList(EnumTool.get(FieldCollectionAliases, result_object["fields_alias"]).value), obtain_data())
         else:
             fields = None if "fields" not in result_object else result_object["fields"]
         field_list: list[FieldItem] = None
         if fields is not None:
             field_list = []
             for field_item in fields:
                 for field_name in field_item:
@@ -481,15 +481,15 @@
         return None
 
 class ResultTool:
 
     @staticmethod
     def pack(fields: Any, data: Any) -> dict:
         result: dict = {"data": data}
-        if isinstance(fields, FIELD_COLLECTION_ALIAS):
+        if isinstance(fields, FieldCollectionAliases):
             result["fields_alias"] = fields.name
         else:
             result["fields"] = fields
         return result
 
     @staticmethod
     def is_empty(result: Result | None) -> bool:
@@ -648,15 +648,15 @@
     @staticmethod
     def unpack(result: dict) -> tuple[FieldItemList, Any]:
         return ResultUnpack.unpack_fields(result), ResultUnpack.unpack_data(result)
 
     @staticmethod
     def unpack_fields(data: dict) -> Any:
         if "fields_alias" in data:
-            return FIELD_COLLECTION_ALIAS._member_map_[data["fields_alias"]].value,
+            return FieldCollectionAliases._member_map_[data["fields_alias"]].value,
         return data["fields"]
 
     @staticmethod
     def unpack_data(result: dict) -> Any:
         return result["data"]
```

### Comparing `pih-1.48033/pih/widgets.py` & `pih-1.48034/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48033/pih_setup.py` & `pih-1.48034/pih_setup.py`

 * *Files identical despite different names*

