# Comparing `tmp/wappstoiot-0.6.7.tar.gz` & `tmp/wappstoiot-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wappstoiot-0.6.7.tar", last modified: Fri Jul  7 11:47:29 2023, max compression
+gzip compressed data, was "wappstoiot-0.6.8.tar", last modified: Fri Aug  4 12:41:26 2023, max compression
```

## Comparing `wappstoiot-0.6.7.tar` & `wappstoiot-0.6.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.280926 wappstoiot-0.6.7/
--rw-r--r--   0 bach      (1000) bach      (1000)     5643 2023-07-07 11:44:05.000000 wappstoiot-0.6.7/CHANGELOG.md
--rw-rw-r--   0 bach      (1000) bach      (1000)     1064 2022-03-14 08:11:46.000000 wappstoiot-0.6.7/LICENSE
--rw-r--r--   0 bach      (1000) bach      (1000)      115 2023-06-22 10:08:03.000000 wappstoiot-0.6.7/MANIFEST.in
--rw-r--r--   0 bach      (1000) bach      (1000)     9202 2023-07-07 11:47:29.279926 wappstoiot-0.6.7/PKG-INFO
--rw-r--r--   0 bach      (1000) bach      (1000)     3128 2023-06-22 10:08:03.000000 wappstoiot-0.6.7/README.md
--rw-r--r--   0 bach      (1000) bach      (1000)       38 2023-07-07 11:47:29.280926 wappstoiot-0.6.7/setup.cfg
--rw-r--r--   0 bach      (1000) bach      (1000)     2368 2023-07-07 09:56:12.000000 wappstoiot-0.6.7/setup.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.255926 wappstoiot-0.6.7/test/
--rw-r--r--   0 bach      (1000) bach      (1000)     3159 2023-06-22 10:08:45.000000 wappstoiot-0.6.7/test/test_real_world.py
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.257926 wappstoiot-0.6.7/wappstoiot/
--rw-r--r--   0 bach      (1000) bach      (1000)    11300 2023-07-07 11:44:18.000000 wappstoiot-0.6.7/wappstoiot/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)     1080 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/__init__.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     8363 2023-06-22 10:08:03.000000 wappstoiot-0.6.7/wappstoiot/__main__.py
--rw-r--r--   0 bach      (1000) bach      (1000)       94 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/__main__.pyi
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.262926 wappstoiot-0.6.7/wappstoiot/connections/
--rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:04:21.000000 wappstoiot-0.6.7/wappstoiot/connections/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/connections/__init__.pyi
--rw-rw-r--   0 bach      (1000) bach      (1000)     2469 2023-07-07 11:10:09.000000 wappstoiot-0.6.7/wappstoiot/connections/protocol.py
--rw-r--r--   0 bach      (1000) bach      (1000)      756 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/connections/protocol.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     9931 2023-07-07 11:25:56.000000 wappstoiot-0.6.7/wappstoiot/connections/sslsocket.py
--rw-r--r--   0 bach      (1000) bach      (1000)      938 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/connections/sslsocket.pyi
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.266926 wappstoiot-0.6.7/wappstoiot/modules/
--rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:04:32.000000 wappstoiot-0.6.7/wappstoiot/modules/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/modules/__init__.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    16018 2023-07-07 11:13:41.000000 wappstoiot-0.6.7/wappstoiot/modules/device.py
--rw-r--r--   0 bach      (1000) bach      (1000)     3496 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/modules/device.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    10801 2023-07-07 11:14:27.000000 wappstoiot-0.6.7/wappstoiot/modules/network.py
--rw-r--r--   0 bach      (1000) bach      (1000)     1695 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/modules/network.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    24084 2023-07-07 11:02:16.000000 wappstoiot-0.6.7/wappstoiot/modules/template.py
--rw-r--r--   0 bach      (1000) bach      (1000)     2309 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/modules/template.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    28482 2023-07-07 11:22:31.000000 wappstoiot-0.6.7/wappstoiot/modules/value.py
--rw-r--r--   0 bach      (1000) bach      (1000)     3585 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/modules/value.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)       62 2023-06-22 10:08:03.000000 wappstoiot-0.6.7/wappstoiot/py.typed
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.269926 wappstoiot-0.6.7/wappstoiot/schema/
--rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:04:46.000000 wappstoiot-0.6.7/wappstoiot/schema/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/schema/__init__.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    12677 2023-06-26 11:19:57.000000 wappstoiot-0.6.7/wappstoiot/schema/base_schema.py
--rw-r--r--   0 bach      (1000) bach      (1000)     8268 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/schema/base_schema.pyi
--rw-rw-r--   0 bach      (1000) bach      (1000)     5591 2023-07-07 11:19:59.000000 wappstoiot-0.6.7/wappstoiot/schema/iot_schema.py
--rw-r--r--   0 bach      (1000) bach      (1000)     1620 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/schema/iot_schema.pyi
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.272926 wappstoiot-0.6.7/wappstoiot/service/
--rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:04:54.000000 wappstoiot-0.6.7/wappstoiot/service/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/service/__init__.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)    22495 2023-06-26 11:19:57.000000 wappstoiot-0.6.7/wappstoiot/service/iot_api.py
--rw-r--r--   0 bach      (1000) bach      (1000)     3510 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/service/iot_api.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     4916 2023-07-07 09:43:39.000000 wappstoiot-0.6.7/wappstoiot/service/template.py
--rw-r--r--   0 bach      (1000) bach      (1000)     3180 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/service/template.pyi
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.278926 wappstoiot-0.6.7/wappstoiot/utils/
--rw-r--r--   0 bach      (1000) bach      (1000)      646 2023-02-27 15:18:27.000000 wappstoiot-0.6.7/wappstoiot/utils/Timestamp.py
--rw-r--r--   0 bach      (1000) bach      (1000)      107 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/Timestamp.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:05:02.000000 wappstoiot-0.6.7/wappstoiot/utils/__init__.py
--rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/__init__.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)      483 2023-07-07 10:02:18.000000 wappstoiot-0.6.7/wappstoiot/utils/certificateread.py
--rw-r--r--   0 bach      (1000) bach      (1000)      143 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/certificateread.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)      718 2023-07-07 11:10:24.000000 wappstoiot-0.6.7/wappstoiot/utils/name_check.py
--rw-r--r--   0 bach      (1000) bach      (1000)      148 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/name_check.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     2711 2023-07-07 11:06:16.000000 wappstoiot-0.6.7/wappstoiot/utils/observer.py
--rw-r--r--   0 bach      (1000) bach      (1000)      403 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/observer.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     2562 2023-07-07 11:21:40.000000 wappstoiot-0.6.7/wappstoiot/utils/offline_storage.py
--rw-r--r--   0 bach      (1000) bach      (1000)      689 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/offline_storage.pyi
--rw-r--r--   0 bach      (1000) bach      (1000)     6523 2023-07-07 11:21:20.000000 wappstoiot-0.6.7/wappstoiot/utils/tracer.py
--rw-r--r--   0 bach      (1000) bach      (1000)     1316 2023-07-07 11:45:57.000000 wappstoiot-0.6.7/wappstoiot/utils/tracer.pyi
-drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-07-07 11:47:29.259926 wappstoiot-0.6.7/wappstoiot.egg-info/
--rw-r--r--   0 bach      (1000) bach      (1000)     9202 2023-07-07 11:47:29.000000 wappstoiot-0.6.7/wappstoiot.egg-info/PKG-INFO
--rw-r--r--   0 bach      (1000) bach      (1000)     1699 2023-07-07 11:47:29.000000 wappstoiot-0.6.7/wappstoiot.egg-info/SOURCES.txt
--rw-r--r--   0 bach      (1000) bach      (1000)        1 2023-07-07 11:47:29.000000 wappstoiot-0.6.7/wappstoiot.egg-info/dependency_links.txt
--rw-r--r--   0 bach      (1000) bach      (1000)       51 2023-07-07 11:47:29.000000 wappstoiot-0.6.7/wappstoiot.egg-info/requires.txt
--rw-r--r--   0 bach      (1000) bach      (1000)       11 2023-07-07 11:47:29.000000 wappstoiot-0.6.7/wappstoiot.egg-info/top_level.txt
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 12:41:26.318612 wappstoiot-0.6.8/
+-rw-r--r--   0 bach      (1000) bach      (1000)     5990 2023-08-04 12:40:47.000000 wappstoiot-0.6.8/CHANGELOG.md
+-rw-rw-r--   0 bach      (1000) bach      (1000)     1064 2022-03-14 08:11:46.000000 wappstoiot-0.6.8/LICENSE
+-rw-r--r--   0 bach      (1000) bach      (1000)      115 2023-06-22 10:08:03.000000 wappstoiot-0.6.8/MANIFEST.in
+-rw-r--r--   0 bach      (1000) bach      (1000)    14960 2023-08-04 12:41:26.317613 wappstoiot-0.6.8/PKG-INFO
+-rw-r--r--   0 bach      (1000) bach      (1000)     8539 2023-07-07 11:55:22.000000 wappstoiot-0.6.8/README.md
+-rw-r--r--   0 bach      (1000) bach      (1000)       38 2023-08-04 12:41:26.318612 wappstoiot-0.6.8/setup.cfg
+-rw-r--r--   0 bach      (1000) bach      (1000)     2368 2023-08-04 12:39:29.000000 wappstoiot-0.6.8/setup.py
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 12:41:26.299612 wappstoiot-0.6.8/test/
+-rw-r--r--   0 bach      (1000) bach      (1000)     3159 2023-06-22 10:08:45.000000 wappstoiot-0.6.8/test/test_real_world.py
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 12:41:26.301612 wappstoiot-0.6.8/wappstoiot/
+-rw-r--r--   0 bach      (1000) bach      (1000)    11359 2023-08-04 12:40:38.000000 wappstoiot-0.6.8/wappstoiot/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1133 2023-08-04 12:39:29.000000 wappstoiot-0.6.8/wappstoiot/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     8363 2023-06-22 10:08:03.000000 wappstoiot-0.6.8/wappstoiot/__main__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)       94 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/__main__.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 12:41:26.305612 wappstoiot-0.6.8/wappstoiot/connections/
+-rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/connections/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/connections/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     2469 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/connections/protocol.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      756 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/connections/protocol.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     9933 2023-07-31 10:10:15.000000 wappstoiot-0.6.8/wappstoiot/connections/sslsocket.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      938 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/connections/sslsocket.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 12:41:26.308612 wappstoiot-0.6.8/wappstoiot/modules/
+-rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/modules/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/modules/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    16018 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/modules/device.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3496 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/modules/device.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    10801 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/modules/network.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1695 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/modules/network.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    24084 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/modules/template.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     2309 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/modules/template.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    31091 2023-08-01 10:44:51.000000 wappstoiot-0.6.8/wappstoiot/modules/value.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3639 2023-08-04 12:39:29.000000 wappstoiot-0.6.8/wappstoiot/modules/value.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)       62 2023-06-22 10:08:03.000000 wappstoiot-0.6.8/wappstoiot/py.typed
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 12:41:26.310613 wappstoiot-0.6.8/wappstoiot/schema/
+-rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/schema/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/schema/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    12883 2023-07-31 13:27:17.000000 wappstoiot-0.6.8/wappstoiot/schema/base_schema.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     8424 2023-08-04 12:39:29.000000 wappstoiot-0.6.8/wappstoiot/schema/base_schema.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     5591 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/schema/iot_schema.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1620 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/schema/iot_schema.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 12:41:26.312612 wappstoiot-0.6.8/wappstoiot/service/
+-rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/service/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/service/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)    24943 2023-08-04 12:39:29.000000 wappstoiot-0.6.8/wappstoiot/service/iot_api.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3631 2023-08-04 12:39:29.000000 wappstoiot-0.6.8/wappstoiot/service/iot_api.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     4916 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/service/template.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     3180 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/service/template.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 12:41:26.317613 wappstoiot-0.6.8/wappstoiot/utils/
+-rw-r--r--   0 bach      (1000) bach      (1000)      646 2023-02-27 15:18:27.000000 wappstoiot-0.6.8/wappstoiot/utils/Timestamp.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      107 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/utils/Timestamp.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)        8 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/utils/__init__.py
+-rw-r--r--   0 bach      (1000) bach      (1000)        0 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/utils/__init__.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)      483 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/utils/certificateread.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      143 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/utils/certificateread.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)      718 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/utils/name_check.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      148 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/utils/name_check.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     2711 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/utils/observer.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      403 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/utils/observer.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     2562 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/utils/offline_storage.py
+-rw-r--r--   0 bach      (1000) bach      (1000)      689 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/utils/offline_storage.pyi
+-rw-r--r--   0 bach      (1000) bach      (1000)     6523 2023-07-07 11:51:40.000000 wappstoiot-0.6.8/wappstoiot/utils/tracer.py
+-rw-r--r--   0 bach      (1000) bach      (1000)     1316 2023-08-01 12:29:22.000000 wappstoiot-0.6.8/wappstoiot/utils/tracer.pyi
+drwxr-xr-x   0 bach      (1000) bach      (1000)        0 2023-08-04 12:41:26.303613 wappstoiot-0.6.8/wappstoiot.egg-info/
+-rw-r--r--   0 bach      (1000) bach      (1000)    14960 2023-08-04 12:41:26.000000 wappstoiot-0.6.8/wappstoiot.egg-info/PKG-INFO
+-rw-r--r--   0 bach      (1000) bach      (1000)     1699 2023-08-04 12:41:26.000000 wappstoiot-0.6.8/wappstoiot.egg-info/SOURCES.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)        1 2023-08-04 12:41:26.000000 wappstoiot-0.6.8/wappstoiot.egg-info/dependency_links.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)       51 2023-08-04 12:41:26.000000 wappstoiot-0.6.8/wappstoiot.egg-info/requires.txt
+-rw-r--r--   0 bach      (1000) bach      (1000)       11 2023-08-04 12:41:26.000000 wappstoiot-0.6.8/wappstoiot.egg-info/top_level.txt
```

### Comparing `wappstoiot-0.6.7/CHANGELOG.md` & `wappstoiot-0.6.8/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+v0.6.8 (Aug 04 2023)
+===============================================================================
+## Added
+ * `report` now take a `LogValue` or a list of `LogValue`s.
+
+## Changed
+ * It will now bulk report data, if a list af `LogValue`s is given.
+ * Bulk report data will now be sorted.
+
+## Fixed
+ * Handle a rare error case from the server.
+
+
 v0.6.7 (Jul 07 2023)
 ===============================================================================
 ## Added
  * Scandinavian special letters to the legal list
 
 ## Changed
  * Updated the `wappstoiot.ValueTemplate` to version v0.0.5
```

### Comparing `wappstoiot-0.6.7/LICENSE` & `wappstoiot-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/setup.py` & `wappstoiot-0.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     #     'pytest',
     #     'tox'
     # ],
     package_data={
         'wappstoiot': ["py.typed", "*.pyi", "**/*.pyi"]
     },
     install_requires=[
-        'slxjsonrpc>=0.8.1',
+        'slxjsonrpc==0.8.1',
         'pydantic==1.9.2',
         'requests>=2.25.1'
     ],
     # entry_points={  # TODO: fix __main__.py to be optional.
     #     "console_scripts": "wappstoiot=wappstoiot:__main__"
     # },
     # extras_require={  # TODO: fix __main__.py to be optional.
```

### Comparing `wappstoiot-0.6.7/test/test_real_world.py` & `wappstoiot-0.6.8/test/test_real_world.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/__init__.py` & `wappstoiot-0.6.8/wappstoiot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
 from .modules.value import Value
 # from .modules.value import Delta  # Note: Not ready yet!
 # from .modules.value import Period  # Note: Not ready yet!
 from .modules.value import PermissionType
 from .modules.template import ValueTemplate
 
+from .schema.base_schema import LogValue
+
 from .service import template as service
 
 from .connections import protocol as connection
 
 from .utils.offline_storage import OfflineStorage
 from .utils.certificateread import certificate_info_extraction
 from .utils.offline_storage import OfflineStorageFiles
@@ -48,15 +50,15 @@
 from .utils import observer
 from .utils import name_check
 
 # #############################################################################
 #                             __init__ Setup Stuff
 # #############################################################################
 
-__version__ = "v0.6.7"
+__version__ = "v0.6.8"
 __auther__ = "Seluxit A/S"
 
 __all__ = [
     'Network',
     'Device',
     'Value',
     'onStatusChange',
@@ -65,15 +67,16 @@
     'connect',
     'disconnect',
     'close',
     'OfflineStorage',
     'service',
     'connection',
     'ValueTemplate',
-    'PermissionType'
+    'PermissionType',
+    'LogValue',
 ]
 
 
 # #############################################################################
 #                  Import Stuff for setting up WappstoIoT
 # #############################################################################
```

### Comparing `wappstoiot-0.6.7/wappstoiot/__init__.pyi` & `wappstoiot-0.6.8/wappstoiot/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .connections import protocol as connection
 from .modules.device import Device as Device
 from .modules.network import Network as Network
 from .modules.template import ValueTemplate as ValueTemplate
 from .modules.value import PermissionType as PermissionType, Value as Value
+from .schema.base_schema import LogValue as LogValue
 from .service import template as service
 from .utils.offline_storage import OfflineStorage as OfflineStorage
 from enum import Enum
 from pathlib import Path
 from typing import Any, Callable, Optional, Union
 
 def onStatusChange(StatusID: Union[service.StatusID, connection.StatusID], callback: Callable[[Union[service.StatusID, connection.StatusID], Any], None]): ...
```

### Comparing `wappstoiot-0.6.7/wappstoiot/__main__.py` & `wappstoiot-0.6.8/wappstoiot/__main__.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/connections/protocol.py` & `wappstoiot-0.6.8/wappstoiot/connections/protocol.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/connections/protocol.pyi` & `wappstoiot-0.6.8/wappstoiot/connections/protocol.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/connections/sslsocket.py` & `wappstoiot-0.6.8/wappstoiot/connections/sslsocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         Socket receive method.
 
         Method that handles receiving data from a socket. Capable of handling
         data chunks.
 
         Args:
             Callable: A parser, that returns the parsed data.
-                      On Parsen Error, it should raise a
+                      On Parsing Error, it should raise a
                       ValueError TypeError or any subClasses of those.
                       (Like 'JSONDecodeError' & 'pydantic.ValidationError' is)
 
         Returns:
             The "parser"'s output.
         """
         data = []
@@ -231,15 +231,15 @@
                 self.log.debug(f"Raw Data Received: {data}")
                 return parsed_data
 
     def connect(self) -> Optional[bool]:
         """
         Connect to the server.
 
-        Attempts a connection to the server on the provided addres and port.
+        Attempts a connection to the server on the provided address and port.
 
         Returns:
             'True' if the connection was successful.
         """
         if self.killed.is_set():
             return False
```

### Comparing `wappstoiot-0.6.7/wappstoiot/connections/sslsocket.pyi` & `wappstoiot-0.6.8/wappstoiot/connections/sslsocket.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/modules/device.py` & `wappstoiot-0.6.8/wappstoiot/modules/device.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/modules/device.pyi` & `wappstoiot-0.6.8/wappstoiot/modules/device.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/modules/network.py` & `wappstoiot-0.6.8/wappstoiot/modules/network.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/modules/network.pyi` & `wappstoiot-0.6.8/wappstoiot/modules/network.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/modules/template.py` & `wappstoiot-0.6.8/wappstoiot/modules/template.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/modules/template.pyi` & `wappstoiot-0.6.8/wappstoiot/modules/template.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/modules/value.py` & `wappstoiot-0.6.8/wappstoiot/modules/value.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 
 from enum import Enum
 from datetime import datetime
 
 from typing import Any
 from typing import Callable
 from typing import Dict
+from typing import List
 from typing import Optional
 from typing import Union
 
 from ..service.template import ServiceClass
 # from .template import dict_diff
 from .template import ValueBaseType
 # from .template import valueSettings
 from ..schema import base_schema as WSchema
 from ..schema.base_schema import PermissionType
+from ..schema.base_schema import LogValue
 from ..schema.iot_schema import WappstoMethod
 
 from ..schema.base_schema import timestamp_converter
 
 from ..utils.Timestamp import str_to_datetime
 
 from typing import TYPE_CHECKING
@@ -684,48 +686,113 @@
         # raise NotImplementedError("Method: 'change' is not Implemented.")
         pass
 
     def delete(self) -> None:
         """Request a delete of the Device, & all it's Children."""
         self.connection.delete_value(uuid=self.uuid)
 
+    def _update_local_report(self, data, timestamp):
+        if (
+            data.timestamp and self.report_state.timestamp or not self.report_state.timestamp
+        ):
+            self.report_state = self.report_state.copy(update=data.dict(exclude_none=True))
+            self.report_state.timestamp = timestamp or data.timestamp
+            if self.report_state.timestamp:
+                self.report_state.timestamp = self.report_state.timestamp.replace(tzinfo=None)
+
     def report(
         self,
-        value: Union[int, float, str, None],
+        value: Union[int, float, str, LogValue, List[LogValue], None],
         timestamp: Optional[datetime] = None
     ) -> None:
         """
         Report the new current value to Wappsto.
 
         The Report value is typical a measured value from a sensor,
         whether it is a GPIO pin, a analog temperature sensor or a
         device over a I2C bus.
 
         ERROR: https://github.com/pydantic/pydantic/issues/4852
 
         """
         # TODO: Check if this value have a state that is read.
         self.log.info(f"Sending Report for: {self.report_state.meta.id}")
-        the_timestamp = timestamp if timestamp is not None else datetime.utcnow()
-        data = WSchema.State(
-            data=value,
-            timestamp=timestamp_converter(the_timestamp)
-        )
-        if (
-            data.timestamp and self.report_state.timestamp or not self.report_state.timestamp
-        ):
-            self.report_state = self.report_state.copy(update=data.dict(exclude_none=True))
-            self.report_state.timestamp = the_timestamp
-            if self.report_state.timestamp:
-                self.report_state.timestamp = self.report_state.timestamp.replace(tzinfo=None)
+
+        if isinstance(value, list):
+            if not len(value):
+                return
+
+            # TODO: Make sure the timestamps are set.
+            sorted_values = sorted(value, key=lambda r: r.timestamp)
+            self._update_local_report(sorted_values[-1], sorted_values[-1].timestamp)
+
+            self.connection.put_bulk_state(
+                uuid=self.children_name_mapping[WSchema.StateType.REPORT.name],
+                data=[
+                    LogValue(
+                        data=x.data,
+                        timestamp=timestamp_converter(x.timestamp) if isinstance(x.timestamp, datetime) else x.timestamp
+                    ) for x in sorted_values
+                ],
+            )
+            return
+
+        if not isinstance(value, LogValue):
+            the_timestamp = timestamp if timestamp is not None else datetime.utcnow()
+            data = LogValue(
+                data=value,
+                timestamp=timestamp_converter(the_timestamp) if isinstance(the_timestamp, datetime) else the_timestamp,
+            )
+        else:
+            # TODO: Make sure the timestamp is set.
+            data = value
+
+        self._update_local_report(data, the_timestamp)
+
+        # NOTE: Single Report
         self.connection.put_state(
             uuid=self.children_name_mapping[WSchema.StateType.REPORT.name],
-            data=data
+            data=data,
         )
 
+    # def report(
+    #     self,
+    #     value: Union[int, float, str, LogValue, List[LogValue], None],
+    #     timestamp: Optional[datetime] = None
+    # ) -> None:
+    #     """
+    #     Report the new current value to Wappsto.
+
+    #     The Report value is typical a measured value from a sensor,
+    #     whether it is a GPIO pin, a analog temperature sensor or a
+    #     device over a I2C bus.
+
+    #     ERROR: https://github.com/pydantic/pydantic/issues/4852
+
+    #     """
+    #     # TODO: Check if this value have a state that is read.
+    #     self.log.info(f"Sending Report for: {self.report_state.meta.id}")
+
+    #     the_timestamp = timestamp if timestamp is not None else datetime.utcnow()
+    #     data = WSchema.State(
+    #         data=value,
+    #         timestamp=timestamp_converter(the_timestamp)
+    #     )
+    #     if (
+    #         data.timestamp and self.report_state.timestamp or not self.report_state.timestamp
+    #     ):
+    #         self.report_state = self.report_state.copy(update=data.dict(exclude_none=True))
+    #         self.report_state.timestamp = the_timestamp
+    #         if self.report_state.timestamp:
+    #             self.report_state.timestamp = self.report_state.timestamp.replace(tzinfo=None)
+    #     self.connection.put_state(
+    #         uuid=self.children_name_mapping[WSchema.StateType.REPORT.name],
+    #         data=data
+    #     )
+
     def control(
         self,
         value: Union[int, float, str, None],
         timestamp: Optional[datetime] = None
     ) -> None:
         """
         Report the a new control value to Wappsto.
```

### Comparing `wappstoiot-0.6.7/wappstoiot/modules/value.pyi` & `wappstoiot-0.6.8/wappstoiot/modules/value.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import uuid
-from ..schema.base_schema import PermissionType as PermissionType, timestamp_converter as timestamp_converter
+from ..schema.base_schema import LogValue as LogValue, PermissionType as PermissionType, timestamp_converter as timestamp_converter
 from ..schema.iot_schema import WappstoMethod as WappstoMethod
 from ..service.template import ServiceClass as ServiceClass
 from ..utils.Timestamp import str_to_datetime as str_to_datetime
 from .device import Device as Device
 from .template import ValueBaseType as ValueBaseType
 from _typeshed import Incomplete
 from datetime import datetime
 from enum import Enum
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
 class Period(str, Enum):
     PERIODIC_REFRESH: str
     DROP_UNTIL: str
 
 class Delta(str, Enum):
     ONLY_UPDATE_IF: str
@@ -65,10 +65,10 @@
     def onRefresh(self, callback: Callable[[Value], None]) -> Callable[[Value], None]: ...
     def cancelOnRefresh(self) -> None: ...
     def onDelete(self, callback: Callable[[Value], None]) -> Callable[[Value], None]: ...
     def cancelOnDelete(self) -> None: ...
     def refresh(self) -> None: ...
     def change(self, name: str, value: Any) -> None: ...
     def delete(self) -> None: ...
-    def report(self, value: Union[int, float, str, None], timestamp: Optional[datetime] = ...) -> None: ...
+    def report(self, value: Union[int, float, str, LogValue, List[LogValue], None], timestamp: Optional[datetime] = ...) -> None: ...
     def control(self, value: Union[int, float, str, None], timestamp: Optional[datetime] = ...) -> None: ...
     def close(self) -> None: ...
```

### Comparing `wappstoiot-0.6.7/wappstoiot/schema/base_schema.py` & `wappstoiot-0.6.8/wappstoiot/schema/base_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,14 +298,25 @@
         }
 
 
 class Info(BaseModel):
     enabled: Optional[bool] = None
 
 
+class LogValue(BaseModel):
+    data: str
+    timestamp: Union[str, datetime]
+
+    class Config:
+        extra = Extra.forbid
+        json_encoders = {
+            datetime: timestamp_converter,
+        }
+
+
 class State(BaseModel):
     data: str
     type: Optional[StateType]
 
     meta: Optional[StateMeta] = Field(None, title='meta-2.0:create')
     status: Optional[StateStatus] = None
     status_payment: Optional[str] = None
```

### Comparing `wappstoiot-0.6.7/wappstoiot/schema/base_schema.pyi` & `wappstoiot-0.6.8/wappstoiot/schema/base_schema.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -203,14 +203,21 @@
     meta: Optional[StatusMeta]
     class Config:
         json_encoders: Incomplete
 
 class Info(BaseModel):
     enabled: Optional[bool]
 
+class LogValue(BaseModel):
+    data: str
+    timestamp: Union[str, datetime]
+    class Config:
+        extra: Incomplete
+        json_encoders: Incomplete
+
 class State(BaseModel):
     data: str
     type: Optional[StateType]
     meta: Optional[StateMeta]
     status: Optional[StateStatus]
     status_payment: Optional[str]
     timestamp: Optional[str]
```

### Comparing `wappstoiot-0.6.7/wappstoiot/schema/iot_schema.py` & `wappstoiot-0.6.8/wappstoiot/schema/iot_schema.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/schema/iot_schema.pyi` & `wappstoiot-0.6.8/wappstoiot/schema/iot_schema.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/service/iot_api.py` & `wappstoiot-0.6.8/wappstoiot/service/iot_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import threading
 
 from uuid import UUID
 from pathlib import Path
 
 from concurrent.futures import ThreadPoolExecutor
 
+from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 import slxjsonrpc
@@ -26,14 +27,15 @@
 from ..schema.base_schema import Network
 from ..schema.base_schema import NumberValue
 from ..schema.base_schema import State
 from ..schema.base_schema import StringValue
 from ..schema.base_schema import XmlValue
 from ..schema.base_schema import WappstoObject
 from ..schema.base_schema import IdList
+from ..schema.base_schema import LogValue
 
 from ..schema.iot_schema import JsonData
 from ..schema.iot_schema import Identifier
 from ..schema.iot_schema import JsonReply
 from ..schema.iot_schema import Success
 from ..schema.iot_schema import WappstoMethod
 # from ..schema.iot_scgema import WappstoObjectType
@@ -172,14 +174,18 @@
         while not self.killed.is_set():
             try:
                 data = self.connection.receive(parser=json.loads)
 
                 if not data:
                     continue
 
+                if isinstance(data, str):
+                    self.log.warning(f'Received non JSONRPC data: {data}')
+                    continue
+
                 if not isinstance(data, list):
                     data = [data]
                 for elemt in data:
                     _ids = [elemt.get('id', elemt) for elemt in data]
                     self.log.debug(f"Package received: {elemt.get('id', elemt)}")
 
                 trace = tracer.Trace.trace_list_check(
@@ -277,14 +283,69 @@
                 observer.post(StatusID.SENDERROR, s_data)
         return None
 
     # -------------------------------------------------------------------------
     #                               API Helpers
     # -------------------------------------------------------------------------
 
+    def __create_json_data(self, data: List[Any], url, method):
+        _cb_event = threading.Event()
+        _err_data: Optional[ErrorModel] = None
+
+        def _err_callback(err_data: ErrorModel):
+            nonlocal _err_data
+            nonlocal _cb_event
+            _err_data = err_data
+            _cb_event.set()
+
+        with self.jsonrpc.batch():
+            for values in data:
+                j_data = JsonData(
+                    data=values,
+                    url=url,
+                    meta=Identifier(fast=True) if self.fast_send and method != WappstoMethod.GET else None
+                )
+
+                self.log.debug(f"Sending for: {url}")
+
+                self.jsonrpc.create_request(
+                    method=method,
+                    callback=lambda data: _cb_event.set(),
+                    error_callback=_err_callback,
+                    params=j_data
+                )
+
+        rpc_data = self.jsonrpc.get_batch_data()
+
+        return rpc_data, _cb_event, _err_data
+
+    def _no_reply_bulk_send(self, data: List, url, method) -> bool:
+        rpc_data, _cb_event, _err_data = self.__create_json_data(
+            data=data, url=url, method=method,
+        )
+        rpc_id = "[" + ",".join(
+            [f'"{getattr(rpc_data, "id", None)}"' for rpc_d in rpc_data]
+        ) + "]"
+
+        self._send_logic(rpc_data)
+
+        self.log.debug(f"--CALLBACK Ready! {rpc_id}")
+        if _cb_event.wait(timeout=self.timeout):
+            if _err_data:
+                self.log.debug(f"--CALLBACK Error! {_err_data}")
+                observer.post(StatusID.ERROR, _err_data)
+                # raise ConnectionError(_err_data.message)
+                return False
+            self.log.debug(f"--CALLBACK EVENT! {rpc_id}")
+            observer.post(StatusID.SEND, rpc_data)
+            return True
+        observer.post(StatusID.SENDERROR, rpc_data)
+        self.log.debug(f"--CALLBACK None! {rpc_id}")
+        return False
+
     def _no_reply_send(self, data, url, method) -> bool:
         j_data = JsonData(
             data=data,
             url=url,
             meta=Identifier(fast=True) if self.fast_send and method != WappstoMethod.GET else None
         )
 
@@ -650,15 +711,23 @@
         # url=f"/services/2.0/{uuid}/state",
         return self._no_reply_send(
             data=data,
             url=f"/value/{value_uuid}/state/",
             method=WappstoMethod.POST
         )
 
-    def put_state(self, uuid: UUID, data: State) -> bool:
+    def put_bulk_state(self, uuid: UUID, data: List[LogValue]) -> bool:
+        # url=f"/services/2.0/state/{uuid}",
+        return self._no_reply_bulk_send(
+            data=data,
+            url=f"/state/{uuid}",
+            method=WappstoMethod.PUT
+        )
+
+    def put_state(self, uuid: UUID, data: Union[State, LogValue]) -> bool:
         # url=f"/services/2.0/state/{uuid}",
         return self._no_reply_send(
             data=data,
             url=f"/state/{uuid}",
             method=WappstoMethod.PUT
         )
```

### Comparing `wappstoiot-0.6.7/wappstoiot/service/iot_api.pyi` & `wappstoiot-0.6.8/wappstoiot/service/iot_api.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from ..connections.protocol import Connection as Connection
 from ..connections.sslsocket import TlsSocket as TlsSocket
-from ..schema.base_schema import BlobValue as BlobValue, Device as Device, IdList as IdList, Network as Network, NumberValue as NumberValue, State as State, StringValue as StringValue, WappstoObject as WappstoObject, XmlValue as XmlValue
+from ..schema.base_schema import BlobValue as BlobValue, Device as Device, IdList as IdList, LogValue as LogValue, Network as Network, NumberValue as NumberValue, State as State, StringValue as StringValue, WappstoObject as WappstoObject, XmlValue as XmlValue
 from ..schema.iot_schema import Identifier as Identifier, JsonData as JsonData, JsonReply as JsonReply, Success as Success, WappstoMethod as WappstoMethod
 from ..utils import observer as observer, tracer as tracer
 from ..utils.certificateread import certificate_info_extraction as certificate_info_extraction
 from .template import ServiceClass as ServiceClass, StatusID as StatusID
 from _typeshed import Incomplete
 from pathlib import Path
-from typing import Callable, Optional, Union
+from typing import Callable, List, Optional, Union
 from uuid import UUID
 
 ValueUnion = Union[StringValue, NumberValue, BlobValue, XmlValue]
 
 class IoTAPI(ServiceClass):
     wappstoPort: Incomplete
     log: Incomplete
@@ -47,10 +47,11 @@
     def put_value(self, uuid: UUID, data: ValueUnion) -> bool: ...
     def get_value_where(self, device_uuid: UUID, **kwargs: str) -> Optional[UUID]: ...
     def get_value(self, uuid: UUID) -> Union[ValueUnion, None]: ...
     def delete_value(self, uuid: UUID) -> bool: ...
     def subscribe_state_event(self, uuid: UUID, callback: Callable[[State, WappstoMethod], None]) -> None: ...
     def unsubscribe_state_event(self, uuid: UUID, callback: Callable[[Device, WappstoMethod], None]) -> None: ...
     def post_state(self, value_uuid: UUID, data: State) -> bool: ...
-    def put_state(self, uuid: UUID, data: State) -> bool: ...
+    def put_bulk_state(self, uuid: UUID, data: List[LogValue]) -> bool: ...
+    def put_state(self, uuid: UUID, data: Union[State, LogValue]) -> bool: ...
     def get_state(self, uuid: UUID) -> Union[State, None]: ...
     def delete_state(self, uuid: UUID) -> bool: ...
```

### Comparing `wappstoiot-0.6.7/wappstoiot/service/template.py` & `wappstoiot-0.6.8/wappstoiot/service/template.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/service/template.pyi` & `wappstoiot-0.6.8/wappstoiot/service/template.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/utils/Timestamp.py` & `wappstoiot-0.6.8/wappstoiot/utils/Timestamp.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/utils/name_check.py` & `wappstoiot-0.6.8/wappstoiot/utils/name_check.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/utils/observer.py` & `wappstoiot-0.6.8/wappstoiot/utils/observer.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/utils/offline_storage.py` & `wappstoiot-0.6.8/wappstoiot/utils/offline_storage.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/utils/offline_storage.pyi` & `wappstoiot-0.6.8/wappstoiot/utils/offline_storage.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/utils/tracer.py` & `wappstoiot-0.6.8/wappstoiot/utils/tracer.py`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot/utils/tracer.pyi` & `wappstoiot-0.6.8/wappstoiot/utils/tracer.pyi`

 * *Files identical despite different names*

### Comparing `wappstoiot-0.6.7/wappstoiot.egg-info/SOURCES.txt` & `wappstoiot-0.6.8/wappstoiot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

