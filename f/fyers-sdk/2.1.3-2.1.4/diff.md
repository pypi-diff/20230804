# Comparing `tmp/fyers_sdk-2.1.3.tar.gz` & `tmp/fyers_sdk-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-2.1.3.tar", last modified: Wed Aug  2 03:49:46 2023, max compression
+gzip compressed data, was "fyers_sdk-2.1.4.tar", last modified: Fri Aug  4 13:40:07 2023, max compression
```

## Comparing `fyers_sdk-2.1.3.tar` & `fyers_sdk-2.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-02 03:49:46.533696 fyers_sdk-2.1.3/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.3/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-02 03:49:46.533696 fyers_sdk-2.1.3/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.3/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-02 03:49:46.497690 fyers_sdk-2.1.3/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-02 03:49:46.533696 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    60166 2023-08-02 03:49:31.000000 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     9833 2023-08-01 11:59:36.000000 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    13641 2023-08-01 12:03:31.000000 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.3/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27959 2023-08-01 12:53:43.000000 fyers_sdk-2.1.3/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.3/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-02 03:49:46.521694 fyers_sdk-2.1.3/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-02 03:49:46.000000 fyers_sdk-2.1.3/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-02 03:49:46.000000 fyers_sdk-2.1.3/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-02 03:49:46.000000 fyers_sdk-2.1.3/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      115 2023-08-02 03:49:46.000000 fyers_sdk-2.1.3/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-02 03:49:46.000000 fyers_sdk-2.1.3/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-02 03:49:46.533696 fyers_sdk-2.1.3/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-08-02 03:47:35.000000 fyers_sdk-2.1.3/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-04 13:40:07.285150 fyers_sdk-2.1.4/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.4/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-04 13:40:07.285150 fyers_sdk-2.1.4/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.4/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-04 13:40:07.249151 fyers_sdk-2.1.4/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-04 13:40:07.281150 fyers_sdk-2.1.4/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.4/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    61782 2023-08-04 13:39:41.000000 fyers_sdk-2.1.4/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.1.4/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     9833 2023-08-02 11:15:05.000000 fyers_sdk-2.1.4/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15350 2023-08-04 05:44:36.000000 fyers_sdk-2.1.4/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.4/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27346 2023-08-04 10:33:40.000000 fyers_sdk-2.1.4/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.4/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-04 13:40:07.269150 fyers_sdk-2.1.4/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-04 13:40:06.000000 fyers_sdk-2.1.4/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-04 13:40:07.000000 fyers_sdk-2.1.4/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-04 13:40:06.000000 fyers_sdk-2.1.4/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      115 2023-08-04 13:40:06.000000 fyers_sdk-2.1.4/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-04 13:40:06.000000 fyers_sdk-2.1.4/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-04 13:40:07.285150 fyers_sdk-2.1.4/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-08-04 13:39:18.000000 fyers_sdk-2.1.4/setup.py
```

### Comparing `fyers_sdk-2.1.3/LICENSE.txt` & `fyers_sdk-2.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.3/PKG-INFO` & `fyers_sdk-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 2.1.3
+Version: 2.1.4
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.1.3/README.md` & `fyers_sdk-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-2.1.4/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,15 @@
         self.channels = []
         self.running_channels = set()
         self.data_type = None
         self.OnMessage = on_message
         self.OnError = on_error
         self.OnOpen = on_connect
         self.OnClose = on_close
+        self.UpdateTick = False
         self.ack_count = 0
         self.__ws_run = None
         self.write_to_file = write_to_file
         self.background_flag = False
         self.update_count = 0
         self.literesp = {}
         self.channel_symbol = []
@@ -891,53 +892,55 @@
             data (bytearray): The response data.
             data_type (str): The type of data to be processed.
 
         Returns:
             object: The processed output based on the specified data_type.
         """
         try:
+            # print(data, "\n")
             data_resp = data
+            precision_calcu_value = [
+                                    "ltp",
+                                    "bid_price",
+                                    "ask_price",
+                                    "avg_trade_price",
+                                    "low_price",
+                                    "high_price",
+                                    "open_price",
+                                    "prev_close_price",
+                                ]
             response = {}
             if (
                 "bidPrice1" not in data_resp
                 # and "vol_traded_today" in data_resp
                 and self.lite
             ):
                 for i, val in enumerate(self.lite_val):
                     if val in data_resp and val == "ltp":
-                        response[val] = data_resp[val] / (10 ** data_resp["precision"])
+                        response[val] = data_resp[val] / (10 ** (data_resp["precision"] * 1) )
                     else:
                         response[val] = data_resp[val]
             else:
                 if data_type == "depth":
 
                     for i, val in enumerate(self.depthvalue):
                         if val in data_resp and i < 10:
                             response[val] = data_resp[val] / (
-                                10 ** data_resp["precision"]
-                            )
+                                10 ** data_resp["precision"] * data_resp["multiplier"])
+
                         elif val in data_resp:
                             response[val] = data_resp[val]
                 elif data_type == "scrips":
                     for i, val in enumerate(self.data_val):
-                        if val in data_resp and i in [
-                            0,
-                            6,
-                            7,
-                            11,
-                            13,
-                            14,
-                            17,
-                            18,
-                            19,
-                            20
-                        ]:
+                        if val in data_resp and val in precision_calcu_value and val not in ["upper_ckt", "lower_ckt"]:
                             response[val] = data_resp[val] / (
-                                10 ** data_resp["precision"]
+                                10 ** (data_resp["precision"] * data_resp["multiplier"])
                             )
+                            # response[val] = data_resp[val] / (
+
                         elif val in data_resp:
                             response[val] = data_resp[val]
                     if "prev_close_price" in response and "ltp" in response:
                         response["ch"] = round((response['ltp']  - response['prev_close_price']),2) 
                         response["chp"] = round((response["ch"]  / response['prev_close_price'] * 100) , 2)
                     if "OI" in response:
                         response.pop("OI")
@@ -945,22 +948,24 @@
                         response.pop("Yhigh")
                     if "Ylow" in response:
                         response.pop("Ylow")
                 else:
                     for i, val in enumerate(self.index_val):
                         if val in data_resp and i in [0, 1, 3, 4, 5]:
                             response[val] = data_resp[val] / (
-                                10 ** data_resp["precision"]
+                                10 ** (data_resp["precision"] * data_resp["multiplier"])
                             )
                         elif val in data_resp:
                             response[val] = data_resp[val]
                         if "prev_close_price" in response and "ltp" in response:
                             response["ch"] = round((response['ltp']  - response['prev_close_price']),2) 
                             response["chp"] = round((response["ch"]  / response['prev_close_price'] * 100) , 2)
-
+            response["lower_ckt"] = 0
+            response["upper_ckt"] = 0
+            
             self.On_message(response)
 
         except Exception as e:
             self.data_logger.exception(e)
 
     def __datafeed_resp(self, data: bytearray):
 
@@ -1012,18 +1017,17 @@
                             offset += 4
                             self.resp[self.dp_sym[topic_id]][
                                 self.depthvalue[index]
                             ] = value
 
                         offset += 2
 
-                        multiplier = struct.unpack("H", data[offset : offset + 2])[0]
+                        multiplier = struct.unpack(">H", data[offset : offset + 2])[0]
                         self.resp[self.dp_sym[topic_id]]["multiplier"] = multiplier
                         offset += 2
-
                         precision = struct.unpack("B", data[offset : offset + 1])[0]
                         self.resp[self.dp_sym[topic_id]]["precision"] = precision
                         offset += 1
 
                         val = ["exchange", "exchange_token", "symbol"]
                         for i in range(3):
                             string_len = struct.unpack("B", data[offset : offset + 1])[
@@ -1049,22 +1053,22 @@
                         # field_count - 21 in scrips , 25 in depth , 6 in index
                         field_count = struct.unpack("B", data[offset : offset + 1])[0]
                         offset += 1
 
                         for index in range(field_count):
                             value = struct.unpack(">I", data[offset : offset + 4])[0]
                             offset += 4
-
+                            print(struct.unpack(">I", data[offset : offset + 4]))
                             self.resp[self.index_sym[topic_id]][
                                 self.index_val[index]
                             ] = value
 
                         offset += 2
 
-                        multiplier = struct.unpack("H", data[offset : offset + 2])[0]
+                        multiplier = struct.unpack(">H", data[offset : offset + 2])[0]
                         self.resp[self.index_sym[topic_id]]["multiplier"] = multiplier
                         offset += 2
 
                         precision = struct.unpack("B", data[offset : offset + 1])[0]
                         self.resp[self.index_sym[topic_id]]["precision"] = precision
                         offset += 1
 
@@ -1098,17 +1102,19 @@
                             offset += 4
                             self.resp[self.scrips_sym[topic_id]][
                                 self.data_val[index]
                             ] = value
 
                         offset += 2
 
-                        multiplier = struct.unpack("H", data[offset : offset + 2])[0]
+                        multiplier = struct.unpack(">H", data[offset : offset + 2])[0]
                         self.resp[self.scrips_sym[topic_id]]["multiplier"] = multiplier
                         offset += 2
+                        print("multiplier : ", multiplier)
+
 
                         precision = struct.unpack("B", data[offset : offset + 1])[0]
                         self.resp[self.scrips_sym[topic_id]]["precision"] = precision
                         offset += 1
                         val = ["exchange", "exchange_token", "symbol"]
                         for i in range(3):
                             string_len = struct.unpack("B", data[offset : offset + 1])[
@@ -1130,47 +1136,58 @@
                     offset += 1
                     topic_id = struct.unpack("H", data[offset : offset + 2])[0]
                     offset += 2
 
                     field_count = struct.unpack("B", data[offset : offset + 1])[0]
                     offset += 1
                     sf_flag, idx_flag, dp_flag = False, False, False
-
+                    self.UpdateTick = False
                     for index in range(field_count):
                         value = struct.unpack(">I", data[offset : offset + 4])[0]
                         offset += 4
                         # if field_count == 20 or field_count == 21:
                         if topic_id in self.scrips_sym:
-                            self.resp[self.scrips_sym[topic_id]][
-                                self.data_val[index]
-                            ] = value
+                            if self.resp[self.scrips_sym[topic_id]][
+                                self.data_val[index]] != value and value != "2147483648":
+                                self.resp[self.scrips_sym[topic_id]][
+                                    self.data_val[index]
+                                ] = value
+                                self.UpdateTick = True
                             sf_flag = True
                         elif topic_id in self.index_sym:
-                            self.resp[self.index_sym[topic_id]][
-                                self.index_val[index]
-                            ] = value
+                            if self.resp[self.index_sym[topic_id]][
+                                self.index_val[index]] != value:
+
+                                self.resp[self.index_sym[topic_id]][
+                                    self.index_val[index]
+                                ] = value
+                                self.UpdateTick = True
                             idx_flag = True
                         elif topic_id in self.dp_sym:
-                            self.resp[self.dp_sym[topic_id]][
-                                self.depthvalue[index]
-                            ] = value
-                            dp_flag = True
-                    if sf_flag:
-                        self.__response_output(
-                            self.resp[self.scrips_sym[topic_id]], "scrips"
-                        )
-                    elif idx_flag:
+                            if self.resp[self.dp_sym[topic_id]][
+                                self.depthvalue[index]] != value:
+                                self.resp[self.dp_sym[topic_id]][
+                                    self.depthvalue[index]
+                                ] = value
+                                self.UpdateTick = True
 
-                        self.__response_output(
-                            self.resp[self.index_sym[topic_id]], "index"
-                        )
-                    elif dp_flag:
-                        self.__response_output(
-                            self.resp[self.dp_sym[topic_id]], "depth"
-                        )
+                            dp_flag = True
+                    if self.UpdateTick:
+                        if sf_flag:
+                            self.__response_output(
+                                self.resp[self.scrips_sym[topic_id]], "scrips"
+                            )
+                        elif idx_flag:
+                            self.__response_output(
+                                self.resp[self.index_sym[topic_id]], "index"
+                            )
+                        elif dp_flag:
+                            self.__response_output(
+                                self.resp[self.dp_sym[topic_id]], "depth"
+                            )
 
                 elif data_type == 76:  # lite mode datafeed
 
                     offset += 1
                     topic_id = struct.unpack("H", data[offset : offset + 2])[0]
                     offset += 2
                     sf_flag, idx_flag = False, False
@@ -1399,15 +1416,19 @@
 
         if self.OnOpen:
             self.OnOpen()
 
 
     def connect(self) -> None:
         """
-        Performs initialization and waits before executing further actions.
+        Establishes a connection to the WebSocket.
+
+        If the WebSocket object is not already initialized, this method will create the
+        WebSocket connection.
+
         """
         if self.__ws_object is None:
             self.__init_connection()
             time.sleep(2)
         self.on_open()
             
 
@@ -1469,15 +1490,15 @@
                     )
                 else:
                     print(
                         f"Attempting reconnect {self.reconnect_attempts} of {self.max_reconnect_attempts}..."
                     )
                 time.sleep(self.reconnect_delay)
                 self.__ws_object = None
-                self.__init_connection()
+                self.connect()
             else:
                 if self.write_to_file:
                     self.data_logger.debug(
                         f"Response:{'Max reconnect attempts reached. Connection abandoned.'}"
                     )
                 else:
                     print("Max reconnect attempts reached. Connection abandoned.")
@@ -1554,14 +1575,20 @@
 
     def infinite_loop(self):
         while self.__ws_run:
             pass
 
 
     def is_connected(self):
+        """
+        Check if the websocket is connected.
+
+        Returns:
+            bool: True if the websocket is connected, False otherwise.
+        """
         if self.__ws_object:
             return True
         else:
             return False
 
     def unsubscribe(
         self, symbols: list, data_type: str = "SymbolUpdate", channel: int = 1
```

### Comparing `fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-2.1.4/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/map.json` & `fyers_sdk-2.1.4/fyers_sdk/FyersWebsocket/map.json`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-2.1.4/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,43 +20,54 @@
         return cls._instance
 
     def __init__(
         self,
         access_token: str,
         write_to_file: Optional[bool] = False,
         log_path: Optional[str] = None,
-        on_message: Optional[Callable] = None,
+        on_trades : Optional[Callable] = None,
+        on_positions: Optional[Callable] = None,
+        on_orders: Optional[Callable] = None,
+        on_general: Optional[Callable] = None,
         on_error: Optional[Callable] = None,
         on_connect: Optional[Callable] = None,
         on_close: Optional[Callable] = None,
+        reconnect : Optional[Callable] = False
     ) -> None:
         """
         Initializes the class instance.
 
         Args:
             access_token (str): The access token to authenticate with.
-            write_to_file (bool): Flag indicating whether to save data to file.
+            write_to_file (bool, optional): Flag indicating whether to save data to a file. Defaults to False.
             log_path (str, optional): The path to the log file. Defaults to None.
-            on_message (callable, optional): Callback function for message events. Defaults to None.
+            on_trades (callable, optional): Callback function for trade events. Defaults to None.
+            on_positions (callable, optional): Callback function for position events. Defaults to None.
+            on_orders (callable, optional): Callback function for order events. Defaults to None.
+            on_general (callable, optional): Callback function for general events. Defaults to None.
             on_error (callable, optional): Callback function for error events. Defaults to None.
-            on_connect (callable, optional): Callback function for open events. Defaults to None.
+            on_connect (callable, optional): Callback function for connect events. Defaults to None.
             on_close (callable, optional): Callback function for close events. Defaults to None.
+            reconnect (bool, optional): Flag indicating whether to attempt reconnection on disconnection. Defaults to False.
         """
         self.__access_token = access_token
-        self.__url = "wss://socket.fydev.tech/trade/v3"
         self.log_path = log_path
         self.__ws_object = None
         self.__ws_run = False
         self.ping_thread = None
         self.write_to_file = write_to_file
         self.background_flag = False
-        self.OnMessage = on_message
-        self.OnError = on_error
-        self.OnOpen = on_connect
-        self.OnClose = on_close
+        self.ontrades = on_trades
+        self.onposition = on_positions
+        self.restart_flag = reconnect
+        self.onorder = on_orders
+        self.ongeneral = on_general
+        self.onerror = on_error
+        self.onopen = on_connect
+        self.onclose = on_close
         self.__ws_object = None
         self.__url = "wss://socket.fyers.in/trade/v3"
         file_path = resource_filename('fyers_sdk.FyersWebsocket', 'map.json')
         with open(file_path, "r") as file:
             # Imported json file
             mapper = json.load(file)
         self.position_mapper = mapper["position_mapper"]
@@ -98,19 +109,19 @@
 
         Returns:
             Dict[str, Any] : The parsed position data in a specific format.
 
         """
         try:
             position_data = {}
-            for key , value in self.position_mapper:
+            for key , value in self.position_mapper.items():
                 if key in msg["positions"]:
                     position_data[value] = msg["positions"][key]
 
-            return {"ws_type": 1, "s": msg["s"], "d": position_data}
+            return { "s": msg["s"], "positions": position_data}
 
         except Exception as e:
             self.order_logger.error(e)
 
     def __parse_trade_data(self, msg: Dict[str, Any]) -> Dict[str, Any]:
         """
         Parses trade data from a message and returns it in a specific format.
@@ -119,23 +130,22 @@
             msg (str): The message containing trade data.
 
         Returns:
             Dict[str, Any] : The parsed trade data in a specific format.
 
         """
         try:
-        
             trade_data = {}
             for key , value in self.trade_mapper.items():
-                if key in msg["orders"]:
-                    trade_data[value] = msg["orders"][key]
+                if key in msg["trades"]:
+                    trade_data[value] = msg["trades"][key]
 
 
 
-            return {"ws_type": 1, "s": msg["s"], "d": trade_data}
+            return { "s": msg["s"], "trades": trade_data}
 
         except Exception as e:
             self.order_logger.error(e)
 
     def __parse_order_data(self, msg: Dict[str, Any]) -> Dict[str, Any]:
         """
         Parses order update data from a dictionary and returns it in a specific format.
@@ -147,45 +157,73 @@
             Dict[str, Any]: The parsed order update data in a specific format.
         """
         try:
             order_data = {}
             for key , value in self.order_mapper.items():
                 if key in msg["orders"]:
                     order_data[value] = msg["orders"][key]
-
-            return {"ws_type": 1, "s": msg["s"], "d": order_data}
+            order_data["orderNumStatus"] =  msg["orders"]["id"] + ":" + str(msg["orders"]["org_ord_status"])
+            return { "s": msg["s"], "orders": order_data}
 
         except Exception as e:
             self.order_logger.error(e)
 
+    def on_trades(self, message):
+        if self.ontrades is not None:
+            self.ontrades(message)
+        else:
+            print(f"Trade : {message}")
+
+    def on_positions(self, message):
+        if self.onposition is not None:
+            self.onposition(message)
+        else:
+            print(f"Position : {message}")
+
+    def on_order(self, message):
+        if self.onorder is not None:
+            self.onorder(message)
+        else:
+            print(f"Order : {message}")
+
+    def on_general(self, message):
+        if self.ongeneral is not None:
+            self.ongeneral(message)
+        else:
+            print(f"General : {message}")
+
+
     def __on_message(self, message: Dict[str, Any]):
         """
         Parses the response data based on its content.
 
         Args:
             message (str): The response message to be parsed.
 
         Returns:
             Any: The parsed response data.
         """
         try:
             response = json.loads(message)
-
+            # print(response,"\n")
             if "orders" in response:
                 response = self.__parse_order_data(response)
+                self.on_order(response)
             elif "positions" in response:
                 response = self.__parse_position_data(response)
+                self.on_positions(response)
             elif "trades" in response:
                 response = self.__parse_trade_data(response)
+                self.on_trades(response)
+            else:
+                self.on_general(response)
             
             if self.write_to_file:
                 self.order_logger.debug(f"Response:{response}")
-            else:
-                self.order_logger.debug(f"Response:{response}")
-                self.On_message(response)
+
 
         except Exception as e:
             self.order_logger.error(e)
 
     def On_message(self, message: Any) -> None:
         """
         Callback function for handling message events.
@@ -204,16 +242,16 @@
         Callback function for handling error events.
 
         Args:
             message (str): The error message.
 
         """
         self.order_logger.error(message)
-        if self.OnError is not None:
-            self.OnError(message)
+        if self.onerror is not None:
+            self.onerror(message)
         else:
             if self.write_to_file:
                 self.order_logger.debug(f"Response:{message}")
             else:
                 print(f"Error Response : {message}")
 
     def __on_open(self, ws):
@@ -238,38 +276,31 @@
         Returns:
             dict: A dictionary containing the response code, message, and s.
         """
         if self.restart_flag:
             if self.reconnect_attempts < self.max_reconnect_attempts:
                 self.reconnect_attempts += 1
 
-                if self.write_to_file:
-                    self.order_logger.debug(
-                        f"Response:{f'Attempting reconnect {self.reconnect_attempts} of {self.max_reconnect_attempts}...'}"
-                    )
-                else:
-                    print(
-                        f"Attempting reconnect {self.reconnect_attempts} of {self.max_reconnect_attempts}..."
-                    )
+               
+                print(
+                    f"Attempting reconnect {self.reconnect_attempts} of {self.max_reconnect_attempts}..."
+                )
                 time.sleep(self.reconnect_delay)
-                self.on_open()
+                self.__ws_object = None
+                self.connect()
             else:
-                if self.write_to_file:
-                    self.order_logger.debug(
-                        f"Response:{'Max reconnect attempts reached. Connection abandoned.'}"
-                    )
-                else:
-                    print("Max reconnect attempts reached. Connection abandoned.")
+
+                print("Max reconnect attempts reached. Connection abandoned.")
         else:
 
             self.on_close(
                 {
                     "code": defines.SUCCESS_CODE,
                     "message": defines.CONNECTION_CLOSED,
-                    "s": defines.success,
+                    "s": defines.SUCCESS,
                 }
             )
 
     def __ping(self) -> None:
         """
         Sends periodic ping messages to the server to maintain the WebSocket connection.
 
@@ -290,30 +321,40 @@
         """
         Handles the close event.
 
         Args:
             message (dict): The close message .
         """
 
-        if self.OnClose:
-            self.OnClose(message)
+        if self.onclose:
+            self.onclose(message)
         else:
             print(f"Response: {message}")
 
     def on_open(self) -> None:
         """
         Performs initialization and waits before executing further actions.
         """
-        self.init_connection()
-        time.sleep(2)
+        if self.onopen:
+            self.onopen()
 
-        if self.OnOpen:
-            self.OnOpen()
+    def is_connected(self):
+        """
+        Check if the websocket is connected.
+
+        Returns:
+            bool: True if the websocket is connected, False otherwise.
+        """
+        if self.__ws_object:
+            return True
+        else:
+            return False
+        
 
-    def init_connection(self):
+    def __init_connection(self):
         """
         Initializes the WebSocket connection and starts the WebSocketApp.
 
         The method creates a WebSocketApp object with the specified URL and sets the appropriate event handlers.
         It then starts the WebSocketApp in a separate thread.
         """
         try:
@@ -350,14 +391,28 @@
     def stop_running(self):
         self.__ws_run = False
 
     def infinite_loop(self):
         while self.__ws_run:
             pass
 
+    def connect(self) -> None:
+        """
+        Establishes a connection to the WebSocket.
+
+        If the WebSocket object is not already initialized, this method will create the
+        WebSocket connection.
+
+        """
+        if self.__ws_object is None:
+            self.__init_connection()
+            time.sleep(2)
+        self.on_open()
+
+            
     def close_connection(self):
         """
         Closes the WebSocket connection 
 
         """
         if self.__ws_object is not None:
             self.__ws_object.close(reason=json.dumps({}))
@@ -372,25 +427,24 @@
         Args:
             data_type (str): The type of data to subscribe to, such as orders, position, or holdings.
 
 
         """
 
         try:
-            self.init_connection()
+            self.__init_connection()
             time.sleep(1)
             if self.__ws_object is not None:
                 self.data_type = []
                 for elem in data_type.split(","):
                     if isinstance(self.socket_type[elem], list):
                         self.data_type.extend(self.socket_type[elem])
                     else:
                         self.data_type.append(self.socket_type[elem])
                                 
-                print(self.data_type)
                 message = json.dumps(
                     {"T": "SUB_ORD", "SLIST": self.data_type, "SUB_T": 1}
                 )
                 self.__ws_object.send(message)
 
         except Exception as e:
             self.order_logger.error(e)
```

### Comparing `fyers_sdk-2.1.3/fyers_sdk/fyersModel.py` & `fyers_sdk-2.1.4/fyers_sdk/fyersModel.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 
 except Exception as e:
 	print("moduleName: {}, ERR: could not import module : {}".format(moduleName,e))
 
 
 class Config:
     API = 'https://api-t1.fyers.in/api/v3'
-    HISTORY_URL = "https://api.fyers.in/data-rest/v2"
+    # HISTORY_URL = "https://api.fyers.in/data-rest/v2"
     DATA_API = "https://api-t1.fyers.in/data"
     AUTH_URL = "https://api.fyers.in/api/v2"
-
+    API_V2 = "https://api.fyers.in/api/v2"
     # Endpoint
     get_profile = "/profile"
     tradebook = "/tradebook"
     positions = "/positions"
     holdings = "/holdings"
     convert_position = "/positions"
     funds = "/funds"
-    place_orders = "/orders/sync"
+    orders_endpoint = "/orders/sync"
     orderbook = "/orders"
     minquantity = "/minquantity"
     market_status = "/marketStatus"
     auth = "/generate-authcode"
     generate_access_token = "/validate-authcode"
     generate_data_token = "/data-token"
     data_vendor_td = "/truedata-ws"
@@ -71,15 +71,15 @@
         Returns:
             The response JSON as a dictionary, or the response object if an error occurs.
         """
         try:
             response = requests.post(
                 Config.API + api,
                 data=json.dumps(data),
-                headers={"Authorization": header, "Content-Type": self.content},
+                headers={"Authorization": header, "Content-Type": self.content ,"version": "3"},
             )
             return response.json()
         except Exception as e:
             self.api_logger.error(e)
 
     def get_call(self, api: str, header: str, data=None, data_flag=False) -> dict:
         """
@@ -92,31 +92,31 @@
             data_flag: A flag indicating whether to use custom data URLs.
 
         Returns:
             The response JSON as a dictionary, or the response object if an error occurs.
         """
         try:
             if data_flag:
-                if api == Config.history:
-                    URL = Config.HISTORY_URL + api
+                if api == Config.get_profile:
+                    URL = Config.API_V2 + api
                 else:
                     URL = Config.DATA_API + api
             else:
                 URL = Config.API + api
 
             if data is not None:
                 url_params = urllib.parse.urlencode(data)
                 URL = URL + "?" + url_params
 
             response = requests.get(
                 url=URL,
                 headers={
                     "Authorization": header,
                     "Content-Type": self.content,
-                    "version": "2.1",
+                    "version": "3"
                 },
             )
             return response.json()
         except Exception as e:
             self.api_logger.error(e)
 
     def delete_call(self, api: str, header: str, data) -> dict:
@@ -131,15 +131,15 @@
         Returns:
             The response JSON as a dictionary, or the response object if an error occurs.
         """
         try:
             response = requests.delete(
                 url=Config.API + api,
                 data=json.dumps(data),
-                headers={"Authorization": header, "Content-Type": self.content},
+                headers={"Authorization": header, "Content-Type": self.content ,"version": "3"},
             )
             return response.json()
         except Exception as e:
             self.api_logger.error(e)
 
     def patch_call(self, api: str, header: str, data) -> dict:
         """
@@ -153,15 +153,15 @@
         Returns:
             The response JSON as a dictionary, or the response object if an error occurs.
         """
         try:
             response = requests.patch(
                 url=Config.API + api,
                 data=json.dumps(data),
-                headers={"Authorization": header, "Content-Type": self.content},
+                headers={"Authorization": header, "Content-Type": self.content ,"version": "3"},
             )
             return response.json()
         except Exception as e:
             self.api_logger.error(e)
 
 
 class FyersServiceAsync:
@@ -185,20 +185,20 @@
             data: The data to send in the request payload.
 
         Returns:
             The response JSON as a dictionary, or the response object if an error occurs.
         """
         try:
             async with aiohttp.ClientSession(
-                headers={"Authorization": header, "Content-Type": self.content}
+                headers={"Authorization": header, "Content-Type": self.content ,"version": "3"}
             ) as session:
                 url = Config.API + api
                 async with session.post(url, data=json.dumps(data)) as response:
-                    response = await response.json()
-                    return response
+                    return await response.json()
+                
         except Exception as e:
             self.api_logger.error(e)
             return response
 
     async def get_async_call(
         self, api: str, header: str, params=None, data_flag=False
     ) -> dict:
@@ -212,25 +212,26 @@
             data_flag: A flag indicating whether to use custom data URLs.
 
         Returns:
             The response JSON as a dictionary, or the response object if an error occurs.
         """
         try:
             if data_flag:
-                if api == "/history":
-                    URL = Config.HISTORY_URL + api
+                if api == Config.get_profile:
+                    URL = Config.API_V2 + api
                 else:
                     URL = Config.DATA_API + api
             else:
                 URL = Config.API + api
+                
             async with aiohttp.ClientSession(
                 headers={
                     "Authorization": header,
                     "Content-Type": self.content,
-                    "version": "2.1",
+                    "version": "3",
                 }
             ) as session:
                 async with session.get(URL, params=params) as response:
                     response = await response.json()
                     return response
 
         except Exception as e:
@@ -247,15 +248,15 @@
             data: The data to send in the request payload.
 
         Returns:
             The response JSON as a dictionary, or the response object if an error occurs.
         """
         try:
             async with aiohttp.ClientSession(
-                headers={"Authorization": header, "Content-Type": self.content}
+                headers={"Authorization": header, "Content-Type": self.content ,"version": "3"}
             ) as session:
                 url = Config.API + api
                 async with session.delete(url, data=json.dumps(data)) as response:
                     return await response.json()
         except Exception as e:
             self.api_logger.error(e)
             return response
@@ -270,15 +271,15 @@
             data: The data to send in the request payload.
 
         Returns:
             The response JSON as a dictionary, or the response object if an error occurs.
         """
         try:
             async with aiohttp.ClientSession(
-                headers={"Authorization": header, "Content-Type": self.content}
+                headers={"Authorization": header, "Content-Type": self.content ,"version": "3"}
             ) as session:
                 url = Config.API + api
                 json_data = json.dumps(data).encode("utf-8")
 
                 async with session.patch(url, data=json_data) as response:
                     return await response.json()
         except Exception as e:
@@ -383,75 +384,70 @@
 
     def get_profile(self) -> dict:
         """
         Retrieves the user profile information.
 
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(Config.get_profile, self.header)
-            )
+            response = self.service.get_async_call(Config.get_profile, self.header, data_flag=True)
+            
         else:
-            response = self.service.get_call(Config.get_profile, self.header)
+            response = self.service.get_call(Config.get_profile, self.header,data_flag=True)
         return response
 
     def tradebook(self) -> dict:
         """
         Retrieves daily trade details of the day.
 
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(Config.tradebook, self.header)
-            )
+            response = self.service.get_async_call(Config.tradebook, self.header)
+            
         else:
             response = self.service.get_call(Config.tradebook, self.header)
         return response
 
     def funds(self) -> dict:
         """
         Retrieves funds details.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(Config.funds, self.header)
-            )
+            response = self.service.get_async_call(Config.funds, self.header)
+            
         else:
             response = self.service.get_call(Config.funds, self.header)
         return response
 
     def positions(self) -> dict:
         """
         Retrieves information about current open positions.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(Config.positions, self.header)
-            )
+            response = self.service.get_async_call(Config.positions, self.header)
+            
         else:
             response = self.service.get_call(Config.positions, self.header)
         return response
 
     def holdings(self) -> dict:
         """
         Retrieves information about current holdings.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(Config.holdings, self.header)
-            )
+            response = self.service.get_async_call(Config.holdings, self.header)
+            
         else:
             response = self.service.get_call(Config.holdings, self.header)
         return response
 
     def get_orders(self, data) -> dict:
         """
         Retrieves order details by ID.
@@ -459,53 +455,50 @@
         Args:
             data: The data containing the order ID.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(Config.orderbook, self.header)
-            )
+            response = self.service.get_async_call(Config.orderbook, self.header)
+            
         else:
             response = self.service.get_call(Config.orderbook, self.header)
         id_list = data['id'].split(",")
         print(id_list)
         response["orderBook"]= [order for order in response["orderBook"] if order["id"] in id_list]
 
         return response
 
-    def orderbook(self) -> dict:
+    def orderbook(self, data = None) -> dict:
         """
         Retrieves the order information.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(Config.orderbook, self.header)
-            )
+            response = self.service.get_async_call(Config.orderbook, self.header, data)
+            
         else:
-            response = self.service.get_call(Config.orderbook, self.header)
+            response = self.service.get_call(Config.orderbook, self.header, data)
         return response
 
     def market_status(self) -> dict:
         """
         Retrieves market status.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(
+            response = self.service.get_async_call(
                     Config.market_status, self.header, data_flag=True
                 )
-            )
+            
         else:
             response = self.service.get_call(
                 Config.market_status, self.header, data_flag=True
             )
         return response
 
     def convert_position(self, data) -> dict:
@@ -519,21 +512,20 @@
             convertFrom (str): Existing product type of the positions. (CNC positions cannot be converted)
             convertTo (str): The new product type to convert the positions to.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.patch_async_call(
+            response = self.service.post_async_call(
                     Config.convert_position, self.header, data
                 )
-            )
+            
         else:
-            response = self.service.patch_call(
+            response = self.service.post_call(
                 Config.convert_position, self.header, data
             )
         return response
 
     def cancel_order(self, data) -> dict:
         """
         Cancel order.
@@ -542,19 +534,18 @@
             id (str, optional): ID of the position to close. If not provided, all open positions will be closed.
 
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.delete_async_call(Config.orders, self.header, data)
-            )
+            response = self.service.delete_async_call(Config.orders_endpoint, self.header, data)
+            
         else:
-            response = self.service.delete_call(Config.orders, self.header, data)
+            response = self.service.delete_call(Config.orders_endpoint, self.header, data)
         return response
 
     def place_order(self, data) -> dict:
         """
         Places an order based on the provided data.
 
         Args:
@@ -572,19 +563,17 @@
             - 'stopPrice' (float): Valid price for Stop and Stoplimit orders. Default: 0.
             - 'offlineOrder' (bool): Specifies if the order is placed when the market is open (False) or as an AMO order (True).
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.post_async_call(Config.place_orders, self.header, data)
-            )
+            response = self.service.post_async_call(Config.orders_endpoint, self.header, data)
         else:
-            response = self.service.post_call(Config.place_orders, self.header, data)
+            response = self.service.post_call(Config.orders_endpoint, self.header, data)
         return response
 
     def modify_order(self, data) -> dict:
         """
         Modifies the parameters of a pending order based on the provided details.
 
         Parameters:
@@ -594,36 +583,37 @@
             qty (int, optional): New quantity for the order.
             type (int, optional): New order type for the order.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.patch_async_call(Config.orders, self.header, data)
-            )
+            response = self.service.patch_async_call(Config.orders_endpoint, self.header, data)
+            
         else:
-            response = self.service.patch_call(Config.orders, self.header, data)
+            response = self.service.patch_call(Config.orders_endpoint, self.header, data)
         return response
 
-    def exit_positions(self, data=None) -> dict:
+    def exit_positions(self, data={}) -> dict:
         """
         Closes open positions based on the provided ID or closes all open positions if ID is not passed.
 
         Args:
             id (str, optional): ID of the position to close. If not provided, all open positions will be closed.
 
 
         Returns:
             The response JSON as a dictionary.
         """
+        if len(data) == 0 :
+            data = {"exit_all": 1}
+
         if self.is_async:
-            response = asyncio.run(
-                self.service.delete_async_call(Config.positions, self.header, data)
-            )
+            response = self.service.delete_async_call(Config.positions, self.header, data)
+            
         else:
             response = self.service.delete_call(Config.positions, self.header, data)
         return response
 
     def generate_data_token(self, data):
         allPackages = subprocess.check_output([sys.executable, "-m", "pip", "freeze"])
         installed_packages = [r.decode().split("==")[0] for r in allPackages.split()]
@@ -639,19 +629,18 @@
         Parameters:
             order_ids (list): A list of order IDs to be cancelled.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.delete_async_call(
+            response = self.service.delete_async_call(
                     Config.multi_orders, self.header, data
                 )
-            )
+            
         else:
             response = self.service.delete_call(
                 Config.multi_orders, self.header, data
             )
         return response
 
     def place_basket_orders(self, data):
@@ -675,17 +664,16 @@
             - 'takeProfit' (float): Valid price for BO orders.
 
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.post_async_call(Config.multi_orders, self.header, data)
-            )
+            response = self.service.post_async_call(Config.multi_orders, self.header, data)
+            
         else:
             response = self.service.post_call(
                 Config.multi_orders, self.header, data
             )
         return response
 
     def modify_basket_orders(self, data):
@@ -701,19 +689,18 @@
             - 'qty' (int): New quantity for the order.
             - 'type' (int): New order type for the order.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.patch_async_call(
+            response = self.service.patch_async_call(
                     Config.multi_orders, self.header, data
                 )
-            )
+            
         else:
             response = self.service.patch_call(
                 Config.multi_orders, self.header, data
             )
         return response
 
     def history(self, data=None):
@@ -732,19 +719,18 @@
         cont_flag (int): Flag indicating continuous data and future options. Set to 1 for continuous data.
 
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(
+            response = self.service.get_async_call(
                     Config.history, self.header, data, data_flag=True
                 )
-            )
+            
         else:
             response = self.service.get_call(
                 Config.history, self.header, data, data_flag=True
             )
         return response
 
     def quotes(self, data=None):
@@ -755,19 +741,19 @@
             symbols (str): Comma-separated symbols of the products. Maximum symbol limit is 50. Eg: 'NSE:SBIN-EQ,NSE:HDFC-EQ'.
 
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(
+            
+            response =   self.service.get_async_call(
                     Config.quotes, self.header, data, data_flag=True
                 )
-            )
+            
         else:
             response = self.service.get_call(
                 Config.quotes, self.header, data, data_flag=True
             )
         return response
 
     def depth(self, data=None):
@@ -778,30 +764,16 @@
             symbol (str): Symbol of the product. Eg: 'NSE:SBIN-EQ'.
             ohlcv_flag (int): Flag to indicate whether to retrieve open, high, low, closing, and volume quantity. Set to 1 for yes.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(
+                response = self.service.get_async_call(
                     Config.market_depth, self.header, data, data_flag=True
                 )
-            )
+            
         else:
             response = self.service.get_call(
                 Config.market_depth, self.header, data, data_flag=True
             )
         return response
-    
-
-    def minquantity(self):
-        if self.is_async:
-            response = asyncio.run(
-                self.service.get_async_call(
-                    Config.minquantity, self.header)
-            )
-        else:
-            response = self.service.get_call(
-                Config.minquantity, self.header)
-        return response
-
```

### Comparing `fyers_sdk-2.1.3/fyers_sdk/fyers_logger.py` & `fyers_sdk-2.1.4/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.3/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-2.1.4/fyers_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 2.1.3
+Version: 2.1.4
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.1.3/setup.py` & `fyers_sdk-2.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='2.1.3',
+     version='2.1.4',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

