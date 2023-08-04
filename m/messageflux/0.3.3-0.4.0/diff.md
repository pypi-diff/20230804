# Comparing `tmp/messageflux-0.3.3.tar.gz` & `tmp/messageflux-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messageflux-0.3.3.tar", last modified: Thu Aug  3 12:45:28 2023, max compression
+gzip compressed data, was "messageflux-0.4.0.tar", last modified: Thu Aug  3 20:57:12 2023, max compression
```

## Comparing `messageflux-0.3.3.tar` & `messageflux-0.4.0.tar`

### file list

```diff
@@ -1,114 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.869708 messageflux-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 12:45:12.000000 messageflux-0.3.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 12:45:12.000000 messageflux-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-03 12:45:12.000000 messageflux-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-03 12:45:28.869708 messageflux-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-08-03 12:45:12.000000 messageflux-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 12:45:14.000000 messageflux-0.3.3/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:12.000000 messageflux-0.3.3/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 12:45:12.000000 messageflux-0.3.3/_custom_build/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 12:45:12.000000 messageflux-0.3.3/_custom_build/make_all_extra_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/base_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/fastmessage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/iodevices/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/iodevices/base/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/base/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/base/input_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/base/input_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/base/output_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/iodevices/failover_output_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/failover_output_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux/iodevices/file_system/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/file_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/file_system/file_system_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24734 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/file_system/file_system_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/file_system/file_system_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/file_system/file_system_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/in_memory_device/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/in_memory_device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/objectstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/objectstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/objectstorage/s3_message_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/s3bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/s3client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/fs_poison_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/round_robin_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/round_robin_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.865708 messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.869708 messageflux-0.3.3/messageflux/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/LogType.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/bulk_rotating_device_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/bulk_rotating_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/bulk_rotating_handler_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/logging/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/message_handling_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/metadata_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.869708 messageflux-0.3.3/messageflux/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/multiprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/multiprocessing/multiprocessrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/multiprocessing/singleprocesshandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/pipeline_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/server_loop_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.869708 messageflux-0.3.3/messageflux/service_addons/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/service_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/service_addons/loop_health_addon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.869708 messageflux-0.3.3/messageflux/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-08-03 12:45:12.000000 messageflux-0.3.3/messageflux/utils/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:45:28.861708 messageflux-0.3.3/messageflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-08-03 12:45:28.000000 messageflux-0.3.3/messageflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-08-03 12:45:28.000000 messageflux-0.3.3/messageflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:45:28.000000 messageflux-0.3.3/messageflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-03 12:45:28.000000 messageflux-0.3.3/messageflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 12:45:28.000000 messageflux-0.3.3/messageflux.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 12:45:12.000000 messageflux-0.3.3/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-08-03 12:45:12.000000 messageflux-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-03 12:45:12.000000 messageflux-0.3.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-08-03 12:45:28.000000 messageflux-0.3.3/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-fastmessage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-objectstorage.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-objectstorage_mypy.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-rabbitmq.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements-rabbitmq_mypy.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:45:12.000000 messageflux-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:45:28.869708 messageflux-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.241033 messageflux-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 20:56:57.000000 messageflux-0.4.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-03 20:56:57.000000 messageflux-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-03 20:56:57.000000 messageflux-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-08-03 20:57:12.241033 messageflux-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-08-03 20:56:57.000000 messageflux-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 20:56:59.000000 messageflux-0.4.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.233033 messageflux-0.4.0/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:56:57.000000 messageflux-0.4.0/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-03 20:56:57.000000 messageflux-0.4.0/_custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-03 20:56:57.000000 messageflux-0.4.0/_custom_build/make_all_extra_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.233033 messageflux-0.4.0/messageflux/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/base_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.233033 messageflux-0.4.0/messageflux/iodevices/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.233033 messageflux-0.4.0/messageflux/iodevices/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/base/input_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/base/input_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/base/output_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.237033 messageflux-0.4.0/messageflux/iodevices/collection_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/collection_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/collection_device_wrapper/collection_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/collection_device_wrapper/collection_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.237033 messageflux-0.4.0/messageflux/iodevices/failover_output_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/failover_output_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.237033 messageflux-0.4.0/messageflux/iodevices/file_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/file_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/file_system/file_system_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24734 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/file_system/file_system_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/file_system/file_system_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/file_system/file_system_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.237033 messageflux-0.4.0/messageflux/iodevices/in_memory_device/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/in_memory_device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/in_memory_device/in_memory_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.237033 messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/message_store_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.237033 messageflux-0.4.0/messageflux/iodevices/objectstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/objectstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/objectstorage/s3_message_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.237033 messageflux-0.4.0/messageflux/iodevices/objectstorage/s3api/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/objectstorage/s3api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/objectstorage/s3api/s3bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/objectstorage/s3api/s3client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.241033 messageflux-0.4.0/messageflux/iodevices/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/rabbitmq/fs_poison_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15636 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.241033 messageflux-0.4.0/messageflux/iodevices/round_robin_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/round_robin_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.241033 messageflux-0.4.0/messageflux/iodevices/short_circuit_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/short_circuit_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/short_circuit_device_wrapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.241033 messageflux-0.4.0/messageflux/iodevices/transformer_device_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/transformer_device_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.241033 messageflux-0.4.0/messageflux/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/logging/LogType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/logging/bulk_rotating_device_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/logging/bulk_rotating_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/logging/bulk_rotating_handler_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/logging/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/message_handling_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/metadata_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.241033 messageflux-0.4.0/messageflux/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/multiprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/multiprocessing/multiprocessrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/multiprocessing/singleprocesshandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/pipeline_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/server_loop_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.241033 messageflux-0.4.0/messageflux/service_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/service_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/service_addons/loop_health_addon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.241033 messageflux-0.4.0/messageflux/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-08-03 20:56:57.000000 messageflux-0.4.0/messageflux/utils/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 20:57:12.233033 messageflux-0.4.0/messageflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-08-03 20:57:12.000000 messageflux-0.4.0/messageflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-08-03 20:57:12.000000 messageflux-0.4.0/messageflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:57:12.000000 messageflux-0.4.0/messageflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-03 20:57:12.000000 messageflux-0.4.0/messageflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 20:57:12.000000 messageflux-0.4.0/messageflux.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 20:56:57.000000 messageflux-0.4.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-03 20:56:57.000000 messageflux-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-03 20:56:57.000000 messageflux-0.4.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-03 20:57:12.000000 messageflux-0.4.0/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 20:56:57.000000 messageflux-0.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 20:56:57.000000 messageflux-0.4.0/requirements-objectstorage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-03 20:56:57.000000 messageflux-0.4.0/requirements-objectstorage_mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-03 20:56:57.000000 messageflux-0.4.0/requirements-rabbitmq.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-03 20:56:57.000000 messageflux-0.4.0/requirements-rabbitmq_mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 20:56:57.000000 messageflux-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 20:57:12.241033 messageflux-0.4.0/setup.cfg
```

### Comparing `messageflux-0.3.3/LICENSE` & `messageflux-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/PKG-INFO` & `messageflux-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.3.3
+Version: 0.4.0
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <3.12,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: fastmessage
 Provides-Extra: objectstorage
 Provides-Extra: objectstorage_mypy
 Provides-Extra: rabbitmq
 Provides-Extra: rabbitmq_mypy
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `messageflux-0.3.3/README.md` & `messageflux-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/_custom_build/make_all_extra_requirements.py` & `messageflux-0.4.0/_custom_build/make_all_extra_requirements.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/base_service.py` & `messageflux-0.4.0/messageflux/base_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/base/__init__.py` & `messageflux-0.4.0/messageflux/iodevices/base/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/base/common.py` & `messageflux-0.4.0/messageflux/iodevices/base/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/base/input_devices.py` & `messageflux-0.4.0/messageflux/iodevices/base/input_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/base/input_transaction.py` & `messageflux-0.4.0/messageflux/iodevices/base/input_transaction.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/base/output_devices.py` & `messageflux-0.4.0/messageflux/iodevices/base/output_devices.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/collection_input_device.py` & `messageflux-0.4.0/messageflux/iodevices/collection_device_wrapper/collection_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/collection_device_wrapper/collection_output_device.py` & `messageflux-0.4.0/messageflux/iodevices/collection_device_wrapper/collection_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py` & `messageflux-0.4.0/messageflux/iodevices/failover_output_device_wrapper/failover_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/file_system/__init__.py` & `messageflux-0.4.0/messageflux/iodevices/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/file_system/file_system_device_manager_base.py` & `messageflux-0.4.0/messageflux/iodevices/file_system/file_system_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/file_system/file_system_input_device.py` & `messageflux-0.4.0/messageflux/iodevices/file_system/file_system_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/file_system/file_system_output_device.py` & `messageflux-0.4.0/messageflux/iodevices/file_system/file_system_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/file_system/file_system_serializer.py` & `messageflux-0.4.0/messageflux/iodevices/file_system/file_system_serializer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/in_memory_device/in_memory_device_manager.py` & `messageflux-0.4.0/messageflux/iodevices/in_memory_device/in_memory_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py` & `messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/file_system_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_base.py` & `messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/message_store_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py` & `messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/message_store_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py` & `messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/message_store_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py` & `messageflux-0.4.0/messageflux/iodevices/message_store_device_wrapper/message_store_transformer_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/objectstorage/s3_message_store.py` & `messageflux-0.4.0/messageflux/iodevices/objectstorage/s3_message_store.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/s3bucket.py` & `messageflux-0.4.0/messageflux/iodevices/objectstorage/s3api/s3bucket.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/objectstorage/s3api/s3client.py` & `messageflux-0.4.0/messageflux/iodevices/objectstorage/s3api/s3client.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/rabbitmq/fs_poison_counter.py` & `messageflux-0.4.0/messageflux/iodevices/rabbitmq/fs_poison_counter.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py` & `messageflux-0.4.0/messageflux/iodevices/rabbitmq/rabbitmq_device_manager_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py` & `messageflux-0.4.0/messageflux/iodevices/rabbitmq/rabbitmq_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py` & `messageflux-0.4.0/messageflux/iodevices/rabbitmq/rabbitmq_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py` & `messageflux-0.4.0/messageflux/iodevices/rabbitmq/rabbitmq_poison_counting_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py` & `messageflux-0.4.0/messageflux/iodevices/round_robin_device_wrapper/roundrobin_io_device_manager.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/common.py` & `messageflux-0.4.0/messageflux/iodevices/short_circuit_device_wrapper/common.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py` & `messageflux-0.4.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py` & `messageflux-0.4.0/messageflux/iodevices/short_circuit_device_wrapper/short_circuit_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py` & `messageflux-0.4.0/messageflux/iodevices/transformer_device_wrapper/transformer_input_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py` & `messageflux-0.4.0/messageflux/iodevices/transformer_device_wrapper/transformer_output_device.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py` & `messageflux-0.4.0/messageflux/iodevices/transformer_device_wrapper/zlib_transformer.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/logging/bulk_rotating_device_handler.py` & `messageflux-0.4.0/messageflux/logging/bulk_rotating_device_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/logging/bulk_rotating_file_handler.py` & `messageflux-0.4.0/messageflux/logging/bulk_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/logging/bulk_rotating_handler_base.py` & `messageflux-0.4.0/messageflux/logging/bulk_rotating_handler_base.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/message_handling_service.py` & `messageflux-0.4.0/messageflux/message_handling_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/multiprocessing/multiprocessrunner.py` & `messageflux-0.4.0/messageflux/multiprocessing/multiprocessrunner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 import logging
-import os
 import threading
-from multiprocessing.process import BaseProcess
-
 import time
+from multiprocessing.process import BaseProcess
 from typing import List, Optional
 
 from messageflux.base_service import BaseService
 from messageflux.multiprocessing.singleprocesshandler import ServiceFactory, SingleProcessHandler
 
-INSTANCE_COUNT_ENV_VAR = 'MULTI_PROCESS_INSTANCE_COUNT'
-
 
 class MultiProcessRunner(BaseService):
     """
     a class that runs multiple services in processes. it handles the child process, and check liveness
     """
 
     def __init__(self, *,
@@ -49,31 +45,31 @@
         for handler in self._process_handlers:
             if handler.is_alive():
                 return True
 
         return False
 
     def _run_service(self, cancellation_token: threading.Event):
-        os.environ[INSTANCE_COUNT_ENV_VAR] = str(self._instance_count)
         for i in range(self._instance_count):
             self._logger.info(f'Starting service instance {i}')
             self._run_service_instance(i)
 
     @property
     def processes(self) -> List[BaseProcess]:
         """
         the list of child processes that runs the service instances
         """
         return [handler.process for handler in self._process_handlers if handler.process is not None]
 
     def _run_service_instance(self, instance_index: int):
-        handler = SingleProcessHandler(self._service_factory,
-                                       instance_index,
-                                       self._live_check_interval,
-                                       self._live_check_timeout)
+        handler = SingleProcessHandler(service_factory=self._service_factory,
+                                       instance_index=instance_index,
+                                       total_instances=self._instance_count,
+                                       live_check_interval=self._live_check_interval,
+                                       live_check_timeout=self._live_check_timeout)
         handler.start(self._on_handler_exit)
         self._process_handlers.append(handler)
 
     def _on_handler_exit(self, handler: SingleProcessHandler):
         if not self._restart_on_failure:
             return
 
@@ -129,15 +125,15 @@
     :param instance_count: the number of processes to run
     :param shutdown_timeout: the time (seconds) to wait after calling 'stop' to violently stop the subprocesses
     :param live_check_interval: the interval in seconds to send the liveness message to queue
     :param live_check_timeout: the time to wait for the process answer to liveness test
     :param restart_on_failure: should we restart a process if it fails?
     """
     if instance_count <= 1:
-        return service_factory.create_service()
+        return service_factory.create_service(instance_index=0, total_instances=1)
     else:
         return MultiProcessRunner(service_factory=service_factory,
                                   instance_count=instance_count,
                                   shutdown_timeout=shutdown_timeout,
                                   live_check_interval=live_check_interval,
                                   live_check_timeout=live_check_timeout,
                                   restart_on_failure=restart_on_failure,
```

### Comparing `messageflux-0.3.3/messageflux/multiprocessing/singleprocesshandler.py` & `messageflux-0.4.0/messageflux/multiprocessing/singleprocesshandler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from multiprocessing import process
-
 import logging
 import multiprocessing
 import os
 import threading
 from abc import ABCMeta, abstractmethod
+from multiprocessing import process
 from multiprocessing.process import BaseProcess
 from typing import Optional, Callable, TYPE_CHECKING
 
 from messageflux.base_service import BaseService
 
 if TYPE_CHECKING:
     from multiprocessing.connection import _ConnectionBase
@@ -16,35 +15,43 @@
 
 class ServiceFactory(metaclass=ABCMeta):
     """
     This class is used to create a service instance.
     """
 
     @abstractmethod
-    def create_service(self) -> BaseService:
+    def create_service(self, instance_index: int, total_instances: int) -> BaseService:
         """
         creates the service instance. this will run in the child service
+
+        :param instance_index: the instance index (0 based) out of all the indexes
+        :param total_instances: the total number of indexes
         :return: an instance of BaseService
         """
         pass
 
 
 _STOP_MESSAGE = 'STOP'
 _TEST_ALIVE_MESSAGE = 'TEST_ALIVE'
 
 INSTANCE_INDEX_ENV_VAR = 'MULTI_PROCESS_INSTANCE_INDEX'
+INSTANCE_COUNT_ENV_VAR = 'MULTI_PROCESS_INSTANCE_COUNT'
+
 _logger = logging.getLogger(__name__)
 
 
 def _start_service_and_listen_queue(service_factory: ServiceFactory,
                                     child_pipe: '_ConnectionBase',
-                                    instance_index: int):
+                                    instance_index: int,
+                                    total_instances: int):
     try:
         os.environ[INSTANCE_INDEX_ENV_VAR] = str(instance_index)
-        service = service_factory.create_service()
+        os.environ[INSTANCE_COUNT_ENV_VAR] = str(total_instances)
+
+        service = service_factory.create_service(instance_index=instance_index, total_instances=total_instances)
 
         def _listen_to_pipe(inner_service: BaseService, pipe: '_ConnectionBase'):
             try:
                 while True:
                     message = pipe.recv()
                     if message == _TEST_ALIVE_MESSAGE:
                         pipe.send(inner_service.is_alive)
@@ -74,24 +81,26 @@
     """
     This class is used to handle a single process.
     """
 
     def __init__(self,
                  service_factory: ServiceFactory,
                  instance_index: int,
+                 total_instances: int,
                  live_check_interval: int = 60,
                  live_check_timeout: int = 10):
         self._service_factory = service_factory
         self._live_check_interval = live_check_interval
         self._live_check_timeout = live_check_timeout
         self._liveness_thread: Optional[threading.Thread] = None
         self._stop_was_called = threading.Event()
         self._parent_pipe: Optional['_ConnectionBase'] = None
         self._process: Optional[process.BaseProcess] = None
         self._instance_index = instance_index
+        self._total_instances = total_instances
 
     @property
     def instance_index(self) -> int:
         """
         the index of this service instance
         """
         return self._instance_index
@@ -121,15 +130,17 @@
 
         context = multiprocessing.get_context('spawn')
         child_pipe: '_ConnectionBase'
         self._parent_pipe, child_pipe = context.Pipe()
         self._stop_was_called.clear()
 
         self._process = context.Process(target=_start_service_and_listen_queue,
-                                        args=(self._service_factory, child_pipe, self._instance_index))
+                                        args=(
+                                            self._service_factory, child_pipe, self._instance_index,
+                                            self._total_instances))
 
         def _run_process():
             assert self._process is not None
             self._process.start()
             self._process.join()
             self._cleanup()
```

### Comparing `messageflux-0.3.3/messageflux/pipeline_service.py` & `messageflux-0.4.0/messageflux/pipeline_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/server_loop_service.py` & `messageflux-0.4.0/messageflux/server_loop_service.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/service_addons/loop_health_addon.py` & `messageflux-0.4.0/messageflux/service_addons/loop_health_addon.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/utils/__init__.py` & `messageflux-0.4.0/messageflux/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/utils/context.py` & `messageflux-0.4.0/messageflux/utils/context.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux/utils/filesystem.py` & `messageflux-0.4.0/messageflux/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `messageflux-0.3.3/messageflux.egg-info/PKG-INFO` & `messageflux-0.4.0/messageflux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messageflux
-Version: 0.3.3
+Version: 0.4.0
 Author-email: Aviv Salem <avivsalem@gmail.com>
 Maintainer-email: Aviv Salem <avivsalem@gmail.com>, Nir Schulman <narsssx@gmail.com>, Rafael Zilberman <Zilberman.rafi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Avivsalem/MessageFlux/
 Project-URL: Documentation, https://messageflux.readthedocs.io/
 Platform: win32
 Platform: linux
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: <3.12,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
-Provides-Extra: fastmessage
 Provides-Extra: objectstorage
 Provides-Extra: objectstorage_mypy
 Provides-Extra: rabbitmq
 Provides-Extra: rabbitmq_mypy
 Provides-Extra: all
 License-File: LICENSE
```

### Comparing `messageflux-0.3.3/messageflux.egg-info/SOURCES.txt` & `messageflux-0.4.0/messageflux.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 README.md
 VERSION
 mypy.ini
 pyproject.toml
 pytest.ini
 requirements-all.txt
 requirements-dev.txt
-requirements-fastmessage.txt
 requirements-objectstorage.txt
 requirements-objectstorage_mypy.txt
 requirements-rabbitmq.txt
 requirements-rabbitmq_mypy.txt
 requirements.txt
 _custom_build/__init__.py
 _custom_build/backend.py
 _custom_build/make_all_extra_requirements.py
 messageflux/__init__.py
 messageflux/base_service.py
-messageflux/fastmessage_handler.py
 messageflux/message_handling_service.py
 messageflux/metadata_headers.py
 messageflux/pipeline_service.py
 messageflux/py.typed
 messageflux/server_loop_service.py
 messageflux.egg-info/PKG-INFO
 messageflux.egg-info/SOURCES.txt
```

### Comparing `messageflux-0.3.3/pyproject.toml` & `messageflux-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 [tool.setuptools.dynamic]
 dependencies = { file = "requirements.txt" }
 version = { file = "VERSION" }
 
 
 [tool.setuptools.dynamic.optional-dependencies]
 dev = { file = "requirements-dev.txt" }
-fastmessage = { file = "requirements-fastmessage.txt" }
 objectstorage = { file = "requirements-objectstorage.txt" }
 objectstorage_mypy = { file = "requirements-objectstorage_mypy.txt" }
 rabbitmq = { file = "requirements-rabbitmq.txt" }
 rabbitmq_mypy = { file = "requirements-rabbitmq_mypy.txt" }
 all = { file = "requirements-all.txt" }
```

