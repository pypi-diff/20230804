# Comparing `tmp/hivemind_local-0.0.3a3-py3-none-any.whl.zip` & `tmp/hivemind_local-0.0.3a4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 7830 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-Aug-03 19:03 local_hive/__init__.py
--rw-r--r--  2.0 unx      205 b- defN 23-Aug-03 19:03 local_hive/__main__.py
--rw-r--r--  2.0 unx      171 b- defN 23-Aug-03 19:03 local_hive/exceptions.py
--rw-r--r--  2.0 unx      630 b- defN 23-Aug-03 19:03 local_hive/fakebus.py
--rw-r--r--  2.0 unx     2536 b- defN 23-Aug-03 19:03 local_hive/loader.py
--rw-r--r--  2.0 unx     9754 b- defN 23-Aug-03 19:03 local_hive/protocol.py
--rw-r--r--  2.0 unx     3988 b- defN 23-Aug-03 19:03 local_hive/service.py
--rw-r--r--  2.0 unx      177 b- defN 23-Aug-03 19:03 local_hive/version.py
--rw-r--r--  2.0 unx      446 b- defN 23-Aug-03 19:03 hivemind_local-0.0.3a3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 19:03 hivemind_local-0.0.3a3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Aug-03 19:03 hivemind_local-0.0.3a3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      955 b- defN 23-Aug-03 19:03 hivemind_local-0.0.3a3.dist-info/RECORD
-12 files, 18965 bytes uncompressed, 6222 bytes compressed:  67.2%
+Zip file size: 7379 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-Aug-03 22:27 local_hive/__init__.py
+-rw-r--r--  2.0 unx      205 b- defN 23-Aug-03 22:27 local_hive/__main__.py
+-rw-r--r--  2.0 unx      171 b- defN 23-Aug-03 22:27 local_hive/exceptions.py
+-rw-r--r--  2.0 unx     2466 b- defN 23-Aug-03 22:27 local_hive/loader.py
+-rw-r--r--  2.0 unx     9942 b- defN 23-Aug-03 22:27 local_hive/protocol.py
+-rw-r--r--  2.0 unx     4014 b- defN 23-Aug-03 22:27 local_hive/service.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Aug-03 22:27 local_hive/version.py
+-rw-r--r--  2.0 unx      446 b- defN 23-Aug-03 22:27 hivemind_local-0.0.3a4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-03 22:27 hivemind_local-0.0.3a4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Aug-03 22:27 hivemind_local-0.0.3a4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Aug-03 22:27 hivemind_local-0.0.3a4.dist-info/RECORD
+11 files, 18402 bytes uncompressed, 5889 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -3,35 +3,32 @@
 
 Filename: local_hive/__main__.py
 Comment: 
 
 Filename: local_hive/exceptions.py
 Comment: 
 
-Filename: local_hive/fakebus.py
-Comment: 
-
 Filename: local_hive/loader.py
 Comment: 
 
 Filename: local_hive/protocol.py
 Comment: 
 
 Filename: local_hive/service.py
 Comment: 
 
 Filename: local_hive/version.py
 Comment: 
 
-Filename: hivemind_local-0.0.3a3.dist-info/METADATA
+Filename: hivemind_local-0.0.3a4.dist-info/METADATA
 Comment: 
 
-Filename: hivemind_local-0.0.3a3.dist-info/WHEEL
+Filename: hivemind_local-0.0.3a4.dist-info/WHEEL
 Comment: 
 
-Filename: hivemind_local-0.0.3a3.dist-info/top_level.txt
+Filename: hivemind_local-0.0.3a4.dist-info/top_level.txt
 Comment: 
 
-Filename: hivemind_local-0.0.3a3.dist-info/RECORD
+Filename: hivemind_local-0.0.3a4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## local_hive/loader.py

```diff
@@ -1,76 +1,81 @@
 import os
-from time import sleep
 
-from ovos_workshop.skill_launcher import SkillLoader
-from ovos_bus_client import Message
+from hivemind_bus_client import HiveMessageBusClient, HiveMessage, HiveMessageType
+from hivemind_bus_client.protocol import HiveMindSlaveProtocol
 from ovos_utils.log import LOG
+from ovos_utils.messagebus import FakeBus
+from ovos_workshop.skill_launcher import SkillLoader
 
-from hivemind_bus_client import HiveMessageBusClient, HiveMessage, HiveMessageType
-from local_hive.fakebus import FakeBus
+
+class SkillProtocol(HiveMindSlaveProtocol):
+
+    def handle_bus(self, message):
+        LOG.debug(f">>: {message.payload.msg_type}")
+        # inject the hivemind to the skill FakeBus
+        # flag SkillBus to not re-emit it to HM connection
+        message.payload.context["source"] = "IntentService"
+        self.internal_protocol.bus.emit(message.payload, send2hm=False)
+
+
+class SkillBus(FakeBus):
+
+    def __init__(self, skill_id, hive, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.skill_id = skill_id
+        self.hive = hive
+
+    def emit(self, message, send2hm=True):
+        # ensure skill_id in all messages
+        message.context["skill_id"] = self.skill_id
+        if not message.context.get("source"):
+            message.context["source"] = self.skill_id
+
+        super().emit(message)
+
+        if send2hm:
+            msg = HiveMessage(HiveMessageType.BUS, payload=message)
+            LOG.debug(f"<<: {message.msg_type}")
+            self.hive.emit(msg)
 
 
 class HiveMindExternalSkillWrapper:
     def __init__(self, skill_directory, port=6989, host="127.0.0.1"):
         skill_id = os.path.basename(skill_directory)
 
         self.path = skill_directory
         self.skill_id = skill_id
 
-        # fakebus so we can intercept and modify before sending to hivemind
-        # we could technically pass the hivemind connection directly,
-        # especially since ovos-core ensures the skill_id is present in the context
-        # however this makes it easier to expand functionality in the future
-        self.bus = FakeBus()
-        self.bus.on("message", self.handle_skill_emit)
-        self.bus.bind(self.skill_id)
-
         self.hive = HiveMessageBusClient(self.skill_id, port=port, host=host)
-        self.hive.connect(self.bus)
-
         self.hive.on_close = self.handle_shutdown
-        self.hive.on(HiveMessageType.BUS, self.handle_hive_message)
+
+        self.bus = SkillBus(self.skill_id, self.hive)
+
+        protocol = SkillProtocol(self.hive)
+
+        protocol.bind(self.bus)
+        self.hive.connect(self.bus, protocol=protocol)
 
         self.skill_loader = SkillLoader(self.bus, self.path)
         self.load()
 
     @property
     def instance(self):
         return self.skill_loader.instance
 
     def handle_shutdown(self):
         try:
             self.instance.shutdown()
         except:
             pass
 
-    def connect_to_hive(self):
-        self.hive.run_in_thread()
-        while not self.hive.connected_event.is_set():
-            sleep(0.1)
-
     def load(self):
-        self.connect_to_hive()
         self.skill_loader.load()
         return self
 
-    def handle_skill_emit(self, message):
-        if isinstance(message, str):
-            message = Message.deserialize(message)
-        message.context["skill_id"] = self.skill_id
-        if not message.context.get("source"):
-            message.context["source"] = self.skill_id
-        msg = HiveMessage(HiveMessageType.BUS, payload=message)
-        LOG.debug(f"<<: {message.msg_type}")
-        self.hive.emit(msg)
-
-    def handle_hive_message(self, message):
-        LOG.debug(f">>: {message.payload.msg_type}")
-        self.bus.emit(message.payload)
-
 
 def load_skills_folder(folder):
     for f in os.listdir(folder):
         if f.startswith("_") or f.startswith("."):
             continue
         path = os.path.join(folder, f)
         if os.path.isdir(path):
```

## local_hive/protocol.py

```diff
@@ -1,26 +1,24 @@
 from hivemind_bus_client.message import HiveMessage, HiveMessageType
 from hivemind_core.protocol import HiveMindListenerProtocol, HiveMindClientConnection, \
     HiveMindListenerInternalProtocol
 from ovos_bus_client import Message
 from ovos_core.intent_services import IntentService
 from ovos_utils.log import LOG
-
-from local_hive.fakebus import FakeBus
+from ovos_utils.messagebus import FakeBus
 
 
 class LocalHiveInternalProtocol(HiveMindListenerInternalProtocol):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.intent_service = None
         self.intent2skill = {}
         self.permission_overrides = {}
 
     def register_bus_handlers(self):
-        LOG.info("registering intent service bus handlers")
         self.intent_service = IntentService(self.bus)
         self.bus.on("message", self.handle_internal_mycroft)  # catch all
 
     def skill2peer(self, skill_id):
         for peer, client in self.clients.items():
             if client.key == skill_id:
                 return peer
@@ -31,70 +29,70 @@
         """ forward internal messages to clients if they are the target
         here is where the client isolation happens,
         clients only get responses to their own messages"""
 
         # "message" event is a special case in ovos-bus-client that is not deserialized
         message = Message.deserialize(message)
 
+        if message.msg_type in ["skill.converse.ping"]:
+            LOG.info("Converse ping")
+            # TODO - careful to avoid infinite loop
+            #for client in self.clients.values():
+            #    client.send(
+            #        HiveMessage(HiveMessageType.BUS, message)
+            #    )
+            #return
+
         skill_id = message.context.get("skill_id")
+
+        skill_peer = self.skill2peer(skill_id)
+        if not skill_peer:
+            print(666, message.msg_type)
+            return
+
+        client = self.clients[skill_peer]
+
         peers = message.context.get("destination") or []
 
         # converse method handling
         if message.msg_type in ["skill.converse.request"]:
-            skill_id = message.data.get("skill_id")
-            message.context["skill_id"] = skill_id
-            skill_peer = self.skill2peer(skill_id)
             LOG.info(f"Converse: {message.msg_type} "
                      f"Skill: {skill_id} "
                      f"Peer: {skill_peer}")
-            message.context['source'] = "IntentService"
-            message.context['destination'] = peers
-            client = self.clients[skill_peer]
-            client.send(
-                HiveMessage(HiveMessageType.BUS, message)
-            )
-
+            #client.send(
+            #    HiveMessage(HiveMessageType.BUS, message)
+            #)
         elif message.msg_type in ["skill.converse.response"]:
-            # just logging that it was received, converse method handled by
-            # skill
-            skill_id = message.data.get("skill_id")
             response = message.data.get("result")
-            message.context["skill_id"] = skill_id
-            skill_peer = self.skill2peer(skill_id)
             LOG.info(f"Converse Response: {response} "
                      f"Skill: {skill_id} "
                      f"Peer: {skill_peer}")
-            message.context['source'] = skill_id
-            message.context['destination'] = peers
-
         # intent found
         elif message.msg_type in self.intent2skill:
-            skill_id = self.intent2skill[message.msg_type]
-            skill_peer = self.skill2peer(skill_id)
-            message.context["skill_id"] = skill_id
-
             LOG.info(f"Intent: {message.msg_type} "
                      f"Skill: {skill_id} "
                      f"Source: {peers} "
                      f"Target: {skill_peer}")
-
             # trigger the skill
-            message.context['source'] = "IntentService"
             LOG.debug(f"Triggering intent: {skill_peer}")
-            client = self.clients[skill_peer]
             client.send(
                 HiveMessage(HiveMessageType.BUS, message)
             )
-
+            return
         # skill registering intent - keep track internally
         elif message.msg_type in ["register_intent",
                                   "padatious:register_intent"]:
             LOG.info(f"Register Intent: {message.data['name']} "
                      f"Skill: {message.context['skill_id']}")
             self.intent2skill[message.data["name"]] = skill_id
+            # print(self.intent_service.__dict__)
+
+        for peer, client in self.clients.items():
+            if peer in peers and peer != skill_peer:
+                client.send(HiveMessage(HiveMessageType.BUS, message))
 
 
 class LocalHiveProtocol(HiveMindListenerProtocol):
     intent_messages = [
         "recognizer_loop:utterance",
         "intent.service.intent.get",
         "intent.service.skills.get",
@@ -108,33 +106,43 @@
         "register_vocab",
         "register_intent",
         "detach_intent",
         "detach_skill",
         "add_context",
         "remove_context",
         "clear_context",
-        "mycroft.skills.loaded",
-        "active_skill_request",
-        'mycroft.speech.recognition.unknown',
         'padatious:register_intent',
         'padatious:register_entity',
-        'mycroft.skills.initialized'
+        "mycroft.skill.set_cross_context",
+        "mycroft.skill.remove_cross_context"
     ]
-    default_permissions = intent_messages + [
-        "speak",
-        "mycroft.skill.handler.start",
-        "mycroft.skill.handler.complete",
-        "skill.converse.request",
-        "skill.converse.response"
+    converse_permissions = [
+       # "skill.converse.request",
+        "skill.converse.response",
+       # "skill.converse.ping",
+        "skill.converse.pong",
+        "active_skill_request",
+        "intent.service.skills.activated",
+        "intent.service.skills.deactivated",
     ]
+    speak_permissions = ["speak"]
+    stop_permissions = ["mycroft.stop"]
+    default_permissions = intent_messages + \
+                          converse_permissions + \
+                          speak_permissions + \
+                          stop_permissions + \
+                          [
+                              "mycroft.skill.handler.start",
+                              "mycroft.skill.handler.complete",
+                              "mycroft.skills.loaded",
+
+                          ]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.bus = None
-        self.intent2skill = {}
         self.permission_overrides = {}
 
     def handle_new_client(self, client: HiveMindClientConnection):
         LOG.info(f"new client: {client.peer}")
         self.clients[client.peer] = client
         message = Message("hive.client.connect",
                           {"ip": client.ip, "session_id": client.sess.session_id},
@@ -142,101 +150,94 @@
         self.internal_protocol.bus.emit(message)
 
         msg = HiveMessage(HiveMessageType.HELLO,
                           payload={"handshake": False,
                                    "crypto": False,
                                    "peer": client.peer,  # this identifies the connected client in ovos message.context
                                    "node_id": self.peer})
-        LOG.info(f"saying HELLO to: {client.peer}")
+        # LOG.debug(f"saying HELLO to: {client.peer}")
         client.send(msg)
 
         # request client to start handshake (by sending client pubkey)
         payload = {
             "handshake": False,  # tell the client it must do a handshake or connection will be dropped
             "binarize": False,  # report we support the binarization scheme
             "preshared_key": False,  # do we have a pre-shared key (V0 proto)
             "password": False,  # is password available (V1 proto, replaces pre-shared key)
             "crypto_required": False  # do we allow unencrypted payloads
         }
         msg = HiveMessage(HiveMessageType.HANDSHAKE, payload)
-        LOG.info(f"starting {client.peer} HANDSHAKE: {payload}")
+        LOG.debug(f"starting {client.peer} HANDSHAKE: {payload}")
         client.send(msg)
         # if client is in protocol V1 -> self.handle_handshake_message
         # clients can rotate their pubkey or session_key by sending a new handshake
 
     def handle_handshake_message(self, message: HiveMessage,
                                  client: HiveMindClientConnection):
-        LOG.info("handshake received, ignoring")
+        payload = {
+            "handshake": False,  # tell the client it must do a handshake or connection will be dropped
+            "binarize": False,  # report we support the binarization scheme
+            "preshared_key": False,  # do we have a pre-shared key (V0 proto)
+            "password": False,  # is password available (V1 proto, replaces pre-shared key)
+            "crypto_required": False  # do we allow unencrypted payloads
+        }
+        msg = HiveMessage(HiveMessageType.HANDSHAKE, payload)
+        LOG.debug(f"skipping {client.peer} HANDSHAKE: {payload}")
+        client.send(msg)
 
     @property
     def intent_service(self):
         return self.internal_protocol.intent_service
 
     def bind(self, websocket, bus=None):
         websocket.protocol = self
         if bus is None:
             bus = FakeBus()
-        self.bus = bus
-        self.internal_protocol = LocalHiveInternalProtocol(self.bus)
+        self.internal_protocol = LocalHiveInternalProtocol(bus)
         self.internal_protocol.register_bus_handlers()
 
     # messages from skill -> LocalHive
     def handle_inject_mycroft_msg(self, message: Message, client: HiveMindClientConnection):
         """
         message (Message): mycroft bus message object
         """
         # message from a terminal
         if message.msg_type == "recognizer_loop:utterance":
             LOG.info(f"Utterance: {message.data['utterances']} "
                      f"Peer: {client.peer}")
             message.context["source"] = client.peer
-            self.intent_service.handle_utterance(message)
+            self.internal_protocol.bus.emit(message)
 
         # message from a skill
         elif message.context.get("skill_id"):
             message.context["source"] = client.peer
             self.handle_skill_message(message)
 
     def handle_skill_message(self, message):
         """ message sent by skill"""
         if isinstance(message, str):
             message = Message.deserialize(message)
 
-        skill_id = message.context.get("skill_id")
-        intent_skill = self.intent2skill.get(message.msg_type)
+        is_intent_for_skill = self.internal_protocol.intent2skill.get(message.msg_type)
+        skill_id = message.context.get("skill_id") or is_intent_for_skill or ""
         permitted = False
 
         # skill intents
-        if intent_skill:
+        if is_intent_for_skill:
             permitted = True
         # skill_id permission override
-        elif skill_id and skill_id in self.permission_overrides:
+        elif skill_id in self.permission_overrides:
             if message.msg_type in self.permission_overrides[skill_id]:
                 permitted = True
         # default permissions
         elif message.msg_type in self.default_permissions:
             permitted = True
 
-        if permitted:
-            peers = message.context.get('destination') or []
-            if isinstance(peers, str):
-                peers = [peers]
-
-            # check if it should be forwarded to some peer (skill/terminal)
-            for peer in peers:
-                client = self.clients.get(peer)
-                if client:
-                    LOG.debug(f"destination: {message.context['destination']} "
-                              f"skill:{skill_id} "
-                              f"type:{message.msg_type}")
-                    client.send(
-                        HiveMessage(HiveMessageType.BUS, message)
-                    )
-
-            # check if this message should be forwarded to intent service
-            if message.msg_type in self.intent_messages or "IntentService" in peers:
-                self.bus.emit(message)
+        LOG.debug(f"{message.msg_type} allowed for {skill_id}: {permitted}")
+        message.context["skill_id"] = skill_id
+        if permitted:  # forward to intent service
+            self.internal_protocol.bus.emit(message)
         else:
             self.handle_ignored_message(message)
 
     def handle_ignored_message(self, message):
         pass
```

## local_hive/service.py

```diff
@@ -8,17 +8,19 @@
 from ovos_bus_client.session import Session
 from ovos_config import Configuration
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import ProcessStatus, StatusCallbackMap
 from tornado import web, ioloop
 from tornado.platform.asyncio import AnyThreadEventLoopPolicy
 
-from local_hive.fakebus import FakeBus
+from ovos_utils.messagebus import FakeBus
 from local_hive.protocol import LocalHiveProtocol
 
+LOG.set_level("INFO")
+
 
 def on_ready():
     LOG.info('LocalHive service ready!')
 
 
 def on_alive():
     LOG.info('LocalHive service alive')
```

## local_hive/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 0
 VERSION_BUILD = 3
-VERSION_ALPHA = 3
+VERSION_ALPHA = 4
 # END_VERSION_BLOCK
```

## Comparing `hivemind_local-0.0.3a3.dist-info/RECORD` & `hivemind_local-0.0.3a4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 local_hive/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 local_hive/__main__.py,sha256=i0KdrWgebcXPn9tY_StApZYf4bhc6Ir0AuBwQvtstcU,205
 local_hive/exceptions.py,sha256=7EnqukCRXILLooe2Zx_vBWG5FI7sGtAqbd3dq7CbEtM,171
-local_hive/fakebus.py,sha256=467-b0EDckFSCRp83paJe-JvSQjS2Nwhm24wJFiiHE0,630
-local_hive/loader.py,sha256=tj-SqTdZv_WwmlAhvrttG1g-7cKzo1NUqUHvEHOrzcA,2536
-local_hive/protocol.py,sha256=_MdV5ahFh8xbKqwr8Z-ifq3otCtQRRli3sOKejGHZIg,9754
-local_hive/service.py,sha256=ngo5p6D3r6ZOi2L5pvg_I0lrV6dlfdg4nXRtJMIo88k,3988
-local_hive/version.py,sha256=FlJ6O33MI1M2L8ayalX-SlHp6MmYdWpYIp7HUGGpLUA,177
-hivemind_local-0.0.3a3.dist-info/METADATA,sha256=_n-hGTLwStXuKY0v7LVB7-WxyuS3gk6hGgPHsZwsr-A,446
-hivemind_local-0.0.3a3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-hivemind_local-0.0.3a3.dist-info/top_level.txt,sha256=EWzMwwCOi1MoVXmTmj0NCSt3wlBOHms1ZLo8Vk97nQw,11
-hivemind_local-0.0.3a3.dist-info/RECORD,,
+local_hive/loader.py,sha256=1oXbCIblbh6h7Bq6oMZsDhPypaR_rj8PzDuxX-9Z6pI,2466
+local_hive/protocol.py,sha256=GLRVkEaIztR7La_q09JZB5_H8mOQnd9lsFLh3-c-S78,9942
+local_hive/service.py,sha256=S6Gv1ByQwfs4pBdXaTwmQZmvB7LHBFUZOkxycrPLkP4,4014
+local_hive/version.py,sha256=CQRXBPmiJFy-y610Y0ivVJwKwYh-YBlxcEgRI4IUDxU,177
+hivemind_local-0.0.3a4.dist-info/METADATA,sha256=wRGEskeqrdOgKlM7EPZYwvXa3j7m24GVqfMA3bY89IM,446
+hivemind_local-0.0.3a4.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+hivemind_local-0.0.3a4.dist-info/top_level.txt,sha256=EWzMwwCOi1MoVXmTmj0NCSt3wlBOHms1ZLo8Vk97nQw,11
+hivemind_local-0.0.3a4.dist-info/RECORD,,
```

