# Comparing `tmp/pyhyypapihawkmod-1.3.0b5.tar.gz` & `tmp/pyhyypapihawkmod-1.3.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.3.0b5.tar", last modified: Tue Aug  1 14:43:44 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.3.0b6.tar", last modified: Fri Aug  4 08:49:03 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.3.0b5.tar` & `pyhyypapihawkmod-1.3.0b6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 14:43:44.618865 pyhyypapihawkmod-1.3.0b5/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-08-01 14:43:44.617852 pyhyypapihawkmod-1.3.0b5/PKG-INFO
--rw-rw-rw-   0        0        0     3293 2023-08-01 14:39:14.000000 pyhyypapihawkmod-1.3.0b5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 14:43:44.603356 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      410 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      162 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    12602 2023-08-01 13:37:39.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    32743 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4114 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     1999 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/imei.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    18507 2023-08-01 14:37:39.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-08-01 14:43:44.615855 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-08-01 14:43:44.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2023-08-01 14:43:44.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 14:43:44.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-08-01 14:43:44.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 14:43:44.000000 pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 14:43:44.618865 pyhyypapihawkmod-1.3.0b5/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-08-01 14:39:23.000000 pyhyypapihawkmod-1.3.0b5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:49:03.981857 pyhyypapihawkmod-1.3.0b6/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b6/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b6/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-08-04 08:49:03.980848 pyhyypapihawkmod-1.3.0b6/PKG-INFO
+-rw-rw-rw-   0        0        0     3348 2023-08-04 08:48:12.000000 pyhyypapihawkmod-1.3.0b6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 08:49:03.878562 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      410 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    12602 2023-08-01 16:50:47.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2780 2023-08-01 17:13:20.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2825 2023-08-01 17:14:02.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    32743 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4114 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     1999 2023-08-01 13:37:33.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/imei.py
+-rw-rw-rw-   0        0        0     7584 2023-08-01 17:13:20.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    19095 2023-08-04 08:46:43.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:49:03.978828 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-08-04 08:49:03.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-08-04 08:49:03.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 08:49:03.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-04 08:49:03.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-04 08:49:03.000000 pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 08:49:03.981857 pyhyypapihawkmod-1.3.0b6/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-08-01 19:51:24.000000 pyhyypapihawkmod-1.3.0b6/setup.py
```

### Comparing `pyhyypapihawkmod-1.3.0b5/LICENSE.md` & `pyhyypapihawkmod-1.3.0b6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b5/PKG-INFO` & `pyhyypapihawkmod-1.3.0b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.3.0b5
+Version: 1.3.0b6
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.3.0b5/README.md` & `pyhyypapihawkmod-1.3.0b6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,18 @@
 
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
 Changelog 
+
+1.3.0b6
+- Added 30 min ping (Ping is broken ...)
+
 1.3.0b5
 - Added reconnect for timeouts
 
 1.3.0b4
 - Minor Refactoring
 
 1.3.0b3
```

### Comparing `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: android_checkin.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61ndroid_checkin.proto\x12\rcheckin_proto\"\x8a\x03\n\x10\x43hromeBuildProto\x12:\n\x08platform\x18\x01 \x01(\x0e\x32(.checkin_proto.ChromeBuildProto.Platform\x12\x16\n\x0e\x63hrome_version\x18\x02 \x01(\t\x12\x38\n\x07\x63hannel\x18\x03 \x01(\x0e\x32\'.checkin_proto.ChromeBuildProto.Channel\"}\n\x08Platform\x12\x10\n\x0cPLATFORM_WIN\x10\x01\x12\x10\n\x0cPLATFORM_MAC\x10\x02\x12\x12\n\x0ePLATFORM_LINUX\x10\x03\x12\x11\n\rPLATFORM_CROS\x10\x04\x12\x10\n\x0cPLATFORM_IOS\x10\x05\x12\x14\n\x10PLATFORM_ANDROID\x10\x06\"i\n\x07\x43hannel\x12\x12\n\x0e\x43HANNEL_STABLE\x10\x01\x12\x10\n\x0c\x43HANNEL_BETA\x10\x02\x12\x0f\n\x0b\x43HANNEL_DEV\x10\x03\x12\x12\n\x0e\x43HANNEL_CANARY\x10\x04\x12\x13\n\x0f\x43HANNEL_UNKNOWN\x10\x05\"\xf6\x01\n\x13\x41ndroidCheckinProto\x12\x19\n\x11last_checkin_msec\x18\x02 \x01(\x03\x12\x15\n\rcell_operator\x18\x06 \x01(\t\x12\x14\n\x0csim_operator\x18\x07 \x01(\t\x12\x0f\n\x07roaming\x18\x08 \x01(\t\x12\x13\n\x0buser_number\x18\t \x01(\x05\x12:\n\x04type\x18\x0c \x01(\x0e\x32\x19.checkin_proto.DeviceType:\x11\x44\x45VICE_ANDROID_OS\x12\x35\n\x0c\x63hrome_build\x18\r \x01(\x0b\x32\x1f.checkin_proto.ChromeBuildProto*g\n\nDeviceType\x12\x15\n\x11\x44\x45VICE_ANDROID_OS\x10\x01\x12\x11\n\rDEVICE_IOS_OS\x10\x02\x12\x19\n\x15\x44\x45VICE_CHROME_BROWSER\x10\x03\x12\x14\n\x10\x44\x45VICE_CHROME_OS\x10\x04\x42\x02H\x03')
-
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'android_checkin_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'H\003'
-  _globals['_DEVICETYPE']._serialized_start=686
-  _globals['_DEVICETYPE']._serialized_end=789
-  _globals['_CHROMEBUILDPROTO']._serialized_start=41
-  _globals['_CHROMEBUILDPROTO']._serialized_end=435
-  _globals['_CHROMEBUILDPROTO_PLATFORM']._serialized_start=203
-  _globals['_CHROMEBUILDPROTO_PLATFORM']._serialized_end=328
-  _globals['_CHROMEBUILDPROTO_CHANNEL']._serialized_start=330
-  _globals['_CHROMEBUILDPROTO_CHANNEL']._serialized_end=435
-  _globals['_ANDROIDCHECKINPROTO']._serialized_start=438
-  _globals['_ANDROIDCHECKINPROTO']._serialized_end=684
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: android_checkin.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61ndroid_checkin.proto\x12\rcheckin_proto\"\x8a\x03\n\x10\x43hromeBuildProto\x12:\n\x08platform\x18\x01 \x01(\x0e\x32(.checkin_proto.ChromeBuildProto.Platform\x12\x16\n\x0e\x63hrome_version\x18\x02 \x01(\t\x12\x38\n\x07\x63hannel\x18\x03 \x01(\x0e\x32\'.checkin_proto.ChromeBuildProto.Channel\"}\n\x08Platform\x12\x10\n\x0cPLATFORM_WIN\x10\x01\x12\x10\n\x0cPLATFORM_MAC\x10\x02\x12\x12\n\x0ePLATFORM_LINUX\x10\x03\x12\x11\n\rPLATFORM_CROS\x10\x04\x12\x10\n\x0cPLATFORM_IOS\x10\x05\x12\x14\n\x10PLATFORM_ANDROID\x10\x06\"i\n\x07\x43hannel\x12\x12\n\x0e\x43HANNEL_STABLE\x10\x01\x12\x10\n\x0c\x43HANNEL_BETA\x10\x02\x12\x0f\n\x0b\x43HANNEL_DEV\x10\x03\x12\x12\n\x0e\x43HANNEL_CANARY\x10\x04\x12\x13\n\x0f\x43HANNEL_UNKNOWN\x10\x05\"\xf6\x01\n\x13\x41ndroidCheckinProto\x12\x19\n\x11last_checkin_msec\x18\x02 \x01(\x03\x12\x15\n\rcell_operator\x18\x06 \x01(\t\x12\x14\n\x0csim_operator\x18\x07 \x01(\t\x12\x0f\n\x07roaming\x18\x08 \x01(\t\x12\x13\n\x0buser_number\x18\t \x01(\x05\x12:\n\x04type\x18\x0c \x01(\x0e\x32\x19.checkin_proto.DeviceType:\x11\x44\x45VICE_ANDROID_OS\x12\x35\n\x0c\x63hrome_build\x18\r \x01(\x0b\x32\x1f.checkin_proto.ChromeBuildProto*g\n\nDeviceType\x12\x15\n\x11\x44\x45VICE_ANDROID_OS\x10\x01\x12\x11\n\rDEVICE_IOS_OS\x10\x02\x12\x19\n\x15\x44\x45VICE_CHROME_BROWSER\x10\x03\x12\x14\n\x10\x44\x45VICE_CHROME_OS\x10\x04\x42\x02H\x03')
+
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'android_checkin_pb2', _globals)
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'H\003'
+  _globals['_DEVICETYPE']._serialized_start=686
+  _globals['_DEVICETYPE']._serialized_end=789
+  _globals['_CHROMEBUILDPROTO']._serialized_start=41
+  _globals['_CHROMEBUILDPROTO']._serialized_end=435
+  _globals['_CHROMEBUILDPROTO_PLATFORM']._serialized_start=203
+  _globals['_CHROMEBUILDPROTO_PLATFORM']._serialized_end=328
+  _globals['_CHROMEBUILDPROTO_CHANNEL']._serialized_start=330
+  _globals['_CHROMEBUILDPROTO_CHANNEL']._serialized_end=435
+  _globals['_ANDROIDCHECKINPROTO']._serialized_start=438
+  _globals['_ANDROIDCHECKINPROTO']._serialized_end=684
+# @@protoc_insertion_point(module_scope)
```

### Comparing `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/checkin_pb2.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: checkin.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-from . import android_checkin_pb2 as android__checkin__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rcheckin.proto\x12\rcheckin_proto\x1a\x15\x61ndroid_checkin.proto\"/\n\x10GservicesSetting\x12\x0c\n\x04name\x18\x01 \x02(\x0c\x12\r\n\x05value\x18\x02 \x02(\x0c\"\xcb\x03\n\x15\x41ndroidCheckinRequest\x12\x0c\n\x04imei\x18\x01 \x01(\t\x12\x0c\n\x04meid\x18\n \x01(\t\x12\x10\n\x08mac_addr\x18\t \x03(\t\x12\x15\n\rmac_addr_type\x18\x13 \x03(\t\x12\x15\n\rserial_number\x18\x10 \x01(\t\x12\x0b\n\x03\x65sn\x18\x11 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\x12\x12\n\nlogging_id\x18\x07 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x03 \x01(\t\x12\x0e\n\x06locale\x18\x06 \x01(\t\x12\x33\n\x07\x63heckin\x18\x04 \x02(\x0b\x32\".checkin_proto.AndroidCheckinProto\x12\x15\n\rdesired_build\x18\x05 \x01(\t\x12\x16\n\x0emarket_checkin\x18\x08 \x01(\t\x12\x16\n\x0e\x61\x63\x63ount_cookie\x18\x0b \x03(\t\x12\x11\n\ttime_zone\x18\x0c \x01(\t\x12\x16\n\x0esecurity_token\x18\r \x01(\x06\x12\x0f\n\x07version\x18\x0e \x01(\x05\x12\x10\n\x08ota_cert\x18\x0f \x03(\t\x12\x10\n\x08\x66ragment\x18\x14 \x01(\x05\x12\x11\n\tuser_name\x18\x15 \x01(\t\x12\x1a\n\x12user_serial_number\x18\x16 \x01(\x05\"\x83\x02\n\x16\x41ndroidCheckinResponse\x12\x10\n\x08stats_ok\x18\x01 \x02(\x08\x12\x11\n\ttime_msec\x18\x03 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x04 \x01(\t\x12\x15\n\rsettings_diff\x18\t \x01(\x08\x12\x16\n\x0e\x64\x65lete_setting\x18\n \x03(\t\x12\x30\n\x07setting\x18\x05 \x03(\x0b\x32\x1f.checkin_proto.GservicesSetting\x12\x11\n\tmarket_ok\x18\x06 \x01(\x08\x12\x12\n\nandroid_id\x18\x07 \x01(\x06\x12\x16\n\x0esecurity_token\x18\x08 \x01(\x06\x12\x14\n\x0cversion_info\x18\x0b \x01(\tB\x02H\x03')
-
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'checkin_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'H\003'
-  _globals['_GSERVICESSETTING']._serialized_start=55
-  _globals['_GSERVICESSETTING']._serialized_end=102
-  _globals['_ANDROIDCHECKINREQUEST']._serialized_start=105
-  _globals['_ANDROIDCHECKINREQUEST']._serialized_end=564
-  _globals['_ANDROIDCHECKINRESPONSE']._serialized_start=567
-  _globals['_ANDROIDCHECKINRESPONSE']._serialized_end=826
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: checkin.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+from . import android_checkin_pb2 as android__checkin__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rcheckin.proto\x12\rcheckin_proto\x1a\x15\x61ndroid_checkin.proto\"/\n\x10GservicesSetting\x12\x0c\n\x04name\x18\x01 \x02(\x0c\x12\r\n\x05value\x18\x02 \x02(\x0c\"\xcb\x03\n\x15\x41ndroidCheckinRequest\x12\x0c\n\x04imei\x18\x01 \x01(\t\x12\x0c\n\x04meid\x18\n \x01(\t\x12\x10\n\x08mac_addr\x18\t \x03(\t\x12\x15\n\rmac_addr_type\x18\x13 \x03(\t\x12\x15\n\rserial_number\x18\x10 \x01(\t\x12\x0b\n\x03\x65sn\x18\x11 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x03\x12\x12\n\nlogging_id\x18\x07 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x03 \x01(\t\x12\x0e\n\x06locale\x18\x06 \x01(\t\x12\x33\n\x07\x63heckin\x18\x04 \x02(\x0b\x32\".checkin_proto.AndroidCheckinProto\x12\x15\n\rdesired_build\x18\x05 \x01(\t\x12\x16\n\x0emarket_checkin\x18\x08 \x01(\t\x12\x16\n\x0e\x61\x63\x63ount_cookie\x18\x0b \x03(\t\x12\x11\n\ttime_zone\x18\x0c \x01(\t\x12\x16\n\x0esecurity_token\x18\r \x01(\x06\x12\x0f\n\x07version\x18\x0e \x01(\x05\x12\x10\n\x08ota_cert\x18\x0f \x03(\t\x12\x10\n\x08\x66ragment\x18\x14 \x01(\x05\x12\x11\n\tuser_name\x18\x15 \x01(\t\x12\x1a\n\x12user_serial_number\x18\x16 \x01(\x05\"\x83\x02\n\x16\x41ndroidCheckinResponse\x12\x10\n\x08stats_ok\x18\x01 \x02(\x08\x12\x11\n\ttime_msec\x18\x03 \x01(\x03\x12\x0e\n\x06\x64igest\x18\x04 \x01(\t\x12\x15\n\rsettings_diff\x18\t \x01(\x08\x12\x16\n\x0e\x64\x65lete_setting\x18\n \x03(\t\x12\x30\n\x07setting\x18\x05 \x03(\x0b\x32\x1f.checkin_proto.GservicesSetting\x12\x11\n\tmarket_ok\x18\x06 \x01(\x08\x12\x12\n\nandroid_id\x18\x07 \x01(\x06\x12\x16\n\x0esecurity_token\x18\x08 \x01(\x06\x12\x14\n\x0cversion_info\x18\x0b \x01(\tB\x02H\x03')
+
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'checkin_pb2', _globals)
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'H\003'
+  _globals['_GSERVICESSETTING']._serialized_start=55
+  _globals['_GSERVICESSETTING']._serialized_end=102
+  _globals['_ANDROIDCHECKINREQUEST']._serialized_start=105
+  _globals['_ANDROIDCHECKINREQUEST']._serialized_end=564
+  _globals['_ANDROIDCHECKINRESPONSE']._serialized_start=567
+  _globals['_ANDROIDCHECKINRESPONSE']._serialized_end=826
+# @@protoc_insertion_point(module_scope)
```

### Comparing `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/imei.py` & `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/imei.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/mcs_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-# -*- coding: utf-8 -*-
-# Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: mcs.proto
-"""Generated protocol buffer code."""
-from google.protobuf import descriptor as _descriptor
-from google.protobuf import descriptor_pool as _descriptor_pool
-from google.protobuf import symbol_database as _symbol_database
-from google.protobuf.internal import builder as _builder
-# @@protoc_insertion_point(imports)
-
-_sym_db = _symbol_database.Default()
-
-
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tmcs.proto\x12\tmcs_proto\"S\n\rHeartbeatPing\x12\x11\n\tstream_id\x18\x01 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\x03\"R\n\x0cHeartbeatAck\x12\x11\n\tstream_id\x18\x01 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\x03\"a\n\tErrorInfo\x12\x0c\n\x04\x63ode\x18\x01 \x02(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\'\n\textension\x18\x04 \x01(\x0b\x32\x14.mcs_proto.Extension\"&\n\x07Setting\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\r\n\x05value\x18\x02 \x02(\t\"A\n\rHeartbeatStat\x12\n\n\x02ip\x18\x01 \x02(\t\x12\x0f\n\x07timeout\x18\x02 \x02(\x08\x12\x13\n\x0binterval_ms\x18\x03 \x02(\x05\"G\n\x0fHeartbeatConfig\x12\x13\n\x0bupload_stat\x18\x01 \x01(\x08\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x13\n\x0binterval_ms\x18\x03 \x01(\x05\"\xd3\x02\n\x0b\x43lientEvent\x12)\n\x04type\x18\x01 \x01(\x0e\x32\x1b.mcs_proto.ClientEvent.Type\x12\x1f\n\x17number_discarded_events\x18\x64 \x01(\r\x12\x15\n\x0cnetwork_type\x18\xc8\x01 \x01(\x05\x12#\n\x1atime_connection_started_ms\x18\xca\x01 \x01(\x04\x12!\n\x18time_connection_ended_ms\x18\xcb\x01 \x01(\x04\x12\x13\n\nerror_code\x18\xcc\x01 \x01(\x05\x12\'\n\x1etime_connection_established_ms\x18\xac\x02 \x01(\x04\"[\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x14\n\x10\x44ISCARDED_EVENTS\x10\x01\x12\x15\n\x11\x46\x41ILED_CONNECTION\x10\x02\x12\x19\n\x15SUCCESSFUL_CONNECTION\x10\x03\"\xed\x03\n\x0cLoginRequest\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0e\n\x06\x64omain\x18\x02 \x02(\t\x12\x0c\n\x04user\x18\x03 \x02(\t\x12\x10\n\x08resource\x18\x04 \x02(\t\x12\x12\n\nauth_token\x18\x05 \x02(\t\x12\x11\n\tdevice_id\x18\x06 \x01(\t\x12\x13\n\x0blast_rmq_id\x18\x07 \x01(\x03\x12#\n\x07setting\x18\x08 \x03(\x0b\x32\x12.mcs_proto.Setting\x12\x1e\n\x16received_persistent_id\x18\n \x03(\t\x12\x1a\n\x12\x61\x64\x61ptive_heartbeat\x18\x0c \x01(\x08\x12\x30\n\x0eheartbeat_stat\x18\r \x01(\x0b\x32\x18.mcs_proto.HeartbeatStat\x12\x10\n\x08use_rmq2\x18\x0e \x01(\x08\x12\x12\n\naccount_id\x18\x0f \x01(\x03\x12\x39\n\x0c\x61uth_service\x18\x10 \x01(\x0e\x32#.mcs_proto.LoginRequest.AuthService\x12\x14\n\x0cnetwork_type\x18\x11 \x01(\x05\x12\x0e\n\x06status\x18\x12 \x01(\x03\x12,\n\x0c\x63lient_event\x18\x16 \x03(\x0b\x32\x16.mcs_proto.ClientEvent\"\x1d\n\x0b\x41uthService\x12\x0e\n\nANDROID_ID\x10\x02\"\xf6\x01\n\rLoginResponse\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0b\n\x03jid\x18\x02 \x01(\t\x12#\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x14.mcs_proto.ErrorInfo\x12#\n\x07setting\x18\x04 \x03(\x0b\x32\x12.mcs_proto.Setting\x12\x11\n\tstream_id\x18\x05 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x06 \x01(\x05\x12\x34\n\x10heartbeat_config\x18\x07 \x01(\x0b\x32\x1a.mcs_proto.HeartbeatConfig\x12\x18\n\x10server_timestamp\x18\x08 \x01(\x03\"/\n\x11StreamErrorStanza\x12\x0c\n\x04type\x18\x01 \x02(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\"\x07\n\x05\x43lose\"%\n\tExtension\x12\n\n\x02id\x18\x01 \x02(\x05\x12\x0c\n\x04\x64\x61ta\x18\x02 \x02(\x0c\"\xdd\x02\n\x08IqStanza\x12\x0e\n\x06rmq_id\x18\x01 \x01(\x03\x12(\n\x04type\x18\x02 \x02(\x0e\x32\x1a.mcs_proto.IqStanza.IqType\x12\n\n\x02id\x18\x03 \x02(\t\x12\x0c\n\x04\x66rom\x18\x04 \x01(\t\x12\n\n\x02to\x18\x05 \x01(\t\x12#\n\x05\x65rror\x18\x06 \x01(\x0b\x32\x14.mcs_proto.ErrorInfo\x12\'\n\textension\x18\x07 \x01(\x0b\x32\x14.mcs_proto.Extension\x12\x15\n\rpersistent_id\x18\x08 \x01(\t\x12\x11\n\tstream_id\x18\t \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\n \x01(\x05\x12\x12\n\naccount_id\x18\x0b \x01(\x03\x12\x0e\n\x06status\x18\x0c \x01(\x03\"4\n\x06IqType\x12\x07\n\x03GET\x10\x00\x12\x07\n\x03SET\x10\x01\x12\n\n\x06RESULT\x10\x02\x12\x0c\n\x08IQ_ERROR\x10\x03\"%\n\x07\x41ppData\x12\x0b\n\x03key\x18\x01 \x02(\t\x12\r\n\x05value\x18\x02 \x02(\t\"\xf4\x02\n\x11\x44\x61taMessageStanza\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0c\n\x04\x66rom\x18\x03 \x02(\t\x12\n\n\x02to\x18\x04 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x05 \x02(\t\x12\r\n\x05token\x18\x06 \x01(\t\x12$\n\x08\x61pp_data\x18\x07 \x03(\x0b\x32\x12.mcs_proto.AppData\x12\x1b\n\x13\x66rom_trusted_server\x18\x08 \x01(\x08\x12\x15\n\rpersistent_id\x18\t \x01(\t\x12\x11\n\tstream_id\x18\n \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x0b \x01(\x05\x12\x0e\n\x06reg_id\x18\r \x01(\t\x12\x16\n\x0e\x64\x65vice_user_id\x18\x10 \x01(\x03\x12\x0b\n\x03ttl\x18\x11 \x01(\x05\x12\x0c\n\x04sent\x18\x12 \x01(\x03\x12\x0e\n\x06queued\x18\x13 \x01(\x05\x12\x0e\n\x06status\x18\x14 \x01(\x03\x12\x10\n\x08raw_data\x18\x15 \x01(\x0c\x12\x15\n\rimmediate_ack\x18\x18 \x01(\x08\"\x0b\n\tStreamAck\"\x1a\n\x0cSelectiveAck\x12\n\n\x02id\x18\x01 \x03(\tB\x02H\x03')
-
-_globals = globals()
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mcs_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'H\003'
-  _globals['_HEARTBEATPING']._serialized_start=24
-  _globals['_HEARTBEATPING']._serialized_end=107
-  _globals['_HEARTBEATACK']._serialized_start=109
-  _globals['_HEARTBEATACK']._serialized_end=191
-  _globals['_ERRORINFO']._serialized_start=193
-  _globals['_ERRORINFO']._serialized_end=290
-  _globals['_SETTING']._serialized_start=292
-  _globals['_SETTING']._serialized_end=330
-  _globals['_HEARTBEATSTAT']._serialized_start=332
-  _globals['_HEARTBEATSTAT']._serialized_end=397
-  _globals['_HEARTBEATCONFIG']._serialized_start=399
-  _globals['_HEARTBEATCONFIG']._serialized_end=470
-  _globals['_CLIENTEVENT']._serialized_start=473
-  _globals['_CLIENTEVENT']._serialized_end=812
-  _globals['_CLIENTEVENT_TYPE']._serialized_start=721
-  _globals['_CLIENTEVENT_TYPE']._serialized_end=812
-  _globals['_LOGINREQUEST']._serialized_start=815
-  _globals['_LOGINREQUEST']._serialized_end=1308
-  _globals['_LOGINREQUEST_AUTHSERVICE']._serialized_start=1279
-  _globals['_LOGINREQUEST_AUTHSERVICE']._serialized_end=1308
-  _globals['_LOGINRESPONSE']._serialized_start=1311
-  _globals['_LOGINRESPONSE']._serialized_end=1557
-  _globals['_STREAMERRORSTANZA']._serialized_start=1559
-  _globals['_STREAMERRORSTANZA']._serialized_end=1606
-  _globals['_CLOSE']._serialized_start=1608
-  _globals['_CLOSE']._serialized_end=1615
-  _globals['_EXTENSION']._serialized_start=1617
-  _globals['_EXTENSION']._serialized_end=1654
-  _globals['_IQSTANZA']._serialized_start=1657
-  _globals['_IQSTANZA']._serialized_end=2006
-  _globals['_IQSTANZA_IQTYPE']._serialized_start=1954
-  _globals['_IQSTANZA_IQTYPE']._serialized_end=2006
-  _globals['_APPDATA']._serialized_start=2008
-  _globals['_APPDATA']._serialized_end=2045
-  _globals['_DATAMESSAGESTANZA']._serialized_start=2048
-  _globals['_DATAMESSAGESTANZA']._serialized_end=2420
-  _globals['_STREAMACK']._serialized_start=2422
-  _globals['_STREAMACK']._serialized_end=2433
-  _globals['_SELECTIVEACK']._serialized_start=2435
-  _globals['_SELECTIVEACK']._serialized_end=2461
-# @@protoc_insertion_point(module_scope)
+# -*- coding: utf-8 -*-
+# Generated by the protocol buffer compiler.  DO NOT EDIT!
+# source: mcs.proto
+"""Generated protocol buffer code."""
+from google.protobuf import descriptor as _descriptor
+from google.protobuf import descriptor_pool as _descriptor_pool
+from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
+# @@protoc_insertion_point(imports)
+
+_sym_db = _symbol_database.Default()
+
+
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tmcs.proto\x12\tmcs_proto\"S\n\rHeartbeatPing\x12\x11\n\tstream_id\x18\x01 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\x03\"R\n\x0cHeartbeatAck\x12\x11\n\tstream_id\x18\x01 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\x03\"a\n\tErrorInfo\x12\x0c\n\x04\x63ode\x18\x01 \x02(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\'\n\textension\x18\x04 \x01(\x0b\x32\x14.mcs_proto.Extension\"&\n\x07Setting\x12\x0c\n\x04name\x18\x01 \x02(\t\x12\r\n\x05value\x18\x02 \x02(\t\"A\n\rHeartbeatStat\x12\n\n\x02ip\x18\x01 \x02(\t\x12\x0f\n\x07timeout\x18\x02 \x02(\x08\x12\x13\n\x0binterval_ms\x18\x03 \x02(\x05\"G\n\x0fHeartbeatConfig\x12\x13\n\x0bupload_stat\x18\x01 \x01(\x08\x12\n\n\x02ip\x18\x02 \x01(\t\x12\x13\n\x0binterval_ms\x18\x03 \x01(\x05\"\xdb\x02\n\x0b\x43lientEvent\x12)\n\x04type\x18\x01 \x01(\x0e\x32\x1b.mcs_proto.ClientEvent.Type\x12\x1f\n\x17number_discarded_events\x18\x64 \x01(\r\x12\x15\n\x0cnetwork_type\x18\xc8\x01 \x01(\x05\x12#\n\x1atime_connection_started_ms\x18\xca\x01 \x01(\x04\x12!\n\x18time_connection_ended_ms\x18\xcb\x01 \x01(\x04\x12\x13\n\nerror_code\x18\xcc\x01 \x01(\x05\x12\'\n\x1etime_connection_established_ms\x18\xac\x02 \x01(\x04\"[\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x14\n\x10\x44ISCARDED_EVENTS\x10\x01\x12\x15\n\x11\x46\x41ILED_CONNECTION\x10\x02\x12\x19\n\x15SUCCESSFUL_CONNECTION\x10\x03J\x06\x08\xc9\x01\x10\xca\x01\"\xff\x03\n\x0cLoginRequest\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0e\n\x06\x64omain\x18\x02 \x02(\t\x12\x0c\n\x04user\x18\x03 \x02(\t\x12\x10\n\x08resource\x18\x04 \x02(\t\x12\x12\n\nauth_token\x18\x05 \x02(\t\x12\x11\n\tdevice_id\x18\x06 \x01(\t\x12\x13\n\x0blast_rmq_id\x18\x07 \x01(\x03\x12#\n\x07setting\x18\x08 \x03(\x0b\x32\x12.mcs_proto.Setting\x12\x1e\n\x16received_persistent_id\x18\n \x03(\t\x12\x1a\n\x12\x61\x64\x61ptive_heartbeat\x18\x0c \x01(\x08\x12\x30\n\x0eheartbeat_stat\x18\r \x01(\x0b\x32\x18.mcs_proto.HeartbeatStat\x12\x10\n\x08use_rmq2\x18\x0e \x01(\x08\x12\x12\n\naccount_id\x18\x0f \x01(\x03\x12\x39\n\x0c\x61uth_service\x18\x10 \x01(\x0e\x32#.mcs_proto.LoginRequest.AuthService\x12\x14\n\x0cnetwork_type\x18\x11 \x01(\x05\x12\x0e\n\x06status\x18\x12 \x01(\x03\x12,\n\x0c\x63lient_event\x18\x16 \x03(\x0b\x32\x16.mcs_proto.ClientEvent\"\x1d\n\x0b\x41uthService\x12\x0e\n\nANDROID_ID\x10\x02J\x04\x08\x13\x10\x14J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16\"\xf6\x01\n\rLoginResponse\x12\n\n\x02id\x18\x01 \x02(\t\x12\x0b\n\x03jid\x18\x02 \x01(\t\x12#\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x14.mcs_proto.ErrorInfo\x12#\n\x07setting\x18\x04 \x03(\x0b\x32\x12.mcs_proto.Setting\x12\x11\n\tstream_id\x18\x05 \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x06 \x01(\x05\x12\x34\n\x10heartbeat_config\x18\x07 \x01(\x0b\x32\x1a.mcs_proto.HeartbeatConfig\x12\x18\n\x10server_timestamp\x18\x08 \x01(\x03\"/\n\x11StreamErrorStanza\x12\x0c\n\x04type\x18\x01 \x02(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\"\x07\n\x05\x43lose\"%\n\tExtension\x12\n\n\x02id\x18\x01 \x02(\x05\x12\x0c\n\x04\x64\x61ta\x18\x02 \x02(\x0c\"\xdd\x02\n\x08IqStanza\x12\x0e\n\x06rmq_id\x18\x01 \x01(\x03\x12(\n\x04type\x18\x02 \x02(\x0e\x32\x1a.mcs_proto.IqStanza.IqType\x12\n\n\x02id\x18\x03 \x02(\t\x12\x0c\n\x04\x66rom\x18\x04 \x01(\t\x12\n\n\x02to\x18\x05 \x01(\t\x12#\n\x05\x65rror\x18\x06 \x01(\x0b\x32\x14.mcs_proto.ErrorInfo\x12\'\n\textension\x18\x07 \x01(\x0b\x32\x14.mcs_proto.Extension\x12\x15\n\rpersistent_id\x18\x08 \x01(\t\x12\x11\n\tstream_id\x18\t \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\n \x01(\x05\x12\x12\n\naccount_id\x18\x0b \x01(\x03\x12\x0e\n\x06status\x18\x0c \x01(\x03\"4\n\x06IqType\x12\x07\n\x03GET\x10\x00\x12\x07\n\x03SET\x10\x01\x12\n\n\x06RESULT\x10\x02\x12\x0c\n\x08IQ_ERROR\x10\x03\"%\n\x07\x41ppData\x12\x0b\n\x03key\x18\x01 \x02(\t\x12\r\n\x05value\x18\x02 \x02(\t\"\xf4\x02\n\x11\x44\x61taMessageStanza\x12\n\n\x02id\x18\x02 \x01(\t\x12\x0c\n\x04\x66rom\x18\x03 \x02(\t\x12\n\n\x02to\x18\x04 \x01(\t\x12\x10\n\x08\x63\x61tegory\x18\x05 \x02(\t\x12\r\n\x05token\x18\x06 \x01(\t\x12$\n\x08\x61pp_data\x18\x07 \x03(\x0b\x32\x12.mcs_proto.AppData\x12\x1b\n\x13\x66rom_trusted_server\x18\x08 \x01(\x08\x12\x15\n\rpersistent_id\x18\t \x01(\t\x12\x11\n\tstream_id\x18\n \x01(\x05\x12\x1f\n\x17last_stream_id_received\x18\x0b \x01(\x05\x12\x0e\n\x06reg_id\x18\r \x01(\t\x12\x16\n\x0e\x64\x65vice_user_id\x18\x10 \x01(\x03\x12\x0b\n\x03ttl\x18\x11 \x01(\x05\x12\x0c\n\x04sent\x18\x12 \x01(\x03\x12\x0e\n\x06queued\x18\x13 \x01(\x05\x12\x0e\n\x06status\x18\x14 \x01(\x03\x12\x10\n\x08raw_data\x18\x15 \x01(\x0c\x12\x15\n\rimmediate_ack\x18\x18 \x01(\x08\"\x0b\n\tStreamAck\"\x1a\n\x0cSelectiveAck\x12\n\n\x02id\x18\x01 \x03(\tB\x02H\x03')
+
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'mcs_pb2', _globals)
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  DESCRIPTOR._serialized_options = b'H\003'
+  _globals['_HEARTBEATPING']._serialized_start=24
+  _globals['_HEARTBEATPING']._serialized_end=107
+  _globals['_HEARTBEATACK']._serialized_start=109
+  _globals['_HEARTBEATACK']._serialized_end=191
+  _globals['_ERRORINFO']._serialized_start=193
+  _globals['_ERRORINFO']._serialized_end=290
+  _globals['_SETTING']._serialized_start=292
+  _globals['_SETTING']._serialized_end=330
+  _globals['_HEARTBEATSTAT']._serialized_start=332
+  _globals['_HEARTBEATSTAT']._serialized_end=397
+  _globals['_HEARTBEATCONFIG']._serialized_start=399
+  _globals['_HEARTBEATCONFIG']._serialized_end=470
+  _globals['_CLIENTEVENT']._serialized_start=473
+  _globals['_CLIENTEVENT']._serialized_end=820
+  _globals['_CLIENTEVENT_TYPE']._serialized_start=721
+  _globals['_CLIENTEVENT_TYPE']._serialized_end=812
+  _globals['_LOGINREQUEST']._serialized_start=823
+  _globals['_LOGINREQUEST']._serialized_end=1334
+  _globals['_LOGINREQUEST_AUTHSERVICE']._serialized_start=1287
+  _globals['_LOGINREQUEST_AUTHSERVICE']._serialized_end=1316
+  _globals['_LOGINRESPONSE']._serialized_start=1337
+  _globals['_LOGINRESPONSE']._serialized_end=1583
+  _globals['_STREAMERRORSTANZA']._serialized_start=1585
+  _globals['_STREAMERRORSTANZA']._serialized_end=1632
+  _globals['_CLOSE']._serialized_start=1634
+  _globals['_CLOSE']._serialized_end=1641
+  _globals['_EXTENSION']._serialized_start=1643
+  _globals['_EXTENSION']._serialized_end=1680
+  _globals['_IQSTANZA']._serialized_start=1683
+  _globals['_IQSTANZA']._serialized_end=2032
+  _globals['_IQSTANZA_IQTYPE']._serialized_start=1980
+  _globals['_IQSTANZA_IQTYPE']._serialized_end=2032
+  _globals['_APPDATA']._serialized_start=2034
+  _globals['_APPDATA']._serialized_end=2071
+  _globals['_DATAMESSAGESTANZA']._serialized_start=2074
+  _globals['_DATAMESSAGESTANZA']._serialized_end=2446
+  _globals['_STREAMACK']._serialized_start=2448
+  _globals['_STREAMACK']._serialized_end=2459
+  _globals['_SELECTIVEACK']._serialized_start=2461
+  _globals['_SELECTIVEACK']._serialized_end=2487
+# @@protoc_insertion_point(module_scope)
```

### Comparing `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod/push_receiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 REGISTER_URL = "https://android.clients.google.com/c2dm/register3"
 CHECKIN_URL = "https://android.clients.google.com/checkin"
 FCM_SUBSCRIBE = "https://fcm.googleapis.com/fcm/connect/subscribe"
 FCM_ENDPOINT = "https://fcm.googleapis.com/fcm/send"
 GOOGLE_MTALK_ENDPOINT = "mtalk.google.com"
 READ_TIMEOUT_SECS = 60 * 60
 MIN_RESET_INTERVAL_SECS = 60 * 5
-MAX_SILENT_INTERVAL_SECS = 60 * 60
+MAX_SILENT_INTERVAL_SECS = 60 * 30
 STATUS_TIMEOUT = 1
 
 MCS_VERSION = 41
 PACKET_BY_TAG = [
     HeartbeatPing,
     HeartbeatAck,
     LoginRequest,
@@ -249,16 +249,18 @@
 
     
     def __init__(
         self,
     ) -> None:
         self.fcm_registration = FCMRegistration()
         self.received_persistent_ids = []
-        self.time_last_message_received = time.time()
         self.time_of_last_reset = 0
+        self.last_stream_id_received = 0
+        self.time_of_last_receive = time.time()
+        self.current_ping_thread = 0
 
 
     def __read(self, sock, size):
         buf = b""
         while len(buf) < size:
             buf += sock.recv(size - len(buf))
         return buf
@@ -333,15 +335,16 @@
             if version < MCS_VERSION and version != 38:
                 raise RuntimeError("protocol version {} unsupported".format(version))
         else:
             (tag,) = struct.unpack("B", self.__read(data, 1))
         _LOGGER.debug("tag %s (%s)", tag, PACKET_BY_TAG[tag])
         size = self.__read_varint32(data)
         _LOGGER.debug("size %s", size)
-        self.time_last_message_received = time.time()
+        self.last_stream_id_received += 1
+        self.time_of_last_receive = time.time()
         if size >= 0:
             buf = self.__read(data, size)
             _LOGGER.debug(hexlify(buf))
             packet = PACKET_BY_TAG[tag]
             payload = packet()
             payload.ParseFromString(buf)
             _LOGGER.debug(payload)
@@ -367,15 +370,14 @@
         )
         _LOGGER.debug("connected to ssl socket")
         return google_socket
 
 
     def __login(self, credentials, persistent_ids):
         google_socket = self.__open()
-
         self.fcm_registration.gcm_check_in(**credentials["gcm"])
         req = LoginRequest()
         req.adaptive_heartbeat = False
         req.auth_service = 2
         req.auth_token = credentials["gcm"]["securityToken"]
         req.id = "chrome-63.0.3234.0"
         req.domain = "mcs.android.com"
@@ -385,14 +387,15 @@
         req.user = credentials["gcm"]["androidId"]
         req.use_rmq2 = True
         req.setting.add(name="new_vc", value="1")  # pylint: disable=maybe-no-member
         req.received_persistent_id.extend(persistent_ids)  # pylint: disable=maybe-no-member
         self.__send(google_socket, req)
         login_response = self.__recv(google_socket, first=True)
         _LOGGER.debug("Received login response: %s", login_response)
+        thread.Thread(target=self.__ping_scheduler, args=(google_socket,)).start()
         return google_socket
 
 
     def __reset(self, google_socket, credentials, persistent_ids):
         now = time.time()
         if now - self.time_of_last_reset < MIN_RESET_INTERVAL_SECS:
             raise Exception("Too many connection reset attempts.")
@@ -401,21 +404,29 @@
         try:
             google_socket.shutdown(2)
             google_socket.close()
         except OSError as err:
             _LOGGER.debug("Unable to close connection %f", err)
         return self.__login(credentials, persistent_ids)
 
-    def __status_check(self):
-        time_since_last_message = time.time() - self.time_last_message_received
-        if (time_since_last_message > MAX_SILENT_INTERVAL_SECS):
-            _LOGGER.info(f'No communications received in {time_since_last_message}s.  Resetting connection.')
-            return STATUS_TIMEOUT
-        return None
 
+    def __ping_scheduler(self, google_socket):
+        self.current_ping_thread += 1
+        if self.current_ping_thread > 10000:
+            self.current_ping_thread = 1
+        mythread = self.current_ping_thread
+        while mythread == self.current_ping_thread:
+            if time.time() - self.time_of_last_receive > MAX_SILENT_INTERVAL_SECS:
+                _LOGGER.debug("Sending PING now==========================")
+                self.__send_ping(google_socket=google_socket)
+                time.sleep(60)
+            time.sleep(60)
+        _LOGGER.debug("Closing PING thread : " + str(mythread))
+                
+        
 
 
     def __listen(self, credentials, callback, persistent_ids, obj):
         google_socket = self.__login(credentials, persistent_ids)
         while True:
             try:
                 data = self.__recv(google_socket)
@@ -427,18 +438,14 @@
                 elif data is None or isinstance(data, Close):
                     google_socket = self.__reset(google_socket, credentials, persistent_ids)
                 else:
                     _LOGGER.debug("Unexpected message type %s", type(data))
             except ConnectionResetError:
                 _LOGGER.debug("Connection Reset: Reconnecting")
                 google_socket = self.__login(credentials, persistent_ids)
-            if self.__status_check() == STATUS_TIMEOUT:
-                google_socket = self.__reset(google_socket, credentials, persistent_ids)
-           
-                
 
 
     def __handle_data_message(self, data, credentials, callback, obj):
         load_der_private_key = serialization.load_der_private_key
 
         crypto_key = self.__app_data_by_key(
             data, "crypto-key", blow_shit_up=False
@@ -466,14 +473,22 @@
             auth_secret=secret,
         )
         _LOGGER.debug("Received data message %s: %s", data.persistent_id, decrypted)
         callback(obj, json.loads(decrypted.decode("utf-8")), data)
         return data.persistent_id
 
 
+    def __send_ping(self, google_socket):
+        req = HeartbeatPing()
+        #req.stream_id = data.stream_id + 1
+        req.last_stream_id_received = self.last_stream_id_received
+        #req.status = data.status
+        self.__send(google_socket, req)
+        
+
     def __handle_ping(self, google_socket, data):
         _LOGGER.debug(
             "Responding to ping: Stream ID: %s, Last: %s, Status: %s",
             data.stream_id,
             data.last_stream_id_received,
             data.status,
         )
@@ -499,15 +514,15 @@
             received_persistent_ids = []
 
         self.__listen(credentials, callback, received_persistent_ids, obj)
 
 
     def runner(self, callback, credentials = None, persistent_ids = None):
         """sample that registers a token and waits for notifications"""
-        logging.basicConfig(level=logging.INFO)
+        #_LOGGER.setLevel(logging.DEBUG)
         if persistent_ids is None:
             persistent_ids = []
             
         if credentials is None:
             credentials = self.fcm_registration.register(sender_id=int(GCF_SENDER_ID))
             _credentials = {"credentials" : credentials}
             callback(_credentials) #doesn't do anything for now. Using a different method currently
```

### Comparing `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.3.0b5
+Version: 1.3.0b6
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.3.0b5/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.3.0b6/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b5/setup.py` & `pyhyypapihawkmod-1.3.0b6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.3.0b5",
+    version="1.3.0b6",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

