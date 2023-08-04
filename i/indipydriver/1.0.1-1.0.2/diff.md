# Comparing `tmp/indipydriver-1.0.1.tar.gz` & `tmp/indipydriver-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-1.0.1.tar", last modified: Mon Jul 24 21:23:01 2023, max compression
+gzip compressed data, was "indipydriver-1.0.2.tar", last modified: Fri Aug  4 15:56:45 2023, max compression
```

## Comparing `indipydriver-1.0.1.tar` & `indipydriver-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-1.0.1/LICENSE
--rw-r--r--   0        0        0     2411 2023-07-11 05:27:01.000000 indipydriver-1.0.1/README.md
--rw-r--r--   0        0        0      573 2023-07-24 21:14:10.000000 indipydriver-1.0.1/indipydriver/__init__.py
--rw-r--r--   0        0        0    17081 2023-07-09 09:46:38.000000 indipydriver-1.0.1/indipydriver/comms.py
--rw-r--r--   0        0        0    21067 2023-07-09 10:33:24.000000 indipydriver-1.0.1/indipydriver/events.py
--rw-r--r--   0        0        0    21548 2023-07-24 20:31:23.000000 indipydriver-1.0.1/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    10816 2023-07-13 20:27:03.000000 indipydriver-1.0.1/indipydriver/ipyserver.py
--rw-r--r--   0        0        0    11759 2023-07-24 20:59:57.000000 indipydriver-1.0.1/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    42713 2023-07-08 21:53:53.000000 indipydriver-1.0.1/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2023-07-24 21:13:56.000000 indipydriver-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 indipydriver-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2411 2023-07-11 05:27:01.000000 indipydriver-1.0.2/README.md
+-rw-r--r--   0        0        0      573 2023-08-04 15:51:45.000000 indipydriver-1.0.2/indipydriver/__init__.py
+-rw-r--r--   0        0        0    18962 2023-08-03 16:48:04.000000 indipydriver-1.0.2/indipydriver/comms.py
+-rw-r--r--   0        0        0    21067 2023-07-09 10:33:24.000000 indipydriver-1.0.2/indipydriver/events.py
+-rw-r--r--   0        0        0    21548 2023-07-24 20:31:23.000000 indipydriver-1.0.2/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    12071 2023-08-03 09:35:01.000000 indipydriver-1.0.2/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    11759 2023-07-24 20:59:57.000000 indipydriver-1.0.2/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    40577 2023-08-02 17:36:00.000000 indipydriver-1.0.2/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2023-08-04 15:51:36.000000 indipydriver-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 indipydriver-1.0.2/PKG-INFO
```

### Comparing `indipydriver-1.0.1/LICENSE` & `indipydriver-1.0.2/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 bernie-skipole
+Copyright (c) 2023 Bernard Czenkusz
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `indipydriver-1.0.1/README.md` & `indipydriver-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `indipydriver-1.0.1/indipydriver/__init__.py` & `indipydriver-1.0.2/indipydriver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 from .ipyserver import IPyServer
 
-version = "1.0.1"
+version = "1.0.2"
```

### Comparing `indipydriver-1.0.1/indipydriver/comms.py` & `indipydriver-1.0.2/indipydriver/comms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-import asyncio, sys, os
+import asyncio, sys, os, time
 
 import xml.etree.ElementTree as ET
 
 import fcntl
 
 from datetime import datetime
 
@@ -219,17 +219,18 @@
         await asyncio.gather(rx.run_rx(readerque),
                              tx.run_tx(writerque)
                              )
 
 class Port_TX():
     "An object that transmits data on a port, used by Portcomms as one half of the communications path"
 
-    def __init__(self, blobstatus, writer):
+    def __init__(self, blobstatus, writer, timer):
         self.blobstatus = blobstatus
         self.writer = writer
+        self.timer = timer
 
 
     async def run_tx(self, writerque):
         """Gets data from writerque, and transmits it out on the port writer"""
         while True:
             await asyncio.sleep(0)
             # get block of data from writerque and transmit
@@ -240,20 +241,22 @@
                 continue
             # this data can be transmitted
             if txdata.tag == "setBLOBVector" and len(txdata):
                 # txdata is a setBLOBVector containing blobs
                 # the generator blob_xml_bytes yields bytes
                 for binarydata in blob_xml_bytes(txdata):
                     # Send to the port
+                    self.timer.update()
                     self.writer.write(binarydata)
                     await self.writer.drain()
             else:
                 # its straight xml, send it out on the port
                 binarydata = ET.tostring(txdata)
                 # Send to the port
+                self.timer.update()
                 self.writer.write(binarydata)
                 await self.writer.drain()
             writerque.task_done()
 
 
 
 class Port_RX(STDIN_RX):
@@ -303,55 +306,98 @@
                 binarydata = b""
             else:
                 # data has content but no > found
                 binarydata += data
                 # could put a max value here to stop this increasing indefinetly
 
 
+class TXTimer():
+
+    def __init__(self, timeout = 15):
+        self.timer = time.time()
+        self.timeout = timeout
+
+    def update(self):
+        "call this every time a transmission is made, and it resets the timer"
+        self.timer = time.time()
+
+    def elapsed(self):
+        "Return True if more than timeout seconds have elapsed since last update"
+        telapsed = time.time() - self.timer
+        if telapsed > self.timeout:
+            self.timer = time.time()
+            return True
+        return False
+
+
 class Portcomms():
     """If indipydriver.comms is set to an instance of this class it is
        used to implement communications via a port"""
 
     def __init__(self, devices, host="localhost", port=7624):
         # devices is a dictionary of device name to device this driver owns
+        self.devices = devices
         self.blobstatus = BLOBSstatus(devices)
         self.host = host
         self.port = port
         self.connected = False
 
+        # timer used to force a data transmission after timeout seconds
+        # this will cause an exception if the connection is broken and will shut down
+        # the connection
+        self.timer = TXTimer(timeout = 15)
+
     async def __call__(self, readerque, writerque):
         "Called from indipydriver.asyncrun() to run the communications"
         self.readerque = readerque
         self.writerque = writerque
         server = await asyncio.start_server(self.handle_data, self.host, self.port)
         try:
             await server.serve_forever()
         except KeyboardInterrupt as e:
             server.close()
             raise e
 
+
+    async def _monitor_connection(self):
+        """If connected and not transmitting, send def vectors every self.timeout seconds
+           This ensures that if the connection has failed, due to the client disconnecting, the write
+           to the port operation will cause a failure exception which will close the connection"""
+        while True:
+            await asyncio.sleep(5)
+            # this is tested every five seconds
+            if self.connected and self.writerque.empty() and self.readerque.empty():
+                # only need to test if the queue are empty
+                if self.timer.elapsed():
+                    # no transmission in timeout seconds so send defVectors
+                    for device in self.devices.values():
+                        for vector in device.values():
+                            await vector.send_defVector()
+
+
     async def handle_data(self, reader, writer):
         "Used by asyncio.start_server, called to handle a client connection"
         if self.connected:
             # already connected, can only handle one connection
             writer.close()
             await writer.wait_closed()
             return
         self.connected = True
         rx = Port_RX(self.blobstatus, reader)
-        tx = Port_TX(self.blobstatus, writer)
+        tx = Port_TX(self.blobstatus, writer, self.timer)
         try:
             txtask = asyncio.create_task(tx.run_tx(self.writerque))
             rxtask = asyncio.create_task(rx.run_rx(self.readerque))
-            await txtask
-            await rxtask
-        except ConnectionResetError:
+            montask = asyncio.create_task(self._monitor_connection())
+            await asyncio.gather(txtask, rxtask, montask)
+        except Exception as e:
             self.connected = False
             txtask.cancel()
             rxtask.cancel()
+            montask.cancel()
             cleanque(self.writerque)
 
 
 def cleanque(que):
     "Clears out a que"
     try:
         while True:
```

### Comparing `indipydriver-1.0.1/indipydriver/events.py` & `indipydriver-1.0.2/indipydriver/events.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.0.1/indipydriver/ipydriver.py` & `indipydriver-1.0.2/indipydriver/ipydriver.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.0.1/indipydriver/ipyserver.py` & `indipydriver-1.0.2/indipydriver/ipyserver.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import xml.etree.ElementTree as ET
 
 from functools import partialmethod
 
 from .ipydriver import IPyDriver
 
-from .comms import Port_RX, Port_TX, cleanque, BLOBSstatus
+from .comms import Port_RX, Port_TX, cleanque, BLOBSstatus, TXTimer
 
 
 class IPyServer:
 
     """An instance should be created with:
 
        drivers is a list of IPyDriver objects this driver handles.
@@ -237,23 +237,47 @@
 
         # devices is a dictionary of device name to device
         self.devices = devices
         self.serverreaderque = serverreaderque
         # self.connected is True if this pool object is running a connection
         self.connected = False
 
+        # timer used to force a data transmission after timeout seconds
+        # this will cause an exception if the connection is broken and will shut down
+        # the connection
+        self.timer = TXTimer(timeout = 15)
+
+
+    async def _monitor_connection(self):
+        """If connected and self.txque is empty, send def vectors every timeout seconds
+           This ensures that if the connection has failed, due to the client disconnecting, the write
+           to the port operation will cause a failure exception which will close the connection"""
+        while True:
+            await asyncio.sleep(5)
+            # this is tested every five seconds
+            if self.connected and self.txque.empty():
+                 # only need to test if the queue is empty
+                if self.timer.elapsed():
+                    # no transmission in timeout seconds so send defVectors
+                    for device in self.devices.values():
+                        for vector in device.values():
+                            xmldata =  vector._make_defVector()
+                            await self.txque.put(xmldata)
+
+
     async def handle_data(self, reader, writer):
         "Used by asyncio.start_server, called to handle a client connection"
         self.connected = True
         blobstatus = BLOBSstatus(self.devices)
         rx = Port_RX(blobstatus, reader)
-        tx = Port_TX(blobstatus, writer)
+        tx = Port_TX(blobstatus, writer, self.timer)
         try:
             txtask = asyncio.create_task(tx.run_tx(self.txque))
             rxtask = asyncio.create_task(rx.run_rx(self.serverreaderque))
-            await txtask
-            await rxtask
+            montask = asyncio.create_task(self._monitor_connection())
+            await asyncio.gather(txtask, rxtask, montask)
         except ConnectionResetError:
             self.connected = False
             txtask.cancel()
             rxtask.cancel()
+            montask.cancel()
             cleanque(self.txque)
```

### Comparing `indipydriver-1.0.1/indipydriver/propertymembers.py` & `indipydriver-1.0.2/indipydriver/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.0.1/indipydriver/propertyvectors.py` & `indipydriver-1.0.2/indipydriver/propertyvectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,31 @@
             xmldata.set("message", message)
         await self.driver.send(xmldata)
         self.enable = False
         for member in self.data.values():
             # set all members as changed, so when re-enabled, all values are ready to be sent again
             member.changed = True
 
+
+    async def send_defVector(self, message='', timestamp=None, timeout='0'):
+        """Transmits the vector definition to the client.
+
+           message is any suitable string for the client.
+
+           timestamp should be a datetime.datetime object or None, in which
+           case a datetime.datetime.utcnow() value will be inserted.
+
+           The timeout value should be '0' if not used, or a string of a
+           numeric value indicating to the client how long this data is valid.
+        """
+        xmldata = self._make_defVector(message, timestamp, timeout)
+        if not xmldata is None:
+            await self.driver.send(xmldata)
+
+
     def checkvalue(self, value, allowed):
         "allowed is a list of values, checks if value is in it"
         if value not in allowed:
             raise ValueError(f"Value \"{value}\" is not one of {str(allowed).strip('[]')}")
         return value
 
     @property
@@ -79,18 +96,14 @@
     @state.setter
     def state(self, value):
         try:
             self._state = self.checkvalue(value, ['Idle','Ok','Busy','Alert'])
         except ValueError as ex:
             self._reporterror(ex)
 
-    def send_defVector(self, timestamp=None, timeout=0, message=''):
-        "overridden in child classes"
-        pass
-
     def __setitem__(self, membername, value):
         try:
             self.data[membername].membervalue = value
         except ValueError as ex:
             self._reporterror(ex)
 
     def __getitem__(self, membername):
@@ -158,25 +171,16 @@
                     await self.driver.clientevent(event)
             except EventException:
                 # if an error is raised parsing the incoming data, just continue
                 pass
             self.dataque.task_done()
 
 
-    async def send_defVector(self, message='', timestamp=None, timeout='0'):
-        """Transmits the vector definition (defSwitchVector) to the client.
-
-           message is any suitable string for the client.
-
-           timestamp should be a datetime.datetime object or None, in which
-           case a datetime.datetime.utcnow() value will be inserted.
-
-           The timeout value should be '0' if not used, or a string of a
-           numeric value indicating to the client how long this data is valid.
-        """
+    def _make_defVector(self, message='', timestamp=None, timeout='0'):
+        "Creates xml data object for vector definition"
         if not isinstance(timeout, str):
             self._reporterror("Aborting sending defSwitchVector: The given send_defVector timeout value must be a string object")
             return
         if not self.device.enable:
             return
         if not self.enable:
             return
@@ -196,18 +200,17 @@
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
         if message:
             xmldata.set("message", message)
         for switch in self.data.values():
             xmldata.append(switch.defswitch())
-            # after a defswitch sent, assume new client connection, and set all members as changed
-            # so they will all be included in the first 'send_setVector'
-            switch.changed = True
-        await self.driver.send(xmldata)
+        return xmldata
+
+
 
     async def send_setVector(self, message='', timestamp=None, timeout='0', allvalues=True):
         """Transmits the vector (setSwitchVector) and members with their values to the client.
            Typically the vector 'state' should be set, and any changed member value prior to
            transmission.
 
            message is any suitable string for the client.
@@ -342,22 +345,16 @@
                 pass
             self.dataque.task_done()
 
     @property
     def perm(self):
         return "ro"
 
-    async def send_defVector(self, message='', timestamp=None, timeout='0'):
-        """Transmits the vector definition (defLightVector) to the client.
-
-           message is any suitable string for the client.
-
-           timestamp should be a datetime.datetime object or None, in which
-           case a datetime.datetime.utcnow() value will be inserted.
-
+    def _make_defVector(self, message='', timestamp=None, timeout='0'):
+        """Creates xml data object for vector definition
            For Light Vectors the timeout value is not used, but is included
            in the arguments to match other send_vectors.
         """
         if not self.device.enable:
             return
         if not self.enable:
             return
@@ -374,18 +371,15 @@
         xmldata.set("state", self.state)
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         if message:
             xmldata.set("message", message)
         for light in self.data.values():
             xmldata.append(light.deflight())
-            # after a deflight sent, assume new client connection, and set all members as changed
-            # so they will all be included in the first 'send_setVector'
-            light.changed = True
-        await self.driver.send(xmldata)
+        return xmldata
 
 
     async def send_setVector(self, message='', timestamp=None, timeout='0', allvalues=True):
         """Transmits the vector (setLightVector) and members with their values to the client.
            Typically the vector 'state' should be set, and any changed member value prior to
            transmission.
 
@@ -507,25 +501,16 @@
                     event = newTextVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
             except EventException:
                 # if an error is raised parsing the incoming data, just continue
                 pass
             self.dataque.task_done()
 
-    async def send_defVector(self, message='', timestamp=None, timeout='0'):
-        """Transmits the vector definition (defTextVector) to the client.
-
-           message is any suitable string for the client.
-
-           timestamp should be a datetime.datetime object or None, in which
-           case a datetime.datetime.utcnow() value will be inserted.
-
-           The timeout value should be '0' if not used, or a string value
-           indicating to the client how long this data is valid.
-        """
+    def _make_defVector(self, message='', timestamp=None, timeout='0'):
+        "Creates xml data object for vector definition"
         if not isinstance(timeout, str):
             self._reporterror("Aborting sending defTextVector: The given send_defVector timeout value must be a string object")
             return
         if not self.device.enable:
             return
         if not self.enable:
             return
@@ -544,18 +529,15 @@
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
         if message:
             xmldata.set("message", message)
         for text in self.data.values():
             xmldata.append(text.deftext())
-            # after a deftext sent, assume new client connection, and set all members as changed
-            # so they will all be included in the first 'send_setVector'
-            text.changed = True
-        await self.driver.send(xmldata)
+        return xmldata
 
     async def send_setVector(self, message='', timestamp=None, timeout='0', allvalues=True):
         """Transmits the vector (setTextVector) and members with their values to the client.
            Typically the vector 'state' should be set, and any changed member value prior to
            transmission.
 
            message is any suitable string for the client.
@@ -680,25 +662,16 @@
                     event = newNumberVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
             except EventException:
                 # if an error is raised parsing the incoming data, just continue
                 pass
             self.dataque.task_done()
 
-    async def send_defVector(self, message='', timestamp=None, timeout='0'):
-        """Transmits the vector definition (defNumberVector) to the client.
-
-           message is any suitable string for the client.
-
-           timestamp should be a datetime.datetime object or None, in which
-           case a datetime.datetime.utcnow() value will be inserted.
-
-           The timeout value should be '0' if not used, or a string value
-           indicating to the client how long this data is valid.
-        """
+    def _make_defVector(self, message='', timestamp=None, timeout='0'):
+        "Creates xml data object for vector definition"
         if not isinstance(timeout, str):
             self._reporterror("Aborting sending defNumberVector: The given send_defVector timeout value must be a string object")
             return
         if not self.device.enable:
             return
         if not self.enable:
             return
@@ -717,18 +690,15 @@
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
         if message:
             xmldata.set("message", message)
         for number in self.data.values():
             xmldata.append(number.defnumber())
-            # after a defnumber sent, assume new client connection, and set all members as changed
-            # so they will all be included in the first 'send_setVector'
-            number.changed = True
-        await self.driver.send(xmldata)
+        return xmldata
 
     async def send_setVector(self, message='', timestamp=None, timeout='0', allvalues=True):
         """Transmits the vector (setNumberVector) and members with their values to the client.
            Typically the vector 'state' should be set, and any changed member value prior to
            transmission.
 
            message is any suitable string for the client.
@@ -872,25 +842,16 @@
                     event = newBLOBVector(self.devicename, self.name, self, root)
                     await self.driver.clientevent(event)
             except EventException:
                 # if an error is raised parsing the incoming data, just continue
                 pass
             self.dataque.task_done()
 
-    async def send_defVector(self, message='', timestamp=None, timeout='0'):
-        """Transmits the vector definition (defBLOBVector) to the client.
-
-           message is any suitable string for the client.
-
-           timestamp should be a datetime.datetime object or None, in which
-           case a datetime.datetime.utcnow() value will be inserted.
-
-           The timeout value should be '0' if not used, or a string value
-           indicating to the client how long this data is valid.
-        """
+    def _make_defVector(self, message='', timestamp=None, timeout='0'):
+        "Creates xml data object for vector definition"
         if not isinstance(timeout, str):
             self._reporterror("Aborting sending defBLOBVector: The given send_defVector timeout value must be a string object")
             return
         if not self.device.enable:
             return
         if not self.enable:
             return
@@ -909,15 +870,15 @@
         # note - limit timestamp characters to :21 to avoid long fractions of a second
         xmldata.set("timestamp", timestamp.isoformat(sep='T')[:21])
         xmldata.set("timeout", timeout)
         if message:
             xmldata.set("message", message)
         for blob in self.data.values():
             xmldata.append(blob.defblob())
-        await self.driver.send(xmldata)
+        return xmldata
 
     # NOTE: BLOBVectors do not have a send_setVector method
     #       only the more explicit send_setVectorMembers is available
 
     async def send_setVectorMembers(self, message='', timestamp=None, timeout='0', members=[]):
         """Transmits the vector (setBLOBVector) and members with their values to the client.
            The members list specifies the member names which will have their values sent.
```

### Comparing `indipydriver-1.0.1/pyproject.toml` & `indipydriver-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "1.0.1"
+version = "1.0.2"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-1.0.1/PKG-INFO` & `indipydriver-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

