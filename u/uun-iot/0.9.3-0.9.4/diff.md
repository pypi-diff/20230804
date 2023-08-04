# Comparing `tmp/uun-iot-0.9.3.tar.gz` & `tmp/uun-iot-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uun-iot-0.9.3.tar", last modified: Tue Aug  1 14:30:03 2023, max compression
+gzip compressed data, was "uun-iot-0.9.4.tar", last modified: Fri Aug  4 16:01:17 2023, max compression
```

## Comparing `uun-iot-0.9.3.tar` & `uun-iot-0.9.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:30:03.936435 uun-iot-0.9.3/
--rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:43:51.000000 uun-iot-0.9.3/LICENSE.md
--rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 14:30:03.936435 uun-iot-0.9.3/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)     1965 2022-10-16 10:02:57.000000 uun-iot-0.9.3/README.md
--rw-------   0 hello     (1000) hello     (1000)       38 2023-08-01 14:30:03.936435 uun-iot-0.9.3/setup.cfg
--rw-------   0 hello     (1000) hello     (1000)      892 2023-01-22 14:43:43.000000 uun-iot-0.9.3/setup.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:30:03.936435 uun-iot-0.9.3/uun_iot/
--rw-------   0 hello     (1000) hello     (1000)    25084 2022-10-30 12:40:32.000000 uun-iot-0.9.3/uun_iot/Gateway.py
--rw-------   0 hello     (1000) hello     (1000)    20292 2023-08-01 11:59:34.000000 uun-iot-0.9.3/uun_iot/UuAppClient.py
--rw-------   0 hello     (1000) hello     (1000)      224 2023-08-01 14:27:58.000000 uun-iot-0.9.3/uun_iot/__init__.py
--rw-------   0 hello     (1000) hello     (1000)     9179 2023-08-01 07:17:17.000000 uun-iot-0.9.3/uun_iot/decorators.py
--rw-------   0 hello     (1000) hello     (1000)     1916 2022-10-16 10:02:57.000000 uun-iot-0.9.3/uun_iot/diagnostic.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:30:03.936435 uun-iot-0.9.3/uun_iot/modules/
--rw-------   0 hello     (1000) hello     (1000)    14058 2022-10-23 08:04:43.000000 uun-iot-0.9.3/uun_iot/modules/BaseHealthCheck.py
--rw-------   0 hello     (1000) hello     (1000)     2018 2022-10-16 10:02:57.000000 uun-iot-0.9.3/uun_iot/modules/Heartbeat.py
--rw-------   0 hello     (1000) hello     (1000)    10181 2023-08-01 14:03:32.000000 uun-iot-0.9.3/uun_iot/modules/Module.py
--rw-------   0 hello     (1000) hello     (1000)      362 2022-10-16 10:02:57.000000 uun-iot-0.9.3/uun_iot/modules/__init__.py
--rw-------   0 hello     (1000) hello     (1000)      367 2022-10-16 10:02:57.000000 uun-iot-0.9.3/uun_iot/typing.py
--rw-------   0 hello     (1000) hello     (1000)    12903 2023-08-01 09:53:25.000000 uun-iot-0.9.3/uun_iot/utils.py
-drwx------   0 hello     (1000) hello     (1000)        0 2023-08-01 14:30:03.936435 uun-iot-0.9.3/uun_iot.egg-info/
--rw-------   0 hello     (1000) hello     (1000)      468 2023-08-01 14:30:03.000000 uun-iot-0.9.3/uun_iot.egg-info/PKG-INFO
--rw-------   0 hello     (1000) hello     (1000)      442 2023-08-01 14:30:03.000000 uun-iot-0.9.3/uun_iot.egg-info/SOURCES.txt
--rw-------   0 hello     (1000) hello     (1000)        1 2023-08-01 14:30:03.000000 uun-iot-0.9.3/uun_iot.egg-info/dependency_links.txt
--rw-------   0 hello     (1000) hello     (1000)       56 2023-08-01 14:30:03.000000 uun-iot-0.9.3/uun_iot.egg-info/requires.txt
--rw-------   0 hello     (1000) hello     (1000)        8 2023-08-01 14:30:03.000000 uun-iot-0.9.3/uun_iot.egg-info/top_level.txt
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-04 16:01:17.629051 uun-iot-0.9.4/
+-rw-------   0 hello     (1000) hello     (1000)     1075 2023-01-22 14:43:51.000000 uun-iot-0.9.4/LICENSE.md
+-rw-------   0 hello     (1000) hello     (1000)      468 2023-08-04 16:01:17.629051 uun-iot-0.9.4/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)     1965 2022-10-16 10:02:57.000000 uun-iot-0.9.4/README.md
+-rw-------   0 hello     (1000) hello     (1000)       38 2023-08-04 16:01:17.629051 uun-iot-0.9.4/setup.cfg
+-rw-------   0 hello     (1000) hello     (1000)      892 2023-08-01 14:49:12.000000 uun-iot-0.9.4/setup.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-04 16:01:17.629051 uun-iot-0.9.4/uun_iot/
+-rw-------   0 hello     (1000) hello     (1000)    24729 2023-08-04 15:59:39.000000 uun-iot-0.9.4/uun_iot/Gateway.py
+-rw-------   0 hello     (1000) hello     (1000)    20292 2023-08-01 11:59:34.000000 uun-iot-0.9.4/uun_iot/UuAppClient.py
+-rw-------   0 hello     (1000) hello     (1000)      224 2023-08-04 16:00:13.000000 uun-iot-0.9.4/uun_iot/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)     9179 2023-08-01 07:17:17.000000 uun-iot-0.9.4/uun_iot/decorators.py
+-rw-------   0 hello     (1000) hello     (1000)     1916 2022-10-16 10:02:57.000000 uun-iot-0.9.4/uun_iot/diagnostic.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-04 16:01:17.629051 uun-iot-0.9.4/uun_iot/modules/
+-rw-------   0 hello     (1000) hello     (1000)    14058 2022-10-23 08:04:43.000000 uun-iot-0.9.4/uun_iot/modules/BaseHealthCheck.py
+-rw-------   0 hello     (1000) hello     (1000)     1867 2023-08-04 15:55:38.000000 uun-iot-0.9.4/uun_iot/modules/Heartbeat.py
+-rw-------   0 hello     (1000) hello     (1000)    10181 2023-08-01 14:03:32.000000 uun-iot-0.9.4/uun_iot/modules/Module.py
+-rw-------   0 hello     (1000) hello     (1000)      379 2023-08-04 15:54:26.000000 uun-iot-0.9.4/uun_iot/modules/__init__.py
+-rw-------   0 hello     (1000) hello     (1000)      367 2022-10-16 10:02:57.000000 uun-iot-0.9.4/uun_iot/typing.py
+-rw-------   0 hello     (1000) hello     (1000)    12903 2023-08-01 09:53:25.000000 uun-iot-0.9.4/uun_iot/utils.py
+drwx------   0 hello     (1000) hello     (1000)        0 2023-08-04 16:01:17.629051 uun-iot-0.9.4/uun_iot.egg-info/
+-rw-------   0 hello     (1000) hello     (1000)      468 2023-08-04 16:01:17.000000 uun-iot-0.9.4/uun_iot.egg-info/PKG-INFO
+-rw-------   0 hello     (1000) hello     (1000)      442 2023-08-04 16:01:17.000000 uun-iot-0.9.4/uun_iot.egg-info/SOURCES.txt
+-rw-------   0 hello     (1000) hello     (1000)        1 2023-08-04 16:01:17.000000 uun-iot-0.9.4/uun_iot.egg-info/dependency_links.txt
+-rw-------   0 hello     (1000) hello     (1000)       56 2023-08-04 16:01:17.000000 uun-iot-0.9.4/uun_iot.egg-info/requires.txt
+-rw-------   0 hello     (1000) hello     (1000)        8 2023-08-04 16:01:17.000000 uun-iot-0.9.4/uun_iot.egg-info/top_level.txt
```

### Comparing `uun-iot-0.9.3/LICENSE.md` & `uun-iot-0.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.3/README.md` & `uun-iot-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.3/setup.py` & `uun-iot-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.3/uun_iot/Gateway.py` & `uun-iot-0.9.4/uun_iot/Gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -468,33 +468,26 @@
 
         if "gateway" not in self.config:
             self.config["gateway"] = {}
 
     def _uucmd(self):
         # create uucmd function, separate from other cmd due to nature of Config
         uucmd = self.config["uuApp"]['uuCmdList']['gatewayGetConfiguration']
+        r, err = self.g.uuapp_client.get(uucmd)
+        if r is None:
+            return False
         try:
-            r = self.g.uuapp_client.get_request(uucmd)
-            r.raise_for_status()
             new_config = r.json()
             # this is not an actual configuration key, only a remnant of server communication
-            del new_config["uuAppErrorMap"]
-        except requests.exceptions.HTTPError as e:
-            loggerc.warning("Could not fetch new data (error code %s)", r.status_code)
-            loggerc.debug("Received response: %s", r.text)
-            return False
-        except requests.exceptions.RequestException as e:
-            loggerc.info("Error in server communication: %s", e)
-            return False
+            if "uuAppErrorMap" in new_config:
+                del new_config["uuAppErrorMap"]
         except json.decoder.JSONDecodeError:
             loggerc.error("Received invalid configuration JSON from server")
             loggerc.debug("Invalid response: %s", r.text)
             return False
-        except KeyError:
-            pass
 
         if new_config == {}:
             loggerc.error("Received invalid JSON configuration from server")
             loggerc.debug(r.text)
             return False
 
         return new_config
```

### Comparing `uun-iot-0.9.3/uun_iot/UuAppClient.py` & `uun-iot-0.9.4/uun_iot/UuAppClient.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.3/uun_iot/decorators.py` & `uun-iot-0.9.4/uun_iot/decorators.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.3/uun_iot/diagnostic.py` & `uun-iot-0.9.4/uun_iot/diagnostic.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.3/uun_iot/modules/BaseHealthCheck.py` & `uun-iot-0.9.4/uun_iot/modules/BaseHealthCheck.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.3/uun_iot/modules/Heartbeat.py` & `uun-iot-0.9.4/uun_iot/modules/Heartbeat.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,21 +42,16 @@
         boot_timestamp = datetime.fromtimestamp(psutil.boot_time())
         dto_in = {
             "bootTimestamp": get_iso_timestamp(boot_timestamp),
             "cpuUsage": psutil.cpu_percent(),
             "ramUsage": psutil.virtual_memory().percent
         }
 
-        response = None
-        try:
-            response = self._uucmd(dto_in)
-        except requests.exceptions.ConnectionError as e:
-            logger.warning("Error connecting to server: %s", e)
-
-        if response:
+        response = self._uucmd(dto_in)
+        if response is not None:
             if response.status_code >= 200 and response.status_code < 300:
                 if not self.online:
                     logger.info("online")
                     self.online = True
         else:
             if self.online:
                 logger.warning("offline")
```

### Comparing `uun-iot-0.9.3/uun_iot/modules/Module.py` & `uun-iot-0.9.4/uun_iot/modules/Module.py`

 * *Files identical despite different names*

### Comparing `uun-iot-0.9.3/uun_iot/utils.py` & `uun-iot-0.9.4/uun_iot/utils.py`

 * *Files identical despite different names*

