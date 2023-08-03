# Comparing `tmp/redvox-3.5.2.tar.gz` & `tmp/redvox-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvox-3.5.2.tar", last modified: Tue Aug  1 19:46:05 2023, max compression
+gzip compressed data, was "redvox-3.6.0.tar", last modified: Thu Aug  3 22:25:44 2023, max compression
```

## Comparing `redvox-3.5.2.tar` & `redvox-3.6.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.417007 redvox-3.5.2/
--rw-r--r--   0 opq       (1000) opq       (1000)    11343 2023-04-28 19:34:15.000000 redvox-3.5.2/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    13906 2023-08-01 19:46:05.417007 redvox-3.5.2/PKG-INFO
--rw-rw-r--   0 opq       (1000) opq       (1000)      517 2021-06-14 20:37:56.000000 redvox-3.5.2/README.md
--rw-r--r--   0 opq       (1000) opq       (1000)     1470 2023-08-01 19:44:44.000000 redvox-3.5.2/pyproject.toml
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.215010 redvox-3.5.2/redvox/
--rw-r--r--   0 opq       (1000) opq       (1000)      728 2023-08-01 19:42:06.000000 redvox-3.5.2/redvox/__init__.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.216010 redvox-3.5.2/redvox/api1000/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/__init__.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.225010 redvox-3.5.2/redvox/api1000/common/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/common/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    20204 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/common/common.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1050 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/common/decorators.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5359 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/common/generic.py
--rw-r--r--   0 opq       (1000) opq       (1000)      875 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/common/lz4.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2570 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/common/mapping.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2237 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/common/metadata.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2435 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/common/typing.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2114 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/errors.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.226010 redvox-3.5.2/redvox/api1000/gui/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/gui/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4672 2021-04-14 19:22:20.000000 redvox-3.5.2/redvox/api1000/gui/image_viewer.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.226010 redvox-3.5.2/redvox/api1000/proto/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/proto/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    39434 2023-05-25 20:50:49.000000 redvox-3.5.2/redvox/api1000/proto/redvox_api_m_pb2.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.231010 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5639 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/event_streams.py
--rw-r--r--   0 opq       (1000) opq       (1000)    10817 2023-08-01 19:02:37.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/ml.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.269009 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    11949 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.270009 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14890 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
--rw-r--r--   0 opq       (1000) opq       (1000)     7398 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/image.py
--rw-r--r--   0 opq       (1000) opq       (1000)    40936 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/location.py
--rw-r--r--   0 opq       (1000) opq       (1000)    42236 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3425 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/single.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5576 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    50437 2022-04-19 20:47:15.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/station_information.py
--rw-r--r--   0 opq       (1000) opq       (1000)    19060 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/timing_information.py
--rw-r--r--   0 opq       (1000) opq       (1000)    21971 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.345008 redvox-3.5.2/redvox/api900/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    17514 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/concat.py
--rw-r--r--   0 opq       (1000) opq       (1000)      494 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/constants.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1689 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/deprecation.py
--rw-r--r--   0 opq       (1000) opq       (1000)      351 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/exceptions.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.346008 redvox-3.5.2/redvox/api900/lib/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/lib/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     7591 2023-05-25 20:50:49.000000 redvox-3.5.2/redvox/api900/lib/api900_pb2.py
--rw-r--r--   0 opq       (1000) opq       (1000)    43091 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/location_analyzer.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2597 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/migrations.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.347008 redvox-3.5.2/redvox/api900/qa/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/qa/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2813 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/qa/gap_detection.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16939 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/reader.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    17096 2021-06-07 23:35:09.000000 redvox-3.5.2/redvox/api900/reader_utils.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.364008 redvox-3.5.2/redvox/api900/sensors/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2113 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/accelerometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2298 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/barometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2665 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/evenly_sampled_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     6283 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/evenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1989 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/gyroscope_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4854 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/image_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2264 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/infrared_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16540 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/interleaved_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2261 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/light_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)    10051 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/location_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2022 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/magnetometer_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3209 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/microphone_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4655 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/time_synchronization_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3536 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/unevenly_sampled_channel.py
--rw-r--r--   0 opq       (1000) opq       (1000)     6619 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/unevenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5907 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1128 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/stat_utils.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8780 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/summarize.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.365008 redvox-3.5.2/redvox/api900/timesync/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/timesync/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    27606 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/timesync/api900_timesync.py
--rw-r--r--   0 opq       (1000) opq       (1000)    13824 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/timesync/tri_message_stats.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1537 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/types.py
--rw-r--r--   0 opq       (1000) opq       (1000)    54392 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/api900/wrapped_redvox_packet.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.366008 redvox-3.5.2/redvox/cli/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/cli/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    22678 2021-04-14 19:22:20.000000 redvox-3.5.2/redvox/cli/cli.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6683 2021-06-07 23:35:09.000000 redvox-3.5.2/redvox/cli/conversions.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1797 2021-04-14 19:22:20.000000 redvox-3.5.2/redvox/cli/data_req.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.397007 redvox-3.5.2/redvox/cloud/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/cloud/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     2267 2023-06-06 22:12:01.000000 redvox-3.5.2/redvox/cloud/api.py
--rw-r--r--   0 opq       (1000) opq       (1000)   142063 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/cloud/api_m_fqns.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4334 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/cloud/auth_api.py
--rw-r--r--   0 opq       (1000) opq       (1000)    29429 2023-08-01 19:02:37.000000 redvox-3.5.2/redvox/cloud/client.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5905 2021-09-16 19:39:56.000000 redvox-3.5.2/redvox/cloud/config.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6088 2021-04-14 19:22:20.000000 redvox-3.5.2/redvox/cloud/data_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3829 2021-09-16 19:39:56.000000 redvox-3.5.2/redvox/cloud/data_client.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3266 2023-08-01 19:02:37.000000 redvox-3.5.2/redvox/cloud/data_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)      487 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/cloud/errors.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    18946 2022-04-20 20:36:13.000000 redvox-3.5.2/redvox/cloud/metadata_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3770 2021-04-14 23:45:25.000000 redvox-3.5.2/redvox/cloud/query_timing_correction.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1086 2023-08-01 19:02:37.000000 redvox-3.5.2/redvox/cloud/routes.py
--rw-r--r--   0 opq       (1000) opq       (1000)    10985 2023-08-01 19:02:37.000000 redvox-3.5.2/redvox/cloud/session_model_api.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4262 2021-04-14 23:45:25.000000 redvox-3.5.2/redvox/cloud/station_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     7707 2022-06-01 22:08:00.000000 redvox-3.5.2/redvox/cloud/subscription.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.409007 redvox-3.5.2/redvox/common/
--rw-r--r--   0 opq       (1000) opq       (1000)      195 2021-03-29 23:26:30.000000 redvox-3.5.2/redvox/common/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    55240 2022-09-30 02:01:56.000000 redvox-3.5.2/redvox/common/api_conversions.py
--rw-r--r--   0 opq       (1000) opq       (1000)    23894 2023-08-01 19:02:37.000000 redvox-3.5.2/redvox/common/api_reader.py
--rw-r--r--   0 opq       (1000) opq       (1000)     5249 2023-08-01 19:02:37.000000 redvox-3.5.2/redvox/common/api_reader_dw.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1173 2021-04-20 02:39:13.000000 redvox-3.5.2/redvox/common/constants.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4126 2021-07-07 20:00:14.000000 redvox-3.5.2/redvox/common/cross_stats.py
--rw-r--r--   0 opq       (1000) opq       (1000)    42995 2023-08-01 19:02:37.000000 redvox-3.5.2/redvox/common/data_window.py
--rw-r--r--   0 opq       (1000) opq       (1000)     8266 2023-08-01 19:02:37.000000 redvox-3.5.2/redvox/common/data_window_configuration.py
--rw-r--r--   0 opq       (1000) opq       (1000)     7154 2023-08-01 19:02:37.000000 redvox-3.5.2/redvox/common/data_window_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16785 2023-04-25 00:47:07.000000 redvox-3.5.2/redvox/common/date_time_utils.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3252 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/errors.py
--rw-r--r--   0 opq       (1000) opq       (1000)    41889 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/event_stream.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3104 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/event_stream_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    13655 2023-05-25 20:50:49.000000 redvox-3.5.2/redvox/common/file_statistics.py
--rw-r--r--   0 opq       (1000) opq       (1000)    17541 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/gap_and_pad_utils.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.410007 redvox-3.5.2/redvox/common/gui/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-04-14 19:22:20.000000 redvox-3.5.2/redvox/common/gui/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    16251 2021-04-14 23:46:42.000000 redvox-3.5.2/redvox/common/gui/cloud_data_retrieval.py
--rw-r--r--   0 opq       (1000) opq       (1000)    56756 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    26597 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/offset_model.py
--rw-r--r--   0 opq       (1000) opq       (1000)    26988 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/packet_to_pyarrow.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5022 2022-01-03 23:28:51.000000 redvox-3.5.2/redvox/common/parallel_utils.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1256 2022-06-29 18:15:55.000000 redvox-3.5.2/redvox/common/run_me.py
--rw-r--r--   0 opq       (1000) opq       (1000)    94752 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/sensor_data.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1086 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/sensor_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    17894 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/sensor_reader_utils.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2947 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/session_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    17172 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/session_model.py
--rw-r--r--   0 opq       (1000) opq       (1000)    15794 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/session_model_utils.py
--rw-r--r--   0 opq       (1000) opq       (1000)    70576 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/station.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1441 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/station_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)     4909 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/station_model.py
--rw-r--r--   0 opq       (1000) opq       (1000)    17605 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/station_utils.py
--rw-r--r--   0 opq       (1000) opq       (1000)     3964 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/stats_helper.py
--rw-r--r--   0 opq       (1000) opq       (1000)    21550 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/timesync.py
--rw-r--r--   0 opq       (1000) opq       (1000)     1175 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/timesync_io.py
--rw-r--r--   0 opq       (1000) opq       (1000)    13810 2023-08-01 19:02:38.000000 redvox-3.5.2/redvox/common/tri_message_stats.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     1867 2021-07-07 20:00:14.000000 redvox-3.5.2/redvox/common/versioning.py
--rw-r--r--   0 opq       (1000) opq       (1000)     2205 2023-05-25 20:50:49.000000 redvox-3.5.2/redvox/settings.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-08-01 19:46:05.216010 redvox-3.5.2/redvox.egg-info/
--rw-r--r--   0 opq       (1000) opq       (1000)    13906 2023-08-01 19:46:05.000000 redvox-3.5.2/redvox.egg-info/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     4560 2023-08-01 19:46:05.000000 redvox-3.5.2/redvox.egg-info/SOURCES.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-08-01 19:46:05.000000 redvox-3.5.2/redvox.egg-info/dependency_links.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       51 2023-08-01 19:46:05.000000 redvox-3.5.2/redvox.egg-info/entry_points.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      417 2023-08-01 19:46:05.000000 redvox-3.5.2/redvox.egg-info/requires.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        7 2023-08-01 19:46:05.000000 redvox-3.5.2/redvox.egg-info/top_level.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-08-01 19:46:05.417007 redvox-3.5.2/setup.cfg
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.087981 redvox-3.6.0/
+-rw-r--r--   0 tyler      (501) staff       (20)    11343 2023-08-01 00:48:51.000000 redvox-3.6.0/LICENSE
+-rw-r--r--   0 tyler      (501) staff       (20)    13906 2023-08-03 22:25:44.087388 redvox-3.6.0/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)      517 2021-06-16 20:22:36.000000 redvox-3.6.0/README.md
+-rw-r--r--   0 tyler      (501) staff       (20)     1470 2023-08-02 23:40:34.000000 redvox-3.6.0/pyproject.toml
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:43.993026 redvox-3.6.0/redvox/
+-rw-r--r--   0 tyler      (501) staff       (20)      728 2023-08-03 22:14:27.000000 redvox-3.6.0/redvox/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:43.996066 redvox-3.6.0/redvox/api1000/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.000483 redvox-3.6.0/redvox/api1000/common/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/common/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    20204 2021-03-31 23:04:52.000000 redvox-3.6.0/redvox/api1000/common/common.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1050 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/common/decorators.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5359 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/common/generic.py
+-rw-r--r--   0 tyler      (501) staff       (20)      875 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/common/lz4.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2570 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/common/mapping.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2237 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/common/metadata.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2435 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/common/typing.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2114 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/errors.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.001443 redvox-3.6.0/redvox/api1000/gui/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/gui/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4672 2021-04-09 20:02:21.000000 redvox-3.6.0/redvox/api1000/gui/image_viewer.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.003067 redvox-3.6.0/redvox/api1000/proto/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/proto/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    39434 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/api1000/proto/redvox_api_m_pb2.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.007589 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5639 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/event_streams.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10791 2023-08-03 22:14:27.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/ml.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.012487 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    11949 2021-03-31 23:04:52.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.013786 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    14890 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7398 2021-03-31 23:04:52.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/image.py
+-rw-r--r--   0 tyler      (501) staff       (20)    40936 2021-03-31 23:04:52.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/location.py
+-rw-r--r--   0 tyler      (501) staff       (20)    42236 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3425 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/single.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5576 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
+-rw-r--r--   0 tyler      (501) staff       (20)    50437 2023-05-23 21:20:02.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/station_information.py
+-rw-r--r--   0 tyler      (501) staff       (20)    19060 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/timing_information.py
+-rw-r--r--   0 tyler      (501) staff       (20)    21971 2021-03-31 23:04:52.000000 redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.024351 redvox-3.6.0/redvox/api900/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17514 2021-03-31 23:04:52.000000 redvox-3.6.0/redvox/api900/concat.py
+-rw-r--r--   0 tyler      (501) staff       (20)      494 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/constants.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1689 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/deprecation.py
+-rw-r--r--   0 tyler      (501) staff       (20)      351 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/exceptions.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.025831 redvox-3.6.0/redvox/api900/lib/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/lib/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7591 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/api900/lib/api900_pb2.py
+-rw-r--r--   0 tyler      (501) staff       (20)    43091 2023-08-02 22:00:16.000000 redvox-3.6.0/redvox/api900/location_analyzer.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2597 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/migrations.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.027086 redvox-3.6.0/redvox/api900/qa/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/qa/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2813 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/qa/gap_detection.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16939 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/reader.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17096 2021-06-01 21:32:52.000000 redvox-3.6.0/redvox/api900/reader_utils.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.038929 redvox-3.6.0/redvox/api900/sensors/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2113 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/accelerometer_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2298 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/barometer_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2665 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/evenly_sampled_channel.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6283 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/evenly_sampled_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1989 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/gyroscope_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4854 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/image_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2264 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/infrared_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16540 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/interleaved_channel.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2261 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/light_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10051 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/location_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2022 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/magnetometer_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3209 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/microphone_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4655 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/time_synchronization_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3536 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/unevenly_sampled_channel.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6619 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/unevenly_sampled_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5907 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1128 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/stat_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8780 2021-03-31 23:04:52.000000 redvox-3.6.0/redvox/api900/summarize.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.041146 redvox-3.6.0/redvox/api900/timesync/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/timesync/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    27606 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/timesync/api900_timesync.py
+-rw-r--r--   0 tyler      (501) staff       (20)    13824 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/timesync/tri_message_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1537 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/api900/types.py
+-rw-r--r--   0 tyler      (501) staff       (20)    54392 2021-03-31 23:04:52.000000 redvox-3.6.0/redvox/api900/wrapped_redvox_packet.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.044185 redvox-3.6.0/redvox/cli/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/cli/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    22678 2021-04-09 20:02:21.000000 redvox-3.6.0/redvox/cli/cli.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6683 2021-06-01 21:32:52.000000 redvox-3.6.0/redvox/cli/conversions.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1797 2021-04-09 20:02:21.000000 redvox-3.6.0/redvox/cli/data_req.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.057379 redvox-3.6.0/redvox/cloud/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/cloud/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2267 2023-06-26 20:48:55.000000 redvox-3.6.0/redvox/cloud/api.py
+-rw-r--r--   0 tyler      (501) staff       (20)   142063 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/cloud/api_m_fqns.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4334 2021-03-31 23:04:52.000000 redvox-3.6.0/redvox/cloud/auth_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)    29429 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/cloud/client.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5905 2022-12-15 01:35:54.000000 redvox-3.6.0/redvox/cloud/config.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6088 2021-04-09 20:02:21.000000 redvox-3.6.0/redvox/cloud/data_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3829 2022-12-15 01:35:54.000000 redvox-3.6.0/redvox/cloud/data_client.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3266 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/cloud/data_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)      487 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/cloud/errors.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18946 2023-05-23 21:20:02.000000 redvox-3.6.0/redvox/cloud/metadata_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3770 2021-04-14 22:44:11.000000 redvox-3.6.0/redvox/cloud/query_timing_correction.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1086 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/cloud/routes.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10985 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/cloud/session_model_api.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4262 2021-04-14 22:44:11.000000 redvox-3.6.0/redvox/cloud/station_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7707 2023-05-23 21:20:02.000000 redvox-3.6.0/redvox/cloud/subscription.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.085498 redvox-3.6.0/redvox/common/
+-rw-r--r--   0 tyler      (501) staff       (20)      195 2021-03-30 21:57:13.000000 redvox-3.6.0/redvox/common/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    55240 2023-06-23 23:40:13.000000 redvox-3.6.0/redvox/common/api_conversions.py
+-rw-r--r--   0 tyler      (501) staff       (20)    23894 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/api_reader.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5249 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/api_reader_dw.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1173 2021-04-19 23:26:28.000000 redvox-3.6.0/redvox/common/constants.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4126 2021-06-29 20:11:21.000000 redvox-3.6.0/redvox/common/cross_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)    42995 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/data_window.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8266 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/data_window_configuration.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7154 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/data_window_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16785 2023-05-23 21:20:02.000000 redvox-3.6.0/redvox/common/date_time_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3252 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/errors.py
+-rw-r--r--   0 tyler      (501) staff       (20)    44602 2023-08-03 22:14:27.000000 redvox-3.6.0/redvox/common/event_stream.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3104 2023-08-03 20:24:49.000000 redvox-3.6.0/redvox/common/event_stream_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    13655 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/file_statistics.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17541 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/gap_and_pad_utils.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:44.086570 redvox-3.6.0/redvox/common/gui/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2021-04-09 20:02:21.000000 redvox-3.6.0/redvox/common/gui/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16251 2021-04-15 01:00:48.000000 redvox-3.6.0/redvox/common/gui/cloud_data_retrieval.py
+-rw-r--r--   0 tyler      (501) staff       (20)    56756 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    26597 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/offset_model.py
+-rw-r--r--   0 tyler      (501) staff       (20)    26988 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/packet_to_pyarrow.py
+-rw-r--r--   0 tyler      (501) staff       (20)     5022 2022-12-15 01:35:54.000000 redvox-3.6.0/redvox/common/parallel_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1256 2023-05-23 21:20:02.000000 redvox-3.6.0/redvox/common/run_me.py
+-rw-r--r--   0 tyler      (501) staff       (20)    94752 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/sensor_data.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1086 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/sensor_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17894 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/sensor_reader_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2947 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/session_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17172 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/session_model.py
+-rw-r--r--   0 tyler      (501) staff       (20)    15794 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/session_model_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)    70608 2023-08-03 22:14:27.000000 redvox-3.6.0/redvox/common/station.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1441 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/station_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4909 2023-08-02 22:00:16.000000 redvox-3.6.0/redvox/common/station_model.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17605 2023-08-02 23:40:34.000000 redvox-3.6.0/redvox/common/station_utils.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3964 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/stats_helper.py
+-rw-r--r--   0 tyler      (501) staff       (20)    21550 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/timesync.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1175 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/timesync_io.py
+-rw-r--r--   0 tyler      (501) staff       (20)    13810 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/common/tri_message_stats.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1867 2021-06-29 20:11:21.000000 redvox-3.6.0/redvox/common/versioning.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2205 2023-08-01 00:48:51.000000 redvox-3.6.0/redvox/settings.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-08-03 22:25:43.995441 redvox-3.6.0/redvox.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)    13906 2023-08-03 22:25:43.000000 redvox-3.6.0/redvox.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)     4560 2023-08-03 22:25:43.000000 redvox-3.6.0/redvox.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2023-08-03 22:25:43.000000 redvox-3.6.0/redvox.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       51 2023-08-03 22:25:43.000000 redvox-3.6.0/redvox.egg-info/entry_points.txt
+-rw-r--r--   0 tyler      (501) staff       (20)      417 2023-08-03 22:25:43.000000 redvox-3.6.0/redvox.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        7 2023-08-03 22:25:43.000000 redvox-3.6.0/redvox.egg-info/top_level.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       38 2023-08-03 22:25:44.088124 redvox-3.6.0/setup.cfg
```

### Comparing `redvox-3.5.2/LICENSE` & `redvox-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/PKG-INFO` & `redvox-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox
-Version: 3.5.2
+Version: 3.6.0
 Summary: Library for working with RedVox files. 
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-3.5.2/README.md` & `redvox-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/pyproject.toml` & `redvox-3.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/__init__.py` & `redvox-3.6.0/redvox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Provides library level metadata and constants.
 """
 
 NAME: str = "redvox"
-VERSION: str = "3.5.2"
+VERSION: str = "3.6.0"
 
 
 def version() -> str:
     """Returns the version number of this library."""
     return VERSION
```

### Comparing `redvox-3.5.2/redvox/api1000/common/common.py` & `redvox-3.6.0/redvox/api1000/common/common.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/common/decorators.py` & `redvox-3.6.0/redvox/api1000/common/decorators.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/common/generic.py` & `redvox-3.6.0/redvox/api1000/common/generic.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/common/lz4.py` & `redvox-3.6.0/redvox/api1000/common/lz4.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/common/mapping.py` & `redvox-3.6.0/redvox/api1000/common/mapping.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/common/metadata.py` & `redvox-3.6.0/redvox/api1000/common/metadata.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/common/typing.py` & `redvox-3.6.0/redvox/api1000/common/typing.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/errors.py` & `redvox-3.6.0/redvox/api1000/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/gui/image_viewer.py` & `redvox-3.6.0/redvox/api1000/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/proto/redvox_api_m_pb2.py` & `redvox-3.6.0/redvox/api1000/proto/redvox_api_m_pb2.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/event_streams.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/event_streams.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/ml.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/ml.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 This module provides methods and datatypes for the efficient extraction and manipulation of machine learning data stored
  in RedVox packet EventStreams.
 """
 
 from dataclasses import dataclass
+from dataclasses_json import dataclass_json
 from enum import Enum
 from math import isfinite
 from typing import Optional, Dict, List
 
 import numpy as np
 from redvox.common.errors import RedVoxError
 
@@ -25,14 +26,15 @@
 
 
 class MlError(RedVoxError):
     def __init__(self, msg: str):
         super().__init__(f"MlError: {msg}")
 
 
+@dataclass_json
 @dataclass
 class ExtractedMl:
     """
     Contains the extracted ML classes and scores as well as metadata relating to the utilized model.
     """
 
     metadata: "MlMetadata"
@@ -76,54 +78,52 @@
         if n <= 0:
             raise MlError(f"n={n} must be > 0")
 
         self.windows = list(map(lambda window: window.retain_top(n), self.windows))
         return self
 
 
+@dataclass_json
 @dataclass
 class MlMetadata:
     """
     Metadata relating to the utilized ML model.
     """
 
     model_name: str
     model_version: str
     input_samples_per_hop: int
     input_sample_rate: int
     input_samples_per_window: int
 
 
+@dataclass_json
 @dataclass
 class MlWindow:
     """
     Labels from a single time window.
     """
 
     timestamp: int
     labels: List["Label"]
 
     def sort(self, sort_by: "SortBy") -> "MlWindow":
         """
-        Sorts the labels in ascending or descending order by either score of class name.
+        Sorts the labels in ascending or descending order by either score or class name.
         :param sort_by: The sort operation to use.
         :return: An updated instance of MlWindow.
         """
         if sort_by is SortBy.CLASS_ASC:
             self.labels = sorted(self.labels, key=lambda label: label.class_name)
         elif sort_by is SortBy.CLASS_DESC:
-            self.labels = sorted(
-                self.labels, key=lambda label: label.class_name, reverse=True
-            )
+            self.labels = sorted(self.labels, key=lambda label: label.class_name, reverse=True)
         elif sort_by is SortBy.SCORE_ASC:
             self.labels = sorted(self.labels, key=lambda label: label.score)
         else:
-            self.labels = sorted(
-                self.labels, key=lambda label: label.score, reverse=True
-            )
+            self.labels = sorted(self.labels, key=lambda label: label.score, reverse=True)
 
         return self
 
     def prune_zeros(self) -> "MlWindow":
         """
         Removes labels that have a score of 0.
         :return: An updated instance of MlWindow.
@@ -153,14 +153,15 @@
             raise MlError(f"n={n} must be > 0")
 
         sorted_window: MlWindow = self.sort(SortBy.SCORE_DESC)
         sorted_window.labels = sorted_window.labels[:n]
         return sorted_window
 
 
+@dataclass_json
 @dataclass
 class Label:
     """
     A pair containing a class name and a score.
     """
 
     class_name: str
@@ -181,17 +182,15 @@
 def extract_ml_metadata(stream: EventStream) -> MlMetadata:
     """
     Extracts ML metadata from an event stream.
     :param stream: The event stream to extract the ML metadata from.
     :return: An instance of MlMetadata.
     """
     if stream.get_name() != ML_EVENT_STREAM_NAME:
-        raise MlError(
-            f"Invalid ML event stream name={stream.get_name()} != {ML_EVENT_STREAM_NAME}"
-        )
+        raise MlError(f"Invalid ML event stream name={stream.get_name()} != {ML_EVENT_STREAM_NAME}")
 
     if stream.get_events().get_count() == 0:
         raise MlError("ML EventStream contains 0 Events")
 
     name: str = stream.get_events().get_values()[0].get_description()
     meta: Dict[str, str] = stream.get_metadata().get_metadata()
 
@@ -228,17 +227,15 @@
     for stream in streams.get_values():
         if stream.get_name() == ML_EVENT_STREAM_NAME:
             return stream
 
     return None
 
 
-def label_at(
-    str_payload: Dict[str, str], num_payload: Dict[str, float], idx: int
-) -> Label:
+def label_at(str_payload: Dict[str, str], num_payload: Dict[str, float], idx: int) -> Label:
     """
     Finds the label and score in the event payloads.
     :param str_payload: The event string payload.
     :param num_payload: The event numeric payload.
     :param idx: The index of the class and score.
     :return: An instance of a Label.
     """
@@ -263,29 +260,27 @@
 def extract_ml_windows(stream: EventStream) -> List[MlWindow]:
     """
     Extracts ML windows from an event stream.
     :param stream: The stream to extract windows from.
     :return: A list of ML windows.
     """
     if stream.get_name() != ML_EVENT_STREAM_NAME:
-        raise MlError(
-            f"Invalid ML event stream name={stream.get_name()} != {ML_EVENT_STREAM_NAME}"
-        )
+        raise MlError(f"Invalid ML event stream name={stream.get_name()} != {ML_EVENT_STREAM_NAME}")
 
     timestamps: np.ndarray = stream.get_timestamps().get_timestamps()
     windows: List[MlWindow] = []
 
     events: List[Event] = stream.get_events().get_values()
 
     if len(timestamps) != len(events):
         raise MlError(f"len(timestamps={len(timestamps)}) != len(events={len(events)})")
 
     idx_window: int
     timestamp: float
-    for (idx_window, timestamp) in enumerate(timestamps):
+    for idx_window, timestamp in enumerate(timestamps):
         event: Event = events[idx_window]
         str_payload: Dict[str, str] = event.get_string_payload().get_metadata()
         num_payload: Dict[str, float] = event.get_numeric_payload().get_metadata()
 
         labels: List[Label] = []
         for i in range(len(str_payload)):
             label: Label = label_at(str_payload, num_payload, i)
@@ -300,17 +295,15 @@
 def extract_ml_from_event_stream(stream: EventStream) -> ExtractedMl:
     """
     Extract ML parameters from an event stream.
     :param stream: The event stream to extract ML parameters from.
     :return: The extracted ML parameters or None.
     """
     if stream.get_name() != ML_EVENT_STREAM_NAME:
-        raise MlError(
-            f"Invalid ML event stream name={stream.get_name()} != {ML_EVENT_STREAM_NAME}"
-        )
+        raise MlError(f"Invalid ML event stream name={stream.get_name()} != {ML_EVENT_STREAM_NAME}")
 
     metadata: MlMetadata = extract_ml_metadata(stream)
     windows: List[MlWindow] = extract_ml_windows(stream)
     return ExtractedMl(metadata, windows)
 
 
 def extract_ml_from_packet(packet: WrappedRedvoxPacketM) -> Optional[ExtractedMl]:
```

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/audio.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/audio.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/image.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/image.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/location.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/location.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/single.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/single.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/station_information.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/station_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/timing_information.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/timing_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py` & `redvox-3.6.0/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/concat.py` & `redvox-3.6.0/redvox/api900/concat.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/deprecation.py` & `redvox-3.6.0/redvox/api900/deprecation.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/lib/api900_pb2.py` & `redvox-3.6.0/redvox/api900/lib/api900_pb2.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/location_analyzer.py` & `redvox-3.6.0/redvox/api900/location_analyzer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/migrations.py` & `redvox-3.6.0/redvox/api900/migrations.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/qa/gap_detection.py` & `redvox-3.6.0/redvox/api900/qa/gap_detection.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/reader.py` & `redvox-3.6.0/redvox/api900/reader.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/reader_utils.py` & `redvox-3.6.0/redvox/api900/reader_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/accelerometer_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/accelerometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/barometer_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/barometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/evenly_sampled_channel.py` & `redvox-3.6.0/redvox/api900/sensors/evenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/evenly_sampled_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/evenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/gyroscope_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/gyroscope_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/image_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/image_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/infrared_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/infrared_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/interleaved_channel.py` & `redvox-3.6.0/redvox/api900/sensors/interleaved_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/light_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/light_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/location_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/location_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/magnetometer_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/magnetometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/microphone_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/microphone_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/time_synchronization_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/time_synchronization_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/unevenly_sampled_channel.py` & `redvox-3.6.0/redvox/api900/sensors/unevenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/unevenly_sampled_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py` & `redvox-3.6.0/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/stat_utils.py` & `redvox-3.6.0/redvox/api900/stat_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/summarize.py` & `redvox-3.6.0/redvox/api900/summarize.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/timesync/api900_timesync.py` & `redvox-3.6.0/redvox/api900/timesync/api900_timesync.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/timesync/tri_message_stats.py` & `redvox-3.6.0/redvox/api900/timesync/tri_message_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/types.py` & `redvox-3.6.0/redvox/api900/types.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/api900/wrapped_redvox_packet.py` & `redvox-3.6.0/redvox/api900/wrapped_redvox_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cli/cli.py` & `redvox-3.6.0/redvox/cli/cli.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cli/conversions.py` & `redvox-3.6.0/redvox/cli/conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cli/data_req.py` & `redvox-3.6.0/redvox/cli/data_req.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/api.py` & `redvox-3.6.0/redvox/cloud/api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/api_m_fqns.py` & `redvox-3.6.0/redvox/cloud/api_m_fqns.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/auth_api.py` & `redvox-3.6.0/redvox/cloud/auth_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/client.py` & `redvox-3.6.0/redvox/cloud/client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/config.py` & `redvox-3.6.0/redvox/cloud/config.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/data_api.py` & `redvox-3.6.0/redvox/cloud/data_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/data_client.py` & `redvox-3.6.0/redvox/cloud/data_client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/data_io.py` & `redvox-3.6.0/redvox/cloud/data_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/metadata_api.py` & `redvox-3.6.0/redvox/cloud/metadata_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/query_timing_correction.py` & `redvox-3.6.0/redvox/cloud/query_timing_correction.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/routes.py` & `redvox-3.6.0/redvox/cloud/routes.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/session_model_api.py` & `redvox-3.6.0/redvox/cloud/session_model_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/station_stats.py` & `redvox-3.6.0/redvox/cloud/station_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/cloud/subscription.py` & `redvox-3.6.0/redvox/cloud/subscription.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/api_conversions.py` & `redvox-3.6.0/redvox/common/api_conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/api_reader.py` & `redvox-3.6.0/redvox/common/api_reader.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/api_reader_dw.py` & `redvox-3.6.0/redvox/common/api_reader_dw.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/constants.py` & `redvox-3.6.0/redvox/common/constants.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/cross_stats.py` & `redvox-3.6.0/redvox/common/cross_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/data_window.py` & `redvox-3.6.0/redvox/common/data_window.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/data_window_configuration.py` & `redvox-3.6.0/redvox/common/data_window_configuration.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/data_window_io.py` & `redvox-3.6.0/redvox/common/data_window_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/date_time_utils.py` & `redvox-3.6.0/redvox/common/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/errors.py` & `redvox-3.6.0/redvox/common/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/event_stream.py` & `redvox-3.6.0/redvox/common/event_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """
 This module provides classes to organize events recorded on a station.
+It will ignore machine learning events.
 """
 from typing import List, Optional, Dict, Union
 from dataclasses import dataclass, field
 from pathlib import Path
 import enum
 import os
 import re
 
 import numpy as np
 from dataclasses_json import dataclass_json
 
 from redvox.api1000.common.mapping import Mapping
 from redvox.api1000.proto.redvox_api_m_pb2 import RedvoxPacketM
 from redvox.api1000.wrapped_redvox_packet import event_streams as es
+from redvox.api1000.wrapped_redvox_packet import ml
+from redvox.api1000.wrapped_redvox_packet.wrapped_packet import WrappedRedvoxPacketM
 from redvox.common.errors import RedVoxExceptions
 from redvox.common import offset_model as om
 from redvox.common.io import FileSystemWriter as Fsw, FileSystemSaveMode, json_file_to_dict
 import redvox.common.event_stream_io as io
 
 
 class EventDataTypes(enum.Enum):
@@ -73,23 +76,19 @@
                             Default FileSystemSaveMode.MEM (use RAM).  Other options are DISK (save to directory)
                             and TEMP (save to temporary directory)
         :param base_dir: the location of the parquet file that holds the data.  Not used if save_data is False.
                             Default current directory (".")
         """
         self.name = name
         self.metadata = {}
-
         self._errors = RedVoxExceptions("Event")
         self._fs_writer = Fsw(f"event_{name}", "json", base_dir, save_mode)
         self._timestamp = timestamp
         self._uncorrected_timestamp = timestamp
-        if data is not None:
-            self._data = data
-        else:
-            self._data = get_empty_event_data_dict()
+        self._data = get_empty_event_data_dict() if data is None else data
 
     def __repr__(self):
         return (
             f"name: {self.name}, "
             f"timestamp: {self._timestamp}, "
             f"uncorrected_timestamp: {self._uncorrected_timestamp}, "
             f"schema: {self.get_schema()}, "
@@ -493,14 +492,20 @@
         """
         set the save mode
 
         :param save_mode: new save mode
         """
         self._fs_writer.set_save_mode(save_mode)
 
+    def save_mode(self) -> FileSystemSaveMode:
+        """
+        :return: the save mode
+        """
+        return self._fs_writer.save_mode()
+
     def set_file_name(self, new_file: Optional[str] = None):
         """
         * set the pyarrow file name or use the default: event_{Event.name}
         * Do not give an extension
 
         :param new_file: optional file name to change to; default None (use default name)
         """
@@ -982,44 +987,56 @@
     stores multiple event streams per station.
 
     ALL timestamps in microseconds since epoch UTC unless otherwise stated
 
     Properties:
         streams: List[EventStream]; list of all EventStream.  Default empty list
 
+        ml_data: Optional ExtractedMl from the packets.  Default None
+
         debug: bool; if True, output additional information during runtime.  Default False
     """
 
     streams: List[EventStream] = field(default_factory=lambda: [])
+    ml_data: Optional[ml.ExtractedMl] = None
     debug: bool = False
 
     def __repr__(self):
-        return f"streams: {[s.__repr__() for s in self.streams]}, " f"debug: {self.debug}"
+        return f"streams: {[s.__repr__() for s in self.streams]}, ml: {self.ml_data}, debug: {self.debug}"
 
     def __str__(self):
-        return str([s.__str__() for s in self.streams])
+        return f"streams: {[s.__str__() for s in self.streams]}, ml: {self.ml_data}"
 
     def as_dict(self) -> dict:
         """
         :return: EventStreams as dict
         """
-        return {"streams": [s.as_dict() for s in self.streams]}
+        return {
+            "streams": [s.as_dict() for s in self.streams],
+            "ml_data": self.ml_data.to_dict() if self.ml_data else None,
+        }
 
     def read_from_packet(self, packet: RedvoxPacketM):
         """
         read the eventstream payload from a single Redvox Api1000 packet
 
         :param packet: packet to read data from
         """
         for st in packet.event_streams:
-            if st.name in self.get_stream_names() and self.get_stream(st.name).has_data():
-                self.get_stream(st.name).add_events(st)
+            if st.name == ml.ML_EVENT_STREAM_NAME:
+                if self.ml_data:
+                    self.ml_data.windows.extend(ml.extract_ml_windows(_find_ml_event_stream(packet)))
+                else:
+                    self.ml_data = ml.extract_ml_from_packet(WrappedRedvoxPacketM(packet))
             else:
-                self.remove_stream(st.name)
-                self.streams.append(EventStream.from_eventstream(st))
+                if st.name in self.get_stream_names() and self.get_stream(st.name).has_data():
+                    self.get_stream(st.name).add_events(st)
+                else:
+                    self.remove_stream(st.name)
+                    self.streams.append(EventStream.from_eventstream(st))
 
     def read_from_packets_list(self, packets: List[RedvoxPacketM]):
         """
         read the eventstream payload from multiple Redvox Api1000 packets
 
         :param packets: packets to read data from
         """
@@ -1034,14 +1051,26 @@
         :param other_stream: other EventStream to add
         """
         if other_stream.name in self.get_stream_names():
             self.get_stream(other_stream.name).add_events(other_stream)
         else:
             self.streams.append(other_stream)
 
+    def append_ml(self, other_ml: ml.ExtractedMl):
+        """
+        append the windows from another extracted machine learning object or
+        set the existing ML object if its empty.
+
+        :param other_ml: other ExtractedMl to add
+        """
+        if self.ml_data:
+            self.ml_data.windows.extend(other_ml.windows)
+        else:
+            self.ml_data = other_ml
+
     def append_streams(self, other_streams: "EventStreams"):
         """
         append another EventStreams object to an existing EventStreams object
 
         :param other_streams: EventStreams to add
         """
         for s in other_streams.streams:
@@ -1071,23 +1100,25 @@
         """
         :return: names of all streams
         """
         return [s.name for s in self.streams]
 
     def create_event_window(self, start: float = -np.inf, end: float = np.inf):
         """
-        removes any event in the streams that doesn't match start <= event < end
+        removes any event in the streams and ML that doesn't match start <= event < end
         default start is negative infinity, default end is infinity
         all times in microseconds since epoch UTC
 
         :param start: inclusive start time of events to keep
         :param end: exclusive end time of events to keep
         """
         for s in self.streams:
             s.create_event_window(start, end)
+        if self.ml_data:
+            self.ml_data.windows = [s for s in self.ml_data.windows if start <= s.timestamp < end]
 
     def set_save_dir(self, new_dir: str):
         """
         change the directory where events are saved to
 
         :param new_dir: new directory path
         """
@@ -1109,46 +1140,82 @@
 
         :param offset_model: model used to update the timestamps
         :param use_model_function: if True, use the model's slope function to update the timestamps.
                                     otherwise uses the best offset (model's intercept value).  Default False
         """
         for evnt in self.streams:
             evnt.update_timestamps(offset_model, use_model_function)
+        if self.ml_data:
+            for w in self.ml_data.windows:
+                w.timestamp = offset_model.update_time(w.timestamp)
 
     def original_timestamps(self, offset_model: om.OffsetModel, use_model_function: bool = False):
         """
         undo the update to the timestamps in the data
 
         :param offset_model: model used to update the timestamps
         :param use_model_function: if True, use the model's slope function to update the timestamps.
                                     otherwise uses the best offset (model's intercept value).  Default False
         """
         for evnt in self.streams:
             evnt.original_timestamps(offset_model, use_model_function)
+        if self.ml_data:
+            for w in self.ml_data.windows:
+                w.timestamp = offset_model.get_original_time(w.timestamp)
+
+    @staticmethod
+    def from_dict(in_dict: dict) -> "EventStreams":
+        """
+        :param in_dict: dictionary representing an EventStreams object
+        :return: the EventStreams object from the dictionary
+        """
+        result = EventStreams()
+        if "streams" in in_dict.keys():
+            result.streams = [EventStream.from_json_dict(s) for s in in_dict["streams"]]
+        if "ml_data" in in_dict.keys():
+            result.ml_data = ml.ExtractedMl.from_dict(in_dict["ml_data"])
+        return result
 
     @staticmethod
     def from_json_file(file_dir: str, file_name: str) -> "EventStreams":
         """
         :param file_dir: full path to containing directory for the file
         :param file_name: name of file to load data from
         :return: EventStreams from json file
         """
-        json_data = json_file_to_dict(os.path.join(file_dir, f"{file_name}"))
-        if "streams" in json_data.keys():
-            result = EventStreams([EventStream.from_json_dict(s) for s in json_data["streams"]])
-            result.set_save_mode(FileSystemSaveMode.DISK)
-            result.set_save_dir(file_dir)
-        else:
-            result = EventStreams()
-        return result
+        return EventStreams.from_dict(json_file_to_dict(os.path.join(file_dir, f"{file_name}")))
 
     def to_json_file(self, file_dir: str = ".", file_name: Optional[str] = None) -> Path:
         """
         saves the EventStream as a json file
 
         :param file_dir: the directory to save the file into.  default current directory (".")
         :param file_name: the optional base file name.  Do not include a file extension.
                             If None, a default file name is created using this format:
                             eventstreams.json
         :return: path to json file
         """
         return io.eventstreams_to_json_file(self, file_dir, file_name)
+
+
+def _find_ml_event_stream(packet: RedvoxPacketM) -> Optional[es.EventStream]:
+    """
+    Attempts to find an event stream with ML data.
+
+    :param packet: The packet to search in.
+    :return: An instance of the matching event stream or None.
+    """
+    stream: RedvoxPacketM.EventStream
+    for stream in packet.event_streams:
+        if stream.name == ml.ML_EVENT_STREAM_NAME:
+            return es.EventStream(stream)
+    return None
+
+
+def _get_ml_from_packet(packet: RedvoxPacketM) -> Optional[ml.ExtractedMl]:
+    """
+    reads the machine learning payload from a single Redvox Api1000 packet
+
+    :param packet: packet to read machine learning data from
+    """
+    stream: Optional[es.EventStream] = _find_ml_event_stream(packet)
+    return None if stream is None else ml.extract_ml_from_event_stream(stream)
```

### Comparing `redvox-3.5.2/redvox/common/event_stream_io.py` & `redvox-3.6.0/redvox/common/event_stream_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/file_statistics.py` & `redvox-3.6.0/redvox/common/file_statistics.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/gap_and_pad_utils.py` & `redvox-3.6.0/redvox/common/gap_and_pad_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/gui/cloud_data_retrieval.py` & `redvox-3.6.0/redvox/common/gui/cloud_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/io.py` & `redvox-3.6.0/redvox/common/io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/offset_model.py` & `redvox-3.6.0/redvox/common/offset_model.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/packet_to_pyarrow.py` & `redvox-3.6.0/redvox/common/packet_to_pyarrow.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/parallel_utils.py` & `redvox-3.6.0/redvox/common/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/run_me.py` & `redvox-3.6.0/redvox/common/run_me.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/sensor_data.py` & `redvox-3.6.0/redvox/common/sensor_data.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/sensor_io.py` & `redvox-3.6.0/redvox/common/sensor_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/sensor_reader_utils.py` & `redvox-3.6.0/redvox/common/sensor_reader_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/session_io.py` & `redvox-3.6.0/redvox/common/session_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/session_model.py` & `redvox-3.6.0/redvox/common/session_model.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/session_model_utils.py` & `redvox-3.6.0/redvox/common/session_model_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/station.py` & `redvox-3.6.0/redvox/common/station.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import redvox.api1000.proto.redvox_api_m_pb2 as api_m
 from redvox.common import packet_to_pyarrow as ptp
 from redvox.common import gap_and_pad_utils as gpu
 from redvox.common.date_time_utils import datetime_from_epoch_microseconds_utc, seconds_to_microseconds as s_to_us
 from redvox.common.event_stream import EventStreams
 
 
-STATION_ID_LENGTH = 10  # the length of a station ID string
+STATION_ID_LENGTH: int = 10  # the length of a station ID string
 
 
 class Station:
     """
     generic station for api-independent stuff; uses API M as the core data object since it's quite versatile
 
     In order for a list of data to be a station, all the data packets must:
@@ -1500,24 +1500,26 @@
         uses the Station's location sensor to set the gps offset.
         """
         if self.has_location_data():
             loc_sensor = self.location_sensor()
         elif self.has_best_location_data():
             loc_sensor = self.best_location_sensor()
         else:
+            loc_sensor = None
+        if loc_sensor:
+            gps_timestamps = loc_sensor.get_gps_timestamps_data()
+            gps_offsets = gps_timestamps - loc_sensor.data_timestamps() + GPS_LATENCY_MICROS
+            if all(np.nan_to_num(gps_offsets) == 0.0):
+                self._errors.append("Location data is all invalid, cannot set GPS offset.")
+                return
+            self._gps_offset_model = OffsetModel(
+                np.empty(0), gps_offsets, gps_timestamps, gps_timestamps[0], gps_timestamps[-1]
+            )
+        else:
             self._errors.append("No location data to set GPS offset.")
-            return
-        gps_timestamps = loc_sensor.get_gps_timestamps_data()
-        gps_offsets = gps_timestamps - loc_sensor.data_timestamps() + GPS_LATENCY_MICROS
-        if all(np.nan_to_num(gps_offsets) == 0.0):
-            self._errors.append("Location data is all invalid, cannot set GPS offset.")
-            return
-        self._gps_offset_model = OffsetModel(
-            np.empty(0), gps_offsets, gps_timestamps, gps_timestamps[0], gps_timestamps[-1]
-        )
 
     def _app_version_major(self) -> Tuple[int, int]:
         """
         :return: tuple of app version to 2 significant version numbers (i.e: version number x.y.z returns x and y)
         """
         nums = self.metadata().app_version.split(".")
         if self.metadata().os == st_utils.OsType["IOS"]:
@@ -1687,31 +1689,30 @@
         for snr in self._data:
             snr.set_use_temp_dir(use_temp_dir)
 
     def use_timesync_for_correction(self) -> bool:
         """
         Note: This function means nothing if the station is not set to correct timestamps
 
-        :return: True if timesync is used for correction, False if GPS is used instead.
+        :return: False if timesync has NAN mean latency or best offset is 0. True otherwise
         """
-        if np.isnan(self._timesync_data.mean_latency()) or self._timesync_data.best_offset() == 0.0:
-            return False
-        return True
+        return (
+            False if np.isnan(self._timesync_data.mean_latency()) or self._timesync_data.best_offset() == 0.0 else True
+        )
 
     def update_timestamps(self) -> "Station":
         """
         updates the timestamps in the station using the offset model
 
         :return: updated Station
         """
         if not self._is_timestamps_updated and self._correct_timestamps:
-            if self.use_timesync_for_correction():
-                offset_model = self._timesync_data.offset_model()
-            else:
-                offset_model = self._gps_offset_model
+            offset_model = (
+                self._timesync_data.offset_model() if self.use_timesync_for_correction() else self._gps_offset_model
+            )
             self._start_date = offset_model.update_time(self._start_date, self._use_model_correction)
             for sensor in self._data:
                 sensor.update_data_timestamps(offset_model)
             for packet in self._packet_metadata:
                 packet.update_timestamps(offset_model, self._use_model_correction)
             for g in range(len(self._gaps)):
                 self._gaps[g] = (offset_model.update_time(self._gaps[g][0]), offset_model.update_time(self._gaps[g][1]))
@@ -1734,18 +1735,17 @@
         """
         undoes non-sensor timestamp updates of the timestamps in the station using the offset model
         sensors already have unaltered timestamps
 
         :return: updated Station
         """
         if self._is_timestamps_updated:
-            if self.use_timesync_for_correction():
-                offset_model = self._timesync_data.offset_model()
-            else:
-                offset_model = self._gps_offset_model
+            offset_model = (
+                self._timesync_data.offset_model() if self.use_timesync_for_correction() else self._gps_offset_model
+            )
             self._start_date = offset_model.get_original_time(self._start_date, self._use_model_correction)
             for sensor in self._data:
                 sensor.set_original_timestamps()
             for packet in self._packet_metadata:
                 packet.original_timestamps(offset_model, self._use_model_correction)
             for g in range(len(self._gaps)):
                 self._gaps[g] = (
```

### Comparing `redvox-3.5.2/redvox/common/station_io.py` & `redvox-3.6.0/redvox/common/station_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/station_model.py` & `redvox-3.6.0/redvox/common/station_model.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/station_utils.py` & `redvox-3.6.0/redvox/common/station_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/stats_helper.py` & `redvox-3.6.0/redvox/common/stats_helper.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/timesync.py` & `redvox-3.6.0/redvox/common/timesync.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/timesync_io.py` & `redvox-3.6.0/redvox/common/timesync_io.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/tri_message_stats.py` & `redvox-3.6.0/redvox/common/tri_message_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/common/versioning.py` & `redvox-3.6.0/redvox/common/versioning.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox/settings.py` & `redvox-3.6.0/redvox/settings.py`

 * *Files identical despite different names*

### Comparing `redvox-3.5.2/redvox.egg-info/PKG-INFO` & `redvox-3.6.0/redvox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox
-Version: 3.5.2
+Version: 3.6.0
 Summary: Library for working with RedVox files. 
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-3.5.2/redvox.egg-info/SOURCES.txt` & `redvox-3.6.0/redvox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

