# Comparing `tmp/logger_extras-0.3.2.tar.gz` & `tmp/logger_extras-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger_extras-0.3.2.tar", last modified: Mon Jul 31 20:57:00 2023, max compression
+gzip compressed data, was "logger_extras-0.3.3.tar", last modified: Fri Aug  4 21:14:07 2023, max compression
```

## Comparing `logger_extras-0.3.2.tar` & `logger_extras-0.3.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.954458 logger_extras-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-31 20:56:38.000000 logger_extras-0.3.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.950458 logger_extras-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.950458 logger_extras-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-31 20:56:38.000000 logger_extras-0.3.2/.github/workflows/test_build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-31 20:56:38.000000 logger_extras-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 20:56:38.000000 logger_extras-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-31 20:56:38.000000 logger_extras-0.3.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-31 20:57:00.954458 logger_extras-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-31 20:56:38.000000 logger_extras-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.954458 logger_extras-0.3.2/logger_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-31 20:56:38.000000 logger_extras-0.3.2/logger_extras/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.954458 logger_extras-0.3.2/logger_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 20:57:00.000000 logger_extras-0.3.2/logger_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-31 20:56:38.000000 logger_extras-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:57:00.954458 logger_extras-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:57:00.954458 logger_extras-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-31 20:56:38.000000 logger_extras-0.3.2/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-04 21:13:52.000000 logger_extras-0.3.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-04 21:13:52.000000 logger_extras-0.3.3/.github/workflows/test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-08-04 21:13:52.000000 logger_extras-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-04 21:13:52.000000 logger_extras-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-04 21:13:52.000000 logger_extras-0.3.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-04 21:14:07.704247 logger_extras-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-08-04 21:13:52.000000 logger_extras-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/logger_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-04 21:13:52.000000 logger_extras-0.3.3/logger_extras/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/logger_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 21:14:07.000000 logger_extras-0.3.3/logger_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-08-04 21:13:52.000000 logger_extras-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:14:07.704247 logger_extras-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:14:07.704247 logger_extras-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-08-04 21:13:52.000000 logger_extras-0.3.3/tests/test_tools.py
```

### Comparing `logger_extras-0.3.2/.github/workflows/test_build.yml` & `logger_extras-0.3.3/.github/workflows/test_build.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 name: Lint & build
 
-on: [push]
+on:
+  - push
+  - workflow_dispatch
 
 jobs:
   test:
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest]
```

### Comparing `logger_extras-0.3.2/.gitignore` & `logger_extras-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.2/LICENSE` & `logger_extras-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.2/PKG-INFO` & `logger_extras-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger_extras
-Version: 0.3.2
+Version: 0.3.3
 Summary: A collection of useful logging tools
 Author: Will Barber
 License: MIT License
         
         Copyright (c) 2023 Will Barber
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `logger_extras-0.3.2/README.md` & `logger_extras-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.2/logger_extras/filters.py` & `logger_extras-0.3.3/logger_extras/filters.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.2/logger_extras/formatters.py` & `logger_extras-0.3.3/logger_extras/formatters.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.2/logger_extras/mqtt.py` & `logger_extras-0.3.3/logger_extras/mqtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,28 +43,38 @@
             self.mqtt.tls_set()
             if use_tls == 'insecure':
                 self.mqtt.tls_insecure_set(True)
 
         if username:
             self.mqtt.username_pw_set(username, password)
 
+        self.mqtt.on_connect = self._on_connect
+        if self._connected_topic:
+            # This must be set before connecting
+            self.mqtt.will_set(
+                self._connected_topic, '{"state": "disconnected"}', qos=1, retain=True)
+
         try:
             self.mqtt.connect(
                 host=host,
                 port=port,
                 keepalive=keepalive,
                 bind_address=bind_address)
         except (TimeoutError, ValueError, ConnectionRefusedError):
             print(f"Failed to connect to MQTT broker at {host}:{port}")
             return
         self.mqtt.loop_start()
-        if connected_topic:
-            self.mqtt.publish(connected_topic, '{"state": "connected"}', qos=1, retain=True)
-            self.mqtt.will_set(
-                connected_topic, '{"state": "disconnected"}', qos=1, retain=True)
+
+    def _on_connect(
+        self, client: mqtt.Client, userdata: Any, flags: dict[str, int], rc: int,
+        properties: mqtt.Properties | None = None,
+    ) -> None:
+        if self._connected_topic:
+            client.publish(
+                self._connected_topic, '{"state": "connected"}', qos=1, retain=True)
 
     def __del__(self) -> None:
         if self._connected_topic:
             res = self.mqtt.publish(
                 self._connected_topic, '{"state": "disconnected"}', qos=1, retain=True)
             res.wait_for_publish(1)
         self.mqtt.disconnect()
```

### Comparing `logger_extras-0.3.2/logger_extras/utils.py` & `logger_extras-0.3.3/logger_extras/utils.py`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.2/logger_extras.egg-info/PKG-INFO` & `logger_extras-0.3.3/logger_extras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-extras
-Version: 0.3.2
+Version: 0.3.3
 Summary: A collection of useful logging tools
 Author: Will Barber
 License: MIT License
         
         Copyright (c) 2023 Will Barber
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `logger_extras-0.3.2/pyproject.toml` & `logger_extras-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `logger_extras-0.3.2/tests/test_tools.py` & `logger_extras-0.3.3/tests/test_tools.py`

 * *Files identical despite different names*

