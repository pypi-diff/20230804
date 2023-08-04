# Comparing `tmp/erpc-1.9.0.tar.gz` & `tmp/erpc-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/erpc-1.9.0.tar", last modified: Mon Jan 17 10:04:36 2022, max compression
+gzip compressed data, was "erpc-1.9.1.tar", last modified: Wed Jul 20 08:22:58 2022, max compression
```

## Comparing `erpc-1.9.0.tar` & `erpc-1.9.1.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-01-17 10:04:37.000000 erpc-1.9.0/
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-01-17 10:04:37.000000 erpc-1.9.0/erpc/
--rwxrwx---   0 root         (0) vboxsf     (999)     4417 2018-11-02 18:37:41.000000 erpc-1.9.0/erpc/arbitrator.py
--rwxrwx---   0 root         (0) vboxsf     (999)     4036 2018-11-02 18:37:41.000000 erpc-1.9.0/erpc/basic_codec.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2725 2018-11-02 18:37:41.000000 erpc-1.9.0/erpc/client.py
--rwxrwx---   0 root         (0) vboxsf     (999)     3422 2018-11-02 18:37:41.000000 erpc-1.9.0/erpc/codec.py
--rwxrwx---   0 root         (0) vboxsf     (999)      879 2018-11-02 18:37:41.000000 erpc-1.9.0/erpc/crc16.py
--rwxrwx---   0 root         (0) vboxsf     (999)      184 2022-01-17 10:01:11.000000 erpc-1.9.0/erpc/erpc_version.py
--rwxrwx---   0 root         (0) vboxsf     (999)     2302 2020-09-30 11:30:19.000000 erpc-1.9.0/erpc/server.py
--rwxrwx---   0 root         (0) vboxsf     (999)     1319 2018-11-02 18:37:41.000000 erpc-1.9.0/erpc/simple_server.py
--rwxrwx---   0 root         (0) vboxsf     (999)    14166 2022-01-05 09:00:13.000000 erpc-1.9.0/erpc/transport.py
--rwxrwx---   0 root         (0) vboxsf     (999)      846 2018-11-02 18:37:41.000000 erpc-1.9.0/erpc/__init__.py
-drwxrwx---   0 root         (0) vboxsf     (999)        0 2022-01-17 10:04:37.000000 erpc-1.9.0/erpc.egg-info/
--rwxrwx---   0 root         (0) vboxsf     (999)        1 2022-01-17 10:04:37.000000 erpc-1.9.0/erpc.egg-info/dependency_links.txt
--rwxrwx---   0 root         (0) vboxsf     (999)     1714 2022-01-17 10:04:37.000000 erpc-1.9.0/erpc.egg-info/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)       16 2022-01-17 10:04:37.000000 erpc-1.9.0/erpc.egg-info/requires.txt
--rwxrwx---   0 root         (0) vboxsf     (999)      332 2022-01-17 10:04:37.000000 erpc-1.9.0/erpc.egg-info/SOURCES.txt
--rwxrwx---   0 root         (0) vboxsf     (999)        5 2022-01-17 10:04:37.000000 erpc-1.9.0/erpc.egg-info/top_level.txt
--rwxrwx---   0 root         (0) vboxsf     (999)     1714 2022-01-17 10:04:37.000000 erpc-1.9.0/PKG-INFO
--rwxrwx---   0 root         (0) vboxsf     (999)       67 2022-01-17 10:04:37.000000 erpc-1.9.0/setup.cfg
--rwxrwx---   0 root         (0) vboxsf     (999)     1591 2019-12-20 13:16:31.000000 erpc-1.9.0/setup.py
+drwxr-xr-x   0 nxa17570 (12039517) nxp       (1000)        0 2022-07-20 08:22:58.571372 erpc-1.9.1/
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)     1699 2022-07-20 08:22:58.571372 erpc-1.9.1/PKG-INFO
+drwxr-xr-x   0 nxa17570 (12039517) nxp       (1000)        0 2022-07-20 08:22:58.567372 erpc-1.9.1/erpc/
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)      812 2021-04-17 13:18:16.000000 erpc-1.9.1/erpc/__init__.py
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)     4280 2021-04-17 13:18:16.000000 erpc-1.9.1/erpc/arbitrator.py
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)     3885 2021-04-17 13:18:16.000000 erpc-1.9.1/erpc/basic_codec.py
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)     2622 2021-04-17 13:18:16.000000 erpc-1.9.1/erpc/client.py
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)     3272 2021-04-17 13:18:16.000000 erpc-1.9.1/erpc/codec.py
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)      846 2021-04-17 13:18:16.000000 erpc-1.9.1/erpc/crc16.py
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)      175 2022-07-20 08:08:42.000000 erpc-1.9.1/erpc/erpc_version.py
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)     2221 2021-04-17 13:18:16.000000 erpc-1.9.1/erpc/server.py
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)     1270 2021-04-17 13:18:16.000000 erpc-1.9.1/erpc/simple_server.py
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)    13943 2022-07-20 08:08:42.000000 erpc-1.9.1/erpc/transport.py
+drwxr-xr-x   0 nxa17570 (12039517) nxp       (1000)        0 2022-07-20 08:22:58.567372 erpc-1.9.1/erpc.egg-info/
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)     1699 2022-07-20 08:22:58.000000 erpc-1.9.1/erpc.egg-info/PKG-INFO
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)      305 2022-07-20 08:22:58.000000 erpc-1.9.1/erpc.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)        1 2022-07-20 08:22:58.000000 erpc-1.9.1/erpc.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)        5 2022-07-20 08:22:58.000000 erpc-1.9.1/erpc.egg-info/top_level.txt
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)       67 2022-07-20 08:22:58.571372 erpc-1.9.1/setup.cfg
+-rw-r--r--   0 nxa17570 (12039517) nxp       (1000)     1601 2022-07-20 08:08:42.000000 erpc-1.9.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `erpc-1.9.0/erpc/arbitrator.py` & `erpc-1.9.1/erpc/arbitrator.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-#!/usr/bin/env python
-
-# Copyright 2016 NXP
-# All rights reserved.
-#
-# SPDX-License-Identifier: BSD-3-Clause
-
-import threading
-from collections import namedtuple
-from .codec import MessageType
-from .transport import Transport
-
-class ClientInfo:
-    event = None
-    msg = None
-
-##
-# @brief Shares a transport between a server and multiple clients.
-class TransportArbitrator(Transport):
-    def __init__(self, sharedTransport=None, codec=None):
-        self._transport = sharedTransport
-        self._codec = codec
-        self._pending_clients = {}
-        self._lock = threading.Lock()
-
-    @property
-    def shared_transport(self):
-        return self._transport
-
-    @shared_transport.setter
-    def shared_transport(self, transport):
-        self._transport = transport
-
-    @property
-    def codec(self):
-        return self._codec
-
-    @codec.setter
-    def codec(self, theCodec):
-        self._codec = theCodec
-
-    def send(self, message):
-        assert self._transport is not None, "No shared transport was set"
-        self._transport.send(message)
-
-    def receive(self):
-        assert self._transport is not None, "No shared transport was set"
-        assert self._codec is not None, "No codec was set"
-
-        # Repeatedly receive until we get an invocation request.
-        while True:
-            # Receive a message from the shared transport.
-            msg = self._transport.receive()
-
-            # Parse the message header.
-            self._codec.buffer = msg
-            info = self._codec.start_read_message()
-
-            # If it's an invocation or oneway, return it to the server.
-            if info.type in (MessageType.kInvocationMessage, MessageType.kOnewayMessage):
-                return msg
-            # Ignore unexpected message types.
-            elif info.type != MessageType.kReplyMessage:
-                continue
-
-            # Look up the client waiting for this reply.
-            try:
-                try:
-                    self._lock.acquire()
-                    client = self._pending_clients[info.sequence]
-                finally:
-                    self._lock.release()
-                client.msg = msg
-                client.event.set()
-            except KeyError:
-                # No client was found, unexpected sequence number!
-                pass
-
-    ##
-    # @brief Add a client request to the client list.
-    #
-    # This call is made by the client thread prior to sending the invocation to the server. It
-    # ensures that the transport arbitrator has the client's response message buffer ready in
-    # case it sees the response before the client even has a chance to call client_receive().
-    #
-    # @param self
-    # @param requestContext
-    # @return A token value to be passed to client_receive().
-    def prepare_client_receive(self, requestContext):
-        # Create pending client info.
-        info = ClientInfo()
-        info.event = threading.Event()
-
-        # Add this client to the pending clients dict.
-        try:
-            self._lock.acquire()
-            self._pending_clients[requestContext.sequence] = info
-        finally:
-            self._lock.release()
-
-        return requestContext.sequence
-
-    ##
-    # @brief Receive method for the client.
-    #
-    # Blocks until the a reply message is received with the expected sequence number that is
-    # associated with @a token. The client must have called prepare_client_receive() previously.
-    #
-    # @param self
-    # @param token The token previously returned by prepare_client_receive().
-    # @return bytearray containing the received message.
-    def client_receive(self, token):
-        try:
-            # Look up our client info.
-            try:
-                self._lock.acquire()
-                client = self._pending_clients[token]
-            finally:
-                self._lock.release()
-
-            # Wait for the reply to be received.
-            client.event.wait()
-
-            # Remove this client from the pending clients dict.
-            try:
-                self._lock.acquire()
-                del self._pending_clients[token]
-            finally:
-                self._lock.release()
-
-            # Return the received message.
-            return client.msg
-        except KeyError:
-            pass
-
-
-
+#!/usr/bin/env python
+
+# Copyright 2016 NXP
+# All rights reserved.
+#
+# SPDX-License-Identifier: BSD-3-Clause
+
+import threading
+from collections import namedtuple
+from .codec import MessageType
+from .transport import Transport
+
+class ClientInfo:
+    event = None
+    msg = None
+
+##
+# @brief Shares a transport between a server and multiple clients.
+class TransportArbitrator(Transport):
+    def __init__(self, sharedTransport=None, codec=None):
+        self._transport = sharedTransport
+        self._codec = codec
+        self._pending_clients = {}
+        self._lock = threading.Lock()
+
+    @property
+    def shared_transport(self):
+        return self._transport
+
+    @shared_transport.setter
+    def shared_transport(self, transport):
+        self._transport = transport
+
+    @property
+    def codec(self):
+        return self._codec
+
+    @codec.setter
+    def codec(self, theCodec):
+        self._codec = theCodec
+
+    def send(self, message):
+        assert self._transport is not None, "No shared transport was set"
+        self._transport.send(message)
+
+    def receive(self):
+        assert self._transport is not None, "No shared transport was set"
+        assert self._codec is not None, "No codec was set"
+
+        # Repeatedly receive until we get an invocation request.
+        while True:
+            # Receive a message from the shared transport.
+            msg = self._transport.receive()
+
+            # Parse the message header.
+            self._codec.buffer = msg
+            info = self._codec.start_read_message()
+
+            # If it's an invocation or oneway, return it to the server.
+            if info.type in (MessageType.kInvocationMessage, MessageType.kOnewayMessage):
+                return msg
+            # Ignore unexpected message types.
+            elif info.type != MessageType.kReplyMessage:
+                continue
+
+            # Look up the client waiting for this reply.
+            try:
+                try:
+                    self._lock.acquire()
+                    client = self._pending_clients[info.sequence]
+                finally:
+                    self._lock.release()
+                client.msg = msg
+                client.event.set()
+            except KeyError:
+                # No client was found, unexpected sequence number!
+                pass
+
+    ##
+    # @brief Add a client request to the client list.
+    #
+    # This call is made by the client thread prior to sending the invocation to the server. It
+    # ensures that the transport arbitrator has the client's response message buffer ready in
+    # case it sees the response before the client even has a chance to call client_receive().
+    #
+    # @param self
+    # @param requestContext
+    # @return A token value to be passed to client_receive().
+    def prepare_client_receive(self, requestContext):
+        # Create pending client info.
+        info = ClientInfo()
+        info.event = threading.Event()
+
+        # Add this client to the pending clients dict.
+        try:
+            self._lock.acquire()
+            self._pending_clients[requestContext.sequence] = info
+        finally:
+            self._lock.release()
+
+        return requestContext.sequence
+
+    ##
+    # @brief Receive method for the client.
+    #
+    # Blocks until the a reply message is received with the expected sequence number that is
+    # associated with @a token. The client must have called prepare_client_receive() previously.
+    #
+    # @param self
+    # @param token The token previously returned by prepare_client_receive().
+    # @return bytearray containing the received message.
+    def client_receive(self, token):
+        try:
+            # Look up our client info.
+            try:
+                self._lock.acquire()
+                client = self._pending_clients[token]
+            finally:
+                self._lock.release()
+
+            # Wait for the reply to be received.
+            client.event.wait()
+
+            # Remove this client from the pending clients dict.
+            try:
+                self._lock.acquire()
+                del self._pending_clients[token]
+            finally:
+                self._lock.release()
+
+            # Return the received message.
+            return client.msg
+        except KeyError:
+            pass
+
+
+
```

### Comparing `erpc-1.9.0/erpc/basic_codec.py` & `erpc-1.9.1/erpc/basic_codec.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-#!/usr/bin/env python
-
-# Copyright (c) 2015 Freescale Semiconductor, Inc.
-# Copyright 2016-2017 NXP
-# All rights reserved.
-#
-# SPDX-License-Identifier: BSD-3-Clause
-
-import struct
-from .codec import (MessageType, MessageInfo, Codec, CodecError)
-
-class BasicCodec(Codec):
-    ## Version of this codec.
-    BASIC_CODEC_VERSION = 1
-
-    def start_write_message(self, msgInfo):
-        header = (self.BASIC_CODEC_VERSION << 24) \
-                        | ((msgInfo.service & 0xff) << 16) \
-                        | ((msgInfo.request & 0xff) << 8) \
-                        | (msgInfo.type.value & 0xff)
-        self.write_uint32(header)
-        self.write_uint32(msgInfo.sequence)
-
-    def _write(self, fmt, value):
-        self._buffer += struct.pack(fmt, value)
-        self._cursor += struct.calcsize(fmt)
-
-    def write_bool(self, value):
-        self._write('<?', value)
-
-    def write_int8(self, value):
-        self._write('<b', value)
-
-    def write_int16(self, value):
-        self._write('<h', value)
-
-    def write_int32(self, value):
-        self._write('<i', value)
-
-    def write_int64(self, value):
-        self._write('<q', value)
-
-    def write_uint8(self, value):
-        self._write('<B', value)
-
-    def write_uint16(self, value):
-        self._write('<H', value)
-
-    def write_uint32(self, value):
-        self._write('<I', value)
-
-    def write_uint64(self, value):
-        self._write('<Q', value)
-
-    def write_float(self, value):
-        self._write('<f', value)
-
-    def write_double(self, value):
-        self._write('<d', value)
-
-    def write_string(self, value):
-        self.write_binary(value.encode())
-
-    def write_binary(self, value):
-        self.write_uint32(len(value))
-        self._buffer += value
-
-    def start_write_list(self, length):
-        self.write_uint32(length)
-
-    def start_write_union(self, discriminator):
-        self.write_uint32(discriminator)
-
-    def write_null_flag(self, flag):
-        self.write_uint8(1 if flag else 0)
-
-    ##
-    # @return 4-tuple of msgType, service, request, sequence.
-    def start_read_message(self):
-        header = self.read_uint32()
-        sequence = self.read_uint32()
-        version = header >> 24
-        if version != self.BASIC_CODEC_VERSION:
-            raise CodecError("unsupported codec version %d" % version)
-        service = (header >> 16) & 0xff
-        request = (header >> 8) & 0xff
-        msgType = MessageType(header & 0xff)
-        return MessageInfo(type=msgType, service=service, request=request, sequence=sequence)
-
-    def _read(self, fmt):
-        result = struct.unpack_from(fmt, self._buffer, self._cursor)
-        self._cursor += struct.calcsize(fmt)
-        return result[0]
-
-    def read_bool(self):
-        return self._read('<?')
-
-    def read_int8(self):
-        return self._read('<b')
-
-    def read_int16(self):
-        return self._read('<h')
-
-    def read_int32(self):
-        return self._read('<i')
-
-    def read_int64(self):
-        return self._read('<q')
-
-    def read_uint8(self):
-        return self._read('<B')
-
-    def read_uint16(self):
-        return self._read('<H')
-
-    def read_uint32(self):
-        return self._read('<I')
-
-    def read_uint64(self):
-        return self._read('<Q')
-
-    def read_float(self):
-        return self._read('<f')
-
-    def read_double(self):
-        return self._read('<d')
-
-    def read_string(self):
-        return self.read_binary().decode()
-
-    def read_binary(self):
-        length = self.read_uint32()
-        data = self._buffer[self._cursor:self._cursor+length]
-        self._cursor += length
-        return data
-
-    ##
-    # @return Int of list length.
-    def start_read_list(self):
-        return self.read_uint32()
-
-    ##
-    # @return Int of union discriminator.
-    def start_read_union(self):
-        return self.read_int32()
-
-    def read_null_flag(self):
-        return self.read_uint8()
-
-
-
+#!/usr/bin/env python
+
+# Copyright (c) 2015 Freescale Semiconductor, Inc.
+# Copyright 2016-2017 NXP
+# All rights reserved.
+#
+# SPDX-License-Identifier: BSD-3-Clause
+
+import struct
+from .codec import (MessageType, MessageInfo, Codec, CodecError)
+
+class BasicCodec(Codec):
+    ## Version of this codec.
+    BASIC_CODEC_VERSION = 1
+
+    def start_write_message(self, msgInfo):
+        header = (self.BASIC_CODEC_VERSION << 24) \
+                        | ((msgInfo.service & 0xff) << 16) \
+                        | ((msgInfo.request & 0xff) << 8) \
+                        | (msgInfo.type.value & 0xff)
+        self.write_uint32(header)
+        self.write_uint32(msgInfo.sequence)
+
+    def _write(self, fmt, value):
+        self._buffer += struct.pack(fmt, value)
+        self._cursor += struct.calcsize(fmt)
+
+    def write_bool(self, value):
+        self._write('<?', value)
+
+    def write_int8(self, value):
+        self._write('<b', value)
+
+    def write_int16(self, value):
+        self._write('<h', value)
+
+    def write_int32(self, value):
+        self._write('<i', value)
+
+    def write_int64(self, value):
+        self._write('<q', value)
+
+    def write_uint8(self, value):
+        self._write('<B', value)
+
+    def write_uint16(self, value):
+        self._write('<H', value)
+
+    def write_uint32(self, value):
+        self._write('<I', value)
+
+    def write_uint64(self, value):
+        self._write('<Q', value)
+
+    def write_float(self, value):
+        self._write('<f', value)
+
+    def write_double(self, value):
+        self._write('<d', value)
+
+    def write_string(self, value):
+        self.write_binary(value.encode())
+
+    def write_binary(self, value):
+        self.write_uint32(len(value))
+        self._buffer += value
+
+    def start_write_list(self, length):
+        self.write_uint32(length)
+
+    def start_write_union(self, discriminator):
+        self.write_uint32(discriminator)
+
+    def write_null_flag(self, flag):
+        self.write_uint8(1 if flag else 0)
+
+    ##
+    # @return 4-tuple of msgType, service, request, sequence.
+    def start_read_message(self):
+        header = self.read_uint32()
+        sequence = self.read_uint32()
+        version = header >> 24
+        if version != self.BASIC_CODEC_VERSION:
+            raise CodecError("unsupported codec version %d" % version)
+        service = (header >> 16) & 0xff
+        request = (header >> 8) & 0xff
+        msgType = MessageType(header & 0xff)
+        return MessageInfo(type=msgType, service=service, request=request, sequence=sequence)
+
+    def _read(self, fmt):
+        result = struct.unpack_from(fmt, self._buffer, self._cursor)
+        self._cursor += struct.calcsize(fmt)
+        return result[0]
+
+    def read_bool(self):
+        return self._read('<?')
+
+    def read_int8(self):
+        return self._read('<b')
+
+    def read_int16(self):
+        return self._read('<h')
+
+    def read_int32(self):
+        return self._read('<i')
+
+    def read_int64(self):
+        return self._read('<q')
+
+    def read_uint8(self):
+        return self._read('<B')
+
+    def read_uint16(self):
+        return self._read('<H')
+
+    def read_uint32(self):
+        return self._read('<I')
+
+    def read_uint64(self):
+        return self._read('<Q')
+
+    def read_float(self):
+        return self._read('<f')
+
+    def read_double(self):
+        return self._read('<d')
+
+    def read_string(self):
+        return self.read_binary().decode()
+
+    def read_binary(self):
+        length = self.read_uint32()
+        data = self._buffer[self._cursor:self._cursor+length]
+        self._cursor += length
+        return data
+
+    ##
+    # @return Int of list length.
+    def start_read_list(self):
+        return self.read_uint32()
+
+    ##
+    # @return Int of union discriminator.
+    def start_read_union(self):
+        return self.read_int32()
+
+    def read_null_flag(self):
+        return self.read_uint8()
+
+
+
```

### Comparing `erpc-1.9.0/erpc/client.py` & `erpc-1.9.1/erpc/client.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-#!/usr/bin/env python
-
-# Copyright 2016 NXP
-# All rights reserved.
-#
-# SPDX-License-Identifier: BSD-3-Clause
-
-from .codec import MessageType
-
-class RequestError(RuntimeError):
-    pass
-
-class ClientManager(object):
-    def __init__(self, transport=None, codecClass=None):
-        self._transport = transport
-        self._arbitrator = None
-        self._codecClass = codecClass
-        self._sequence = 0
-
-    @property
-    def transport(self):
-        return self._transport
-
-    @transport.setter
-    def transport(self, value):
-        self._transport = value
-
-    @property
-    def arbitrator(self):
-        return self._arbitrator
-
-    @arbitrator.setter
-    def arbitrator(self, arb):
-        self._arbitrator = arb
-
-    @property
-    def codec_class(self):
-        return self._codecClass
-
-    @codec_class.setter
-    def codec_class(self, value):
-        self._codecClass = value
-
-    @property
-    def sequence(self):
-        self._sequence += 1
-        return self._sequence
-
-    def create_request(self, isOneway=False):
-        msg = bytearray()
-        codec = self.codec_class()
-        codec.buffer = msg
-        return RequestContext(self.sequence, msg, codec, isOneway)
-
-    def perform_request(self, request):
-        # Arbitrate requests.
-        token = None
-        if self._arbitrator is not None and not request.is_oneway:
-            token = self._arbitrator.prepare_client_receive(request)
-
-        # Send serialized request to server.
-        self.transport.send(request.codec.buffer)
-
-        if not request.is_oneway:
-            if token is not None:
-                msg = self._arbitrator.client_receive(token)
-            else:
-                msg = self.transport.receive()
-            request.codec.buffer = msg
-
-            info = request.codec.start_read_message()
-            if info.type != MessageType.kReplyMessage:
-                raise RequestError("invalid reply message type")
-            if info.sequence != request.sequence:
-                raise RequestError("unexpected sequence number in reply (was %d, expected %d)"
-                            % (info.sequence, request.sequence))
-
-
-class RequestContext(object):
-    def __init__(self, sequence, message, codec, isOneway):
-        self._sequence = sequence
-        self._message = message
-        self._codec = codec
-        self._isOneway = isOneway
-
-    @property
-    def sequence(self):
-        return self._sequence
-
-    @property
-    def message(self):
-        return self._message
-
-    @property
-    def codec(self):
-        return self._codec
-
-    @property
-    def is_oneway(self):
-        return self._isOneway
-
-
-
+#!/usr/bin/env python
+
+# Copyright 2016 NXP
+# All rights reserved.
+#
+# SPDX-License-Identifier: BSD-3-Clause
+
+from .codec import MessageType
+
+class RequestError(RuntimeError):
+    pass
+
+class ClientManager(object):
+    def __init__(self, transport=None, codecClass=None):
+        self._transport = transport
+        self._arbitrator = None
+        self._codecClass = codecClass
+        self._sequence = 0
+
+    @property
+    def transport(self):
+        return self._transport
+
+    @transport.setter
+    def transport(self, value):
+        self._transport = value
+
+    @property
+    def arbitrator(self):
+        return self._arbitrator
+
+    @arbitrator.setter
+    def arbitrator(self, arb):
+        self._arbitrator = arb
+
+    @property
+    def codec_class(self):
+        return self._codecClass
+
+    @codec_class.setter
+    def codec_class(self, value):
+        self._codecClass = value
+
+    @property
+    def sequence(self):
+        self._sequence += 1
+        return self._sequence
+
+    def create_request(self, isOneway=False):
+        msg = bytearray()
+        codec = self.codec_class()
+        codec.buffer = msg
+        return RequestContext(self.sequence, msg, codec, isOneway)
+
+    def perform_request(self, request):
+        # Arbitrate requests.
+        token = None
+        if self._arbitrator is not None and not request.is_oneway:
+            token = self._arbitrator.prepare_client_receive(request)
+
+        # Send serialized request to server.
+        self.transport.send(request.codec.buffer)
+
+        if not request.is_oneway:
+            if token is not None:
+                msg = self._arbitrator.client_receive(token)
+            else:
+                msg = self.transport.receive()
+            request.codec.buffer = msg
+
+            info = request.codec.start_read_message()
+            if info.type != MessageType.kReplyMessage:
+                raise RequestError("invalid reply message type")
+            if info.sequence != request.sequence:
+                raise RequestError("unexpected sequence number in reply (was %d, expected %d)"
+                            % (info.sequence, request.sequence))
+
+
+class RequestContext(object):
+    def __init__(self, sequence, message, codec, isOneway):
+        self._sequence = sequence
+        self._message = message
+        self._codec = codec
+        self._isOneway = isOneway
+
+    @property
+    def sequence(self):
+        return self._sequence
+
+    @property
+    def message(self):
+        return self._message
+
+    @property
+    def codec(self):
+        return self._codec
+
+    @property
+    def is_oneway(self):
+        return self._isOneway
+
+
+
```

### Comparing `erpc-1.9.0/erpc/simple_server.py` & `erpc-1.9.1/erpc/simple_server.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-#!/usr/bin/env python
-
-# Copyright 2016 NXP
-# All rights reserved.
-#
-# SPDX-License-Identifier: BSD-3-Clause
-
-from __future__ import print_function
-
-import threading
-from .server import (Service, Server)
-from .client import RequestError
-
-class SimpleServer(Server):
-    def __init__(self, transport=None, codecClass=None):
-        super(SimpleServer, self).__init__(transport, codecClass)
-        self._run = True
-
-    def run(self):
-        self._run = True
-        while self._run:
-            try:
-                self._receive_request()
-            except RequestError as e:
-                print("Error while processing request: %s" % (e))
-
-    def stop(self):
-        self._run = False
-
-    def _receive_request(self):
-        msg = self.transport.receive()
-        
-        codec = self.codec_class()
-        codec.buffer = msg
-        
-        self._process_request(codec)
-
-        if len(codec.buffer):
-            self.transport.send(codec.buffer)
-
-class ServerThread(SimpleServer):
-    def __init__(self, transport, codecClass):
-        super(ServerThread, self).__init__(transport, codecClass)
-        self._thread = threading.Thread(target=self.run, name="erpc_server")
-        self._thread.daemon = True
-
-    def start(self):
-        self._thread.start()
-
+#!/usr/bin/env python
+
+# Copyright 2016 NXP
+# All rights reserved.
+#
+# SPDX-License-Identifier: BSD-3-Clause
+
+from __future__ import print_function
+
+import threading
+from .server import (Service, Server)
+from .client import RequestError
+
+class SimpleServer(Server):
+    def __init__(self, transport=None, codecClass=None):
+        super(SimpleServer, self).__init__(transport, codecClass)
+        self._run = True
+
+    def run(self):
+        self._run = True
+        while self._run:
+            try:
+                self._receive_request()
+            except RequestError as e:
+                print("Error while processing request: %s" % (e))
+
+    def stop(self):
+        self._run = False
+
+    def _receive_request(self):
+        msg = self.transport.receive()
+        
+        codec = self.codec_class()
+        codec.buffer = msg
+        
+        self._process_request(codec)
+
+        if len(codec.buffer):
+            self.transport.send(codec.buffer)
+
+class ServerThread(SimpleServer):
+    def __init__(self, transport, codecClass):
+        super(ServerThread, self).__init__(transport, codecClass)
+        self._thread = threading.Thread(target=self.run, name="erpc_server")
+        self._thread.daemon = True
+
+    def start(self):
+        self._thread.start()
+
```

### Comparing `erpc-1.9.0/erpc/__init__.py` & `erpc-1.9.1/erpc/__init__.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-#!/usr/bin/env python
-
-# Copyright 2016 NXP
-# All rights reserved.
-#
-# SPDX-License-Identifier: BSD-3-Clause
-
-import os
-# Yocto and python27 combination
-if "IS_YOCTO" in os.environ:
-    from . import erpc_version
-else:
-    from . import arbitrator
-    from . import basic_codec
-    from . import codec
-    from . import client
-    from . import crc16
-    from . import server
-    from . import simple_server
-    from . import transport
-
-##
-# @brief Simple container class used for pass by reference.
-class Reference(object):
-    def __init__(self, value=None):
-        ## Read/write attribute holding the referent.
-        self.value = value
-
-    def __str__(self):
-        return "<%s@%x value=%s>" % (self.__class__.__name__, id(self), repr(self.value))
-
-    def __repr__(self):
-        return self.__str__()
-
+#!/usr/bin/env python
+
+# Copyright 2016 NXP
+# All rights reserved.
+#
+# SPDX-License-Identifier: BSD-3-Clause
+
+import os
+# Yocto and python27 combination
+if "IS_YOCTO" in os.environ:
+    from . import erpc_version
+else:
+    from . import arbitrator
+    from . import basic_codec
+    from . import codec
+    from . import client
+    from . import crc16
+    from . import server
+    from . import simple_server
+    from . import transport
+
+##
+# @brief Simple container class used for pass by reference.
+class Reference(object):
+    def __init__(self, value=None):
+        ## Read/write attribute holding the referent.
+        self.value = value
+
+    def __str__(self):
+        return "<%s@%x value=%s>" % (self.__class__.__name__, id(self), repr(self.value))
+
+    def __repr__(self):
+        return self.__str__()
+
```

### Comparing `erpc-1.9.0/erpc.egg-info/PKG-INFO` & `erpc-1.9.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: erpc
-Version: 1.9.0
+Version: 1.9.1
 Summary: eRPC Python infrastructure
 Home-page: https://github.com/embeddedrpc/erpc
 Author: NXP
 License: BSD 3-Clause
-Description: eRPC Python Infrastructure
-        ==========================
-        
-        This folder contains the Python implementation of the eRPC infrastructure.
-        
-        The eRPC project is stored on Github: https://github.com/EmbeddedRPC/erpc
-        
-        The Python implementation of eRPC is fully compatible with the C/C++ implementation at the
-        protocol level. Also, the classes mirror those in the C++ infrastructure.
-        
-        Installation:
-        
-           To install the eRPC Python infrastructure, run the setup.py script like this:
-        
-               pip install erpc
-        
-        
-           Once installed, you can access the infrastructure via a standard import statement.
-        
-               import erpc
-               xport = erpc.transport.SerialTransport("/dev/ttyS1", 115200)
-               client = erpc.client.ClientManager(xport, erpc.basic_codec.BasicCodec)
-        
+Description: # eRPC Python Infrastructure
+        
+        This folder contains the Python implementation of the eRPC infrastructure.
+        
+        The eRPC project is stored on Github: [github.com/EmbeddedRPC/erpc](https://github.com/EmbeddedRPC/erpc)
+        
+        The Python implementation of eRPC is fully compatible with the C/C++ implementation at the
+        protocol level. Also, the classes mirror those in the C++ infrastructure.
+        
+        Installation:
+        
+           To install the eRPC Python infrastructure, run the setup.py script like this:
+        
+        ```sh
+        pip install erpc
+        ```
+        
+           Once installed, you can access the infrastructure via a standard import statement.
+        
+        ```python
+        import erpc
+        xport = erpc.transport.SerialTransport("/dev/ttyS1", 115200)
+        client = erpc.client.ClientManager(xport, erpc.basic_codec.BasicCodec)
+        ```
         
 Keywords: rpc rpc-framework embedded multicore multiprocessor amp rpmsg_lite
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
```

### Comparing `erpc-1.9.0/PKG-INFO` & `erpc-1.9.1/erpc.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: erpc
-Version: 1.9.0
+Version: 1.9.1
 Summary: eRPC Python infrastructure
 Home-page: https://github.com/embeddedrpc/erpc
 Author: NXP
 License: BSD 3-Clause
-Description: eRPC Python Infrastructure
-        ==========================
-        
-        This folder contains the Python implementation of the eRPC infrastructure.
-        
-        The eRPC project is stored on Github: https://github.com/EmbeddedRPC/erpc
-        
-        The Python implementation of eRPC is fully compatible with the C/C++ implementation at the
-        protocol level. Also, the classes mirror those in the C++ infrastructure.
-        
-        Installation:
-        
-           To install the eRPC Python infrastructure, run the setup.py script like this:
-        
-               pip install erpc
-        
-        
-           Once installed, you can access the infrastructure via a standard import statement.
-        
-               import erpc
-               xport = erpc.transport.SerialTransport("/dev/ttyS1", 115200)
-               client = erpc.client.ClientManager(xport, erpc.basic_codec.BasicCodec)
-        
+Description: # eRPC Python Infrastructure
+        
+        This folder contains the Python implementation of the eRPC infrastructure.
+        
+        The eRPC project is stored on Github: [github.com/EmbeddedRPC/erpc](https://github.com/EmbeddedRPC/erpc)
+        
+        The Python implementation of eRPC is fully compatible with the C/C++ implementation at the
+        protocol level. Also, the classes mirror those in the C++ infrastructure.
+        
+        Installation:
+        
+           To install the eRPC Python infrastructure, run the setup.py script like this:
+        
+        ```sh
+        pip install erpc
+        ```
+        
+           Once installed, you can access the infrastructure via a standard import statement.
+        
+        ```python
+        import erpc
+        xport = erpc.transport.SerialTransport("/dev/ttyS1", 115200)
+        client = erpc.client.ClientManager(xport, erpc.basic_codec.BasicCodec)
+        ```
         
 Keywords: rpc rpc-framework embedded multicore multiprocessor amp rpmsg_lite
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
```

### Comparing `erpc-1.9.0/setup.py` & `erpc-1.9.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-#!/usr/bin/env python
-
-# Copyright (c) 2016 Freescale Semiconductor, Inc.
-# Copyright 2016-2019 NXP
-# All rights reserved.
-#
-# SPDX-License-Identifier: BSD-3-Clause
-
-from setuptools import setup
-from erpc import erpc_version
-from codecs import open
-from os import path
-
-here = path.abspath(path.dirname(__file__))
-
-with open(path.join(here, 'README_Pypi.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-#steps: https://packaging.python.org/distributing/
-#source distribution: python setup.py sdist
-#wheel distribution: python setup.py bdist_wheel
-#web: https://pypi.python.org/pypi?%3Aaction=submit_form
-
-setup(
-    name="erpc",
-    version=erpc_version.ERPC_VERSION,
-    description="eRPC Python infrastructure",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author="NXP",
-    url='https://github.com/embeddedrpc/erpc',
-    license="BSD 3-Clause",
-    install_requires=["enum34","pyserial"],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "License :: OSI Approved :: BSD License",
-        "Programming Language :: Python",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Embedded Systems",
-        "Natural Language :: English",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-        "Operating System :: POSIX :: Linux",
-    ],
-    keywords='rpc rpc-framework embedded multicore multiprocessor amp rpmsg_lite',
-    use_2to3=True,
-    packages=['erpc'],
-)
+#!/usr/bin/env python
+
+# Copyright (c) 2016 Freescale Semiconductor, Inc.
+# Copyright 2016-2019 NXP
+# Copyright 2022 ACRIOS Systems s.r.o.
+# All rights reserved.
+#
+# SPDX-License-Identifier: BSD-3-Clause
+
+from setuptools import setup
+from codecs import open
+from os import path
+
+ERPC_VERSION = None
+here = path.abspath(path.dirname(__file__))
+
+with open(path.join(here, 'README_Pypi.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+with open(path.join(here, 'erpc', 'erpc_version.py')) as f:
+    exec(f.read())
+
+#steps: https://packaging.python.org/distributing/
+#source distribution: python setup.py sdist
+#wheel distribution: python setup.py bdist_wheel
+#web: https://pypi.python.org/pypi?%3Aaction=submit_form
+
+setup(
+    name="erpc",
+    version=ERPC_VERSION,
+    description="eRPC Python infrastructure",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author="NXP",
+    url='https://github.com/embeddedrpc/erpc',
+    license="BSD 3-Clause",
+    install_requires=[],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Embedded Systems",
+        "Natural Language :: English",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: POSIX :: Linux",
+    ],
+    keywords='rpc rpc-framework embedded multicore multiprocessor amp rpmsg_lite',
+    packages=['erpc'],
+)
```

