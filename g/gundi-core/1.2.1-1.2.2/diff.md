# Comparing `tmp/gundi_core-1.2.1.tar.gz` & `tmp/gundi_core-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_core-1.2.1.tar", max compression
+gzip compressed data, was "gundi_core-1.2.2.tar", max compression
```

## Comparing `gundi_core-1.2.1.tar` & `gundi_core-1.2.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       40 2023-06-14 17:07:47.722189 gundi_core-1.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-14 20:35:09.913772 gundi_core-1.2.1/gundi_core/__init__.py
--rw-r--r--   0        0        0       47 2023-07-31 13:14:26.547739 gundi_core-1.2.1/gundi_core/events/__init__.py
--rw-r--r--   0        0        0     1019 2023-07-31 13:14:26.547739 gundi_core-1.2.1/gundi_core/events/core.py
--rw-r--r--   0        0        0      308 2023-07-31 13:14:26.547739 gundi_core-1.2.1/gundi_core/events/dispatchers.py
--rw-r--r--   0        0        0      114 2023-06-14 18:33:55.875739 gundi_core-1.2.1/gundi_core/schemas/__init__.py
--rw-r--r--   0        0        0    13847 2023-06-14 19:41:05.310697 gundi_core-1.2.1/gundi_core/schemas/v1.py
--rw-r--r--   0        0        0    15633 2023-07-31 13:14:26.799749 gundi_core-1.2.1/gundi_core/schemas/v2.py
--rw-r--r--   0        0        0      330 2023-07-31 13:14:43.600428 gundi_core-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 gundi_core-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0       40 2023-07-19 19:44:21.701484 gundi_core-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 19:44:21.701601 gundi_core-1.2.2/gundi_core/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-03 18:21:20.987945 gundi_core-1.2.2/gundi_core/events/__init__.py
+-rw-r--r--   0        0        0     1019 2023-08-03 18:21:20.988138 gundi_core-1.2.2/gundi_core/events/core.py
+-rw-r--r--   0        0        0      308 2023-08-03 18:21:20.988285 gundi_core-1.2.2/gundi_core/events/dispatchers.py
+-rw-r--r--   0        0        0      114 2023-07-19 19:44:21.701758 gundi_core-1.2.2/gundi_core/schemas/__init__.py
+-rw-r--r--   0        0        0    13873 2023-08-04 18:37:34.188888 gundi_core-1.2.2/gundi_core/schemas/v1.py
+-rw-r--r--   0        0        0    15633 2023-08-03 18:21:20.989659 gundi_core-1.2.2/gundi_core/schemas/v2.py
+-rw-r--r--   0        0        0      330 2023-08-04 18:37:34.189508 gundi_core-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 gundi_core-1.2.2/PKG-INFO
```

### Comparing `gundi_core-1.2.1/gundi_core/events/core.py` & `gundi_core-1.2.2/gundi_core/events/core.py`

 * *Files identical despite different names*

### Comparing `gundi_core-1.2.1/gundi_core/schemas/v1.py` & `gundi_core-1.2.2/gundi_core/schemas/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     skylight_entry_alert = "entry_alert_rep"
 
 
 class DestinationTypes(Enum):
     EarthRanger = "earth_ranger"
     SmartConnect = "smart_connect"
     WPSWatch = "wps_watch"
+    Movebank = 'movebank'
 
 
 class TokenData(BaseModel):
     subject: Optional[str] = None
     scopes: List[str] = []
```

### Comparing `gundi_core-1.2.1/gundi_core/schemas/v2.py` & `gundi_core-1.2.2/gundi_core/schemas/v2.py`

 * *Files identical despite different names*

### Comparing `gundi_core-1.2.1/PKG-INFO` & `gundi_core-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gundi-core
-Version: 1.2.1
+Version: 1.2.2
 Summary: 
 Author: Mariano M
 Author-email: marianom@earthranger.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

