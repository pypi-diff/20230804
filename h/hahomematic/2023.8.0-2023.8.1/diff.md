# Comparing `tmp/hahomematic-2023.8.0.tar.gz` & `tmp/hahomematic-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.8.0.tar", last modified: Mon Jul 31 17:34:42 2023, max compression
+gzip compressed data, was "hahomematic-2023.8.1.tar", last modified: Fri Aug  4 15:39:34 2023, max compression
```

## Comparing `hahomematic-2023.8.0.tar` & `hahomematic-2023.8.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.481857 hahomematic-2023.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-31 17:34:42.481857 hahomematic-2023.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.473857 hahomematic-2023.8.0/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.473857 hahomematic-2023.8.0/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    55163 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    48392 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.477857 hahomematic-2023.8.0/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.477857 hahomematic-2023.8.0/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.477857 hahomematic-2023.8.0/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.481857 hahomematic-2023.8.0/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/platforms/update.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.481857 hahomematic-2023.8.0/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:34:42.473857 hahomematic-2023.8.0/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-31 17:34:41.000000 hahomematic-2023.8.0/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-31 17:34:42.000000 hahomematic-2023.8.0/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:34:41.000000 hahomematic-2023.8.0/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:34:40.000000 hahomematic-2023.8.0/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 17:34:42.000000 hahomematic-2023.8.0/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 17:34:42.000000 hahomematic-2023.8.0/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-07-31 17:34:08.000000 hahomematic-2023.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-31 17:34:42.481857 hahomematic-2023.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.599002 hahomematic-2023.8.1/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.599002 hahomematic-2023.8.1/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16932 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55112 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48499 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23747 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27916 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11421 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34405 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/platforms/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:39:34.599002 hahomematic-2023.8.1/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-08-04 15:39:33.000000 hahomematic-2023.8.1/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-08-04 15:39:34.000000 hahomematic-2023.8.1/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:39:34.000000 hahomematic-2023.8.1/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:39:32.000000 hahomematic-2023.8.1/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-04 15:39:34.000000 hahomematic-2023.8.1/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 15:39:34.000000 hahomematic-2023.8.1/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17264 2023-08-04 15:39:07.000000 hahomematic-2023.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 15:39:34.603002 hahomematic-2023.8.1/setup.cfg
```

### Comparing `hahomematic-2023.8.0/LICENSE` & `hahomematic-2023.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/PKG-INFO` & `hahomematic-2023.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.8.0
+Version: 2023.8.1
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.8.0/README.md` & `hahomematic-2023.8.1/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/__init__.py` & `hahomematic-2023.8.1/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/caches/dynamic.py` & `hahomematic-2023.8.1/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/caches/persistent.py` & `hahomematic-2023.8.1/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/caches/visibility.py` & `hahomematic-2023.8.1/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/central_unit.py` & `hahomematic-2023.8.1/hahomematic/central_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 from hahomematic.caches.persistent import (
     DeviceDescriptionCache,
     ParamsetDescriptionCache,
 )
 from hahomematic.caches.visibility import ParameterVisibilityCache
 from hahomematic.config import PING_PONG_MISMATCH_COUNT
 from hahomematic.const import (
+    ATTR_AVAILABLE,
+    ATTR_DATA,
+    ATTR_INSTANCE_NAME,
     ATTR_INTERFACE_ID,
-    ATTR_MESSAGE,
     ATTR_TYPE,
-    ATTR_VALUE,
     DEFAULT_TLS,
     DEFAULT_VERIFY_TLS,
     EVENT_PONG,
     HH_EVENT_DELETE_DEVICES,
     HH_EVENT_DEVICES_CREATED,
     HH_EVENT_LIST_DEVICES,
     HH_EVENT_NEW_DEVICES,
@@ -392,24 +393,22 @@
                     _LOGGER.debug(
                         "CREATE_CLIENTS: Adding client %s to %s",
                         client.interface_id,
                         self._attr_name,
                     )
                     self._clients[client.interface_id] = client
             except BaseHomematicException as ex:
-                message = f"No connection to interface {interface_config.interface_id}"
                 self.fire_interface_event(
                     interface_id=interface_config.interface_id,
                     interface_event_type=HmInterfaceEventType.PROXY,
-                    message=message,
-                    available=False,
+                    data={ATTR_AVAILABLE: False},
                 )
                 _LOGGER.warning(
-                    "CREATE_CLIENTS failed: %s [%s]",
-                    message,
+                    "CREATE_CLIENTS failed: No connection to interface %s [%s]",
+                    interface_config.interface_id,
                     ex.args,
                 )
 
         if self.has_clients:
             _LOGGER.debug(
                 "CREATE_CLIENTS: All clients successfully created for %s",
                 self._attr_name,
@@ -436,23 +435,22 @@
         await self._hub.fetch_program_data()
         await self._hub.fetch_sysvar_data()
 
     def fire_interface_event(
         self,
         interface_id: str,
         interface_event_type: HmInterfaceEventType,
-        message: str,
-        available: bool,
+        data: dict[str, Any] | None = None,
     ) -> None:
         """Fire an event about the interface status."""
+        data = data or {}
         event_data: dict[str, Any] = {
             ATTR_INTERFACE_ID: interface_id,
             ATTR_TYPE: interface_event_type,
-            ATTR_MESSAGE: message,
-            ATTR_VALUE: available,
+            ATTR_DATA: data,
         }
 
         self.fire_ha_event_callback(
             event_type=HmEventType.INTERFACE,
             event_data=cast(dict[str, Any], HM_INTERFACE_EVENT_SCHEMA(event_data)),
         )
 
@@ -894,30 +892,30 @@
                 else:
                     self._ping_count[interface_id] = 0
 
     def _fire_ping_pong_event(self, interface_id: str) -> None:
         """Fire an event about the ping pong status."""
         if self._ping_pong_fired:
             return
-        message = (
-            f"There is a mismatch between send ping events and received pong events for HA instance {self.config.name}. "
-            f"Possible reason 1: You are running multiple instances of HA with the same instance name configured for this integration. "
-            f"Re-add one instance! Otherwise one HA instance will not receive update events from your CCU. "
-            f"Possible reason 2: Something is stuck on CCU, so try a restart."
-        )
         event_data: dict[str, Any] = {
             ATTR_INTERFACE_ID: interface_id,
             ATTR_TYPE: HmInterfaceEventType.PINGPONG,
-            ATTR_MESSAGE: message,
+            ATTR_DATA: {ATTR_INSTANCE_NAME: self.config.name},
         }
         self.fire_ha_event_callback(
             event_type=HmEventType.INTERFACE,
             event_data=cast(dict[str, Any], HM_INTERFACE_EVENT_SCHEMA(event_data)),
         )
-        _LOGGER.warning("PING/PONG MISMATCH: %s", message)
+        _LOGGER.warning(
+            "PING/PONG MISMATCH: There is a mismatch between send ping events and received pong events for HA instance %s. "
+            "Possible reason 1: You are running multiple instances of HA with the same instance name configured for this integration. "
+            "Re-add one instance! Otherwise one HA instance will not receive update events from your CCU. "
+            "Possible reason 2: Something is stuck on CCU, so try a restart.",
+            self.config.name,
+        )
         self._ping_pong_fired = True
 
     def create_task(self, target: Awaitable, name: str) -> None:
         """Add task to the executor pool."""
         try:
             self._loop.call_soon_threadsafe(self._async_create_task, target, name)
         except CancelledError:
```

### Comparing `hahomematic-2023.8.0/hahomematic/client.py` & `hahomematic-2023.8.1/hahomematic/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 
 import orjson
 
 from hahomematic import central_unit as hmcu
 from hahomematic.config import CALLBACK_WARN_INTERVAL, RECONNECT_WAIT
 from hahomematic.const import (
     ATTR_ADDRESS,
+    ATTR_AVAILABLE,
     ATTR_CHANNELS,
     ATTR_ID,
     ATTR_INTERFACE,
     ATTR_NAME,
+    ATTR_SECONDS_SINCE_LAST_EVENT,
     BACKEND_CCU,
     BACKEND_HOMEGEAR,
     BACKEND_LOCAL,
     BACKEND_PYDEVCCU,
     DEFAULT_ENCODING,
     HM_ADDRESS,
     HM_NAME,
@@ -172,20 +174,18 @@
                     device.set_forced_availability(forced_availability=forced_availability)
             self._attr_available = available
             _LOGGER.debug(
                 "MARK_ALL_DEVICES_FORCED_AVAILABILITY: marked all devices %s for %s",
                 "available" if available else "unavailable",
                 self.interface_id,
             )
-        message = f"No connection to interface {self.interface_id}"
         self.central.fire_interface_event(
             interface_id=self.interface_id,
             interface_event_type=HmInterfaceEventType.PROXY,
-            message=message,
-            available=available,
+            data={ATTR_AVAILABLE: available},
         )
 
     async def reconnect(self) -> bool:
         """re-init all RPC clients."""
         if await self.is_connected():
             _LOGGER.debug(
                 "RECONNECT: waiting to re-connect client %s for %is",
@@ -238,32 +238,36 @@
         return False
 
     def is_callback_alive(self) -> bool:
         """Return if XmlRPC-Server is alive based on received events for this client."""
         if last_events_time := self.central.last_events.get(self.interface_id):
             seconds_since_last_event = (datetime.now() - last_events_time).total_seconds()
             if seconds_since_last_event > CALLBACK_WARN_INTERVAL:
-                message = f"Callback for {self.interface_id} has not received events for {seconds_since_last_event:.0f}s"
                 if self._is_callback_alive:
                     self.central.fire_interface_event(
                         interface_id=self.interface_id,
                         interface_event_type=HmInterfaceEventType.CALLBACK,
-                        message=message,
-                        available=False,
+                        data={
+                            ATTR_AVAILABLE: False,
+                            ATTR_SECONDS_SINCE_LAST_EVENT: int(seconds_since_last_event),
+                        },
                     )
                     self._is_callback_alive = False
-                _LOGGER.warning("IS_CALLBACK_ALIVE: %s", message)
+                _LOGGER.warning(
+                    "IS_CALLBACK_ALIVE: Callback for %s has not received events for %is",
+                    self.interface_id,
+                    seconds_since_last_event,
+                )
                 return False
 
             if not self._is_callback_alive:
                 self.central.fire_interface_event(
                     interface_id=self.interface_id,
                     interface_event_type=HmInterfaceEventType.CALLBACK,
-                    message="",
-                    available=True,
+                    data={ATTR_AVAILABLE: True},
                 )
                 self._is_callback_alive = True
         return True
 
     @abstractmethod
     async def check_connection_availability(self) -> bool:
         """Send ping to CCU to generate PONG event."""
```

### Comparing `hahomematic-2023.8.0/hahomematic/const.py` & `hahomematic-2023.8.1/hahomematic/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,35 +41,39 @@
 LOCAL_INTERFACE = "Local"
 LOCAL_SERIAL: Final = "0815_4711"
 
 PROGRAM_ADDRESS: Final = "program"
 SYSVAR_ADDRESS: Final = "sysvar"
 
 ATTR_ADDRESS: Final = "address"
+ATTR_AVAILABLE: Final = "available"
 ATTR_CALLBACK_HOST: Final = "callback_host"
 ATTR_CALLBACK_PORT: Final = "callback_port"
 ATTR_CHANNELS: Final = "channels"
 ATTR_CHANNEL_NO: Final = "channel_no"
 ATTR_CONFIG: Final = "config"
+ATTR_DATA: Final = "data"
 ATTR_DEVICE_TYPE: Final = "device_type"
 ATTR_FIRMWARE: Final = "firmware"
 ATTR_HOST: Final = "host"
 ATTR_ID: Final = "id"
+ATTR_INSTANCE_NAME: Final = "instance_name"
 ATTR_INTERFACE: Final = "interface"
 ATTR_INTERFACE_ID: Final = "interface_id"
 ATTR_IP: Final = "ip"
 ATTR_JSON_PORT: Final = "json_port"
 ATTR_MESSAGE: Final = "message"
 ATTR_MODEL: Final = "model"
 ATTR_NAME: Final = "name"
 ATTR_PARAMETER: Final = "parameter"
 ATTR_PARAMSET_KEY: Final = "paramsetKey"
 ATTR_PASSWORD: Final = "password"
 ATTR_PORT: Final = "port"
 ATTR_ROOM: Final = "room"
+ATTR_SECONDS_SINCE_LAST_EVENT: Final = "seconds_since_last_event"
 ATTR_TLS: Final = "tls"
 ATTR_TYPE: Final = "type"
 ATTR_USERNAME: Final = "username"
 ATTR_VALUE: Final = "value"
 ATTR_VALUE_KEY: Final = "valueKey"
 ATTR_VERIFY_TLS: Final = "verify_tls"
```

### Comparing `hahomematic-2023.8.0/hahomematic/decorators.py` & `hahomematic-2023.8.1/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/exceptions.py` & `hahomematic-2023.8.1/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/exporter.py` & `hahomematic-2023.8.1/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/hmcli.py` & `hahomematic-2023.8.1/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/json_rpc_client.py` & `hahomematic-2023.8.1/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/__init__.py` & `hahomematic-2023.8.1/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/const.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/cover.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/light.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/support.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.8.1/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/device.py` & `hahomematic-2023.8.1/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/entity.py` & `hahomematic-2023.8.1/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/event.py` & `hahomematic-2023.8.1/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.8.1/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/generic/action.py` & `hahomematic-2023.8.1/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.8.1/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/generic/button.py` & `hahomematic-2023.8.1/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.8.1/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/generic/number.py` & `hahomematic-2023.8.1/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/generic/select.py` & `hahomematic-2023.8.1/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.8.1/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.8.1/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.8.1/hahomematic/platforms/hub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         """Identify missing variables."""
         variable_names: dict[str, bool] = {x.name: x.extended_sysvar for x in variables}
         missing_variables: set[str] = set()
         for sysvar_entity in self._central.sysvar_entities.values():
             if sysvar_entity.data_type == SYSVAR_TYPE_STRING:
                 continue
             ccu_name = sysvar_entity.ccu_var_name
-            if ccu_name not in variable_names.keys() or (
+            if ccu_name not in variable_names or (
                 sysvar_entity.is_extended is not variable_names.get(ccu_name)
             ):
                 missing_variables.add(ccu_name)
         return missing_variables
 
 
 def _is_excluded(variable: str, excludes: list[str]) -> bool:
```

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.8.1/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/hub/button.py` & `hahomematic-2023.8.1/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.8.1/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/hub/number.py` & `hahomematic-2023.8.1/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/hub/select.py` & `hahomematic-2023.8.1/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.8.1/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/hub/text.py` & `hahomematic-2023.8.1/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/support.py` & `hahomematic-2023.8.1/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/platforms/update.py` & `hahomematic-2023.8.1/hahomematic/platforms/update.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.8.1/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.8.1/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.8.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/support.py` & `hahomematic-2023.8.1/hahomematic/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 import socket
 import ssl
 from typing import Any
 
 import voluptuous as vol
 
 from hahomematic.const import (
+    ATTR_DATA,
     ATTR_INTERFACE_ID,
-    ATTR_MESSAGE,
     ATTR_TYPE,
-    ATTR_VALUE,
     CCU_PASSWORD_PATTERN,
     FILE_DEVICES,
     FILE_PARAMSETS,
     INIT_DATETIME,
     SYSVAR_HM_TYPE_FLOAT,
     SYSVAR_HM_TYPE_INTEGER,
     SYSVAR_TYPE_ALARM,
@@ -37,16 +36,17 @@
 _LOGGER = logging.getLogger(__name__)
 
 
 HM_INTERFACE_EVENT_SCHEMA = vol.Schema(
     {
         vol.Required(ATTR_INTERFACE_ID): str,
         vol.Required(ATTR_TYPE): HmInterfaceEventType,
-        vol.Required(ATTR_MESSAGE): str,
-        vol.Optional(ATTR_VALUE): bool,
+        vol.Required(ATTR_DATA): vol.Schema(
+            {vol.Required(vol.Any(str)): vol.Schema(vol.Any(str, int, bool))}
+        ),
     }
 )
 
 
 def build_xml_rpc_uri(
     host: str,
     port: int,
```

### Comparing `hahomematic-2023.8.0/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.8.1/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic/xml_rpc_server.py` & `hahomematic-2023.8.1/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.8.1/hahomematic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.8.0
+Version: 2023.8.1
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.8.0/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.8.1/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.8.0/pyproject.toml` & `hahomematic-2023.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.8.0"
+version     = "2023.8.1"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

