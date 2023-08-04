# Comparing `tmp/pyplejd-0.1.tar.gz` & `tmp/pyplejd-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplejd-0.1.tar", last modified: Sat Jul 15 23:08:19 2023, max compression
+gzip compressed data, was "pyplejd-0.2.tar", last modified: Fri Aug  4 07:35:43 2023, max compression
```

## Comparing `pyplejd-0.1.tar` & `pyplejd-0.2.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-15 23:08:19.990136 pyplejd-0.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-07-15 22:53:20.000000 pyplejd-0.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      406 2023-07-15 23:08:19.990136 pyplejd-0.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-07-15 22:53:30.000000 pyplejd-0.1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-15 23:08:19.990136 pyplejd-0.1/pyplejd/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2969 2023-07-15 21:35:33.000000 pyplejd-0.1/pyplejd/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4466 2023-07-15 21:35:33.000000 pyplejd-0.1/pyplejd/api.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      520 2023-07-15 21:35:33.000000 pyplejd-0.1/pyplejd/ble_device.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      391 2023-07-15 21:35:33.000000 pyplejd-0.1/pyplejd/const.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      837 2023-07-15 21:35:33.000000 pyplejd-0.1/pyplejd/crypto.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     9417 2023-07-15 21:35:33.000000 pyplejd-0.1/pyplejd/mesh.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3766 2023-07-15 21:35:33.000000 pyplejd-0.1/pyplejd/plejd_device.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-15 23:08:19.990136 pyplejd-0.1/pyplejd.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      406 2023-07-15 23:08:19.000000 pyplejd-0.1/pyplejd.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      322 2023-07-15 23:08:19.000000 pyplejd-0.1/pyplejd.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-15 23:08:19.000000 pyplejd-0.1/pyplejd.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-07-15 23:08:19.000000 pyplejd-0.1/pyplejd.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-07-15 23:08:19.000000 pyplejd-0.1/pyplejd.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       79 2023-07-15 23:08:19.990136 pyplejd-0.1/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      629 2023-07-15 23:08:18.000000 pyplejd-0.1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-04 07:35:43.060730 pyplejd-0.2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-07-15 23:38:48.000000 pyplejd-0.2/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      406 2023-08-04 07:35:43.060730 pyplejd-0.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      498 2023-07-15 23:38:48.000000 pyplejd-0.2/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-04 07:35:43.060730 pyplejd-0.2/pyplejd/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2360 2023-08-03 21:42:15.000000 pyplejd-0.2/pyplejd/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-04 07:35:43.060730 pyplejd-0.2/pyplejd/ble/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    10929 2023-08-03 22:14:54.000000 pyplejd-0.2/pyplejd/ble/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1056 2023-08-04 07:28:17.000000 pyplejd-0.2/pyplejd/ble/crypto.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-04 07:35:43.060730 pyplejd-0.2/pyplejd/cloud/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6717 2023-08-01 20:43:40.000000 pyplejd-0.2/pyplejd/cloud/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4380 2023-08-01 20:43:37.000000 pyplejd-0.2/pyplejd/cloud/site_details.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      238 2023-07-22 21:13:18.000000 pyplejd-0.2/pyplejd/cloud/site_list.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1826 2023-07-25 20:47:20.000000 pyplejd-0.2/pyplejd/const.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2640 2023-08-04 07:33:47.000000 pyplejd-0.2/pyplejd/interface.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-08-04 07:35:43.060730 pyplejd-0.2/pyplejd.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      406 2023-08-04 07:35:43.000000 pyplejd-0.2/pyplejd.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      377 2023-08-04 07:35:43.000000 pyplejd-0.2/pyplejd.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-08-04 07:35:43.000000 pyplejd-0.2/pyplejd.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       45 2023-08-04 07:35:43.000000 pyplejd-0.2/pyplejd.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        8 2023-08-04 07:35:43.000000 pyplejd-0.2/pyplejd.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       79 2023-08-04 07:35:43.060730 pyplejd-0.2/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      675 2023-08-04 07:34:49.000000 pyplejd-0.2/setup.py
```

### Comparing `pyplejd-0.1/LICENSE` & `pyplejd-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyplejd-0.1/pyplejd/__init__.py` & `pyplejd-0.2/pyplejd/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 import logging
 from datetime import timedelta
 
 from bleak_retry_connector import close_stale_connections
 
-from .mesh import PlejdMesh
-from .api import get_cryptokey, get_devices, get_site_data, get_scenes
-from .plejd_device import PlejdDevice, PlejdScene
+from .ble import PlejdMesh
+from .cloud import PlejdCloudSite
 
-from .const import PLEJD_SERVICE, LIGHT, SWITCH
+from .const import PLEJD_SERVICE, LIGHT, SENSOR, SWITCH, UNKNOWN
 
 _LOGGER = logging.getLogger(__name__)
 
-class PlejdManager:
+__all__ = [
+    "PlejdManager",
+    "get_sites",
+    "PLEJD_SERVICE",
+    "LIGHT",
+    "SENSOR",
+    "SWITCH",
+    "UNKNOWN",
+]
+
+get_sites = PlejdCloudSite.get_sites
 
+
+class PlejdManager:
     def __init__(self, credentials):
         self.credentials = credentials
         self.mesh = PlejdMesh()
-        self.mesh.statecallback = self._update_device
-        self.devices = { }
+        self.devices = []
         self.scenes = []
+        self.cloud = PlejdCloudSite(**credentials)
+
+    async def init(self):
+        await self.cloud.ensure_details_loaded()
+
+        self.mesh.set_key(self.cloud.cryptokey)
+        self.mesh.subscribe_state(self._update_device)
+
+        self.devices = self.cloud.devices
+        for d in self.devices:
+            self.mesh.expect_device(d.BLEaddress)
+            d.connect_mesh(self.mesh)
+
+        self.scenes = self.cloud.scenes
+        for s in self.scenes:
+            s.connect_mesh(self.mesh)
+
+        if _LOGGER.isEnabledFor(logging.DEBUG):
+            _LOGGER.debug("Devices:")
+            for d in self.devices:
+                _LOGGER.debug(d)
+            _LOGGER.debug("Scenes:")
+            for s in self.scenes:
+                _LOGGER.debug(s)
 
     def add_mesh_device(self, device, rssi):
-        _LOGGER.debug("Adding plejd %s", device)
-        # for d in self.devices.values():
-        #     addr = device.address.replace(":","").replace("-","").upper()
-        #     if d.BLE_address.upper() == addr or addr in device.name:
-        return self.mesh.add_mesh_node(device, rssi)
-        # _LOGGER.debug("Device was not expected in current mesh")
+        _LOGGER.debug("Saw plejd device %s", device)
+        return self.mesh.see_device(device, rssi)
 
     async def close_stale(self, device):
         _LOGGER.debug("Closing stale connections for %s", device)
         await close_stale_connections(device)
 
     @property
     def connected(self):
         return self.mesh is not None and self.mesh.connected
 
-    async def get_site_data(self):
-        return await get_site_data(**self.credentials)
+    @property
+    def site_data(self):
+        return self.cloud.details
+
+    def _update_device(self, deviceState):
+        _LOGGER.debug("New data: %s", deviceState)
 
-    async def get_devices(self):
-        devices = await get_devices(**self.credentials)
-        self.devices = {k: PlejdDevice(self, **v) for (k,v) in devices.items()}
-        _LOGGER.debug("Devices")
-        _LOGGER.debug(self.devices)
-        return self.devices
-
-    async def get_scenes(self):
-        scenes = await get_scenes(**self.credentials)
-        self.scenes = [PlejdScene(self, **s) for s in scenes]
-        _LOGGER.debug("Scenes")
-        _LOGGER.debug(self.scenes)
-        return self.scenes
-
-    async def _update_device(self, deviceState):
-        address = deviceState["address"]
-        if address in self.devices:
-            await self.devices[address].new_state(deviceState.get("state"), deviceState.get("dim", 0))
+        for d in self.devices:
+            if d.address == deviceState["address"]:
+                d.update_state(**deviceState)
 
     @property
-    def keepalive_interval(self):
-        if self.mesh.pollonWrite:
-            return timedelta(seconds=10)
-        else:
-            return timedelta(minutes=10)
-
-    async def keepalive(self):
-        if self.mesh.crypto_key is None:
-            self.mesh.set_crypto_key(await get_cryptokey(**self.credentials))
-        if not self.mesh.connected:
-            if not await self.mesh.connect():
-                return False
+    def ping_interval(self):
+        return timedelta(minutes=10)
+
+    async def ping(self):
         retval = await self.mesh.ping()
-        if retval and self.mesh.pollonWrite:
-            await self.mesh.poll()
         return retval
 
     async def disconnect(self):
         _LOGGER.debug("DISCONNECT")
         await self.mesh.disconnect()
-
-    async def poll(self):
-        await self.mesh.poll()
-
-    async def ping(self):
-        retval = await self.mesh.ping()
-        if self.mesh.pollonWrite:
-            await self.poll()
-        return retval
```

### Comparing `pyplejd-0.1/pyplejd/mesh.py` & `pyplejd-0.2/pyplejd/ble/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,255 +1,312 @@
 import asyncio
 import binascii
 import logging
 import os
-import struct
-from datetime import datetime
+from typing import Callable
+
 from bleak import BleakClient, BleakError
-from bleak_retry_connector import establish_connection
 from bleak.backends.device import BLEDevice
+from bleak_retry_connector import establish_connection
 
-from .ble_device import BLEDeviceWithRssi
-from .const import PLEJD_AUTH, PLEJD_LASTDATA, PLEJD_LIGHTLEVEL, PLEJD_PING, PLEJD_DATA
 from .crypto import auth_response, encrypt_decrypt
+from ..const import PLEJD_AUTH, PLEJD_LASTDATA, PLEJD_LIGHTLEVEL, PLEJD_PING, PLEJD_DATA
 
 _LOGGER = logging.getLogger(__name__)
 
-class PlejdMesh():
 
+class PlejdMesh:
     def __init__(self):
-        self._connected = False
-        self.client = None
-        self.connected_node = None
-        self.crypto_key = None
-        self.mesh_nodes = []
-
-        self.pollonWrite = True # TODO: Deprecate this
-        self.statecallback = None
-        self.scenecallback = None
-        self.buttoncallback = None
+        self._seen_nodes: dict[BLEDevice, int] = {}
+        self._expected_nodes = set()
+        self._gateway_node = None
+        self._crypto_key: bytearray = None
+        self._client: BleakClient = None
+
+        self._connect_listeners = set()
+        self._state_listeners = set()
+        self._scene_listeners = set()
+        self._button_listeners = set()
 
         self._ble_lock = asyncio.Lock()
 
-    def add_mesh_node(self, ble_device: BLEDevice, rssi: int):
-        device = BLEDeviceWithRssi(ble_device, rssi)
-        if device not in self.mesh_nodes:
-            self.mesh_nodes.append(device)
-        else:
-            _LOGGER.debug("Plejd already added")
-
-    def set_crypto_key(self, key):
-        self.crypto_key = binascii.a2b_hex(key.replace("-", ""))
-
     @property
     def connected(self):
-        if self._connected and self.client and self.client.is_connected:
-            return True
-        return False
+        return self._client is not None
+
+    def expect_device(self, BLEaddress: str):
+        self._expected_nodes.add(BLEaddress.upper())
+
+    def see_device(self, node: BLEDevice, rssi: int):
+        self._seen_nodes[node] = rssi
+
+    def set_key(self, key: str):
+        self._crypto_key = key
+
+    def _subscribe(self, set_: set, listener: Callable):
+        set_.add(listener)
+
+        def remover():
+            if listener in set_:
+                set_.remove(listener)
+
+        return remover
+
+    def _publish(self, set_: set, *args, **kwargs):
+        for listener in set_:
+            listener(*args, **kwargs)
+
+    def subscribe_connect(self, listener: Callable):
+        return self._subscribe(self._connect_listeners, listener)
+
+    def subscribe_state(self, listener: Callable):
+        return self._subscribe(self._state_listeners, listener)
+
+    def subscribe_scene(self, listener: Callable):
+        return self._subscribe(self._scene_listeners, listener)
+
+    def subscribe_button(self, listener: Callable):
+        return self._subscribe(self._button_listeners, listener)
 
     async def disconnect(self):
-        if self.connected and self.client:
-            try:
-                await self.client.stop_notify(PLEJD_LASTDATA)
-                await self.client.stop_notify(PLEJD_LIGHTLEVEL)
-                await self.client.disconnect()
-            except BleakError:
-                pass
-            self._connected = False
-            self.client = None
-    
-    async def connect(self, disconnect_callback=None, key=None):
-        await self.disconnect()
-        _LOGGER.debug("Trying to connect to mesh")
+        if not self._client:
+            return False
+        try:
+            await self._client.stop_notify(PLEJD_LASTDATA)
+            await self._client.stop_notify(PLEJD_LIGHTLEVEL)
+            await self._client.disconnect()
+        except BleakError:
+            pass
+        self._client = None
+        self._publish(self._connect_listeners, {"connected": False})
 
-        def _disconnect(arg):
-            if not self.connected: return
-            _LOGGER.debug("_disconnect %s", arg)
-            self.client = None
-            self._connected = False
-            if disconnect_callback:
-                disconnect_callback()
+    async def connect(self):
+        _LOGGER.debug("Trying to connect to mesh")
+        if self.connected:
+            return True
 
-        self.mesh_nodes.sort(key = lambda a: a.rssi, reverse = True)
-        for plejd in self.mesh_nodes:
+        def _disconnect(reason):
+            _LOGGER.debug("_disconnect(%s)", reason)
+            self._client = None
+            self._gateway_node = None
+            self._publish(self._connect_listeners, {"connected": False})
+
+        # Try to connect to nodes in order of decreasing RSSI
+        sorted_nodes = dict(
+            sorted(self._seen_nodes.items(), key=lambda n: n[1], reverse=True)
+        )
+        sorted_nodes = {
+            node: rssi
+            for node, rssi in sorted_nodes.items()
+            if node.address.replace(":", "").upper() in self._expected_nodes
+        }
+
+        if not sorted_nodes:
+            _LOGGER.debug(
+                "Failed to connect to plejd mesh - No valid devices: %s (%s)",
+                self._seen_nodes,
+                self._expected_nodes,
+            )
+            return False
+        client = None
+        for node in sorted_nodes:
             try:
-                _LOGGER.debug("Connecting to %s", plejd)
-                client = await establish_connection(BleakClient, plejd.device, "plejd", _disconnect)
-                address = plejd.device.address
-                self._connected = True
-                self.client = client
-                _LOGGER.debug("Connected to Plejd mesh")
-                if not await self._authenticate():
-                    await self.client.disconnect()
-                    self._connected = False
+                _LOGGER.debug("Attempting to connect to %s", node)
+                client = await establish_connection(
+                    BleakClient, node, "plejd", _disconnect
+                )
+
+                if not await self._authenticate(client):
+                    await client.disconnect()
                     continue
+                self._gateway_node = node.address
                 break
+
             except (BleakError, asyncio.TimeoutError) as e:
-                _LOGGER.warning("Error connecting to Plejd device: %s", str(e))
+                _LOGGER.warning("Failed to connect to %s: %s", node, str(e))
+
         else:
-            if len(self.mesh_nodes) == 0:
-                _LOGGER.debug("Failed to connect to plejd mesh - no devices discovered")
-            else:
-                _LOGGER.warning("Failed to connect to plejd mesh - %s", self.mesh_nodes)
+            _LOGGER.warning("Failed to connect to plejd mesh - %s", sorted_nodes)
             return False
 
-        self.connected_node = binascii.a2b_hex(address.replace(":", "").replace("-", ""))[::-1]
+        async def _lastdata_listener(_, lastdata: bytearray):
+            self._parse_lastdata(lastdata)
 
-        async def _lastdata(_, lastdata):
-            self.pollonWrite = False
-            data = encrypt_decrypt(self.crypto_key, self.connected_node, lastdata)
-            _LOGGER.debug("Received LastData %s", data.hex())
-            deviceState = decode_state(data)
-            _LOGGER.debug("Decoded LastData %s", deviceState)
-            if deviceState is None:
-                return
-            if self.statecallback and "state" in deviceState:
-                await self.statecallback(deviceState)
-            if self.scenecallback and "scene" in deviceState:
-                await self.scenecallback(deviceState)
-            if self.buttoncallback and "button" in deviceState:
-                await self.buttoncallback(deviceState)
-
-        async def _lightlevel(_, lightlevel):
-            _LOGGER.debug("Received LightLevel %s", lightlevel.hex())
-            for i in range(0, len(lightlevel), 10):
-                ll = lightlevel[i:i+10]
-                deviceState = {
-                    "address": int(ll[0]),
-                    "state": bool(ll[1]),
-                    "dim": int.from_bytes(ll[5:7], "little"),
-                }
-                _LOGGER.debug("Decoded LightLevel %s", deviceState)
-                if self.statecallback and deviceState is not None:
-                    await self.statecallback(deviceState)
-
-        await client.start_notify(PLEJD_LASTDATA, _lastdata)
-        await client.start_notify(PLEJD_LIGHTLEVEL, _lightlevel)
-        
-        await self.poll()
+        async def _lightlevel_listener(_, lightlevel: bytearray):
+            self._parse_lightlevel(lightlevel)
+
+        await client.start_notify(PLEJD_LASTDATA, _lastdata_listener)
+        await client.start_notify(PLEJD_LIGHTLEVEL, _lightlevel_listener)
+        self._client = client
 
+        self._publish(self._connect_listeners, {"connected": True})
+        await self.poll()
         return True
 
-    async def write(self, payload):
+    async def poll(self):
+        client = self._client
+        if client is None:
+            return
+        _LOGGER.debug("Polling mesh for current state")
+        await client.write_gatt_char(PLEJD_LIGHTLEVEL, b"\x01", response=True)
+
+    async def ping(self):
+        async with self._ble_lock:
+            if not await self.connect():
+                return False
+            if await self._ping(self._client):
+                await self.poll()
+                return True
+        return False
+
+    async def set_state(self, address: int, state: bool, dim=0):
+        if state:
+            if dim is None:
+                payload = binascii.a2b_hex(f"{address:02x}0110009701")
+            else:
+                payload = binascii.a2b_hex(f"{address:02x}0110009801{dim:04x}")
+        else:
+            payload = binascii.a2b_hex(f"{address:02x}0110009700")
+
+        return await self._write(payload)
+
+    async def activate_scene(self, index: int):
+        payload = binascii.a2b_hex(f"0201100021{index:02x}")
+        return await self._write(payload)
+
+    async def _write(self, payload):
+        client = self._client
+        if client is None:
+            return False
         try:
-            # TODO:
             async with self._ble_lock:
-                _LOGGER.debug("Writing data to Plejd mesh CT: %s", payload.hex())
-                data = encrypt_decrypt(self.crypto_key, self.connected_node, payload)
-                await self.client.write_gatt_char(PLEJD_DATA, data, response=True)
+                _LOGGER.debug("Writing to plejd mesh: %s", payload.hex())
+                data = encrypt_decrypt(self._crypto_key, self._gateway_node, payload)
+                await self._client.write_gatt_char(PLEJD_DATA, data, response=True)
         except (BleakError, asyncio.TimeoutError) as e:
-            _LOGGER.warning("Plejd mesh write command failed: %s", str(e))
+            _LOGGER.warning("Writing to plejd mesh failed: %s", str(e))
             return False
         return True
 
-    async def set_state(self, address, state, dim=0):
-        payload = encode_state(address, state, dim)
-        retval = await self.write(payload)
-        if self.pollonWrite:
-            await self.poll()
-        return retval
-
-    async def activate_scene(self, index):
-        payload = binascii.a2b_hex(f"0201100021{index:02x}")
-        retval = await self.write(payload)
-        if self.pollonWrite:
-            await self.poll()
-        return retval
-
-    async def ping(self):
-        async with self._ble_lock:
-            return await self._ping()
-                
-    async def _ping(self):
-        if self.client is None:
+    async def _ping(self, client):
+        if client is None:
             return False
         try:
             ping = bytearray(os.urandom(1))
             _LOGGER.debug("Ping(%s)", int.from_bytes(ping, "little"))
-            await self.client.write_gatt_char(PLEJD_PING, ping, response=True)
-            pong = await self.client.read_gatt_char(PLEJD_PING)
+            await client.write_gatt_char(PLEJD_PING, ping, response=True)
+            pong = await client.read_gatt_char(PLEJD_PING)
             _LOGGER.debug("Pong(%s)", int.from_bytes(pong, "little"))
             if (ping[0] + 1) & 0xFF == pong[0]:
                 return True
         except (BleakError, asyncio.TimeoutError) as e:
             _LOGGER.warning("Plejd mesh keepalive signal failed: %s", str(e))
-        self.pollonWrite = True
         return False
 
-    async def poll(self):
-        if self.client is None:
-            return
-        _LOGGER.debug("Polling Plejd mesh for current state")
-        async with self._ble_lock:
-            await self.client.write_gatt_char(PLEJD_LIGHTLEVEL, b"\x01", response=True)
-
-    async def _authenticate(self):
-        if self.client is None:
+    async def _authenticate(self, client: BleakClient):
+        if client is None:
             return False
         try:
-            async with self._ble_lock:
-                _LOGGER.debug("Authenticating to plejd mesh")
-                await self.client.write_gatt_char(PLEJD_AUTH, b"\0x00", response=True)
-                challenge = await self.client.read_gatt_char(PLEJD_AUTH)
-                response = auth_response(self.crypto_key, challenge)
-                await self.client.write_gatt_char(PLEJD_AUTH, response, response=True)
-                if not await self._ping():
-                    _LOGGER.debug("Authenticion failed")
-                    return False
-                _LOGGER.debug("Authenticated successfully")
-                return True
+            _LOGGER.debug("Authenticating with plejd mesh")
+            await client.write_gatt_char(PLEJD_AUTH, b"\0x00", response=True)
+            challenge = await client.read_gatt_char(PLEJD_AUTH)
+            response = auth_response(self._crypto_key, challenge)
+            await client.write_gatt_char(PLEJD_AUTH, response, response=True)
+            if not await self._ping(client):
+                _LOGGER.debug("Authentication failed!")
+                return False
+            _LOGGER.debug("Authentication successful")
+            return True
         except (BleakError, asyncio.TimeoutError) as e:
-            _LOGGER.warning("Plejd authentication failed: %s", str(e))
+            _LOGGER.warning("Plejd mesh authentication failed: %s", str(e))
         return False
 
+    def _parse_lastdata(self, lastdata: bytearray):
+        data = encrypt_decrypt(self._crypto_key, self._gateway_node, lastdata)
+        _LOGGER.debug("Parsing LASTDATA: %s", data.hex())
+
+        address = int(data[0])
+        cmd = data[1:3]
+        if not cmd == b"\x01\x10":
+            _LOGGER.debug("Got non-command LASTDATA: %s", data.hex())
+            return
+        cmd = data[3:5]
+
+        if address == 0:
+            # Broadcast packet
+            pass
+
+        if address == 1 and cmd == b"\x00\x1b":
+            _LOGGER.debug("Got time data")
+            # Ignored. Consider adding ability to send time data periodically instead
+            # ts = struct.unpack_from("<1", data, 5)[0]
+            # Is this the same thing?
+            # ts2 = int.from_bytes(data[6:8], "little")
+            # dt = datetime.fromtimestamp(ts)
+            return
 
-def decode_state(data):
-    address = int(data[0])
-    cmdtype = data[1:3]
-    if not cmdtype == b"\x01\x10":
-        _LOGGER.debug("Got non-command data: %s", cmdtype)
-        return None
-    cmd = data[3:5]
-
-    # if address == 0:
-    #     # Broadcast
-    #     pass
-    if address == 1 and cmd == b"\x00\x1b":
-        _LOGGER.debug("Got time data?")
-        ts = struct.unpack_from("<I", data, 5)[0]
-        dt = datetime.fromtimestamp(ts)
-        _LOGGER.debug("Timestamp: %s (%s)", ts, dt)
-        return None
-    # if address == 2:
-    #     # Scene update?
-    #     pass
-
-    retval = {"address": address}
-
-    if cmd == b"\x00\xc8" or cmd == b"\x00\x98":
-        retval["state"] = bool(data[5])
-        retval["dim"] = int.from_bytes(data[6:8], "little")        
-    elif cmd == b"\x00\x97":
-        retval["state"] = bool(data[5])
-    elif cmd == b"\x00\x16":
-        retval["address"] = int(data[5])
-        retval["button"] = int(data[6])
-        _LOGGER.info("Button pressed: %s", retval)
-    elif cmd == b"\x00\x21":
-        del retval["address"]
-        retval["scene"] = int(data[5])
-        _LOGGER.info("Scene triggered: %s", retval)
-    else:
-        _LOGGER.debug("Unknown command %s", cmd)
-        return None
-
-    return retval
-
-
-def encode_state(address, state, dim):
-    if state:
-        if dim is None:
-            return binascii.a2b_hex(f"{address:02x}0110009701")
-        brightness = dim << 8 | dim
-        return binascii.a2b_hex(f"{address:02x}0110009801{brightness:04x}")
-    else:
-        return binascii.a2b_hex(f"{address:02x}0110009700")
+        if address == 2:
+            # Scene update
+            pass
+
+        match cmd:
+            case b"\x00\xc8" | b"\x00\x98":
+                state = bool(data[5])
+                dim = int.from_bytes(data[6:8], "little")
+                _LOGGER.debug("Address: %s, state: %s, dim: %s", address, state, dim)
+                self._publish(
+                    self._state_listeners,
+                    {
+                        "address": address,
+                        "state": state,
+                        "dim": dim,
+                    },
+                )
+            case b"\x00\x97":
+                state = bool(data[5])
+                _LOGGER.debug("Address: %s, state: %s", address, state)
+                self._publish(
+                    self._state_listeners,
+                    {
+                        "address": address,
+                        "state": state,
+                    },
+                )
+            case b"\x00\x16":
+                address = int(data[5])
+                button = int(data[6])
+                _LOGGER.debug("Address: %s, button: %s", address, button)
+                self._publish(
+                    self._button_listeners,
+                    {
+                        "address": address,
+                        "button": button,
+                    },
+                )
+            case b"\x00\x21":
+                _LOGGER.debug("Scene triggered")
+                scene = int(data[5])
+                _LOGGER.debug("Scene: %s", scene)
+                self._publish(
+                    self._scene_listeners,
+                    {
+                        "scene": scene,
+                    },
+                )
+
+    def _parse_lightlevel(self, lightlevel: bytearray):
+        _LOGGER.debug("Parsing LIGHTLEVEL: %s", lightlevel.hex())
+        for i in range(0, len(lightlevel), 10):
+            ll = lightlevel[i : i + 10]
+            address = int(ll[0])
+            state = bool(ll[1])
+            dim = int.from_bytes(ll[5:7], "little")
+            _LOGGER.debug("Address: %s, state: %s, dim: %s", address, state, dim)
+            self._publish(
+                self._state_listeners,
+                {
+                    "address": address,
+                    "state": state,
+                    "dim": dim,
+                },
+            )
+        pass
```

