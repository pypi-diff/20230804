# Comparing `tmp/openct-0.1.1.tar.gz` & `tmp/openct-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openct-0.1.1.tar", max compression
+gzip compressed data, was "openct-0.1.2.tar", max compression
```

## Comparing `openct-0.1.1.tar` & `openct-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-07-18 18:59:08.983315 openct-0.1.1/LICENSE
--rw-r--r--   0        0        0      661 2023-07-18 18:59:08.983315 openct-0.1.1/README.md
--rw-r--r--   0        0        0       89 2023-07-18 18:59:08.983315 openct-0.1.1/openct/__init__.py
--rw-r--r--   0        0        0      859 2023-07-18 18:59:08.983315 openct-0.1.1/openct/__main__.py
--rw-r--r--   0        0        0       83 2023-07-18 18:59:08.983315 openct-0.1.1/openct/connections/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-18 18:59:08.983315 openct-0.1.1/openct/connections/connections.py
--rw-r--r--   0        0        0       73 2023-07-18 18:59:08.983315 openct-0.1.1/openct/datastore/__init__.py
--rw-r--r--   0        0        0     1359 2023-07-18 18:59:08.983315 openct-0.1.1/openct/datastore/datastore.py
--rw-r--r--   0        0        0       65 2023-07-18 18:59:08.983315 openct-0.1.1/openct/devices/__init__.py
--rw-r--r--   0        0        0      817 2023-07-18 18:59:08.983315 openct-0.1.1/openct/devices/devices.py
--rw-r--r--   0        0        0      201 2023-07-18 18:59:08.983315 openct-0.1.1/openct/setup/__init__.py
--rw-r--r--   0        0        0      556 2023-07-18 18:59:08.983315 openct-0.1.1/openct/setup/__main__.py
--rw-r--r--   0        0        0     1440 2023-07-18 18:59:08.983315 openct-0.1.1/openct/setup/config.py
--rw-r--r--   0        0        0      626 2023-07-18 18:59:08.983315 openct-0.1.1/openct/setup/config_schema.py
--rw-r--r--   0        0        0     1354 2023-07-18 18:59:08.983315 openct-0.1.1/openct/setup/setup.py
--rw-r--r--   0        0        0      592 2023-07-18 18:59:08.983315 openct-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 openct-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-04 19:50:41.006445 openct-0.1.2/LICENSE
+-rw-r--r--   0        0        0      996 2023-08-04 19:50:41.006445 openct-0.1.2/README.md
+-rw-r--r--   0        0        0       89 2023-08-04 19:50:41.006445 openct-0.1.2/openct/__init__.py
+-rw-r--r--   0        0        0      895 2023-08-04 19:50:41.006445 openct-0.1.2/openct/__main__.py
+-rw-r--r--   0        0        0       83 2023-08-04 19:50:41.006445 openct-0.1.2/openct/connections/__init__.py
+-rw-r--r--   0        0        0     1776 2023-08-04 19:50:41.006445 openct-0.1.2/openct/connections/connections.py
+-rw-r--r--   0        0        0       73 2023-08-04 19:50:41.006445 openct-0.1.2/openct/datastore/__init__.py
+-rw-r--r--   0        0        0     1359 2023-08-04 19:50:41.006445 openct-0.1.2/openct/datastore/datastore.py
+-rw-r--r--   0        0        0       65 2023-08-04 19:50:41.006445 openct-0.1.2/openct/devices/__init__.py
+-rw-r--r--   0        0        0      918 2023-08-04 19:50:41.006445 openct-0.1.2/openct/devices/devices.py
+-rw-r--r--   0        0        0      201 2023-08-04 19:50:41.006445 openct-0.1.2/openct/setup/__init__.py
+-rw-r--r--   0        0        0      556 2023-08-04 19:50:41.006445 openct-0.1.2/openct/setup/__main__.py
+-rw-r--r--   0        0        0     1440 2023-08-04 19:50:41.006445 openct-0.1.2/openct/setup/config.py
+-rw-r--r--   0        0        0      626 2023-08-04 19:50:41.006445 openct-0.1.2/openct/setup/config_schema.py
+-rw-r--r--   0        0        0     1354 2023-08-04 19:50:41.006445 openct-0.1.2/openct/setup/setup.py
+-rw-r--r--   0        0        0      592 2023-08-04 19:50:41.010445 openct-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 openct-0.1.2/PKG-INFO
```

### Comparing `openct-0.1.1/LICENSE` & `openct-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openct-0.1.1/openct/__main__.py` & `openct-0.1.2/openct/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,13 +21,14 @@
         pbar.update(100 / len(devices))
 
         device = RouterOSDevice(
             host,
             config.identity.username,
             config.settings.connection_timeout,
             config.identity.key_file,
+            config.dirs.backup_dir,
         )
 
         if device.is_available():
             device.fetch_backup()
         else:
             logging.error("Could not connect to device")
```

### Comparing `openct-0.1.1/openct/connections/connections.py` & `openct-0.1.2/openct/connections/connections.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,20 +16,26 @@
         ...
 
 
 class SshConnection(DeviceConnection):
     """DeviceConnection using Fabric"""
 
     def __init__(
-        self, ip_address: str, username: str, connection_timeout: int, key_file: str
+        self,
+        ip_address: str,
+        username: str,
+        connection_timeout: int,
+        key_file: str,
+        backup_dir: str,
     ) -> None:
         self.ip_address = ip_address
         self.username = username
         self.connection_timeout = connection_timeout
         self.key_file = key_file
+        self.backup_dir = backup_dir
 
     def test_connection(self) -> bool:
         with FabricConnection(
             host=self.ip_address,
             user=self.username,
             connect_timeout=self.connection_timeout,
             connect_kwargs={"key_filename": self.key_file},
@@ -44,9 +50,11 @@
         with FabricConnection(
             host=self.ip_address,
             user=self.username,
             connect_timeout=self.connection_timeout,
             connect_kwargs={"key_filename": self.key_file},
         ) as connection:
             connection.run("/export file=backup", hide=True, warn=False)
-            connection.get("backup.rsc", f"backups/backup_{self.ip_address}.rsc")
+            connection.get(
+                "backup.rsc", f"{self.backup_dir}/backup_{self.ip_address}.rsc"
+            )
             connection.run("file/remove backup.rsc", hide=True, warn=False)
```

### Comparing `openct-0.1.1/openct/datastore/datastore.py` & `openct-0.1.2/openct/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.1/openct/setup/__main__.py` & `openct-0.1.2/openct/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.1/openct/setup/config.py` & `openct-0.1.2/openct/setup/config.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.1/openct/setup/config_schema.py` & `openct-0.1.2/openct/setup/config_schema.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.1/openct/setup/setup.py` & `openct-0.1.2/openct/setup/setup.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.1/pyproject.toml` & `openct-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openct"
-version = "0.1.1"
+version = "0.1.2"
 description = "Configuration backup and analysis tools for devices running pfSense and RouterOS"
 authors = ["Weehooey <info@weehooey.com>"]
 license = "GNU GPL v3.0"
 readme = "README.md"
 repository = "https://github.com/weehooey/openct"
 
 [tool.poetry.dependencies]
```

