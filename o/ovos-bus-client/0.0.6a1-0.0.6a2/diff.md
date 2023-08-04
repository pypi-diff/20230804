# Comparing `tmp/ovos-bus-client-0.0.6a1.tar.gz` & `tmp/ovos-bus-client-0.0.6a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-bus-client-0.0.6a1.tar", last modified: Tue Aug  1 15:04:15 2023, max compression
+gzip compressed data, was "ovos-bus-client-0.0.6a2.tar", last modified: Fri Aug  4 17:40:17 2023, max compression
```

## Comparing `ovos-bus-client-0.0.6a1.tar` & `ovos-bus-client-0.0.6a2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:04:15.961305 ovos-bus-client-0.0.6a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-01 15:04:15.961305 ovos-bus-client-0.0.6a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:04:15.961305 ovos-bus-client-0.0.6a1/ovos_bus_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:04:15.961305 ovos-bus-client-0.0.6a1/ovos_bus_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16208 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/client/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/client/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/send_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:04:15.961305 ovos-bus-client-0.0.6a1/ovos_bus_client/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24926 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:04:15.961305 ovos-bus-client-0.0.6a1/ovos_bus_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/ovos_bus_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 15:04:15.961305 ovos-bus-client-0.0.6a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-01 15:04:15.000000 ovos-bus-client-0.0.6a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/ovos_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/ovos_bus_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16208 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/client/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/client/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/send_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/ovos_bus_client/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:40:17.615738 ovos-bus-client-0.0.6a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-04 17:40:17.000000 ovos-bus-client-0.0.6a2/setup.py
```

### Comparing `ovos-bus-client-0.0.6a1/LICENSE.md` & `ovos-bus-client-0.0.6a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/PKG-INFO` & `ovos-bus-client-0.0.6a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.6a1
+Version: 0.0.6a2
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/__init__.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/client/__init__.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/client/client.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/client/client.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/client/collector.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/client/collector.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/client/waiter.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/client/waiter.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/conf.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/conf.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/message.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/message.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/scripts.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/scripts.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/send_func.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/send_func.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/session.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/session.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/util/__init__.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/util/scheduler.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/util/scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,18 +92,21 @@
                     self.schedule_event_handler)
         self.bus.on('mycroft.scheduler.remove_event',
                     self.remove_event_handler)
         self.bus.on('mycroft.scheduler.update_event',
                     self.update_event_handler)
         self.bus.on('mycroft.scheduler.get_event',
                     self.get_event_handler)
-        if autostart:
-            self.start()
 
         self._stopping = Event()
+        if autostart:
+            self.start()
+        else:
+            # Not running
+            self._stopping.set()
 
     @property
     def is_running(self) -> bool:
         """
         Return True while scheduler is running
         """
         return not self._stopping.is_set()
@@ -134,17 +137,22 @@
                     self.events[key] = [tuple(evt) for evt in event_list
                                         if evt[0] > current_time or evt[1]]
 
     def run(self):
         """
         Check events periodically until stopped
         """
+        LOG.info("EventScheduler Started")
+        self._stopping.clear()
         while not self._stopping.wait(0.5):
-            self.check_state()
-        LOG.info(f"Stopped")
+            try:
+                self.check_state()
+            except Exception as e:
+                LOG.exception(e)
+        LOG.info("EventScheduler Stopped")
 
     def check_state(self):
         """
         Check if any event should be triggered.
         """
         with self.event_lock:
             # Check all events
@@ -169,14 +177,15 @@
                 self.events[event] = remaining
 
         # Remove events that are now completed
         self.clear_empty()
 
         # Finally, emit the queued up events that triggered
         for msg in pending_messages:
+            LOG.debug(f"Call scheduled event: {msg.msg_type}")
             self.bus.emit(msg)
 
     def schedule_event(self, event: str, sched_time: float,
                        repeat: Optional[float] = None,
                        data: Optional[dict] = None,
                        context: Optional[dict] = None):
         """
@@ -197,17 +206,21 @@
             event_list = self.events.get(event, [])
 
             # Don't schedule if the event is repeating and already scheduled
             if repeat and event in self.events:
                 LOG.debug(f'Repeating event {event} is already scheduled, '
                           f'discarding')
             else:
+                LOG.debug(f"Scheduled event: {event} for time {sched_time}")
                 # add received event and time
                 event_list.append((sched_time, repeat, data, context))
                 self.events[event] = event_list
+                if sched_time < time.time():
+                    LOG.warning(f"Added event is scheduled in the past and "
+                                f"will be called immediately: {event}")
 
     def schedule_event_handler(self, message: Message):
         """
         Messagebus interface to the schedule_event method.
         Required data in the message envelope is
             event: event to emit
             time:  time to emit the event
```

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client/util/utils.py` & `ovos-bus-client-0.0.6a2/ovos_bus_client/util/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client.egg-info/PKG-INFO` & `ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.6a1
+Version: 0.0.6a2
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.6a1/ovos_bus_client.egg-info/SOURCES.txt` & `ovos-bus-client-0.0.6a2/ovos_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.6a1/setup.py` & `ovos-bus-client-0.0.6a2/setup.py`

 * *Files identical despite different names*

