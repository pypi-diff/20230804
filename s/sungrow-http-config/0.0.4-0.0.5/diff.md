# Comparing `tmp/sungrow_http_config-0.0.4.tar.gz` & `tmp/sungrow_http_config-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sungrow_http_config-0.0.4.tar", last modified: Thu Aug  3 12:37:27 2023, max compression
+gzip compressed data, was "sungrow_http_config-0.0.5.tar", last modified: Fri Aug  4 09:31:26 2023, max compression
```

## Comparing `sungrow_http_config-0.0.4.tar` & `sungrow_http_config-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 12:37:27.032416 sungrow_http_config-0.0.4/
--rw-r--r--   0 ross       (501) staff       (20)     1072 2023-08-01 09:53:21.000000 sungrow_http_config-0.0.4/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)     1760 2023-08-03 12:37:27.032133 sungrow_http_config-0.0.4/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     1202 2023-08-03 12:35:38.000000 sungrow_http_config-0.0.4/README.md
--rw-r--r--   0 ross       (501) staff       (20)      711 2023-08-03 12:36:43.000000 sungrow_http_config-0.0.4/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2023-08-03 12:37:27.032536 sungrow_http_config-0.0.4/setup.cfg
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 12:37:27.027213 sungrow_http_config-0.0.4/src/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 12:37:27.029603 sungrow_http_config-0.0.4/src/sungrow_http_config/
--rw-r--r--   0 ross       (501) staff       (20)     9980 2023-08-03 12:32:17.000000 sungrow_http_config-0.0.4/src/sungrow_http_config/SungrowHttpConfig.py
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-01 09:55:24.000000 sungrow_http_config-0.0.4/src/sungrow_http_config/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-03 12:37:27.031673 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     1760 2023-08-03 12:37:27.000000 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      347 2023-08-03 12:37:27.000000 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-03 12:37:27.000000 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)       46 2023-08-03 12:37:27.000000 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       20 2023-08-03 12:37:27.000000 sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/top_level.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-04 09:31:26.690481 sungrow_http_config-0.0.5/
+-rw-r--r--   0 ross       (501) staff       (20)     1072 2023-08-01 09:53:21.000000 sungrow_http_config-0.0.5/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)     1760 2023-08-04 09:31:26.690020 sungrow_http_config-0.0.5/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     1202 2023-08-03 12:35:38.000000 sungrow_http_config-0.0.5/README.md
+-rw-r--r--   0 ross       (501) staff       (20)      711 2023-08-04 09:31:03.000000 sungrow_http_config-0.0.5/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2023-08-04 09:31:26.690618 sungrow_http_config-0.0.5/setup.cfg
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-04 09:31:26.683187 sungrow_http_config-0.0.5/src/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-04 09:31:26.685999 sungrow_http_config-0.0.5/src/sungrow_http_config/
+-rw-r--r--   0 ross       (501) staff       (20)    10146 2023-08-04 09:30:47.000000 sungrow_http_config-0.0.5/src/sungrow_http_config/SungrowHttpConfig.py
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-01 09:55:24.000000 sungrow_http_config-0.0.5/src/sungrow_http_config/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2023-08-04 09:31:26.689244 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     1760 2023-08-04 09:31:26.000000 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      347 2023-08-04 09:31:26.000000 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2023-08-04 09:31:26.000000 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)       46 2023-08-04 09:31:26.000000 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       20 2023-08-04 09:31:26.000000 sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/top_level.txt
```

### Comparing `sungrow_http_config-0.0.4/LICENSE` & `sungrow_http_config-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sungrow_http_config-0.0.4/PKG-INFO` & `sungrow_http_config-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sungrow_http_config
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to manipulate settings on Sungrow Inverters
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/sungrow_exportlimit
 Project-URL: Bug Tracker, https://github.com/ross-w/sungrow_exportlimit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sungrow_http_config-0.0.4/README.md` & `sungrow_http_config-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sungrow_http_config-0.0.4/pyproject.toml` & `sungrow_http_config-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sungrow_http_config"
-version = "0.0.4"
+version = "0.0.5"
 dependencies = [
   "requests_retry_on_exceptions",
   "urllib3",
   "pymodbus"
 ]
 authors = [
   { name="Ross Williamson", email="ross@inertia.net.nz" },
```

### Comparing `sungrow_http_config-0.0.4/src/sungrow_http_config/SungrowHttpConfig.py` & `sungrow_http_config-0.0.5/src/sungrow_http_config/SungrowHttpConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,17 +132,21 @@
             "lang": self.lang,
             "msgLength": (len(msgValue) // 2),
             "msgType": msgType,
             "msgValue": msgValue,
             "token": self.token
         }
         resp = self._callAPI("/device/passthroughway", req)
-        if not resp.get("result_code")==1:
+        if resp.get("result_code")==1:
+            return resp.get("result_data")
+        elif resp.get("result_code")==106: # Token expired
+            self.token=""
+            return self._sendHexMessageToDevice(msgValue, msgType)
+        else:
             raise Exception("Got unsuccessful message back from device: {resp}".format(resp=resp))
-        return resp.get("result_data")
 
     def _generateExportLimitCommand(self, dekawattLimit):
         """ Generates the appropriate modbus command to send for the given limit
         :param dekawattLimit: Limit to set, in dekawatts (kW * 100)
         :returns: String containing modbus command string
         """
         framer = ModbusRtuFramer(None)
```

### Comparing `sungrow_http_config-0.0.4/src/sungrow_http_config.egg-info/PKG-INFO` & `sungrow_http_config-0.0.5/src/sungrow_http_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sungrow-http-config
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to manipulate settings on Sungrow Inverters
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/sungrow_exportlimit
 Project-URL: Bug Tracker, https://github.com/ross-w/sungrow_exportlimit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

