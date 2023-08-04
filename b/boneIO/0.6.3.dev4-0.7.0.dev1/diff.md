# Comparing `tmp/boneIO-0.6.3.dev4.tar.gz` & `tmp/boneIO-0.7.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boneIO-0.6.3.dev4.tar", last modified: Sun Jun 18 17:54:51 2023, max compression
+gzip compressed data, was "boneIO-0.7.0.dev1.tar", last modified: Fri Aug  4 20:09:07 2023, max compression
```

## Comparing `boneIO-0.6.3.dev4.tar` & `boneIO-0.7.0.dev1.tar`

### file list

```diff
@@ -1,79 +1,83 @@
--rw-r--r--   0        0        0    35149 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/LICENSE
--rw-r--r--   0        0        0      474 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/README.md
--rw-r--r--   0        0        0      147 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/__init__.py
--rw-r--r--   0        0        0     3341 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/bonecli.py
--rw-r--r--   0        0        0     2924 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/const.py
--rw-r--r--   0        0        0     8454 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/cover.py
--rw-r--r--   0        0        0        0 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/example_config/__init__.py
--rw-r--r--   0        0        0      168 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/example_config/adc.yaml
--rw-r--r--   0        0        0      326 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/example_config/config.yaml
--rw-r--r--   0        0        0      150 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/example_config/cover.yaml
--rw-r--r--   0        0        0     2883 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/example_config/input.yaml
--rw-r--r--   0        0        0     3392 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/example_config/led32x4A.yaml
--rw-r--r--   0        0        0     1691 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/example_config/output24x16A.yaml
--rw-r--r--   0        0        0     2403 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/example_config/output32x5A.yaml
--rw-r--r--   0        0        0    19372 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/fonts/danube__.ttf
--rw-r--r--   0        0        0     2039 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/__init__.py
--rw-r--r--   0        0        0      985 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/async_updater.py
--rw-r--r--   0        0        0     1138 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/click_timer.py
--rw-r--r--   0        0        0     2277 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/config.py
--rw-r--r--   0        0        0     7494 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/events.py
--rw-r--r--   0        0        0      717 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/exceptions.py
--rw-r--r--   0        0        0      885 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/filter.py
--rw-r--r--   0        0        0     3249 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/gpio.py
--rw-r--r--   0        0        0     6278 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/ha_discovery.py
--rw-r--r--   0        0        0    13547 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/loader.py
--rw-r--r--   0        0        0     1801 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/logger.py
--rw-r--r--   0        0        0      765 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/mqtt.py
--rw-r--r--   0        0        0      351 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/oled.py
--rw-r--r--   0        0        0     2430 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/onewire/W1ThermSensor.py
--rw-r--r--   0        0        0      448 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/onewire/__init__.py
--rw-r--r--   0        0        0     5169 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/onewire/ds2482.py
--rw-r--r--   0        0        0     2497 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/onewire/onewire.py
--rw-r--r--   0        0        0     1066 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/queue.py
--rw-r--r--   0        0        0     1994 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/state_manager.py
--rw-r--r--   0        0        0     5853 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/stats.py
--rw-r--r--   0        0        0     5806 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/timeperiod.py
--rw-r--r--   0        0        0      508 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/util.py
--rw-r--r--   0        0        0    11304 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/helper/yaml_util.py
--rw-r--r--   0        0        0       99 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/input/__init__.py
--rw-r--r--   0        0        0     3286 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/input/gpio.py
--rw-r--r--   0        0        0    21129 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/manager.py
--rw-r--r--   0        0        0     4176 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/modbus.py
--rw-r--r--   0        0        0     8331 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/mqtt_client.py
--rw-r--r--   0        0        0     5244 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/oled.py
--rw-r--r--   0        0        0      181 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/relay/__init__.py
--rw-r--r--   0        0        0     2623 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/relay/basic.py
--rw-r--r--   0        0        0     1163 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/relay/gpio.py
--rw-r--r--   0        0        0     2669 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/relay/mcp.py
--rw-r--r--   0        0        0     4873 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/relay/pca.py
--rw-r--r--   0        0        0     2569 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/runner.py
--rw-r--r--   0        0        0     1030 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/schema/actions.yaml
--rw-r--r--   0        0        0      124 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/schema/actions_sensor.yaml
--rw-r--r--   0        0        0      129 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/schema/actions_switch.yaml
--rw-r--r--   0        0        0      286 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/schema/filters.yaml
--rw-r--r--   0        0        0      304 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/schema/filters_adc.yaml
--rw-r--r--   0        0        0       75 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/schema/id.yaml
--rw-r--r--   0        0        0    12988 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/schema/schema.yaml
--rw-r--r--   0        0        0       65 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/schema/temp_unit.yaml
--rw-r--r--   0        0        0      133 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/schema/update_interval.yaml
--rw-r--r--   0        0        0      431 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/sensor/__init__.py
--rw-r--r--   0        0        0     1281 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/sensor/adc.py
--rw-r--r--   0        0        0     1303 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/sensor/gpio.py
--rw-r--r--   0        0        0     8520 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/sensor/modbus/__init__.py
--rw-r--r--   0        0        0     8810 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/sensor/modbus/dts1964_3f.json
--rw-r--r--   0        0        0      526 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/sensor/modbus/pt100.json
--rw-r--r--   0        0        0     2735 2023-06-18 17:54:13.538075 boneIO-0.6.3.dev4/boneio/sensor/modbus/r4dcb08.json
--rw-r--r--   0        0        0     4145 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/boneio/sensor/modbus/sdm120.json
--rw-r--r--   0        0        0    10969 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/boneio/sensor/modbus/sdm630.json
--rw-r--r--   0        0        0     5592 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/boneio/sensor/modbus/sofar.json
--rw-r--r--   0        0        0     1808 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/boneio/sensor/temp/__init__.py
--rw-r--r--   0        0        0     2485 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/boneio/sensor/temp/dallas.py
--rw-r--r--   0        0        0      243 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/boneio/sensor/temp/lm75.py
--rw-r--r--   0        0        0      271 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/boneio/sensor/temp/mcp9808.py
--rw-r--r--   0        0        0       42 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/boneio/version.py
--rw-r--r--   0        0        0     1873 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/pyproject.toml
--rw-r--r--   0        0        0      166 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/tests/32_5_config.yaml
--rw-r--r--   0        0        0      224 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/tests/bandit.yaml
--rw-r--r--   0        0        0     1070 2023-06-18 17:54:13.542075 boneIO-0.6.3.dev4/tests/relay_32_5.py
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.6.3.dev4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/LICENSE
+-rw-r--r--   0        0        0      474 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/README.md
+-rw-r--r--   0        0        0      147 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/__init__.py
+-rw-r--r--   0        0        0     3341 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/bonecli.py
+-rw-r--r--   0        0        0     2947 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/const.py
+-rw-r--r--   0        0        0     8454 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/cover.py
+-rw-r--r--   0        0        0        0 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/__init__.py
+-rw-r--r--   0        0        0      168 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/adc_v0_4.yaml
+-rw-r--r--   0        0        0      238 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/binary_sensor.yaml
+-rw-r--r--   0        0        0      369 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/config.yaml
+-rw-r--r--   0        0        0      150 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/cover.yaml
+-rw-r--r--   0        0        0     2644 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/event.yaml
+-rw-r--r--   0        0        0     3392 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/led32x4A.yaml
+-rw-r--r--   0        0        0     1691 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/output24x16A.yaml
+-rw-r--r--   0        0        0     1713 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/output24x16A_v0.3.yaml
+-rw-r--r--   0        0        0     2403 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/example_config/output32x5A.yaml
+-rw-r--r--   0        0        0    19372 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/fonts/danube__.ttf
+-rw-r--r--   0        0        0     2039 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/__init__.py
+-rw-r--r--   0        0        0      985 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/async_updater.py
+-rw-r--r--   0        0        0     1138 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/click_timer.py
+-rw-r--r--   0        0        0     2321 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/config.py
+-rw-r--r--   0        0        0     7494 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/events.py
+-rw-r--r--   0        0        0      717 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/exceptions.py
+-rw-r--r--   0        0        0      885 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/filter.py
+-rw-r--r--   0        0        0     3249 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/gpio.py
+-rw-r--r--   0        0        0     6359 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/ha_discovery.py
+-rw-r--r--   0        0        0    14895 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/loader.py
+-rw-r--r--   0        0        0     1801 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/logger.py
+-rw-r--r--   0        0        0      765 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/mqtt.py
+-rw-r--r--   0        0        0      351 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/oled.py
+-rw-r--r--   0        0        0     2430 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/onewire/W1ThermSensor.py
+-rw-r--r--   0        0        0      448 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/onewire/__init__.py
+-rw-r--r--   0        0        0     5169 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/onewire/ds2482.py
+-rw-r--r--   0        0        0     2497 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/onewire/onewire.py
+-rw-r--r--   0        0        0     1066 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/queue.py
+-rw-r--r--   0        0        0     1994 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/state_manager.py
+-rw-r--r--   0        0        0     5853 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/stats.py
+-rw-r--r--   0        0        0     5806 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/timeperiod.py
+-rw-r--r--   0        0        0      508 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/util.py
+-rw-r--r--   0        0        0    11304 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/helper/yaml_util.py
+-rw-r--r--   0        0        0      178 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/input/__init__.py
+-rw-r--r--   0        0        0     2611 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/input/gpio.py
+-rw-r--r--   0        0        0     3133 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/input/gpio_beta.py
+-rw-r--r--   0        0        0    21785 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/manager.py
+-rw-r--r--   0        0        0     4176 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/modbus.py
+-rw-r--r--   0        0        0     8302 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/mqtt_client.py
+-rw-r--r--   0        0        0     5244 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/oled.py
+-rw-r--r--   0        0        0      181 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/relay/__init__.py
+-rw-r--r--   0        0        0     2623 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/relay/basic.py
+-rw-r--r--   0        0        0     1163 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/relay/gpio.py
+-rw-r--r--   0        0        0     2669 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/relay/mcp.py
+-rw-r--r--   0        0        0     4873 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/relay/pca.py
+-rw-r--r--   0        0        0     2653 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/runner.py
+-rw-r--r--   0        0        0     1030 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/actions.yaml
+-rw-r--r--   0        0        0      124 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/actions_sensor.yaml
+-rw-r--r--   0        0        0      129 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/actions_switch.yaml
+-rw-r--r--   0        0        0      286 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/filters.yaml
+-rw-r--r--   0        0        0      304 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/filters_adc.yaml
+-rw-r--r--   0        0        0       75 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/id.yaml
+-rw-r--r--   0        0        0    15072 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/schema.yaml
+-rw-r--r--   0        0        0       65 2023-08-04 20:08:27.770635 boneIO-0.7.0.dev1/boneio/schema/temp_unit.yaml
+-rw-r--r--   0        0        0      133 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/schema/update_interval.yaml
+-rw-r--r--   0        0        0      538 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/__init__.py
+-rw-r--r--   0        0        0     1328 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/adc.py
+-rw-r--r--   0        0        0     1296 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/gpio.py
+-rw-r--r--   0        0        0     1284 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/gpio_beta.py
+-rw-r--r--   0        0        0     8520 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/__init__.py
+-rw-r--r--   0        0        0     8810 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/dts1964_3f.json
+-rw-r--r--   0        0        0      526 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/pt100.json
+-rw-r--r--   0        0        0     2735 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/r4dcb08.json
+-rw-r--r--   0        0        0     4145 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/sdm120.json
+-rw-r--r--   0        0        0    10969 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/sdm630.json
+-rw-r--r--   0        0        0     5592 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/modbus/sofar.json
+-rw-r--r--   0        0        0     1808 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/temp/__init__.py
+-rw-r--r--   0        0        0     2485 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/temp/dallas.py
+-rw-r--r--   0        0        0      243 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/temp/lm75.py
+-rw-r--r--   0        0        0      271 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/sensor/temp/mcp9808.py
+-rw-r--r--   0        0        0       41 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/boneio/version.py
+-rw-r--r--   0        0        0     1871 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/tests/32_5_config.yaml
+-rw-r--r--   0        0        0      224 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/tests/bandit.yaml
+-rw-r--r--   0        0        0     1070 2023-08-04 20:08:27.774634 boneIO-0.7.0.dev1/tests/relay_32_5.py
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 boneIO-0.7.0.dev1/PKG-INFO
```

### Comparing `boneIO-0.6.3.dev4/LICENSE` & `boneIO-0.7.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/bonecli.py` & `boneIO-0.7.0.dev1/boneio/bonecli.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/const.py` & `boneIO-0.7.0.dev1/boneio/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 MCP = "mcp"
 MCP_ID = "mcp_id"
 PCA_ID = "pca_id"
 INIT_SLEEP = "init_sleep"
 
 # SENSOR CONST
 TEMPERATURE = "temperature"
+EVENT_ENTITY = "event"
 SENSOR = "sensor"
 BINARY_SENSOR = "binary_sensor"
 LM75 = "lm75"
 MCP_TEMP_9808 = "mcp9808"
 INPUT_SENSOR = "inputsensor"
 DS2482 = "ds2482"
 DALLAS = "dallas"
```

### Comparing `boneIO-0.6.3.dev4/boneio/cover.py` & `boneIO-0.7.0.dev1/boneio/cover.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/example_config/input.yaml` & `boneIO-0.7.0.dev1/boneio/example_config/event.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -178,27 +178,7 @@
   pin: P8_16
 - id: IN_44
   pin: P8_15
 - id: IN_45
   pin: P8_14
 - id: IN_46
   pin: P8_13
-
-- id: IN_47
-  pin: P8_12
-  kind: sensor
-- id: IN_48
-  pin: P8_11
-  kind: sensor
-- id: IN_49
-  pin: P8_10
-  kind: sensor
-
-- id: IN_50
-  pin: P8_9
-  kind: sensor
-- id: IN_51
-  pin: P8_8
-  kind: sensor
-- id: IN_52
-  pin: P8_7
-  kind: sensor
```

### Comparing `boneIO-0.6.3.dev4/boneio/example_config/led32x4A.yaml` & `boneIO-0.7.0.dev1/boneio/example_config/led32x4A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/example_config/output24x16A.yaml` & `boneIO-0.7.0.dev1/boneio/example_config/output24x16A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/example_config/output32x5A.yaml` & `boneIO-0.7.0.dev1/boneio/example_config/output32x5A.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/fonts/danube__.ttf` & `boneIO-0.7.0.dev1/boneio/fonts/danube__.ttf`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/__init__.py` & `boneIO-0.7.0.dev1/boneio/helper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     setup_output,
     write_output,
 )
 from boneio.helper.ha_discovery import (
     ha_adc_sensor_availabilty_message,
     ha_binary_sensor_availabilty_message,
     ha_button_availabilty_message,
-    ha_input_availabilty_message,
+    ha_event_availabilty_message,
     ha_light_availabilty_message,
     ha_sensor_availabilty_message,
     ha_sensor_temp_availabilty_message,
     ha_switch_availabilty_message,
     ha_led_availabilty_message,
 )
 from boneio.helper.mqtt import BasicMqtt
@@ -50,15 +50,15 @@
     "ha_light_availabilty_message",
     "ha_switch_availabilty_message",
     "ha_sensor_availabilty_message",
     "ha_adc_sensor_availabilty_message",
     "ha_sensor_temp_availabilty_message",
     "ha_binary_sensor_availabilty_message",
     "ha_button_availabilty_message",
-    "ha_input_availabilty_message",
+    "ha_event_availabilty_message",
     "ha_led_availabilty_message",
     "GPIOInputException",
     "GPIOOutputException",
     "I2CError",
     "GpioBaseClass",
     "StateManager",
     "configure_pin",
```

### Comparing `boneIO-0.6.3.dev4/boneio/helper/async_updater.py` & `boneIO-0.7.0.dev1/boneio/helper/async_updater.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/click_timer.py` & `boneIO-0.7.0.dev1/boneio/helper/click_timer.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/config.py` & `boneIO-0.7.0.dev1/boneio/helper/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Module to provide basic config options.
 """
 from __future__ import annotations
 from _collections_abc import dict_values
 from typing import Union
-from boneio.const import BONEIO, HOMEASSISTANT, LIGHT, SENSOR, COVER, BUTTON, SWITCH, BINARY_SENSOR
+from boneio.const import BONEIO, HOMEASSISTANT, LIGHT, SENSOR, COVER, BUTTON, SWITCH, BINARY_SENSOR, EVENT_ENTITY
 
 
 class ConfigHelper:
     def __init__(
         self,
         topic_prefix: str = BONEIO,
         ha_discovery: bool = True,
@@ -20,15 +20,16 @@
         self._fetch_old_discovery = None
         self._autodiscovery_messages = {
             SWITCH: {},
             LIGHT: {},
             BINARY_SENSOR: {},
             SENSOR: {},
             COVER: {},
-            BUTTON: {}
+            BUTTON: {},
+            EVENT_ENTITY: {}
         }
         self.manager_ready: bool = False
 
     @property
     def topic_prefix(self) -> str:
         return self._topic_prefix
```

### Comparing `boneIO-0.6.3.dev4/boneio/helper/events.py` & `boneIO-0.7.0.dev1/boneio/helper/events.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/exceptions.py` & `boneIO-0.7.0.dev1/boneio/helper/exceptions.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/filter.py` & `boneIO-0.7.0.dev1/boneio/helper/filter.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/gpio.py` & `boneIO-0.7.0.dev1/boneio/helper/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/ha_discovery.py` & `boneIO-0.7.0.dev1/boneio/helper/ha_discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     ON,
     OPEN,
     OPENING,
     RELAY,
     SENSOR,
     STATE,
     STOP,
+    SINGLE,
+    DOUBLE,
+    LONG
 )
 from boneio.version import __version__
 
 
 def ha_availabilty_message(
     id: str,
     name: str,
@@ -82,17 +85,18 @@
     msg["command_topic"] = f"{topic}/cmd/relay/{id}/set"
     msg["payload_off"] = OFF
     msg["payload_on"] = ON
     msg["value_template"] = "{{ value_json.state }}"
     return msg
 
 
-def ha_input_availabilty_message(**kwargs):
+def ha_event_availabilty_message(**kwargs):
     msg = ha_availabilty_message(device_type=INPUT, **kwargs)
     msg["icon"] = "mdi:gesture-double-tap"
+    msg["event_types"] = [SINGLE, DOUBLE, LONG]
     return msg
 
 
 def ha_adc_sensor_availabilty_message(**kwargs):
     msg = ha_availabilty_message(device_type=SENSOR, **kwargs)
     msg["unit_of_measurement"] = "V"
     msg["device_class"] = "voltage"
```

### Comparing `boneIO-0.6.3.dev4/boneio/helper/loader.py` & `boneIO-0.7.0.dev1/boneio/helper/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,48 +33,48 @@
     PIN,
     RELAY,
     RESTORE_STATE,
     SENSOR,
     SHOW_HA,
     UPDATE_INTERVAL,
     DallasBusTypes,
+    EVENT_ENTITY
 )
 from boneio.cover import Cover
 from boneio.helper import (
     GPIOInputException,
     GPIOOutputException,
     I2CError,
     StateManager,
     ha_adc_sensor_availabilty_message,
     ha_binary_sensor_availabilty_message,
-    ha_input_availabilty_message,
+    ha_event_availabilty_message,
     ha_sensor_temp_availabilty_message,
 )
 from boneio.helper.onewire import (
     DS2482,
     DS2482_ADDRESS,
     OneWireBus,
     AsyncBoneIOW1ThermSensor,
     OneWireAddress,
 )
 from boneio.helper.ha_discovery import ha_cover_availabilty_message
 from boneio.helper.timeperiod import TimePeriod
-from boneio.input.gpio import GpioInputButton
-from boneio.sensor import DallasSensorDS2482
+from boneio.input import GpioEventButton, GpioEventButtonBeta
+from boneio.sensor import DallasSensorDS2482, GpioInputBinarySensor, GpioInputBinarySensorBeta
 from boneio.sensor.temp.dallas import DallasSensorW1
 
 # Typing imports that create a circular dependency
 if TYPE_CHECKING:
     from ..manager import Manager
 
 from busio import I2C
 
 from boneio.relay import GpioRelay, MCPRelay, PWMPCA
 from boneio.sensor import GpioADCSensor, initialize_adc
-from boneio.sensor.gpio import GpioInputSensor
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def create_adc(manager: Manager, topic_prefix: str, adc_list: list = []):
     """Create ADC sensor."""
 
@@ -90,14 +90,15 @@
                 id=id,
                 pin=pin,
                 name=name,
                 manager=manager,
                 send_message=manager.send_message,
                 topic_prefix=topic_prefix,
                 update_interval=gpio.get(UPDATE_INTERVAL, TimePeriod(seconds=60)),
+                filters=gpio.get(FILTERS, []),
             )
             if gpio.get(SHOW_HA, True):
                 manager.send_ha_autodiscovery(
                     id=id,
                     name=name,
                     ha_type=SENSOR,
                     availability_msg_func=ha_adc_sensor_availabilty_message,
@@ -317,55 +318,88 @@
 )
 
 
 def input_chooser(input_type: str):
     """Get named tuple based on input."""
     if input_type == SENSOR:
         return InputEntry(
-            GpioInputSensor,
+            GpioInputBinarySensor,
             INPUT_SENSOR,
             BINARY_SENSOR,
             ha_binary_sensor_availabilty_message,
         )
     else:
-        return InputEntry(GpioInputButton, INPUT, SENSOR, ha_input_availabilty_message)
+        return InputEntry(GpioEventButton, INPUT, EVENT_ENTITY, ha_event_availabilty_message)
 
 
-def configure_input(
+def configure_event_sensor(
     gpio: dict,
     pin: str,
     press_callback: Callable,
     send_ha_autodiscovery: Callable,
 ) -> str:
     """Configure input sensor or button."""
     try:
-        input = input_chooser(input_type=gpio.get(KIND))
-        getattr(input, "InputClass")(
+        GpioEventButtonClass = GpioEventButton if gpio.get("detection_type", "stable") == "stable" else GpioEventButtonBeta
+        GpioEventButtonClass(
             pin=pin,
             press_callback=lambda x, i: press_callback(
                 x=x,
                 inpin=i,
                 actions=gpio.get(ACTIONS, {}).get(x, []),
-                input_type=getattr(input, "input_type"),
+                input_type=INPUT,
+                empty_message_after=gpio.get("clear_message", False)
             ),
             **gpio,
         )
         if gpio.get(SHOW_HA, True):
             send_ha_autodiscovery(
                 id=pin,
                 name=gpio.get(ID, pin),
-                ha_type=getattr(input, "ha_type"),
+                ha_type=EVENT_ENTITY,
                 device_class=gpio.get(DEVICE_CLASS, None),
-                availability_msg_func=getattr(input, "availability_msg_f"),
+                availability_msg_func=ha_event_availabilty_message,
             )
         return pin
     except GPIOInputException as err:
         _LOGGER.error("This PIN %s can't be configured. %s", pin, err)
         pass
 
+def configure_binary_sensor(
+    gpio: dict,
+    pin: str,
+    press_callback: Callable,
+    send_ha_autodiscovery: Callable,
+) -> str:
+    """Configure input sensor or button."""
+    try:
+        GpioInputBinarySensorClass = GpioInputBinarySensor if gpio.get("detection_type", "stable") == "stable" else GpioInputBinarySensorBeta
+        GpioInputBinarySensor(
+            pin=pin,
+            press_callback=lambda x, i: press_callback(
+                x=x,
+                inpin=i,
+                actions=gpio.get(ACTIONS, {}).get(x, []),
+                input_type=INPUT_SENSOR,
+                empty_message_after=gpio.get("clear_message", False)
+            ),
+            **gpio,
+        )
+        if gpio.get(SHOW_HA, True):
+            send_ha_autodiscovery(
+                id=pin,
+                name=gpio.get(ID, pin),
+                ha_type=BINARY_SENSOR,
+                device_class=gpio.get(DEVICE_CLASS, None),
+                availability_msg_func=ha_binary_sensor_availabilty_message,
+            )
+        return pin
+    except GPIOInputException as err:
+        _LOGGER.error("This PIN %s can't be configured. %s", pin, err)
+        pass
 
 def configure_cover(
     manager: Manager,
     cover_id: str,
     state_manager: StateManager,
     send_ha_autodiscovery: Callable,
     config: dict,
```

### Comparing `boneIO-0.6.3.dev4/boneio/helper/logger.py` & `boneIO-0.7.0.dev1/boneio/helper/logger.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/mqtt.py` & `boneIO-0.7.0.dev1/boneio/helper/mqtt.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/onewire/W1ThermSensor.py` & `boneIO-0.7.0.dev1/boneio/helper/onewire/W1ThermSensor.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/onewire/ds2482.py` & `boneIO-0.7.0.dev1/boneio/helper/onewire/ds2482.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/onewire/onewire.py` & `boneIO-0.7.0.dev1/boneio/helper/onewire/onewire.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/queue.py` & `boneIO-0.7.0.dev1/boneio/helper/queue.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/state_manager.py` & `boneIO-0.7.0.dev1/boneio/helper/state_manager.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/stats.py` & `boneIO-0.7.0.dev1/boneio/helper/stats.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/timeperiod.py` & `boneIO-0.7.0.dev1/boneio/helper/timeperiod.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/helper/yaml_util.py` & `boneIO-0.7.0.dev1/boneio/helper/yaml_util.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/input/gpio.py` & `boneIO-0.7.0.dev1/boneio/input/gpio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,73 @@
-"""GPIOInputButton to receive signals."""
+"""GpioEventButton to receive signals."""
 from __future__ import annotations
-import time
 import logging
+import asyncio
 from functools import partial
-from boneio.const import DOUBLE, LONG, SINGLE, ClickTypes, BOTH
-from boneio.helper import GpioBaseClass, ClickTimer
-from boneio.helper.gpio import add_event_callback, add_event_detect
-from boneio.helper.timeperiod import TimePeriod
+from boneio.const import DOUBLE, LONG, SINGLE, ClickTypes
+from boneio.helper import GpioBaseClass, ClickTimer, TimePeriod
+
+
 # TIMINGS FOR BUTTONS
 
+DOUBLE_CLICK_DURATION_MS = 350
+LONG_PRESS_DURATION_MS = 600
 
 _LOGGER = logging.getLogger(__name__)
 
-DOUBLE_CLICK_DURATION_MS = 250
-LONG_PRESS_DURATION_MS = 500
 
-class GpioInputButton(GpioBaseClass):
+class GpioEventButton(GpioBaseClass):
     """Represent Gpio input switch."""
 
     def __init__(self, **kwargs) -> None:
         """Setup GPIO Input Button"""
         super().__init__(**kwargs)
         self._state = self.is_pressed
-        self.button_pressed_time = 0.0
-        self._debounce_time: float = self._bounce_time.total_in_seconds
-        self._period_to_wait_for_2nd_click: float = self._debounce_time
-
-        self._timer_single = ClickTimer(
-            delay=TimePeriod(milliseconds=self._period_to_wait_for_2nd_click),
-            action=lambda x: self.press_callback(click_type=SINGLE),
-        )
-
+        _LOGGER.debug("Configured stable listening for input pin %s", self._pin)
         self._timer_double = ClickTimer(
             delay=TimePeriod(milliseconds=DOUBLE_CLICK_DURATION_MS),
-            action=lambda x: None,
+            action=lambda x: self.double_click_press_callback(),
         )
         self._timer_long = ClickTimer(
             delay=TimePeriod(milliseconds=LONG_PRESS_DURATION_MS),
             action=lambda x: self.press_callback(click_type=LONG),
         )
         self._double_click_ran = False
         self._is_waiting_for_second_click = False
         self._long_press_ran = False
+        asyncio.create_task(self._run())
 
-        add_event_detect(pin=self._pin, edge=BOTH)
-        add_event_callback(pin=self._pin, callback=self.check_state)
-        _LOGGER.debug("Configured listening for input pin %s", self._pin)
+    def press_callback(self, click_type: ClickTypes):
+        self._loop.call_soon_threadsafe(
+            partial(self._press_callback, click_type, self._pin)
+        )
 
+    def double_click_press_callback(self):
+        self._is_waiting_for_second_click = False
+        if not self._state and not self._timer_long.is_waiting():
+            self.press_callback(click_type=SINGLE)
 
-    def check_state(self, channel) -> None:
-        self._state = self.is_pressed
-        time_now = time.time()
-        if self._state:
-            if time_now - self.button_pressed_time >= self._debounce_time:
-                self.button_pressed_time = time_now
-                self._timer_long.start_timer()
-                self._timer_single.reset()
-                if self._timer_double.is_waiting():
-                    self._double_click_ran = True
-                    self.press_callback(click_type=DOUBLE)
-                    return
-                else:
-                    self._timer_double.start_timer()
-                    self._is_waiting_for_second_click = True
+    async def _run(self) -> None:
+        while True:
+            self.check_state(state=self.is_pressed)
+            await asyncio.sleep(self._bounce_time.total_in_seconds)
+
+    def check_state(self, state: bool) -> None:
+        if state == self._state:
+            return
+        self._state = state
+        if state: #is pressed?
+            self._timer_long.start_timer()
+            if self._timer_double.is_waiting():
+                self._timer_double.reset()
+                self._double_click_ran = True
+                self.press_callback(click_type=DOUBLE)
+            else:
+                self._timer_double.start_timer()
+                self._is_waiting_for_second_click = True
 
-        else:
+        else: #is released?
             if not self._is_waiting_for_second_click and not self._double_click_ran:
                 if self._timer_long.is_waiting():
                     self.press_callback(click_type=SINGLE)
-            elif self._is_waiting_for_second_click:
-                self._timer_single.start_timer()
             self._timer_long.reset()
             self._double_click_ran = False
-
-    def reset_all_timers(self) -> None:
-        self._is_waiting_for_second_click = False
-        self._timer_single.reset()
-        self._timer_double.reset()
-        self._timer_long.reset()
-
-    def press_callback(self, click_type: ClickTypes):
-        _LOGGER.debug("Detected press %s", click_type)
-        self.reset_all_timers()
-        self._loop.call_soon_threadsafe(
-            partial(self._press_callback, click_type, self._pin)
-        )
```

### Comparing `boneIO-0.6.3.dev4/boneio/manager.py` & `boneIO-0.7.0.dev1/boneio/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,16 @@
     ha_led_availabilty_message,
 )
 from boneio.helper.config import ConfigHelper
 from boneio.helper.events import EventBus
 from boneio.helper.exceptions import ModbusUartException
 from boneio.helper.loader import (
     configure_cover,
-    configure_input,
+    configure_event_sensor,
+    configure_binary_sensor,
     configure_relay,
     create_dallas_sensor,
     create_mcp23017,
     create_pca9685,
     create_temp_sensor,
 )
 from boneio.helper.logger import configure_logger
@@ -81,15 +82,16 @@
         self,
         send_message: Callable[[str, Union[str, dict], bool], None],
         stop_client: Callable[[], Awaitable[None]],
         state_manager: StateManager,
         config_helper: ConfigHelper,
         config_file_path: str,
         relay_pins: List = [],
-        input_pins: List = [],
+        event_pins: List = [],
+        binary_pins: List = [],
         sensors: dict = {},
         modbus: dict = {},
         pca9685: list = [],
         mcp23017: list = [],
         ds2482: Optional[List] = [],
         dallas: Optional[dict] = None,
         oled: dict = {},
@@ -105,15 +107,16 @@
         self._host_data = None
         self._config_file_path = config_file_path
         self._state_manager = state_manager
         self._event_bus = EventBus(self._loop)
 
         self.send_message = send_message
         self.stop_client = stop_client
-        self._input_pins = input_pins
+        self._event_pins = event_pins
+        self._binary_pins = binary_pins
         self._i2cbusio = I2C(SCL, SDA)
         self._mcp = {}
         self._pca = {}
         self._output = {}
         self._oled = None
         self._tasks: List[asyncio.Task] = []
         self._covers = {}
@@ -230,21 +233,34 @@
         self.prepare_ha_buttons()
         _LOGGER.info("BoneIO manager is ready.")
 
     def configure_inputs(self, reload_config: bool = False):
         used_pins = set()
         if reload_config:
             load_config_from_file(self._config_file_path)
-        for gpio in self._input_pins:
+        for gpio in self._event_pins:
             pin = gpio.pop(PIN)
             if pin in used_pins:
                 _LOGGER.warn("This PIN %s is already configured. Omitting it.", pin)
                 continue
             used_pins.add(
-                configure_input(
+                configure_event_sensor(
+                    gpio=gpio,
+                    pin=pin,
+                    press_callback=self.press_callback,
+                    send_ha_autodiscovery=self.send_ha_autodiscovery,
+                )
+            )
+        for gpio in self._binary_pins:
+            pin = gpio.pop(PIN)
+            if pin in used_pins:
+                _LOGGER.warn("This PIN %s is already configured. Omitting it.", pin)
+                continue
+            used_pins.add(
+                configure_binary_sensor(
                     gpio=gpio,
                     pin=pin,
                     press_callback=self.press_callback,
                     send_ha_autodiscovery=self.send_ha_autodiscovery,
                 )
             )
 
@@ -438,29 +454,28 @@
 
     @property
     def pca(self):
         """Get PCA by it's id."""
         return self._pca
 
     def press_callback(
-        self, x: ClickTypes, inpin: str, actions: List, input_type: InputTypes = INPUT
+        self, x: ClickTypes, inpin: str, actions: List, input_type: InputTypes = INPUT, empty_message_after: bool = False
     ) -> None:
         """Press callback to use in input gpio.
         If relay input map is provided also toggle action on relay or cover or mqtt."""
         topic = f"{self._config_helper.topic_prefix}/{input_type}/{inpin}"
         self.send_message(topic=topic, payload=x, retain=False)
         for action_definition in actions:
             _LOGGER.debug("Executing action %s", action_definition)
             if action_definition[ACTION] == OUTPUT:
                 device = action_definition.get(PIN)
                 if not device:
                     continue
                 relay = self._output.get(device.replace(" ", ""))
                 action = relay_actions.get(action_definition["action_output"])
-                print("reya", relay, action)
                 if relay and action:
                     getattr(relay, action)()
                 else:
                     if not action:
                         _LOGGER.warn("Action doesn't exists %s. Check spelling", action)
                     if not relay:
                         _LOGGER.warn("PIN %s for action not found", device)
@@ -476,17 +491,18 @@
                 if not device:
                     continue
                 cover = self._covers.get(device.replace(" ", ""))
                 if cover:
                     getattr(cover, action_definition["action_cover"])()
 
         # This is similar how Z2M is clearing click sensor.
-        self._loop.call_soon_threadsafe(
-            self._loop.call_later, 0.2, self.send_message, topic, ""
-        )
+        if empty_message_after:
+            self._loop.call_soon_threadsafe(
+                self._loop.call_later, 0.2, self.send_message, topic, ""
+            )
 
     def send_ha_autodiscovery(
         self,
         id: str,
         name: str,
         ha_type: str,
         availability_msg_func: Callable,
@@ -495,15 +511,15 @@
     ) -> None:
         """Send HA autodiscovery information for each relay."""
         if not self._config_helper.ha_discovery:
             return
         topic_prefix = topic_prefix or self._config_helper.topic_prefix
         payload = availability_msg_func(topic=topic_prefix, id=id, name=name, **kwargs)
         topic = f"{self._config_helper.ha_discovery_prefix}/{ha_type}/{topic_prefix}/{id}/config"
-        _LOGGER.debug("Sending HA discovery for %s, %s.", ha_type, name)
+        _LOGGER.debug("Sending HA discovery for %s entity, %s.", ha_type, name)
         self._config_helper.add_autodiscovery_msg(topic=topic, ha_type=ha_type, payload=payload)
         self.send_message(topic=topic, payload=payload, retain=True)
 
     def resend_autodiscovery(self) -> None:
         for msg in self._config_helper.autodiscovery_msgs:
             self.send_message(**msg, retain=True)
```

### Comparing `boneIO-0.6.3.dev4/boneio/modbus.py` & `boneIO-0.7.0.dev1/boneio/modbus.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/mqtt_client.py` & `boneIO-0.7.0.dev1/boneio/mqtt_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import json
 import logging
 import uuid
 from contextlib import AsyncExitStack
 from typing import Any, Callable, Optional, Set, Union, Awaitable
 
 import paho.mqtt.client as mqtt
-from asyncio_mqtt import Client as AsyncioClient
-from asyncio_mqtt import MqttError, Will
+from aiomqtt import Client as AsyncioClient, MqttError, Will
 from paho.mqtt.properties import Properties
 from paho.mqtt.subscribeoptions import SubscribeOptions
 
 from boneio.const import ONLINE, PAHO, STATE
 from boneio.helper import UniqueQueue
 from boneio.helper.config import ConfigHelper
 from boneio.manager import Manager
```

### Comparing `boneIO-0.6.3.dev4/boneio/oled.py` & `boneIO-0.7.0.dev1/boneio/oled.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/relay/basic.py` & `boneIO-0.7.0.dev1/boneio/relay/basic.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/relay/gpio.py` & `boneIO-0.7.0.dev1/boneio/relay/gpio.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/relay/mcp.py` & `boneIO-0.7.0.dev1/boneio/relay/mcp.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/relay/pca.py` & `boneIO-0.7.0.dev1/boneio/relay/pca.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/runner.py` & `boneIO-0.7.0.dev1/boneio/runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import asyncio
 import logging
 import os
 from typing import Any
 
 from boneio.const import (
     ADC,
+    BINARY_SENSOR,
     COVER,
     DALLAS,
     DS2482,
     ENABLED,
     HA_DISCOVERY,
     HOST,
-    INPUT,
+    EVENT_ENTITY,
     LM75,
     MCP23017,
     PCA9685,
     MCP_TEMP_9808,
     MODBUS,
     MQTT,
     OLED,
@@ -74,15 +75,16 @@
         for item in config_modules
     }
 
     manager = Manager(
         send_message=client.send_message,
         stop_client=client.stop_client,
         relay_pins=config.get(OUTPUT, []),
-        input_pins=config.get(INPUT, []),
+        event_pins=config.get(EVENT_ENTITY, []),
+        binary_pins=config.get(BINARY_SENSOR, []),
         config_file_path=config_file,
         state_manager=StateManager(
             state_file=f"{os.path.split(config_file)[0]}state.json"
         ),
         config_helper=_config_helper,
         sensors={
             LM75: config.get(LM75, []),
```

### Comparing `boneIO-0.6.3.dev4/boneio/schema/actions.yaml` & `boneIO-0.7.0.dev1/boneio/schema/actions.yaml`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/schema/schema.yaml` & `boneIO-0.7.0.dev1/boneio/schema/schema.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -318,15 +318,15 @@
         allowed: ["switch", "light", "none"]
         default: "switch"
         coerce: lower
         meta:
           label: If HA discovery is used device if relay is light or switch. If None is declared then any state is not published to MQTT (used for cover).
 
 
-input:
+binary_sensor:
   type: list
   meta:
     label: GPIO inputs section
   schema:
     type: dict
     schema:
       id:
@@ -342,60 +342,132 @@
       gpio_mode:
         type: string
         required: True
         default: "gpio"
         allowed: ["gpio", "gpio_pu", "gpio_pd", "gpio_input"]
         meta:
           label: What mode to use in config PIN.
+      detection_type:
+        type: string
+        required: True
+        default: "stable"
+        allowed: ["stable", "beta"]
+        meta:
+          label: There are 2 detector algorithms. Stable consumes more CPU. Beta is more optimized, but needed extra time for testing.
+      clear_message:
+        type: boolean
+        default: False
+        meta:
+          label: Decide if after press/release callback send empty message to mqtt. Same as Zigbee2Mqtt is doing in button actions.
       bounce_time:
         type:
           - string
           - timeperiod
         coerce:
           - str
           - positive_time_period
         required: True
-        default: "50ms"
+        default: "120ms"
         meta:
           label: Bounce time for GPIO in miliseconds. Only for advanced usage.
       show_in_ha:
         type: boolean
         required: True
         default: True
         meta:
           label: If you want you can disable discovering this input in HA.
-      kind:
+      device_class:
+        type: string
+        required: False
+        allowed: ["battery", "battery_charging", "carbon_monoxide", "cold", "connectivity", "door", "garage_door", "gas", "heat", "light", "lock", "moisture", "motion", "moving", "occupancy", "opening", "plug", "power", "presence", "problem", "running", "safety", "smoke", "sound", "tamper", "vibration", "window"]
+        meta:
+          label: Device class to use in HA
+      actions:
+        required: False
+        type: dict
+        coerce: check_actions
+        schema:
+          pressed: !include actions_sensor.yaml
+          released: !include actions_sensor.yaml
+
+
+event:
+  type: list
+  meta:
+    label: GPIO inputs section
+  schema:
+    type: dict
+    schema:
+      id:
+        type: string
+        required: False
+        meta:
+          label: Id to use in HA if needed. Default to pin number.
+      pin:
         type: string
-        allowed: ["switch", "sensor"]
-        default: "switch"
         required: True
         meta:
-          label: Either switch or sensor. If sensor then no clicks are detected, just simple on/off on gpio.
+          label: PIN to use.
+      gpio_mode:
+        type: string
+        required: True
+        default: "gpio"
+        allowed: ["gpio", "gpio_pu", "gpio_pd", "gpio_input"]
+        meta:
+          label: What mode to use in config PIN.
+      detection_type:
+        type: string
+        required: True
+        default: "stable"
+        allowed: ["stable", "beta"]
+        meta:
+          label: There are 2 detector algorithms. Stable consumes more CPU. Beta is more optimized, but needed extra time for testing.
+      clear_message:
+        type: boolean
+        default: False
+        meta:
+          label: Decide if after press/release callback send empty message to mqtt. Same as Zigbee2Mqtt is doing in button actions.
+      bounce_time:
+        type:
+          - string
+          - timeperiod
+        coerce:
+          - str
+          - positive_time_period
+        required: True
+        default: "120ms"
+        meta:
+          label: Bounce time for GPIO in miliseconds. Only for advanced usage.
+      show_in_ha:
+        type: boolean
+        required: True
+        default: True
+        meta:
+          label: If you want you can disable discovering this input in HA.
       inverted:
         type: boolean
         default: False
         required: True
         meta:
           label: Check if sensor type is inverted. Only aplicable for sensor kind.
       device_class:
         type: string
         required: False
-        allowed: ["battery", "battery_charging", "carbon_monoxide", "cold", "connectivity", "door", "garage_door", "gas", "heat", "light", "lock", "moisture", "motion", "moving", "occupancy", "opening", "plug", "power", "presence", "problem", "running", "safety", "smoke", "sound", "tamper", "vibration", "window"]
+        default: "button"
+        allowed: ["button", "doorbell", "motion"]
         meta:
           label: Device class to use in HA
       actions:
         required: False
         type: dict
         coerce: check_actions
         schema:
           single: !include actions_switch.yaml
           double: !include actions_switch.yaml
           long: !include actions_switch.yaml
-          pressed: !include actions_sensor.yaml
-          released: !include actions_sensor.yaml
 adc:
   type: list
   meta:
     label: GPIO ADC section
   schema:
     type: dict
     schema:
@@ -413,14 +485,15 @@
       update_interval: !include update_interval.yaml
       show_in_ha:
         type: boolean
         required: True
         default: True
         meta:
           label: If you want you can disable discovering this input in HA.
+      filters: !include filters_adc.yaml
 cover:
   type: list
   required: False
   meta:
     label: Cover section
   schema:
     type: dict
```

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/adc.py` & `boneIO-0.7.0.dev1/boneio/sensor/adc.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,19 +22,20 @@
 def initialize_adc():
     ADC.setup()
 
 
 class GpioADCSensor(BasicMqtt, AsyncUpdater, Filter):
     """Represent Gpio ADC sensor."""
 
-    def __init__(self, pin: str, **kwargs) -> None:
+    def __init__(self, pin: str, filters: list, **kwargs) -> None:
         """Setup GPIO ADC Sensor"""
         super().__init__(topic_type=SENSOR, **kwargs)
         self._pin = pin
         self._state = None
+        self._filters = filters
         AsyncUpdater.__init__(self, **kwargs)
         _LOGGER.debug("Configured sensor pin %s", self._pin)
 
     @property
     def state(self) -> float:
         """Give rounded value of temperature."""
         return self._state
```

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/gpio.py` & `boneIO-0.7.0.dev1/boneio/sensor/gpio.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""GPIOInputButton to receive signals."""
+"""GpioInputBinarySensor to receive signals."""
 import logging
 from functools import partial
 import asyncio
-from boneio.const import BOTH, PRESSED, RELEASED
-from boneio.helper import GpioBaseClass, edge_detect
+from boneio.const import PRESSED, RELEASED
+from boneio.helper import GpioBaseClass
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class GpioInputSensor(GpioBaseClass):
+class GpioInputBinarySensor(GpioBaseClass):
     """Represent Gpio sensor on input boards."""
 
     def __init__(self, **kwargs) -> None:
         """Setup GPIO Input Button"""
         super().__init__(**kwargs)
         self._state = self.is_pressed
         self._click_type = (
```

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/modbus/__init__.py` & `boneIO-0.7.0.dev1/boneio/sensor/modbus/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/modbus/dts1964_3f.json` & `boneIO-0.7.0.dev1/boneio/sensor/modbus/dts1964_3f.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/modbus/pt100.json` & `boneIO-0.7.0.dev1/boneio/sensor/modbus/pt100.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/modbus/r4dcb08.json` & `boneIO-0.7.0.dev1/boneio/sensor/modbus/r4dcb08.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/modbus/sdm120.json` & `boneIO-0.7.0.dev1/boneio/sensor/modbus/sdm120.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/modbus/sdm630.json` & `boneIO-0.7.0.dev1/boneio/sensor/modbus/sdm630.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/modbus/sofar.json` & `boneIO-0.7.0.dev1/boneio/sensor/modbus/sofar.json`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/temp/__init__.py` & `boneIO-0.7.0.dev1/boneio/sensor/temp/__init__.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/boneio/sensor/temp/dallas.py` & `boneIO-0.7.0.dev1/boneio/sensor/temp/dallas.py`

 * *Files identical despite different names*

### Comparing `boneIO-0.6.3.dev4/pyproject.toml` & `boneIO-0.7.0.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 description = "Python App for BoneIO"
 readme = "README.md"
 dynamic = []
 authors = [
     { name = "Paweł Szafer", email = "pszafer@gmail.com" },
 ]
 dependencies = [
-    "Adafruit-Blinka>=8.19.0",
-    "adafruit-circuitpython-ds18x20>=1.3.16",
-    "adafruit-circuitpython-mcp230xx>=2.5.9",
-    "adafruit-circuitpython-mcp9808>=3.3.19",
-    "adafruit-circuitpython-pct2075>=1.1.18",
-    "asyncio-mqtt>=0.16.1",
+    "Adafruit-Blinka>=8.20.1",
+    "adafruit-circuitpython-ds18x20>=1.3.17",
+    "adafruit-circuitpython-mcp230xx>=2.5.11",
+    "adafruit-circuitpython-mcp9808>=3.3.21",
+    "adafruit-circuitpython-pct2075>=1.1.19",
+    "aiomqtt>=1.1.0",
     "Cerberus>=1.3.4",
     "colorlog>=6.7.0",
     "gpio>=1.0.0",
     "luma-core>=2.4.0",
     "luma-oled>=3.12.0",
     "pymodbus>=2.5.3",
     "pyserial-asyncio>=0.6",
-    "PyYAML>=6.0",
+    "PyYAML>=6.0.1",
     "Adafruit-BBIO>=1.2.0",
     "psutil>=5.9.5",
-    "adafruit-circuitpython-onewire>=2.0.4",
+    "adafruit-circuitpython-onewire>=2.0.5",
     "w1thermsensor[async]>=2.0.0",
-    "adafruit-circuitpython-pca9685>=3.4.8",
+    "adafruit-circuitpython-pca9685>=3.4.10",
 ]
 requires-python = ">=3.7"
-version = "0.6.3.dev4"
+version = "0.7.0.dev1"
 
 [project.license]
 text = "GNU General Public License v3.0"
 
 [project.urls]
 Homepage = "https://boneio.eu"
 Repository = "https://github.com/boneIO-eu/app_bbb"
```

### Comparing `boneIO-0.6.3.dev4/tests/relay_32_5.py` & `boneIO-0.7.0.dev1/tests/relay_32_5.py`

 * *Files identical despite different names*

