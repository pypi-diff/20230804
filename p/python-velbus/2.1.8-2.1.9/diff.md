# Comparing `tmp/python-velbus-2.1.8.tar.gz` & `tmp/python-velbus-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-velbus-2.1.8.tar", last modified: Mon Nov 21 23:12:41 2022, max compression
+gzip compressed data, was "python-velbus-2.1.9.tar", last modified: Sat Dec 10 09:40:39 2022, max compression
```

## Comparing `python-velbus-2.1.8.tar` & `python-velbus-2.1.9.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-11-21 23:12:41.153652 python-velbus-2.1.8/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1052 2022-11-21 22:55:45.000000 python-velbus-2.1.8/LICENSE
--rw-r--r--   0 thomas    (1000) thomas    (1000)       91 2022-11-21 22:55:45.000000 python-velbus-2.1.8/MANIFEST.in
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7834 2022-11-21 23:12:41.153652 python-velbus-2.1.8/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     6439 2022-11-21 22:55:45.000000 python-velbus-2.1.8/README.md
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-11-21 23:12:41.121652 python-velbus-2.1.8/python_velbus.egg-info/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7834 2022-11-21 23:12:40.000000 python-velbus-2.1.8/python_velbus.egg-info/PKG-INFO
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3203 2022-11-21 23:12:40.000000 python-velbus-2.1.8/python_velbus.egg-info/SOURCES.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2022-11-21 23:12:40.000000 python-velbus-2.1.8/python_velbus.egg-info/dependency_links.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)       14 2022-11-21 23:12:40.000000 python-velbus-2.1.8/python_velbus.egg-info/requires.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)        7 2022-11-21 23:12:40.000000 python-velbus-2.1.8/python_velbus.egg-info/top_level.txt
--rw-r--r--   0 thomas    (1000) thomas    (1000)      515 2022-11-21 23:12:41.157652 python-velbus-2.1.8/setup.cfg
--rw-r--r--   0 thomas    (1000) thomas    (1000)      383 2022-11-21 23:12:35.000000 python-velbus-2.1.8/setup.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-11-21 23:12:41.121652 python-velbus-2.1.8/velbus/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      152 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2837 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/command_registry.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-11-21 23:12:41.125652 python-velbus-2.1.8/velbus/connections/
--rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/connections/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      405 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/connections/connection.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3206 2022-11-21 22:58:39.000000 python-velbus-2.1.8/velbus/connections/serial.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3277 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/connections/socket.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      681 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/constants.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    13355 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/controller.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    11434 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/data.json
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7704 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/message.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-11-21 23:12:41.149652 python-velbus-2.1.8/velbus/messages/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4710 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3746 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/blind_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      835 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/bus_active.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1221 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/bus_error_counter_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      746 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/bus_error_counter_status_request.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      668 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/bus_off.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3532 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/channel_name_part1.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3532 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/channel_name_part2.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3533 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/channel_name_part3.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1757 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/channel_name_request.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      942 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/clear_led.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1676 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/counter_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      900 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/counter_status_request.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3450 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/cover_down.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3002 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/cover_off.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3178 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/cover_position.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3371 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/cover_up.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3116 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/dimmer_channel_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3354 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/dimmer_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      946 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/fast_blinking_led.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      700 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/interface_status_request.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1848 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/kwh_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1094 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/memo_text.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1359 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/memory_data.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1082 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/memory_data_block.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      699 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/memory_dump_request.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1285 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/meteo_raw.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     5864 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/module_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1002 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/module_status_request.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1833 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/module_subtype.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2225 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/module_type.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      767 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/module_type_request.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1914 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/push_button_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1020 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/read_data_block_from_memory.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1018 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/read_data_from_memory.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      858 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/receive_buffer_full.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      682 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/receive_ready.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3383 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/relay_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1743 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/restore_dimmer.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      862 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/sensor_settings_request.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1762 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/sensor_temperature.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1785 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/set_date.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1375 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/set_daylight_saving.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2216 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/set_dimmer.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      928 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/set_led.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1645 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/set_realtime_clock.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      995 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/set_temperature.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1999 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/slider_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      946 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/slow_blinking_led.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1342 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/start_relay_blinking_timer.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1326 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/start_relay_timer.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1411 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/switch_relay_off.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1409 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/switch_relay_on.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      969 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/switch_to_comfort.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      961 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/switch_to_day.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      980 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/switch_to_night.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      963 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/switch_to_safe.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3973 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/temp_sensor_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      895 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/temp_set_cooling.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      895 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/temp_set_heating.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1338 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/update_led_status.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      954 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/very_fast_blinking_led.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1078 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/write_data_to_memory.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1070 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/write_memory_block.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1652 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/messages/write_module_address_and_serial_number.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    10639 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/module.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1614 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/module_registry.py
-drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-11-21 23:12:41.153652 python-velbus-2.1.8/velbus/modules/
--rw-r--r--   0 thomas    (1000) thomas    (1000)      730 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/__init__.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1671 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmb1ts.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3461 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmb4dc.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3418 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmb4ry.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     4405 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmbbl.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3427 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmbdme.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     3523 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmbdmi.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    13151 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmbgp.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7210 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmbin.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1701 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmbiro.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     2069 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmbmeteo.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     6974 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/modules/vmbpbn.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)     7459 2022-11-21 23:12:22.000000 python-velbus-2.1.8/velbus/parser.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)      720 2022-11-21 22:55:45.000000 python-velbus-2.1.8/velbus/util.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-12-10 09:40:39.989929 python-velbus-2.1.9/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1052 2022-12-10 09:04:54.000000 python-velbus-2.1.9/LICENSE
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       91 2022-12-10 09:04:54.000000 python-velbus-2.1.9/MANIFEST.in
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7834 2022-12-10 09:40:39.989929 python-velbus-2.1.9/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     6439 2022-12-10 09:04:54.000000 python-velbus-2.1.9/README.md
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-12-10 09:40:39.977929 python-velbus-2.1.9/python_velbus.egg-info/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7834 2022-12-10 09:40:39.000000 python-velbus-2.1.9/python_velbus.egg-info/PKG-INFO
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3203 2022-12-10 09:40:39.000000 python-velbus-2.1.9/python_velbus.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        1 2022-12-10 09:40:39.000000 python-velbus-2.1.9/python_velbus.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)       14 2022-12-10 09:40:39.000000 python-velbus-2.1.9/python_velbus.egg-info/requires.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        7 2022-12-10 09:40:39.000000 python-velbus-2.1.9/python_velbus.egg-info/top_level.txt
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      515 2022-12-10 09:40:39.989929 python-velbus-2.1.9/setup.cfg
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      383 2022-12-10 09:40:22.000000 python-velbus-2.1.9/setup.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-12-10 09:40:39.981929 python-velbus-2.1.9/velbus/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      152 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2837 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/command_registry.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-12-10 09:40:39.981929 python-velbus-2.1.9/velbus/connections/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)        0 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/connections/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      405 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/connections/connection.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3383 2022-12-10 09:08:28.000000 python-velbus-2.1.9/velbus/connections/serial.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3277 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/connections/socket.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      681 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/constants.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    13355 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/controller.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    11434 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/data.json
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7704 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/message.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-12-10 09:40:39.985929 python-velbus-2.1.9/velbus/messages/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4710 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3746 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/blind_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      835 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/bus_active.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1221 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/bus_error_counter_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      746 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/bus_error_counter_status_request.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      668 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/bus_off.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3532 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/channel_name_part1.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3532 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/channel_name_part2.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3533 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/channel_name_part3.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1757 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/channel_name_request.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      942 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/clear_led.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1676 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/counter_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      900 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/counter_status_request.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3450 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/cover_down.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3002 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/cover_off.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3178 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/cover_position.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3371 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/cover_up.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3116 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/dimmer_channel_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3354 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/dimmer_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      946 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/fast_blinking_led.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      700 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/interface_status_request.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1848 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/kwh_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1094 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/memo_text.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1359 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/memory_data.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1082 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/memory_data_block.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      699 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/memory_dump_request.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1285 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/meteo_raw.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     5864 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/module_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1002 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/module_status_request.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1833 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/module_subtype.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2225 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/module_type.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      767 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/module_type_request.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1914 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/push_button_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1020 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/read_data_block_from_memory.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1018 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/read_data_from_memory.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      858 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/receive_buffer_full.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      682 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/receive_ready.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3383 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/relay_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1743 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/restore_dimmer.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      862 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/sensor_settings_request.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1762 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/sensor_temperature.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1785 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/set_date.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1375 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/set_daylight_saving.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2216 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/set_dimmer.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      928 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/set_led.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1645 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/set_realtime_clock.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      995 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/set_temperature.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1999 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/slider_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      946 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/slow_blinking_led.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1342 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/start_relay_blinking_timer.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1326 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/start_relay_timer.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1411 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/switch_relay_off.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1409 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/switch_relay_on.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      969 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/switch_to_comfort.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      961 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/switch_to_day.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      980 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/switch_to_night.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      963 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/switch_to_safe.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3973 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/temp_sensor_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      895 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/temp_set_cooling.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      895 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/temp_set_heating.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1338 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/update_led_status.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      954 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/very_fast_blinking_led.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1078 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/write_data_to_memory.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1070 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/write_memory_block.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1652 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/messages/write_module_address_and_serial_number.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    10639 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/module.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1614 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/module_registry.py
+drwxr-xr-x   0 thomas    (1000) thomas    (1000)        0 2022-12-10 09:40:39.989929 python-velbus-2.1.9/velbus/modules/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      730 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/__init__.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1671 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmb1ts.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3461 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmb4dc.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3418 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmb4ry.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     4405 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmbbl.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3427 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmbdme.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     3523 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmbdmi.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    13151 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmbgp.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7210 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmbin.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1701 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmbiro.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     2069 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmbmeteo.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     6974 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/modules/vmbpbn.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     7459 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/parser.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)      720 2022-12-10 09:04:54.000000 python-velbus-2.1.9/velbus/util.py
```

### Comparing `python-velbus-2.1.8/LICENSE` & `python-velbus-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/PKG-INFO` & `python-velbus-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-velbus
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python Library for the Velbus protocol
 Home-page: https://github.com/thomasdelaet/python-velbus
 Author: Thomas Delaet
 Author-email: thomas@delaet.org
 License: MIT
 Description: ## python-velbus: A python library to control the Velbus home automation system
```

### Comparing `python-velbus-2.1.8/README.md` & `python-velbus-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/python_velbus.egg-info/PKG-INFO` & `python-velbus-2.1.9/python_velbus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-velbus
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python Library for the Velbus protocol
 Home-page: https://github.com/thomasdelaet/python-velbus
 Author: Thomas Delaet
 Author-email: thomas@delaet.org
 License: MIT
 Description: ## python-velbus: A python library to control the Velbus home automation system
```

### Comparing `python-velbus-2.1.8/python_velbus.egg-info/SOURCES.txt` & `python-velbus-2.1.9/python_velbus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/setup.cfg` & `python-velbus-2.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/command_registry.py` & `python-velbus-2.1.9/velbus/command_registry.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/connections/serial.py` & `python-velbus-2.1.9/velbus/connections/serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 from queue import Queue
 import serial
 import serial.threaded
 from velbus.connections.connection import VelbusConnection
 from velbus.util import VelbusException
 from velbus.message import Message
 from velbus.constants import SLEEP_TIME
+import sys
 
 
 class Protocol(serial.threaded.Protocol):
     """Serial protocol."""
 
     def data_received(self, data):
         # pylint: disable-msg=E1101
         self.parser(data)
 
     def connection_lost(self, exc):
+        print('connection lost')
+        sys.exit(1)
         raise exc
 
 class VelbusUSBConnection(VelbusConnection):
     """
     Wrapper for SerialPort connection configuration
     """
 
@@ -94,11 +97,15 @@
 
     def write_daemon(self):
         """Write thread."""
         while True:
             (message, callback) = self._write_queue.get(block=True)
             self.logger.info("Sending message on USB bus: %s", str(message))
             self.logger.debug("Sending binary message:  %s", str(message.to_binary()))
-            self._reader.write(message.to_binary())
+            try:
+                self._reader.write(message.to_binary())
+            except Exception as exc:
+                print(exc)
+                sys.exit(1)
             time.sleep(SLEEP_TIME)
             if callback:
                 callback()
```

### Comparing `python-velbus-2.1.8/velbus/connections/socket.py` & `python-velbus-2.1.9/velbus/connections/socket.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/constants.py` & `python-velbus-2.1.9/velbus/constants.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/controller.py` & `python-velbus-2.1.9/velbus/controller.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/data.json` & `python-velbus-2.1.9/velbus/data.json`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/message.py` & `python-velbus-2.1.9/velbus/message.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/__init__.py` & `python-velbus-2.1.9/velbus/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/blind_status.py` & `python-velbus-2.1.9/velbus/messages/blind_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/bus_active.py` & `python-velbus-2.1.9/velbus/messages/bus_active.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/bus_error_counter_status.py` & `python-velbus-2.1.9/velbus/messages/bus_error_counter_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/bus_error_counter_status_request.py` & `python-velbus-2.1.9/velbus/messages/bus_error_counter_status_request.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/bus_off.py` & `python-velbus-2.1.9/velbus/messages/bus_off.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/channel_name_part1.py` & `python-velbus-2.1.9/velbus/messages/channel_name_part1.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/channel_name_part2.py` & `python-velbus-2.1.9/velbus/messages/channel_name_part2.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/channel_name_part3.py` & `python-velbus-2.1.9/velbus/messages/channel_name_part3.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/channel_name_request.py` & `python-velbus-2.1.9/velbus/messages/channel_name_request.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/clear_led.py` & `python-velbus-2.1.9/velbus/messages/clear_led.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/counter_status.py` & `python-velbus-2.1.9/velbus/messages/counter_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/counter_status_request.py` & `python-velbus-2.1.9/velbus/messages/counter_status_request.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/cover_down.py` & `python-velbus-2.1.9/velbus/messages/cover_down.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/cover_off.py` & `python-velbus-2.1.9/velbus/messages/cover_off.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/cover_position.py` & `python-velbus-2.1.9/velbus/messages/cover_position.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/cover_up.py` & `python-velbus-2.1.9/velbus/messages/cover_up.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/dimmer_channel_status.py` & `python-velbus-2.1.9/velbus/messages/dimmer_channel_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/dimmer_status.py` & `python-velbus-2.1.9/velbus/messages/dimmer_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/fast_blinking_led.py` & `python-velbus-2.1.9/velbus/messages/fast_blinking_led.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/interface_status_request.py` & `python-velbus-2.1.9/velbus/messages/interface_status_request.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/kwh_status.py` & `python-velbus-2.1.9/velbus/messages/kwh_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/memo_text.py` & `python-velbus-2.1.9/velbus/messages/memo_text.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/memory_data.py` & `python-velbus-2.1.9/velbus/messages/memory_data.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/memory_data_block.py` & `python-velbus-2.1.9/velbus/messages/memory_data_block.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/memory_dump_request.py` & `python-velbus-2.1.9/velbus/messages/memory_dump_request.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/meteo_raw.py` & `python-velbus-2.1.9/velbus/messages/meteo_raw.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/module_status.py` & `python-velbus-2.1.9/velbus/messages/module_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/module_status_request.py` & `python-velbus-2.1.9/velbus/messages/module_status_request.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/module_subtype.py` & `python-velbus-2.1.9/velbus/messages/module_subtype.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/module_type.py` & `python-velbus-2.1.9/velbus/messages/module_type.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/module_type_request.py` & `python-velbus-2.1.9/velbus/messages/module_type_request.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/push_button_status.py` & `python-velbus-2.1.9/velbus/messages/push_button_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/read_data_block_from_memory.py` & `python-velbus-2.1.9/velbus/messages/read_data_block_from_memory.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/read_data_from_memory.py` & `python-velbus-2.1.9/velbus/messages/read_data_from_memory.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/receive_buffer_full.py` & `python-velbus-2.1.9/velbus/messages/receive_buffer_full.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/receive_ready.py` & `python-velbus-2.1.9/velbus/messages/receive_ready.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/relay_status.py` & `python-velbus-2.1.9/velbus/messages/relay_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/restore_dimmer.py` & `python-velbus-2.1.9/velbus/messages/restore_dimmer.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/sensor_settings_request.py` & `python-velbus-2.1.9/velbus/messages/sensor_settings_request.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/sensor_temperature.py` & `python-velbus-2.1.9/velbus/messages/sensor_temperature.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/set_date.py` & `python-velbus-2.1.9/velbus/messages/set_date.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/set_daylight_saving.py` & `python-velbus-2.1.9/velbus/messages/set_daylight_saving.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/set_dimmer.py` & `python-velbus-2.1.9/velbus/messages/set_dimmer.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/set_led.py` & `python-velbus-2.1.9/velbus/messages/set_led.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/set_realtime_clock.py` & `python-velbus-2.1.9/velbus/messages/set_realtime_clock.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/set_temperature.py` & `python-velbus-2.1.9/velbus/messages/set_temperature.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/slider_status.py` & `python-velbus-2.1.9/velbus/messages/slider_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/slow_blinking_led.py` & `python-velbus-2.1.9/velbus/messages/slow_blinking_led.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/start_relay_blinking_timer.py` & `python-velbus-2.1.9/velbus/messages/start_relay_blinking_timer.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/start_relay_timer.py` & `python-velbus-2.1.9/velbus/messages/start_relay_timer.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/switch_relay_off.py` & `python-velbus-2.1.9/velbus/messages/switch_relay_off.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/switch_relay_on.py` & `python-velbus-2.1.9/velbus/messages/switch_relay_on.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/switch_to_comfort.py` & `python-velbus-2.1.9/velbus/messages/switch_to_comfort.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/switch_to_day.py` & `python-velbus-2.1.9/velbus/messages/switch_to_day.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/switch_to_night.py` & `python-velbus-2.1.9/velbus/messages/switch_to_night.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/switch_to_safe.py` & `python-velbus-2.1.9/velbus/messages/switch_to_safe.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/temp_sensor_status.py` & `python-velbus-2.1.9/velbus/messages/temp_sensor_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/temp_set_cooling.py` & `python-velbus-2.1.9/velbus/messages/temp_set_cooling.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/temp_set_heating.py` & `python-velbus-2.1.9/velbus/messages/temp_set_heating.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/update_led_status.py` & `python-velbus-2.1.9/velbus/messages/update_led_status.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/very_fast_blinking_led.py` & `python-velbus-2.1.9/velbus/messages/very_fast_blinking_led.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/write_data_to_memory.py` & `python-velbus-2.1.9/velbus/messages/write_data_to_memory.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/write_memory_block.py` & `python-velbus-2.1.9/velbus/messages/write_memory_block.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/messages/write_module_address_and_serial_number.py` & `python-velbus-2.1.9/velbus/messages/write_module_address_and_serial_number.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/module.py` & `python-velbus-2.1.9/velbus/module.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/module_registry.py` & `python-velbus-2.1.9/velbus/module_registry.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/__init__.py` & `python-velbus-2.1.9/velbus/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmb1ts.py` & `python-velbus-2.1.9/velbus/modules/vmb1ts.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmb4dc.py` & `python-velbus-2.1.9/velbus/modules/vmb4dc.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmb4ry.py` & `python-velbus-2.1.9/velbus/modules/vmb4ry.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmbbl.py` & `python-velbus-2.1.9/velbus/modules/vmbbl.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmbdme.py` & `python-velbus-2.1.9/velbus/modules/vmbdme.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmbdmi.py` & `python-velbus-2.1.9/velbus/modules/vmbdmi.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmbgp.py` & `python-velbus-2.1.9/velbus/modules/vmbgp.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmbin.py` & `python-velbus-2.1.9/velbus/modules/vmbin.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmbiro.py` & `python-velbus-2.1.9/velbus/modules/vmbiro.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmbmeteo.py` & `python-velbus-2.1.9/velbus/modules/vmbmeteo.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/modules/vmbpbn.py` & `python-velbus-2.1.9/velbus/modules/vmbpbn.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/parser.py` & `python-velbus-2.1.9/velbus/parser.py`

 * *Files identical despite different names*

### Comparing `python-velbus-2.1.8/velbus/util.py` & `python-velbus-2.1.9/velbus/util.py`

 * *Files identical despite different names*

